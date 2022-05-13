---
filename: api-changes-search
content-type: api
keywords: object,status,search,best,practice,response
navigation-topic: api-navigation-topic
title: "Core API changes: Status search responses"
description: Changes have been made to the way that Workfront stores status objects. These changes do not affect how status search requests are made, but will affect the response returned by API requests that include a search for status objects by returning an incomplete list of group statuses.
---

# Core API&nbsp;changes: Status search responses

Changes have been made to the way that Workfront stores status objects. These changes do not affect how status search requests are made, but will affect the response returned by API requests that include a search for status objects by returning an incomplete list of group statuses.

## Best practices

In order to reliably fetch the full list of statuses available for a group, the following requests are considered best practices.

>[!NOTE]
>
>These request structures are recommended for all users regardless of whether or not the status search changes have been made to your cluster.

For Project Group Status:

**Example:** `/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d`

For Task Group Status:

**Example:** `/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d`

For Issue Group Status:

**Example:** `/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d`

All three of these endpoints accept the **includeHidden=true** parameter in order to fetch the hidden project/task/issue statuses of a given group. Modeling your status search queries after these best practice examples will ensure that all group-status information is included with each response.

Here is an example of a status search query being made to a task group that includes a system-level locked status **Custom_1** and an unlocked status **Custom_2**:

**Example:** `/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868`

Using this format ensures that your response will include all of the following:

[Copy](javascript:void(0);) 

<!--WRITER - fix code throughout this doc. for Bob-->

```
<code>{<br>&nbsp;&nbsp;"data": [<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color": "1C68FF",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"equatesWith": "NEW",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"groupID": "602d27640000bb3b779f770d5fb95d6d",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"label": "New",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"objCode": "CSTEM",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"value": "NEW"<br>&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color": "39FF39",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"equatesWith": "INP",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"groupID": "602d27640000bb3b779f770d5fb95d6d",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"label": "In Progress",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"objCode": "CSTEM",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"value": "INP"<br>&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color": "FF3939",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"equatesWith": "CPL",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"groupID": "602d27640000bb3b779f770d5fb95d6d",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"label": "Complete",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"objCode": "CSTEM",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"value": "CPL"<br>&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color": "8BC34A",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"equatesWith": "NEW",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"groupID": "602d27640000bb3b779f770d5fb95d6d",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"label": "Custom_1",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"objCode": "CSTEM",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"value": "JET"<br>&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color": "8BC34A",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"equatesWith": "NEW",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"groupID": "602d27640000bb3b779f770d5fb95d6d",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"label": "Custom_2",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"objCode": "CSTEM",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"value": "OGC"<br>&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;]<br>}</code>
```

## Understanding changes made to the legacy status search query

Under the legacy system a status search query would copy all of the system statuses available for all of the groups included in a query. The legacy response would then include all of the system statuses and group-level statuses available for each the group in query.

For example, this query (which does not follow the current recommended best practices):

**Example:**`/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK`

Would have the following response under the legacy system, which includes all object statuses:

[Copy](javascript:void(0);) 

```
<code>{<br>&nbsp;&nbsp;"data": [<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color": "1C68FF",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"equatesWith": "NEW",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"groupID": "602d27640000bb3b779f770d5fb95d6d",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"label": "New",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"objCode": "CSTEM",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"value": "NEW"<br>&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color": "39FF39",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"equatesWith": "INP",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"groupID": "602d27640000bb3b779f770d5fb95d6d",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"label": "In Progress",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"objCode": "CSTEM",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"value": "INP"<br>&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color": "FF3939",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"equatesWith": "CPL",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"groupID": "602d27640000bb3b779f770d5fb95d6d",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"label": "Complete",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"objCode": "CSTEM",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"value": "CPL"<br>&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color": "8BC34A",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"equatesWith": "NEW",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"groupID": "602d27640000bb3b779f770d5fb95d6d",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"label": "Custom_1",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"objCode": "CSTEM",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"value": "JET"<br>&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color": "8BC34A",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"equatesWith": "NEW",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"groupID": "602d27640000bb3b779f770d5fb95d6d",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"label": "Custom_2",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"objCode": "CSTEM",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"value": "OGC"<br>&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;]<br>}</code>
```

However, following the updates made to the way that statuses are stored and used, statuses do not copy for groups and are inherited by each group at the system level. As a result, the search API query only reads those statuses which are directly associated with a particular group, so the response includes system-locked and unlocked statuses, but only for those groups that were created after the status in question was added.

Failing to use the updated best practice methods to make status search queries after the legacy system has been updated will result in an incomplete list of group statuses being returned in the response.

Here is an example of what this outdated request structure returns after the legacy system has been updated:

**Example:** `/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK`

Notice that this response includes only group-specific statuses and leaves out those statuses which were declared at system-level:

```
[Copy](javascript:void(0);) 
<code>{<br>&nbsp;&nbsp;<span style="color: #dd1144; ">"data"</span>: [<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"color"</span>: <span style="color: #dd1144; ">"8BC34A"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"equatesWith"</span>: <span style="color: #dd1144; ">"NEW"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"groupID"</span>: <span style="color: #dd1144; ">"602d286d000004fc8f53942de697a868"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"label"</span>: <span style="color: #dd1144; ">"Custom_2"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"objCode"</span>: <span style="color: #dd1144; ">"CSTEM"</span>,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #dd1144; ">"value"</span>: <span style="color: #dd1144; ">"MMI"</span><br>&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;]<br>}</code>
```