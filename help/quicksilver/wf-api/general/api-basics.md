---
content-type: api
navigation-topic: general-api
title: API basics
description: API basics
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
---

# API basics

The goal for the Adobe Workfront API is to simplify building integrations with Workfront by introducing a REST-ful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses and describes the approach taken by the Workfront API.

A familiarity with the Workfront schema will assist you in understanding the database relationships that can be utilized to pull data out of Workfront for integration purposes.

## Limits and Guidelines

To ensure consistent Workfront on-demand system performance, each customer is limited to 10 concurrent API threads. The Sandbox environment has the same limit in place, allowing customers and partners to accurately test API calls before releasing code to production.

For production, preview, and test drive environments end user requests have a maximum URI length of 8892 bytes because they're being routed through the Workfront CDN (Akamai). This limit only applies to URIs that are routed through the CDN.

>[!NOTE]
>
>this limit is not applicable to sandbox environments because sandbox environments are not routed through the CDN.

### Disclaimer

Any use of the API should be tested in the Workfront beta environment prior to being run in the production environment. If any customer uses the API for a process that Workfront reasonably believes to be burdensome to the on-demand software (i.e., the process causes a materially negative effect on the performance of the software for other customers), Workfront reserves the right to request that the customer discontinues that process. If the customer does not comply and the problem persists, Workfront reserves the right to terminate the process.

## Workfront API URL

For information about the URL that you will use to call the Workfront API, see [Domain format for Adobe Workfront API calls](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md).

## REST Basics

This section provides a high-level introduction of how to interact with the Workfront REST API for the following REST principles:

### Object URI

Each object in the system is given a unique URI consisting of the object type and the ID. The following examples show URIs describing three unique objects:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

The object type is case insensitive and can be either the abbreviated ObjCode (such as&nbsp;proj) or the alternate object name (project).

For a list of valid ObjCodes, see&nbsp; [API Explorer](../../wf-api/general/api-explorer.md).

### Operations

Objects are manipulated by sending an HTTP request to their unique URI. The operation to be performed is specified by the HTTP method.

The standard HTTP methods correspond to the following operations:

* **GET** - Retrieves an object by ID, searches for all objects by a query, runs reports, or executes named queries
* **POST** - Inserts a new object
* **PUT** - Edits an existing object
* **DELETE** - Deletes an object

In order to work around client deficiencies or protocol length limits, the method parameter can be used to override HTTP behavior. For example, a GET operation may be implemented by posting the following URI:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### Response

Each request is given a response in JSON format. The response has&nbsp;either a data attribute if the request was successful or an error attribute if there was a problem. For example, the request

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

returns a JSON response similar to the following:


<pre>{<br>&nbsp;&nbsp;&nbsp;&nbsp;"data": [<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"percentComplete": 0,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"status": "CUR",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"priority": 2,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"name": "Brand New Project",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;} <br>&nbsp;&nbsp;&nbsp;&nbsp;] <br>}</pre>

>[!NOTE]
>
>When executing a GET request through your browser's address bar, it is not necessary to include the sessionID as part of the request.

Special security has been added around PUT, POST, and DELETE requests. Any request that results in writing to or deleting from the database can only be executed if the **sessionID=abc123** is included in the URI. The following examples show how this would look for a DELETE request:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&method=delete&sessionID=abc123<br>GET /attask/api/v15.0/project/4c78...54d0?method=delete&sessionID=abc123</pre>

### Authentication

The API authenticates each request to ensure that the client has access to view or modify a requested object.

Authentication is performed by passing in a session ID which can be given using one the following methods:

#### Request Header Authentication

