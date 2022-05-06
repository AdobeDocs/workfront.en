---
filename: event-subs-api
content-type: api
navigation-topic: general-api
title: Event Subscription API
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Event Subscription API

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

&nbsp;

When an action occurs on a Adobe Workfront object that is supported by event subscriptions, you can configure Workfront to send a response to your desired endpoint. This means that third-party applications can receive updates from Workfront interactions via the Workfront API soon after they occur. In general, you can expect to receive webhook notifications in less than 5 seconds from the data change being logged. On average, customers receive webhook notifications in less than 1 second from the data change being logged.&nbsp;&nbsp;

In order to receive event subscriptions payloads through your firewall, you must add the following IP addresses to your allowlist:

**For customers in Europe:**

* 3.122.135.96
* 3.122.150.235
* 52.19.64.185
* 52.212.92.170

**For customers in locations other than Europe:**

* 35.160.0.242
* 34.213.36.118
* 3.209.27.146
* 18.205.251.4

The following topics support the Event Subscription API:

## Objects Supported by Event Subscriptions

The following Workfront objects are supported by event subscriptions.

* Assignment
* Company
* Dashboard
* Document
* Expense
* Hour
* Issue
* Note
* Portfolio
* Program
* Project
* Report
* Task
* Template
* Timesheet
* User

For a list of fields supported by event subscription objects, see [Event subscription resource fields](../../wf-api/api/event-sub-resource-fields.md).

## Event Subscription Authentication

To create, query, or delete an event subscription, your Workfront user needs the following:

* An access level of “System Administrator” 
* An apiKey

  >[!NOTE]
  >
  >If your user is already utilizing Workfront’s API, your user should already have an apiKey. You can retrieve the apiKey via the following HTTP request:

**Request URL:** 

[Copy](javascript:void(0);) 
<pre><code>[PUT]<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;https://<HOSTNAME>/attask/api/v7.0/USER?action=getApiKey&username=<USERNAME>&password=<PASSWORD></code></pre>**Request Headers:** 

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header Name</p> </th> 
   <th> <p>Header Value</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Content-type</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
 </tbody> 
</table>

**Response Codes:** 

| Response Code |Description |
|---|---|
| 200 (OK) |The request was processed successfully, and the existing apiKey for the user should be returned in the response body. |
| 401 (Unauthorized) |The server acknowledges the request but was unable to process it because the requesting apiKey/user does not have access to make this request. |

**Response Body Example:** 

[Copy](javascript:void(0);) 
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"data"</span>: {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"result"</span>: <span style="color: #dd1144; ">"rekxqndrw9783j4v79yhdsakl56bu1jn"</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}</code></pre>

>[!NOTE]
>
>&nbsp;If this is your first time using the Workfront API, then you need to generate an apiKey which you can do via this link:

[Copy](javascript:void(0);) 
<pre><code>[PUT]<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;https://<HOSTNAME>/attask/api/v7.0/USER/generateApiKey?username=<USERNAME>&password=<PASSWORD></code></pre>

## Forming the Subscription&nbsp;Resource

The subscription resource&nbsp;contains the following fields.

* objId (optional)

   * **String** - The ID of the object of the specified objCode for which events are fired. If this field is not specified, the user receives events for all objects of the specified type.

* objCode (required)

   * **String** - The objCode of the object being subscribed to changes. The possible values for objCode are listed in the table below.

     <table cellspacing="15"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>Object</p></th> 
        <th><p>objCode</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">Assignment</td> 
        <td scope="col"><p>ASSGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Company&nbsp;</td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Dashboard</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Document</p></td> 
        <td scope="col">DOCU&nbsp;</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Expense</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Hour</p></td> 
        <td scope="col">HOUR</td> 
       </tr> 
       <tr> 
        <td scope="col">Issue</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Note</td> 
        <td scope="col">NOTE</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Portfolio</p></td> 
        <td scope="col"><p>PORT</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Program</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Project</p></td> 
        <td scope="col"><p>PROJ</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Report</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Task</p></td> 
        <td scope="col"><p>TASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Template</p></td> 
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Timesheet</td> 
        <td scope="col">TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">User</td> 
        <td scope="col">USER</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (required)

   * **String** - A value that represents the type of event to which the object is subscribed. The available event types include:

      * CREATE
      * DELETE&nbsp;
      * UPDATE
      * SHARE

* url (required)

   * **String** - The URL of the endpoint to which subscription event payloads are sent via HTTP.

