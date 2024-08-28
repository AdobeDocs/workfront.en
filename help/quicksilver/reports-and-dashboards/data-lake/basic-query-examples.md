---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect query examples
description: Example queries you can use to familiarize yourself with the syntax and structure of specific kinds of queries.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
---
# Workfront Data Connect query examples

To help you better utilize your Workfront Data Connect data, this page contains basic example queries you can use to familiarize yourself with the syntax and structure of specific kinds of queries.

## Custom data query

This example demonstrates how you can compose a query to return your custom data in Workfront, such as custom forms and custom fields. 

### Scenario: 

Your organization, PeopleSoft, utilizes a custom form named Finance Integration. The form is attached to every project, and contains the following fields:

* **PeopleSoft Business Unit** - A custom field that contains a string.
* **PeopleSoft ProjectID** - A custom field that contains a numerical string.
* **Expanded Project Name** - A calculated custom data field that concatenates the values of PeopleSoft Business Unit, PeopleSoft ProjectID, and the native Workfront project name into a single string.

You need to include this information in the response for a query against Data Connect. Custom data values for a record in the data lake are contained in a column titled `parameterValues`. This column is stored as a JSON object.

### Query:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:PeopleSoft Business Unit" :: int as PeopleSoftBusinessUnit,
    parametervalues:"DE:PeopleSoft Project ID" :: int as PeopleSoftProjectID,
    parametervalues:"DE:Expanded Project Name" :: text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Response

The above query returns the following data:

* `projectid` - the native Workfront project ID
* `parametervalues` - a column storing a JSON object
* `name` - the native Workfront project name
* `PeopleSoft Business Unit` - a custom data value that is included in the `parametervalues` object
* `PeopleSoft Project ID` - a custom data value that is included in the `parametervalues` object
* `Expanded Project Name` - a custom data value that is included in the `parametervalues` object

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
