---
filename: api-changes-search
content-type: api
keywords: object,status,search,best,practice,response
navigation-topic: api-navigation-topic
title: 'Core API changes: Status search responses'
description: Changes in the way WorkFront stores status objects.
feature: Workfront API
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
---
# Core API changes: Status search responses

Changes have been made to the way that Workfront stores status objects. These changes do not affect how status search requests are made, but will affect the response returned by API requests that include a search for status objects by returning an incomplete list of group statuses.

## Best practices

In order to reliably fetch the full list of statuses available for a group, the following requests are considered best practices.

>[!NOTE] 
>
>These request structures are recommended for all users regardless of whether or not the status search changes have been made to your cluster.

For Project Group Status:

>**Example:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

For Task Group Status:

>**Example:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

For Issue Group Status:

>**Example:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

All three of these endpoints accept the **includeHidden=true** parameter in order to fetch the hidden project/task/issue statuses of a given group. Modeling your status search queries after these best practice examples will ensure that all group-status information is included with each response.

Here is an example of a status search query being made to a task group that includes a system-level locked status **Custom_1** and an unlocked status **Custom_2**:

>**Example:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

Using this format ensures that your response will include all of the following:

``` 
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

## Understanding changes made to the legacy status search query

Under the legacy system a status search query would copy all of the system statuses available for all of the groups included in a query. The legacy response would then include all of the system statuses and group-level statuses available for each the group in query.

For example, this query (which does not follow the current recommended best practices):

>**Example:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Would have the following response under the legacy system, which includes all object statuses:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

However, following the updates made to the way that statuses are stored and used, statuses do not copy for groups and are inherited by each group at the system level. As a result, the search API query only reads those statuses which are directly associated with a particular group, so the response includes system-locked and unlocked statuses, but only for those groups that were created after the status in question was added.

Failing to use the updated best practice methods to make status search queries after the legacy system has been updated will result in an incomplete list of group statuses being returned in the response.

Here is an example of what this outdated request structure returns after the legacy system has been updated:

>**Example:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Notice that this response includes only group-specific statuses and leaves out those statuses which were declared at system-level:

```
{
  "data": [
    {
      "color": "8BC34A",
      "equatesWith": "NEW",
      "groupID": "602d286d000004fc8f53942de697a868",
      "label": "Custom_2",
      "objCode": "CSTEM",
      "value": "MMI"
    }
  ]
}
```