* authToken (required)

   * **String** - The OAuth2 bearer token used to authenticate with the URL specified in the “URL” field.&nbsp;

## Creating Event Subscription API&nbsp;Requests

After ensuring the user has administrator access and forming the subscription resource, you are ready to create event subscriptions.

Use the following syntax to construct the URL.

**Request URL:** 

[Copy](javascript:void(0);) 
<pre><code>[POST] https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions</code></pre>**Request Headers:** 

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header Name</p> </th> 
   <th> <p>Header Value</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Content-type</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Authorization</p> </td> 
   <td> <p>apiKey value</p> </td> 
  </tr> 
 </tbody> 
</table>

**Request Body Example:** 

[Copy](javascript:void(0);) 
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"objCode"</span>: <span style="color: #dd1144; ">"PROJ"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"eventType"</span>: <span style="color: #dd1144; ">"UPDATE"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"url"</span>: <span style="color: #dd1144; ">"http://requestb.in/ua5hi2ua"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"authToken"</span>: <span style="color: #dd1144; ">"EauthTokenWorkfrontRocks1234_"</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}</code></pre>**Response Codes:** 

| Response Code |Description |
|---|---|
| 201 (Created) |The event subscription was successfully created. |
| 400 (Bad Request) |The URL field of the subscription resource&nbsp;was deemed invalid. |
| 401 (Unauthorized) |The apiKey provided was empty or deemed invalid. |
| 403 (Forbidden) |The user, which matches the provided apiKey, does not have administrator access. |

Passing a&nbsp;subscription resource&nbsp;as the body of a&nbsp;request (with the content-type being&nbsp;“application/json”) results in an event subscription being created for the object specified. A response code of 201 (Created) indicates the subscription was created. A response code other than 201 means the subscription was **NOT** created.

>[!NOTE]
>
>&nbsp;The “Location” response header contains the URI of the newly created event subscription.

**Response Headers Example:** 

| Response Headers |Example |
|---|---|
| Content-Length |<pre>→0</pre> |
| Date |<pre>→Wed, 05 Apr 2017 21:23:33 GMT</pre> |
| Location |<pre>→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2</pre> |
| Server | &nbsp; <pre>→Apache-Coyote/1.1</pre> |

**Response Body Example:**N/A&nbsp;

## Querying Event Subscriptions

When querying Workfront’s HTTP use the GET method. There are two ways to query for event subscriptions: Query by subscription ID (see below) or query all event subscriptions.

### Query All Events Subscriptions

You can query all events subscriptions for a customer as specified by the apiKey value. You can also use the following options to manage the response:

* **page**: query parameter option to specify the number of pages to return. The default is 1.
* **limit**: query parameter option to specify the number of results to return per page. The default is 100 with a max of 1000.

The request syntax for listing all event subscriptions for a specific customer is as follows:

**Request URL:** 

[Copy](javascript:void(0);) 
<pre><code>[GET] https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions</code></pre>**Request Headers:** 

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header Name</p> </th> 
   <th> <p>Header Value</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Authorization</p> </td> 
   <td> <p>apiKey value</p> </td> 
  </tr> 
 </tbody> 
</table>

**Response Codes:** 

| Response Code |Description |
|---|---|
| 200 (OK)  |The request returned with all event subscriptions found for the customer matching the provided apiKey. |
| 401 (Unauthorized) |The apiKey provided was empty. |
| 403 (Forbidden) |The user, which matches the provided apiKey, does not have administrator access. |

**Response Headers Example:** 

| Response Header |Example |
|---|---|
| Content-Type |<pre>→application/json;charset=UTF-8</pre> |
| Date |<pre>→Wed, 05 Apr 2017 21:29:32 GMT</pre> |
| Server |<pre>→Apache-Coyote/1.1</pre> |
| Transfer-Encoding |<pre>→chunked</pre> |

**Response Body Example:** 

