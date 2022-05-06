---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: Filter event subscription messages
description: You can build intermediary processing components that can help you filter and process only the event subscription messages that your business needs.
---

# Filter event subscription messages

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can build intermediary processing components that can help you filter and process only the event subscription messages that your business needs.

To learn about event subscriptions, see [Event Subscription API](../../wf-api/general/event-subs-api.md).

##  Filtering Event Messages {#filtering-event-messages}

This section contains code snippets of filtering that you can implement to lessen the load of event subscription messages.  ```To help show the differences in various languages' syntax, these snippets illustrate the same set of filters written in the following languages:```

You can view examples of filtering at [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples), where you can see the differences in the syntax for each language and the means of interaction with the AWS SDK.&nbsp;These examples are written as AWS Lambdas, which is a common method for employing intermediary filtering and processing components.

The following code snippets are near deployment-ready and can be used as a starting point for helping you write your own, more complex, filters and processing components.

###  Java {#java}

The following example in Java shows how to filter project payloads based on the Group ID of the project, as done in&nbsp; [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. Establish the group ID that you are looking for and create it as a static constant.   
   <pre><span class="wysiwyg-font-size-small">private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";</span></pre> In this example, the handleRequest method, which is an AWS Lambda standard method name, takes a Map type as its first parameter, which is the event subscription message content.  
   ```The second parameter it takes is the context of the current Lambda Proxy request.  
   ```The Context object is used to obtain a Lambda Logger, which is used to write a message to the CloudWatch&nbsp;Logs.  
   <pre><span class="wysiwyg-font-size-small">public String handleRequest(Map<String, Object> webHookPayload, Context context) {
...
}</span></pre>

1. Upon invocation of the handleRequest method, obtain the “newState” attribute of the event subscription message, which represents the updated state of the resource.  
   <pre><span class="wysiwyg-font-size-small">public String handleRequest(Map<String, Object> webHookPayload, Context context) {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
}</span></pre> To learn about the newState format, see [Outbound message format for event subscriptions](../../wf-api/api/message-format-event-subs.md).

1. ```After parsing the “newState” Map from the message, ensure the object's group ID matches the group ID you identified in Step 1. 
   ``` 
1. ```(Conditional) If the IDs **do not** match, drop the message so that an empty response is returned.   
   ```<pre><span class="wysiwyg-font-size-small">public String handleRequest(Map<String, Object> webHookPayload, Context context) {
        ...
    String projectGroupId = (String) newState.get("groupID");
    logger.log("String projectGroupID is - " + projectGroupId);<br>    if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        ...
    }
    return "";
}</span></pre>

   >[!NOTE]
   >
   >Returning an empty, successful response is crucial. Anything besides a 200-level response is considered a failed delivery.