The preferred method of authentication is to pass a request header named SessionID containing the session token. This has the advantage of being safe against [Cross-site Request Forgery (CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) attacks and not interfering with the URI for caching purposes.

The following is an example of a request header:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Request Parameter Authentication

You can authenticate by passing a request parameter named sessionID, as shown in the following example:&nbsp;

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0?sessionID=abc1234
```

#### Cookie-Based Authentication

The API uses the same cookie-based authentication that is used by the web UI to the system. Where, if a client logs into Workfront using the web UI, any AJAX calls made from within the same browser uses the same authentication.

>[!NOTE]
>
>In order&nbsp;to protect against the possibility of CSRF (Cross Site Request Forgery) attacks, this method of authentication is only available for read-only operations.

## Login

>[!IMPORTANT]
>
>Workfront no longer recommends the use of the `/login` endpoint or API keys. Instead, use one of the following authentication methods:
>
>* Server authentication with JWT
>* User authentication with OAuth2
>
>For instructions on setting up these authentication methods, see [Create OAuth2 applications for Workfront integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>
>For instructions on using server authentication in Workfront, see [Configure and use your organization's custom OAuth 2 applications using JWT flow](../../wf-api/api/oauth-app-jwt-flow.md)
>
>For instructions on using user authentication in Workfront, see [Configure and use your organization's custom OAuth 2 applications using authorization code flow](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
>
>The procedure described in this section applies only to organizations that have not yet been onboarded to the Adobe Business Platform. Logging in to Workfront through the Workfront API is not available if your organization has been onboarded to the Adobe Business Platform.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Using a valid username and password, you can use the following request to obtain a session ID:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

This sets a cookie to authenticate future requests as well as return a JSON response with the newly created sessionID, the userID of the logged in user, and other session attributes.

>[!NOTE]
>
>If you have a designated API user who is also an administrator, Workfront strongly suggests you use an API Key to log in.

**Generating an API Key**

You can generate&nbsp;an API Key when you log into the system as that user, as shown in the following example:


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**Retrieving a Previously-Generated API Key**

You can also retrieve an API Key that has been previously generated for a particular user by running getApiKey:


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

You can then use this result to authenticate any API call by adding "apiKey" as a request parameter with this value in place of a sessionID or username and password. This is beneficial from a security perspective.

The following request is an example of retrieving data from a project using the apiKey:

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Invalidating an API Key**

If the apiKey value has been compromised, you can run "clearApiKey" which invalidates the current API Key, as shown in the following example:

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Once cleared, you can run getApiKey again to generate a new API Key.

### Logout

When a session is complete, you can use the following request to log the user out, preventing any further access with the sessionID.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

The sessionID to be logged out can be specified either as a cookie, request header, or request parameter.

To log out a user:

1. Navigate to your login screen, but do not log in.
1. Change the URL to /attask/api/v15.0/project/search.  
   Notice the page cannot be found.
1. Replace the word *search* with login?username=admin&password=user, substituting your username and password for *admin* and *user  
   *This session is stored in the browser as a cookie and does not need to be restated in each subsequent GET request.

1. Change the URL back to **/attask/api/v15.0/project/search**.
1. Notice the response provided.

You must always include the sessionID provided after login when performing PUT, POST, and DELETE requests.

## GET Behavior

Use the HTTP GET method to retrieve an object or multiple objects and to run reports.

### Retrieving Objects

You can enhance a search for objects using modifiers and filters.

#### Retrieving an Object Using the Object ID

If you know the ID of an object, you can retrieve the object by accessing its unique URI. For example, the request

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

returns a response similar to the following:

<pre>{<br>&nbsp;&nbsp;&nbsp;&nbsp;"percentComplete": 0,<br>&nbsp;&nbsp;&nbsp;&nbsp;"status": "CUR",<br>&nbsp;&nbsp;&nbsp;&nbsp;"priority": 2,<br>&nbsp;&nbsp;&nbsp;&nbsp;"name": "Brand New Project",<br>&nbsp;&nbsp;&nbsp;&nbsp;"ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


You can retrieve multiple objects in the same request by specifying the id request parameter and giving a comma-separated list of IDs, as shown in the following example:


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

Notice the /attask/api/v15.0/project?id=... request is the same as the `/attask/api/v15.0/project/...` request.

#### Retrieving an Object Using the URI

If you want to retrieve an object by criteria other than the ID, you can search for the URI.

For example, you can use the following request to return a list of all the projects in the system:

```
GET /attask/api/v15.0/project/search
```

You can specify filters using the request parameters as name-value pairs. For example, the following example shows a request that would find all current projects:

```
GET /attask/api/v15.0/project/search?status=CUR
```

The following request finds all the tasks that are not yet complete and that are assigned to a user named John.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### Using Search Modifiers

The following table lists some of the modifiers you can use with the Workfront API.

| **Modifier** |**Description** |**Example** |
|---|---|---|
| eq |returns results that are in the status of closed |<pre>...status=cls&status_Mod=eq...</pre> |
| ne |returns results that are not in the status of closed |<pre>...status=cls&status_Mod=ne...</pre> |
| gte |returns results that have a percent complete greater than&nbsp;or equal to 50 |<pre>...percentComplete=50&percentComplete_Mod=gte...</pre> |
| lte |returns results that have a percent complete less than or equal to 50 |<pre>...percentComplete=50&percentComplete_Mod=lte...</pre> |
| isnull |returns results where the description is Null |<pre>...description_Mod=isnull...</pre> |
| notnull |returns results where the description is not Null |<pre>...description_Mod=notnull...</pre> |
| contains |returns results where name contains "Workfront" |<pre>...name=Workfront&name_Mod=contains...</pre> |
| between |returns results that have an entry date within the last 7 days |<pre>...entryDate=$$TODAY-7d&entryDate_Range=$$TODAY&entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
>Search requests are case-sensitive. If you receive an error, ensure&nbsp;&nbsp;**_Mod** and **_Range** have the correct capitalization.

#### Using OR Statements

You can enhance a search by adding a parameter that includes "OR" as well as a number to indicate&nbsp;the level of a filter or series of filters.

An OR statement returns only records in the API call that meet the OR statement's filtering criteria. Filters are not implied across OR statement levels.

For example, if you want to filter for

* Tasks that have a name containing "Planning" OR
* Tasks in a portfolio named "FixedAssets" AND assigned to someone with a name containing "Steve" OR
* Tasks that have a parent task named "Final Task"

then use the following API call with its multiple OR statements:
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&name_Mod=contains<br>&OR:1:portfolio:name=FixedAssets<br>&OR:1:portfolio:name_Mod=eq<br>&OR:1:assignedTo:name=Steve<br>&OR:1:assignedTo:name_Mod=cicontains<br>&OR:2:parent:name=Final Task<br>&OR:2:parent:name_Mod=eq
</pre>

#### Using Filter Parameters

One potential pitfall with using URL parameters for search filters is that Workfront parses certain parameters before checking for different authentication methods (i.e., username, password, apiKey, cookie). When this happens the parameters are not used as filters in the call.&nbsp;

To avoid this problem, you can place these values in filter parameters with JSON formatting. For example, if you want to filter for the username testuser, instead of using&nbsp;
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>pass the URL parameter in a filter, as shown in the following example:
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### Using the Map Request Parameter

By default, the data returned from a search is a JSON array. Depending on&nbsp;your use case, it may be more efficient to get the result as a JSON object indexed by ID. This can be done by using the map request parameter. For example, the request&nbsp;
<pre>/attask/api/v15.0/task/search?map=true</pre>returns a response indexed by ID similar to the following:
<pre>{<br>&nbsp;&nbsp;&nbsp;&nbsp;"data": {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"4c9a97db0000000f13ee4446b9aead9b": {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"percentComplete": 0,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"status": "NEW",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"name": "first task",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"ID": "4c9a97db0000000f13ee4446b9aead9b",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"taskNumber": 1 <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"4ca28ba600002024cd49e75bd43cf601": {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"percentComplete": 0,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"status": "INP:A",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"name": "second task",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"ID": "4ca28ba600002024cd49e75bd43cf601",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"taskNumber": 2 <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;} <br>&nbsp;&nbsp;&nbsp;&nbsp;} <br>}</pre>

#### Using the Fields Request Parameter

By default, retrieving an object returns only the most commonly-used subset of fields.

You can use the fields request parameter to specify a comma-separated list of specific fields is returned. For example, the request
<pre>/attask/api/v15.0/task/search?fields=plannedStartDate,priority</pre>returns a response similar to the following:
<pre>{<br>&nbsp;&nbsp;&nbsp;&nbsp;"priority": 2,<br>&nbsp;&nbsp;&nbsp;&nbsp;"name": "first task",<br>&nbsp;&nbsp;&nbsp;&nbsp;"ID": "4c7c08fa0000002ff924e298ee148df4",<br>&nbsp;&nbsp;&nbsp;&nbsp;"plannedStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
>
>These field names are case-sensitive.

For a list of possible field references, see the&nbsp; [API Explorer](../../wf-api/general/api-explorer.md)

#### Searching for Nested Objects

You can search for nested objects. By default, nested objects are returned with only the name and ID. For instance to get all issues along with their owners, use the following request:
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>If more information is required, you can request a nested field using colon syntax. For example, the following request searches for all issues along with the owner's name, ID, title, and phone number
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>and returns the following:&nbsp;
<pre>{<br>&nbsp;&nbsp;&nbsp;&nbsp;"name": "an important issue",<br>&nbsp;&nbsp;&nbsp;&nbsp;"ID": "4c78285f00000908ea8cfd66e084939f",<br>&nbsp;&nbsp;&nbsp;&nbsp;"owner": {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"title": "Operations Specialist",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"phoneNumber": "555-1234",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"name": "Admin User",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"ID": "4c76ed7a0000054c172b2c2d9f7f81c3" <br>&nbsp;&nbsp;&nbsp;&nbsp;} <br>}</pre>

#### Retrieving Nested Collections

You can retrieve nested collections of objects. For example, to get a project with all its tasks, use the following request:
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>The following request gets task assignments:
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### Searching for Multiple Nested Fields

By default, only the name and ID of each task is returned, but additional nested fields can be specified with colon syntax. To view all available fields for a related object or collection, simply append a colon and asterisk to the object/collection reference.
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### Retrieving Custom Data

You can retrieve custom data fields using the prefix "DE:". For instance, to request a project with a parameter called "CustomText," use the following request:
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>which would return
<pre>{<br>&nbsp;&nbsp;&nbsp;&nbsp;"name": "custom data project",<br>&nbsp;&nbsp;&nbsp;&nbsp;"ID": "4c9a954f0000001afad0687d7b1b4e43",<br>&nbsp;&nbsp;&nbsp;&nbsp;"DE:CustomText": "task b" <br>}</pre>You can also retrieve all the custom data for an object by requesting the parameterValues field. For example,&nbsp;
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>returns similar data to the following:
<pre>{<br>&nbsp;&nbsp;&nbsp;&nbsp;"name": "custom data project",<br>&nbsp;&nbsp;&nbsp;&nbsp;"ID": "4c9a954f0000001afad0687d7b1b4e43",<br>&nbsp;&nbsp;&nbsp;&nbsp;parameterValues: { <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"DE:CustomText": "task b", <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"DE:CustomNumber": 1.4, <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"DE:CustomCheckBoxes": ["first", "second", "third"] <br>&nbsp;&nbsp;&nbsp;&nbsp;} <br>}</pre>

#### Using&nbsp;Named Queries

Some object types have named searches that are commonly executed and are available by appending the name of the query to the end of the object type URI. For example, the following request retrieves the work items (tasks and issues) to which the user is currently assigned:
<pre>/attask/api/v15.0/work/myWork</pre>Named queries support requesting the fields parameter to retrieve additional fields. Some named queries accept additional filters as well. For a list of allowable named queries an object, see the Action tab for the object in the&nbsp; [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

#### Using `Count`

You can use `count` to return the number of results that match your query. This can be useful when you don't need the data in the results. By returning only the count, the server can process the request more quickly and save bandwidth. For example, the request
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>returns the number of results in the following format:
<pre>{<br>&nbsp;&nbsp;&nbsp;&nbsp;"count": 3 <br>}</pre>Returning a count is a much smaller data transfer than if the full objects are returned. The syntax is identical to the search command.

### Requesting a Report

You can perform a report request, where only the aggregate of some field is desired with one or more groupings. As shown in the following example, the report syntax is the same as the syntax for the SOAP API:
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&hours_AggFunc=sum</pre>which returns the following result
<pre>{<br>&nbsp;&nbsp;&nbsp;&nbsp;"First Project": { <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sum_hours": 15 <br>&nbsp;&nbsp;&nbsp;&nbsp;}, <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Second Project": { <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sum_hours": 30 <br>&nbsp;&nbsp;&nbsp;&nbsp;} <br>}</pre>Adding the $$ROLLUP=true parameter includes a total at each grouping level:
<pre>{<br>&nbsp;&nbsp;&nbsp;&nbsp;"First Project": { <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sum_hours": 15 <br>&nbsp;&nbsp;&nbsp;&nbsp;}, <br>&nbsp;&nbsp;&nbsp;&nbsp;"Second Project": { <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sum_hours": 30 <br>&nbsp;&nbsp;&nbsp;&nbsp;}, <br>&nbsp;&nbsp;&nbsp;&nbsp;"$$ROLLUP": { <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sum_hours": 45 <br>&nbsp;&nbsp;&nbsp;&nbsp;} <br>}</pre>

### Sorting Query Results in the API

You can sort your results by any field if you append the following to your API call:

&entryDate_Sort=asc

For example, if you want to sort by task Planned Start Date, remove entryDate and replace it with plannedCompletionDate.

This works for most fields in Workfront.

### Considering Query Limits

When querying an object, special consideration should be taken concerning the relationship of related objects and search limitations.&nbsp;For example, as shown in the following table, a query for projects can return no more than 2,000 projects. These 2,000 projects are considered "primary objects." If you query for the Tasks field on the projects, the Tasks field, which is a collection, becomes a secondary object to the primary object Project. A query for the Tasks field can include thousands of tasks on projects. In total, the combined number of objects (projects and tasks) returned cannot exceed the maximum of 50,000.

To ensure optimum performance the following table shows the limitations placed&nbsp;on search requests.&nbsp;

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Query Result</th> 
   <th>Limitation</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">Default Number of Results</td> 
   <td>100</td> 
   <td> If no limit is specified in the query filter (i.e., $$LIMIT), the result can contain no more than 100 primary objects. <br>See <a href="#using-paginated-responses" class="MCXref xref">Using Paginated Responses</a> for instructions on how to override this limitation. </td> 
  </tr> 
  <tr> 
   <td>Max Number of Results</td> 
   <td>2,000</td> 
   <td>The query filter (i.e., $$LIMIT) can return no more than 2000 results. See "Paginated Responses" for more information.</td> 
  </tr> 
  <tr> 
   <td>Max Field Depth</td> 
   <td>4</td> 
   <td>When identifying the fields you wish to display, you cannot go more than four levels away from the object being queried.</td> 
  </tr> 
  <tr> 
   <td>Max Number of Objects</td> 
   <td>50,000</td> 
   <td>The result set cannot include 50000 primary and secondary objects.</td> 
  </tr> 
  <tr> 
   <td>Max Number of Fields</td> 
   <td nowrap>1,000,000</td> 
   <td>When the result set is fewer than 50000 objects, your results may include at most 1,000,000 fields.</td> 
  </tr> 
  <tr> 
   <td>Max Number of Batch Creates/Updates</td> 
   <td>100</td> 
   <td>The maximum batch create or update limit is 100.</td> 
  </tr> 
 </tbody> 
</table>

### Using Paginated Responses {#using-paginated-responses}

To override the Default Number of Results query limitation and allow 200 results, you can include the `$$LIMIT=200` filter in your query, as shown in the following example:
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>

To ensure reliability and performance for other tenants in the system, the maximum allowed results limit per query is 2000 objects. Attempting to specify a larger limit will result in an `IllegalArgumentException` error message.&nbsp;

Therefore, we recommend you consider using paginated responses for large datasets. To specify the first result that should be returned, add the `$$FIRST` filter. For example, the following request returns results 201-250 for a query:
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&$$LIMIT=50</pre>

Note that in the above example, `$$FIRST=200` returns the 201st result. `$$FIRST=0` would return the first result. It may help to think of the $$FIRST value as the number of results you want to skip before returning results.

To make sure your results are properly paginated, use a sorting parameter. This allows the results to be returned in the same order, so that the pagination does not repeat or skip results. For example, to sort using the object ID, use `ID_Sort=asc`.

### Creating an Access Rule

You can create an access rule to determine who can access to an object. The following are examples of access rules you can set:

To set a project so it is shared only with a user with ID "abc123" use the following request:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>Alternatively, to share only with a new person and keep existing permissions intact:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&accessorID=abc123&accessorObjCode=USER&coreAction=VIEW</pre>To retrieve the existing access rules:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## POST Behavior

POST inserts a new object. The syntax is identical to PUT, but with a few exceptions. Because the new object does not yet exist, it does not have an ID. For this reason, the URI does not include the ID.

### Creating an Object

The following is an example of a request to create a new project:
<pre>POST /attask/api/v15.0/project?name=New Project</pre>The response includes the newly-created project along with its new ID and any other fields specified.

### Copying an Object

Some objects support being copied. For these object types, it is possible to create new objects by posting with a copySourceID parameter. For example, the following request copies the given project and gives it a new name:

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Uploading Documents

You can upload documents through the following API URL: 
<pre>POST /attask/api/v15.0/upload</pre>The API expects the content type to be multipart/form-data. The parameter name for the file must be uploadedFile. The server returns the following JSON data:
<pre>{<br>&nbsp;&nbsp;&nbsp;&nbsp;"handle": "4c7c08fa0000002ff924e298ee148df4"<br>}</pre>You can use the handle and post to the following URL when creating a Workfront document:
<pre>POST /attask/api/v15.0/document?updates={<br>&nbsp;&nbsp;&nbsp;&nbsp;name: aFileName,<br>&nbsp;&nbsp;&nbsp;&nbsp;handle: abc...123, (handle from the file upload)<br>&nbsp;&nbsp;&nbsp;&nbsp;docObjCode: PROJ, (or TASK, OPTASK, etc)<br>&nbsp;&nbsp;&nbsp;&nbsp;objID: abc...123,<br>&nbsp;&nbsp;&nbsp;&nbsp;currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## PUT Behavior

PUT is used to update an existing object.

The response for a PUT is identical to a GET. In both cases, the server returns the new state of the object after the update. All rules used to alter a response to a GET request also work with PUT, such as specifying additional fields to be returned, custom data, and so on.

### Editing Objects

Updates to objects are always done by ID using the object's unique URI. Fields to be updated are specified as request parameters. For instance, to change the name of a project you could send a request similar to the following:
<pre>PUT /attask/api/v15.0/project/4c7...?name=New Project Name <br>PUT /attask/api/v15.0/project?id=4c7...&name=New Project Name</pre>Since update requires an ID, this operation will fail (without insertion) if the object does not exist on the server.

### Specifying JSON Edits

As shown in the following example, you can use the updates request parameter to specify the fields to be updated using JSON syntax:
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>{<br>&nbsp;&nbsp;&nbsp;&nbsp; name: "New Project Name", <br>&nbsp;&nbsp;&nbsp;&nbsp; status: "CUR", <br>&nbsp;&nbsp;&nbsp;&nbsp; ... <br>}</pre>

### Making Nested Updates

Some objects have privately-owned collections that can be updated. For example, the following example demonstrates how to overwrite the existing assignments for a given task:
<pre>PUT /attask/api/v15.0/task/4c7...?updates= <br>{<br>&nbsp;&nbsp;&nbsp;&nbsp;assignments: [ <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{ <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;assignedToID: "2222...54d0, <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;assignmentPercent: 50.0 <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},{ <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;roleID: "1111...54d0"<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;} <br>&nbsp;&nbsp;&nbsp;&nbsp;] <br>}</pre>

>[!NOTE]
>
>While updates made to the top level are sparse, updates to a collection or nested object completely replace the existing collection. To edit a single assignment on a task without affecting the objects, use PUT on the assignment rather than on the task.

The following example makes a project a public help desk queue. Note that the existing queue properties are replaced.
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>{ <br>&nbsp;&nbsp;&nbsp;&nbsp;queueDef: { <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isPublic: 1 <br>&nbsp;&nbsp;&nbsp;&nbsp;} <br>}</pre>

### Using the Action Request Parameter

Some objects support additional actions that can be performed in addition to simple edits. You can specify these actions using the action request parameter. For example, the following request recalculates the timeline for a given project:
<pre>PUT /attask/api/v15.0/project/4c7...?action=calculateTimeline<br><br>or<br><br>PUT /attask/api/v15.0/project/4c7.../calculateTimeline </pre>

### Moving Objects

The following demonstrates the syntax for moving a task from one project to another:
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>An example for each action type is provided here: (??)
<pre>PUT /attask/api/v15.0/project/1234/approveApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/recallApproval<br><br>PUT /attask/api/v15.0/project/1234/rejectApproval<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>Only the move action requires identifying additional attributes to specify the project where the work item is to be moved.

The following is an example of each action type:&nbsp;
<pre>PUT /attask/api/v15.0/project/1234?method=put&updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### Sharing Objects

The following example demonstrates the syntax for sharing a project with a team:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx&accessorObjCode=TEAMOB</pre>When editing an object, you can replace all access rules on an object by doing a PUT and sending updates similar to the following example:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEW'}]}</pre>The following example&nbsp;shows the syntax for moving a task from one project to another:
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>

## DELETE Behavior

DELETE removes an object. In every case, the URI may include the parameter force=true to cause the server to remove the specified data and its dependants. In the following example, a task is deleted by executing the HTTP DELETE method on a URI:
<pre>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## Bulk Updates

A bulk update statement updates multiple objects at the same time within a single API call. A bulk create API call is built similarly to a normal update call, as shown in the following examples:
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&method=POST&apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>which results in a return similar to the following:
<pre>data: [{<br>&nbsp;&nbsp;&nbsp;&nbsp;ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>&nbsp;&nbsp;&nbsp;&nbsp;name: "Test_Project_1",<br>&nbsp;&nbsp;&nbsp;&nbsp;objCode: "PROJ",<br>&nbsp;&nbsp;&nbsp;&nbsp;percentComplete: 0,<br>&nbsp;&nbsp;&nbsp;&nbsp;plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>&nbsp;&nbsp;&nbsp;&nbsp;plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>&nbsp;&nbsp;&nbsp;&nbsp;priority: 0,<br>&nbsp;&nbsp;&nbsp;&nbsp;projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>&nbsp;&nbsp;&nbsp;&nbsp;status: "CUR"<br>},<br>{<br>&nbsp;&nbsp;&nbsp;&nbsp;ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>&nbsp;&nbsp;&nbsp;&nbsp;name: "Test_Project_2",<br>&nbsp;&nbsp;&nbsp;&nbsp;objCode: "PROJ",<br>&nbsp;&nbsp;&nbsp;&nbsp;percentComplete: 0usi,<br>&nbsp;&nbsp;&nbsp;&nbsp;plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>&nbsp;&nbsp;&nbsp;&nbsp;plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>&nbsp;&nbsp;&nbsp;&nbsp;priority: 0,<br>&nbsp;&nbsp;&nbsp;&nbsp;projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>&nbsp;&nbsp;&nbsp;&nbsp;status: "CUR"<br>}]</pre>You also can do a bulk update similar to the following:
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>which results in a return similar to the following:
<pre>data: [ {<br>&nbsp;&nbsp;&nbsp;&nbsp; ID: "53ff8e15003b461d4560f7f65a440078",<br>&nbsp;&nbsp;&nbsp;&nbsp; name: "Test_Project_1_Edit",<br>&nbsp;&nbsp;&nbsp;&nbsp; objCode: "PROJ",<br>&nbsp;&nbsp;&nbsp;&nbsp; percentComplete: 0,<br>&nbsp;&nbsp;&nbsp;&nbsp; plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>&nbsp;&nbsp;&nbsp;&nbsp; plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>&nbsp;&nbsp;&nbsp;&nbsp; priority: 0,<br>&nbsp;&nbsp;&nbsp;&nbsp; projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>&nbsp;&nbsp;&nbsp;&nbsp; status: "CUR"<br>},<br>{<br>&nbsp;&nbsp;&nbsp;&nbsp;ID: "53ff8e19003b46238a58d303608de502",<br>&nbsp;&nbsp;&nbsp;&nbsp;name: "Test_Project_2_Edit",<br>&nbsp;&nbsp;&nbsp;&nbsp;objCode: "PROJ",<br>&nbsp;&nbsp;&nbsp;&nbsp;percentComplete: 0,<br>&nbsp;&nbsp;&nbsp;&nbsp;plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>&nbsp;&nbsp;&nbsp;&nbsp;plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>&nbsp;&nbsp;&nbsp;&nbsp;priority: 0,<br>&nbsp;&nbsp;&nbsp;&nbsp;projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>&nbsp;&nbsp;&nbsp;&nbsp;status: "CUR"<br>}]</pre>If you want all operations to happen in the same transaction, add "atomic=true" to your batch API call as a request parameter. This way, if any of the operations fail, all of the operations rolled back.

>[!NOTE]
>
>Atomic batch operations can only return "success: true" or an error.