[Copy](javascript:void(0);) 
<pre><code><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"subscriptions"</span>:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"id"</span>: <span style="color: #dd1144; ">"37c4bcf5-e0b5-4256-aba3-a51cba7bf997"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"customerId"</span>: <span style="color: #dd1144; ">"504f9640000013401be513579fbebffa"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"objId"</span>: <span style="color: #dd1144; ">"ObjId1234"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"objCode"</span>: <span style="color: #dd1144; ">"TASK"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"url"</span>: <span style="color: #dd1144; ">"http://test.test.net/test/1234"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"eventType"</span>: <span style="color: #dd1144; ">"UPDATE"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"authToken"</span>: <span style="color: #dd1144; ">"auth_token"</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"id"</span>: <span style="color: #dd1144; ">"750a636c-5628-48f5-ba26-26b7ce537ac2"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"customerId"</span>: <span style="color: #dd1144; ">"504f9640000013401be513579fbebffa"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"objId"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"objCode"</span>: <span style="color: #dd1144; ">"PROJ"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"url"</span>: <span style="color: #dd1144; ">"http://requestb.in/ua5hi2ua"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"eventType"</span>: <span style="color: #dd1144; ">"UPDATE"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"authToken"</span>: <span style="color: #dd1144; ">"authTokenWorkfrontRocks1234_"</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;],<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"meta"</span>:<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"page"</span>: <span style="color: #008080; ">1</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"page_count"</span>: <span style="color: #008080; ">2</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"limit"</span>: <span style="color: #008080; ">100</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"total_count"</span>: <span style="color: #008080; ">150</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</code></pre>Where

* **page** and **limit** are the values provided in the request or the default if no values are provided
* **page_count** is the total number of pages that can be queried.
* **total_count** is the total number of subscriptions that match the query.

### Query By the Event Subscription ID

You can query for event subscriptions by the event subscription’s ID. The request syntax for listing event subscriptions is as follows:

**Request URL:** 

[Copy](javascript:void(0);) 
<pre><code>[GET] https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID></code></pre>**Request Headers:** 

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header Name</p> </th> 
   <th> <p>Header Value</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Authorization</p> </td> 
   <td> <p>apiKey value</p> </td> 
  </tr> 
 </tbody> 
</table>

**Response Codes:** 

| Response Code |Description |
|---|---|
| 200 (OK) |The request returned with the event subscription matching the provided subscription ID.  |
| 401 (Unauthorized)  |The apiKey provided was empty. |
| 403 (Forbidden) |The user, which matches the provided apiKey, does not have administrator access. |

**Response Body Example:** 

[Copy](javascript:void(0);) 
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"id"</span>: <span style="color: #dd1144; ">"750a636c-5628-48f5-ba26-26b7ce537ac2"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"customerId"</span>: <span style="color: #dd1144; ">"504f9640000013401be513579fbebffa"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"objId"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"objCode"</span>: <span style="color: #dd1144; ">"PROJ"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"url"</span>: <span style="color: #dd1144; ">"http://requestb.in/ua5hi2ua"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"eventType"</span>: <span style="color: #dd1144; ">"UPDATE"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"authToken"</span>: <span style="color: #dd1144; ">"authTokenWorkfrontRocks1234_"</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</code></pre>

## Event subscription filtering

Event subscription filtering can be used to ensure that you receive only relevant messages. Creating filters for your subscriptions may significantly decrease the number of messages that your endpoint needs to consume.

For example, an **UPDATE - TASK** event subscription can be set to trigger only when the **newState** of an event payload defines the **taskStatus** as **current**.

>[!IMPORTANT]
>
>The following attributes apply to event subscription filtering

* When a filter field has a non-empty value only messages with a **newState** containing the filter keys and values are sent to the subscribed URL
* You may filter by custom data included in the **newState** AND/OR **oldState**of the object
* Filters are evaluated solely on whether or not they are equal to a specific value
* If your filter syntax is incorrect or does not match any data contained in the **newState** of the payload, a validation message will not be returned to indicate an error has occured
* Filters can't be updated on a subscription that currently exists; a new subscription must be created with new filter parameters.
* Multiple filters can be applied to a single subscription and the subscription will only be delivered when all filter conditions have been met.
* Applying multiple filters to a single subscription is a practice equivalent to using an **AND** logical operator.
* Multiple event subscriptions can be applied to a single object as long as one or more event subscription field parameters are different between each event subscription.
* When multiple event subscriptions are assigned to a single object, all event subscriptions associated with that object can be returned to a single endpoint. This practice can be used used as an equivalent substitute for logical operator **OR** which can't be set using filter parameters.

### Using comparison operators

You can specify a comparison field along with the filter field. Use a comparison operator in this to field to filter for comparative results. For example, you can can create an UPDATE - TASK subscription that only sends a payload if the task status does NOT equal current. You can use the following comparison operators:

* eq: equal
* ne: not equal
* gt: greater than
* lt: less than

### Using connector fields