1. Process the message.   
   <pre><span class="wysiwyg-font-size-small">public String handleRequest(Map<String, Object> webHookPayload, Context context) {
        ...
        if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        logger.log("Processing Event Subscription message matching groupId " + DESIRED_GROUP_ID + "...");

        AWSLambda client = AWSLambdaClientBuilder.standard().build();
        InvokeRequest request = new InvokeRequest()
                .withFunctionName("MyFunction")
                .withInvocationType("Event")
                .withLogType("Tail")
                .withPayload(jsonParser.toJson(webHookPayload))
        InvokeResult response = client.invoke(request);
    }
    ... 
}</span></pre>The AWS SDK is used to invoke another Lambda, which is responsible for delivering the filtered message to our desired endpoint.  
   The purpose of passing off the responsibility of delivering the message to another Lambda is to avoid a timeout of the delivery request coming from the Event Subscription service. Currently, the allowable timeout for delivery is set to five seconds. If the filter takes longer than allowed by&nbsp;the setting, you can process the request, but the Event Subscription service will time out and fall into a retry loop until it receives a 200-level response within the timeout period.   
   To learn more about managing message delivery, see [Improving Message Delivery While Accommodating Timeouts](#improving-message-delivery-while-accommodating-timeouts).&nbsp; &nbsp;

### Python

```The main difference between the Java and Python examples is that in the Java example the event subscription message is received as the first parameter, and in the Python example the first parameter is a Lambda proxy "event," which contains the event subscription message along with information about the AWS Lambda proxy request.```

```The following example in Python shows how to filter project payloads based on the Group ID of the project, as done in  [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)```

1. ``` ```Establish the group ID that you are looking for and create it as a static constant.   
   ``````<pre><span class="wysiwyg-font-size-small">DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'</span></pre>```The first parameter is the Lambda proxy "event," which contains the event subscription message and some additional information that needs to be parsed out.   
   ``` ```The second parameter is the context of the current Lambda Proxy request.   
   ```In this example, the Context object is used to obtain a Lambda Logger, which is used to write a message to the CloudWatch&nbsp;Logs.  
   <pre><span class="wysiwyg-font-size-small">def project_group_filter_handler(event, context):
       ...</span></pre>

1. ```Parse out the message from the event.  
   ```<pre><span class="wysiwyg-font-size-small">event_subscription_message = json.loads(event['body'])</span></pre>

1. Obtain the “newState” attribute of the event subscription message.  
   The newState attribute represents the updated state of the resource.  
   <pre><span class="wysiwyg-font-size-small">new_state = json.loads(event_subscription_message['newState'])</span></pre> To learn about the newState format, see [Outbound message format for event subscriptions](../../wf-api/api/message-format-event-subs.md).

1. ```After parsing the “newState” Map from the message, ensure the object's group ID matches the group ID you identified in Step 1.``` 
1. ``` ```(Conditional) If the IDs do not match, drop the message so that an empty response is returned.   
   ``````<pre><span class="wysiwyg-font-size-small">if new_state['groupID'] == DESIRED_GROUP_ID:
    # Process the message
    print('matched group ID')
    process_message(event_subscription_message)

return {
'statusCode': 200<br></span>}</pre>

   >[!NOTE]
   >
   >Returning an empty, successful response is crucial. Anything besides a 200-level response is considered a failed delivery.

1. Process the message.   
   <pre><span class="wysiwyg-font-size-small">def process_message(event_subscription_message):
    aws_lambda.invoke(
        FunctionName='forwardMessageOntoMyEndpoint',
        InvocationType='Event',
        LogType='None',
        Payload=event_subscription_message
    )</span></pre> The AWS SDK is used to invoke another Lambda, which is responsible for delivering the filtered message to our desired endpoint.  
   The purpose of passing off the responsibility of delivering the message to another Lambda is to avoid a timeout of the delivery request coming from the Event Subscription service. Currently, the timeout for delivery is set to five seconds. If the filter takes longer than allowed by&nbsp;the setting, you can process the request, but the Event Subscription service will time out and fall into a retry loop until it receives a 200-level response within the timeout period.   
   To learn more about managing message delivery, see [Improving Message Delivery While Accommodating Timeouts](#improving-message-delivery-while-accommodating-timeouts).

### Node.js

```The Node.js example of project group ID filtering reads similar to the Java and Python examples. As with the Python example, the first parameter is a Lambda proxy event and the second parameter is the Lambda Context.```

```The following example in Node.js shows how to filter project payloads based on the Group ID of the project, as done in  [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)```

1. ``` ```Establish the group ID that you are looking for and create it as a static constant.   
   ``````<pre><span class="wysiwyg-font-size-small">const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';</span></pre>```The first parameter is the Lambda proxy "event," which contains the event subscription message and some additional information that needs to be parsed out.   
   ``` ```The second parameter is the context of the current Lambda Proxy request.   
   ```In this example, the Context object is used to obtain a Lambda Logger, which is used to write a message to the CloudWatch&nbsp;Logs.  
   <pre><span class="wysiwyg-font-size-small">exports.myProjectGroupFilterHandler = function (event, context) {
	...
}</span></pre>

1. ```Parse out the message from the event.  
   ```<pre><span class="wysiwyg-font-size-small">let eventSubscriptionMessage = JSON.parse(event.body);</span></pre>

1. Obtain the projectGroupID&nbsp;from the “newState” attribute of the event subscription message, then match it against the group ID of&nbsp;the group you identified in Step 1. 
   <pre><span class="wysiwyg-font-size-small">let projectGroupId = eventSubscriptionMessage.newState.groupID;</span></pre> To learn about the newState format, see [Outbound message format for event subscriptions](../../wf-api/api/message-format-event-subs.md).

1. (Conditional) If the IDs do not match, drop the message so that an empty response is returned.  
   The following example shows&nbsp;matching group IDs:&nbsp;  
   <pre><span class="wysiwyg-font-size-small">if (projectGroupId === DESIRED_GROUP_ID) {
    // Process the message
    console.log('Processing Event Subscription message matching groupId ' + DESIRED_GROUP_ID + '...');
    forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context);
} else {
    endLambdaRequest(context);
}</span></pre>

   >[!NOTE]
   >
   >Returning an empty, successful response is crucial. Anything besides a 200-level response is considered a failed delivery.

1. Process the message.   
   <pre><span class="wysiwyg-font-size-small">function forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context) {
    let lambdaParams = {
        FunctionName: 'forwardMessageOntoMyEndpoint',
        InvocationType: 'Event',
        LogType: 'None',
        Payload: new Buffer(JSON.stringify(eventSubscriptionMessage))
    };

    lambda.invoke(lambdaParams, function (err, data) {
        if (err) {
            console.error(err, err.stack);
        } else {
            console.log('data = ' + data);
        }
        endLambdaRequest(context);
    });
}</span></pre> The AWS SDK is used to invoke another Lambda, which is responsible for delivering the filtered message to our desired endpoint.  
   The purpose of passing off the responsibility of delivering the message to another Lambda is to avoid a timeout of the delivery request coming from the Event Subscription service. Currently, the timeout for delivery is set to five seconds. If the filter takes longer than allowed by&nbsp;the setting, you can process the request, but the Event Subscription service will time out and fall into a retry loop until it receives a 200-level response within the timeout period.   
   To learn about managing message delivery, see&nbsp; [Improving Message Delivery While Accommodating Timeouts](#improving-message-delivery-while-accommodating-timeouts).&nbsp; &nbsp;&nbsp;&nbsp;

## Improving Message Delivery While Accommodating Timeouts {#improving-message-delivery-while-accommodating-timeouts}

```The Event Subscription service has a strict timeout of``` **five seconds** ```for all delivery requests.``` ```In the event that the delivery of a message exceeds the allowed time, the Event Subscription service begins a retry cycle for that message.```

```For example, you build a project group ID filter similar to one of the examples found in [Filtering Event Messages](#filtering-event-messages) and you include a database lookup to determine whether the message is needed. It is possible that the database lookup along with the time needed for required processing and for the Lambda to cold-start could take more than five seconds, causing the Event Subscription service to retry delivering the message.```

You can avert a retry by&nbsp; ```separating the time-consuming parts of the process from the logic that is responsible for determining whether the message is one you want to process and deliver. By doing so, you can accept the message and send back a 200-level response to the Event Subscription service, while asynchronously continuing to process or filter the message in the background (see Step 5 in [Java](#java) for an example).  
```

```Even if your processing or filtering does not exceed the five-second timeout, it is still advantageous to separate out the first touch-point of message filtering or processing from the other processing or delivery steps on the client side. That way the handoff of the message to the destination from the Event Subscription service has minimal time and performance impact to both parties.```

```To learn more about the retry mechanism, see [Event subscription retries](../../wf-api/api/event-sub-retries.md).```

###  

## Implementing Hosted Filters in Cloudless Architecture

```If you are unable to leverage a cloud architecture for event subscription filtering, you can still use the examples in [Filtering Event Messages](#filtering-event-messages) as roadmaps of how to implement your own hosted filters or processing components.```

### Adjusting Filtering Examples for Stand-alone Services

```Before using the filtering examples in a cloudless environment, do the following:```

* ```Omit the Lambda-specific pieces of the examples, such as the Context parameter.``` 
* Change the invocations of other Lambdas in the examples to making additional asynchronous HTTP requests to other filters or processing components that you host.&nbsp;
* If referring to the Python and Node.js examples, substitute the first event parameter with the first payload parameter shown in the Java example (see Step 1 in [Java](#java)). 
* Deploy&nbsp;the filters or processors with a web-based API.

### Preventing Missed Event Subscription Messages

```Occasionally, in a cloudless architecture, services responsible for receiving event subscription messages may be unreachable. In such an event, messages might exceed the retry limit and be lost, with no way to retrieve the information within the messages.```

```We recommend that during the startup of your service you implement a query asking for the most recent state of all resources that might have been included in the missed messages. As shown in the following example, you can use the filter criteria to query for resources that match that criteria and then process their current state.``` 
<pre><span class="wysiwyg-font-size-small">public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v9.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
    replacing <...> with the appropriate values
    URI projectGroupQueryUri = generateProjectRecoveryQueryURI(logger);

    HttpUriRequest projectGroupIdGetRequest = new HttpGet(projectGroupQueryUri);

    // Our preferred method of authentication 
    projectGroupIdGetRequest.addHeader("apiKey", WORKFRONT_API_KEY);
 
    List<Map<String, Object>> projects = null;

    try {
        HttpResponse response = httpClient.execute(projectGroupIdGetRequest);
        InputStream responseBodyStream = response.getEntity().getContent();
        Reader reader = new InputStreamReader(responseBodyStream);
        Type listType = new TypeToken<List<Map<String, Object>>>(){}.getType();
        projects = new GsonBuilder().create().fromJson(reader, listType);
    } catch (IOException e) {
        logger.log("An IOException was thrown while executing a request to Workfront for projects matching the group ID " + DESIRED_GROUP_ID);
    }
    return projects;
}</span></pre>```By querying for resources, you ensure that your integrating systems have the most current version of resources. `````````

####  

### Implementing Asynchronous Processing in Delivering Messages

```All the examples in the [Filtering Event Messages](#filtering-event-messages) section pass the responsibility of delivering filtered messages to another AWS Lambda. This is done to avoid exceeding the five-second timeout in the delivery request, which is enforced by the Event Subscription service that issues the request.```

```In a cloudless architecture, you might need to implement an asynchronous processing mechanism similar to how the AWS SDK allows for asynchronous calls to other AWS Lambdas. Most modern programming languages have third-party or core libraries that handle asynchronous processing, allowing you to leverage the async-style of processing implemented in our examples.``` 