You can make several AND or OR statements in a single filter by specifying a connector field. When used along with the filter field, this determines which type of operation you want to perform between different filters in your subscription.

``` ```**Example: **``````JSON object defining an event subscription that fires when an optask is updated, with filter parameter set to filter by **projectID**, **enteredByID**, and a custom field specified by **parameterValues** called **customField** with a value equal to **customValue**.

[Copy](javascript:void(0);) 
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"objCode": "OPTASK",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"eventType": "UPDATE",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"url": "https://eventfilter.yourendpoint.com",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"authToken": "EauthTokenWorkfrontRocks1234_",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"filters": [<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"fieldName": "projectID",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"fieldValue": "5db1e0ec007696247fcf2290ecf8a339"<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"fieldName": "enteredByID",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"fieldValue": "5a456f460328289a0cd2c21b34c54741"<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"fieldName": "parameterValues",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"fieldValue": {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"DE: customField": "customValue"<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;]<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</code></pre>

## Deleting Event Subscriptions

When deleting Workfront’s HTTP use the DELETE method. The request syntax for deleting a single event subscription by subscription ID is as follows:

**Request URL:** 

[Copy](javascript:void(0);) 
<pre><code>[DELETE] https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>&nbsp;</code></pre>**Request Headers:** 

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header Name</p> </th> 
   <th> <p>Header Value</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Authorization</p> </td> 
   <td> <p> User’s apiKey </p> </td> 
  </tr> 
 </tbody> 
</table>

**Response Codes:** 

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Response Code</p> </th> 
   <th>&nbsp;Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (No Content)</td> 
   <td>The server successfully removed the event subscription matching the provided subscriptionID.</td> 
  </tr> 
  <tr> 
   <td>401 (Unauthorized)</td> 
   <td>The apiKey provided was empty.</td> 
  </tr> 
  <tr> 
   <td>403 (Forbidden)</td> 
   <td>The User which matches the provided apiKey does not have administrator access.</td> 
  </tr> 
  <tr> 
   <td>404 (Not Found)</td> 
   <td>The server was unable to find an event subscription matching the subscriptionID provided for deletion.</td> 
  </tr> 
 </tbody> 
</table>

**Response Headers Example:** 

| Response Header |Example |
|---|---|
| Date |<pre>→Wed, 05 Apr 2017 21:33:41 GMT</pre> |
| Server |<pre>→Apache-Coyote/1.1</pre> |

**Response Body Example:** N/A

## Examples of Event Payloads

The payload that a user receives varies depending on the object type, but there is a consistent format for which those varying payloads are delivered.

For example, the following properties remain consistent across all event payloads:

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Although consistent in format, the values contained within the properties vary between different objects and object types.

Samples of payloads for an UPDATE event and a CREATE event are shown below. Notice in the UPDATE example the oldState and newState objects are the same, while in the CREATE example the oldState object is empty (not NULL).

The following is an example payload for an UPDATE event:

[Copy](javascript:void(0);) 
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"eventType"</span>: <span style="color: #dd1144; ">"UPDATE"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"subscriptionId"</span>: <span style="color: #dd1144; ">"8a0d839d5ef32c9a015ef336a5ed0002"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"eventTime"</span>: {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"nano"</span>: <span style="color: #008080; ">998000000</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"epochSecond"</span>: <span style="color: #008080; ">1507319336</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"newState"</span>: {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"ID"</span>: <span style="color: #dd1144; ">"59d7ddf7000002322d791eb08bafddfb"</span>,&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"name"</span>: <span style="color: #dd1144; ">"EventSub Test updated"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"objCode"</span>: <span style="color: #dd1144; ">"PROJ"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"entryDate"</span>: <span style="color: #dd1144; ">"2017-10-06T13:48:07.776-0600"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"accessorIDs"</span>: [<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"544820df0000142362741fc0c368de19"</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;],<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"lastUpdateDate"</span>: <span style="color: #dd1144; ">"2017-10-06T13:48:56.980-0600"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"groupID"</span>: <span style="color: #dd1144; ">"544820df0000140f6a9c1faa7cacadd3"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"sponsorID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"description"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"plannedCompletionDate"</span>: <span style="color: #dd1144; ">"2017-10-06T09:00:00.000-0600"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"enteredByID"</span>: <span style="color: #dd1144; ">"544820df0000142362741fc0c368de19"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"ownerID"</span>: <span style="color: #dd1144; ">"544820df0000142362741fc0c368de19"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"templateID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"priority"</span>: <span style="color: #008080; ">0</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"companyID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"portfolioID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"referenceNumber"</span>: <span style="color: #008080; ">1894</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"lastUpdatedByID"</span>: <span style="color: #dd1144; ">"544820df0000142362741fc0c368de19"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"customerID"</span>: <span style="color: #dd1144; ">"544820df0000135b7719dcca654391f6"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"currency"</span>: <span style="color: #008080; ">null</span>,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"categoryID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"status"</span>: <span style="color: #dd1144; ">"CUR"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"parameterValues"</span>: {}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"oldState"</span>: {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"ID"</span>: <span style="color: #dd1144; ">"59d7ddf7000002322d791eb08bafddfb"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"name"</span>: <span style="color: #dd1144; ">"EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"objCode"</span>: <span style="color: #dd1144; ">"PROJ"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"entryDate"</span>: <span style="color: #dd1144; ">"2017-10-06T13:48:07.776-0600"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"accessorIDs"</span>: [<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"544820df0000142362741fc0c368de19"</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;],<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"lastUpdateDate"</span>: <span style="color: #dd1144; ">"2017-10-06T13:48:07.792-0600"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"groupID"</span>: <span style="color: #dd1144; ">"544820df0000140f6a9c1faa7cacadd3"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"sponsorID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"description"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"plannedCompletionDate"</span>: <span style="color: #dd1144; ">"2017-10-06T09:00:00.000-0600"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"enteredByID"</span>: <span style="color: #dd1144; ">"544820df0000142362741fc0c368de19"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"ownerID"</span>: <span style="color: #dd1144; ">"544820df0000142362741fc0c368de19"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"templateID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"priority"</span>: <span style="color: #008080; ">0</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"companyID"</span>: <span style="color: #008080; ">null</span>,<<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"portfolioID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"referenceNumber"</span>: <span style="color: #008080; ">1894</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"lastUpdatedByID"</span>: <span style="color: #dd1144; ">"544820df0000142362741fc0c368de19"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"customerID"</span>: <span style="color: #dd1144; ">"544820df0000135b7719dcca654391f6"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"currency"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"categoryID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"status"</span>: <span style="color: #dd1144; ">"CUR"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"parameterValues"</span>: {}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</code></pre>Following is an example payload for a CREATE event:

[Copy](javascript:void(0);) 
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"eventType"</span>: <span style="color: #dd1144; ">"CREATE"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"subscriptionId"</span>: <span style="color: #dd1144; ">"4028e3815ebf03a7015ebfa53b6d0002"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"eventTime"</span>: {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"nano"</span>: <span style="color: #008080; ">232000000</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"epochSecond"</span>: <span style="color: #008080; ">1506453831</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"newState"</span>: {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"ID"</span>: <span style="color: #dd1144; ">"59caa946000000e07b0afc3383230c67"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"name"</span>: <span style="color: #dd1144; ">"EventSub Test fe16d470-0a40-4290-92f4-6a0389fb536c"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"objCode"</span>: <span style="color: #dd1144; ">"PROJ"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"entryDate"</span>: <span style="color: #dd1144; ">"2017-09-26T13:23:50.746-0600"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"accessorIDs"</span>: [<span style="color: #dd1144; ">"544820df0000142362741fc0c368de19"</span>],<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"lastUpdateDate"</span>: <span style="color: #dd1144; ">"2017-09-26T13:23:50.927-0600"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"groupID"</span>: <span style="color: #dd1144; ">"544820df0000140f6a9c1faa7cacadd3"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"sponsorID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"description"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"plannedCompletionDate"</span>: <span style="color: #dd1144; ">"2017-09-26T09:00:00.000-0600"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"enteredByID"</span>: <span style="color: #dd1144; ">"544820df0000142362741fc0c368de19"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"ownerID"</span>: <span style="color: #dd1144; ">"544820df0000142362741fc0c368de19"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"templateID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"priority"</span>: <span style="color: #008080; ">0</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"companyID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"portfolioID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"referenceNumber"</span>: <span style="color: #008080; ">1750</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"lastUpdatedByID"</span>: <span style="color: #dd1144; ">"544820df0000142362741fc0c368de19"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"customerID"</span>: <span style="color: #dd1144; ">"544820df0000135b7719dcca654391f6"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"currency"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"categoryID"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"status"</span>: <span style="color: #dd1144; ">"CUR"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"parameterValues"</span>: {}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"oldState"</span>: {}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}</code></pre>

## Base 64 Encoding

If an event subscription is being rejected because of a conflict between special characters contained in your event subscriptions and your network settings, then you can use Base64 encoding to pass your event subscriptions. Base64 is a set of encoding schemes that can translate any arbitrary data into an ASCII&nbsp;string format. It is important to note that Base64 is not a form of security encryption.

### Base 64 Encoding Field

The base64Encoding field is an optional field that is used to enable Base64 encoding of event subscription payloads. The default value is false and the possible values are: true, false, and " " (blank).

### Example of a request using the base64Encoding field

If a request is made using the base64Encoding field set to true, then the **newState** and **oldState** objects in the payload are delivered as base 64 encoding strings. If the base64Encoding field is set to false, left blank, or not included in the request, then the returned payload will not be encoded in base 64.

The following is an example of a request that uses the base64Encoding field:

[Copy](javascript:void(0);) 
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"objCode"</span>: <span style="color: #dd1144; ">"PROJ"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"eventType"</span>: <span style="color: #dd1144; ">"UPDATE"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"url"</span>: <span style="color: #dd1144; ">"http://requestb.in/ua5hi2ua"",</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"authToken"</span>: <span style="color: #dd1144; ">"EauthTokenWorkfrontRocks1234_"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"base64Encoding"</span>: <span style="color: #dd1144; ">"true"</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}</code></pre>

### Examples of response payloads in base 64 encoding

[Copy](javascript:void(0);) 
<pre><code><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"eventType"</span>: <span style="color: #dd1144; ">"UPDATE"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"subscriptionId"</span>: <span style="color: #dd1144; ">"8a0d839d5ef32c9a015ef336a5ed0002"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"eventTime"</span>: {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"nano"</span>: <span style="color: #008080; ">998000000</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"epochSecond"</span>: <span style="color: #008080; ">1507319336</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"newState"</span>: <span style="color: #dd1144; ">"ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"oldState"</span>: <span style="color: #dd1144; ">"ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</code></pre>

## Deprecated Method for Querying All Event Subscriptions

The following API endpoint is deprecated and should not be used for new implementations. We also recommend transitioning old implementations to the method in the **Querying Event Subscriptions** section described above.

You can query all event subscriptions for a customer as specified by the apiKey value. The request syntax for listing all event subscriptions for a specific customer is the following URL:

[Copy](javascript:void(0);) 
<pre><code>[GET] https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list</code></pre>**Request Headers:** 

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header Name</p> </th> 
   <th> <p>Header Value</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Authorization</p> </td> 
   <td> <p> User’s apiKey </p> </td> 
  </tr> 
 </tbody> 
</table>

**Response Codes:** 

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Response Code</p> </th> 
   <th>&nbsp;Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (No Content)</td> 
   <td>The request successfully returned all event subscriptions found for user.</td> 
  </tr> 
  <tr> 
   <td>401 (Unauthorized)</td> 
   <td>The apiKey provided was empty.</td> 
  </tr> 
  <tr> 
   <td>403 (Forbidden)</td> 
   <td>The User which matches the provided apiKey does not have administrator access.</td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

### Response Body Example

[Copy](javascript:void(0);) 
<pre><code><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"id"</span>: <span style="color: #dd1144; ">"37c4bcf5-e0b5-4256-aba3-a51cba7bf997"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"customer_id"</span>: <span style="color: #dd1144; ">"504f9640000013401be513579fbebffa"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"obj_id"</span>: <span style="color: #dd1144; ">"ObjId1234"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"obj_code"</span>: <span style="color: #dd1144; ">"TASK"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"url"</span>: <span style="color: #dd1144; ">"http://test.test.net/test/1234"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"event_type"</span>: <span style="color: #dd1144; ">"UPDATE"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"auth_token"</span>: <span style="color: #dd1144; ">"auth_token"</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"id"</span>: <span style="color: #dd1144; ">"750a636c-5628-48f5-ba26-26b7ce537ac2"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"customer_d"</span>: <span style="color: #dd1144; ">"504f9640000013401be513579fbebffa"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"obj_id"</span>: <span style="color: #008080; ">null</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"obj_code"</span>: <span style="color: #dd1144; ">"PROJ"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"url"</span>: <span style="color: #dd1144; ">"http://requestb.in/ua5hi2ua"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"event_type"</span>: <span style="color: #dd1144; ">"UPDATE"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"auth_token"</span>: <span style="color: #dd1144; ">"authTokenWorkfrontRocks1234_"</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;]<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</code></pre>