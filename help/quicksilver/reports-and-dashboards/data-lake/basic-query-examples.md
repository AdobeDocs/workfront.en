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

Your organization utilizes a custom form named Finance Integration. The form is attached to every project, and contains the following fields:

* **Business Unit** - A custom field that contains a string.
* **ProjectID** - A custom field that contains a numerical string.
* **Expanded Project Name** - A calculated custom data field that concatenates the values of Business Unit, ProjectID, and the native Workfront project name into a single string.

You need to include this information in the response for a query against Data Connect. Custom data values for a record in the data lake are contained in a column titled `parametervalues`. This column is stored as a JSON object.

### Query:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Response:

The above query returns the following data:

* `projectid` - the native Workfront project ID
* `parametervalues` - a column storing a JSON object
* `name` - the native Workfront project name
* `Business Unit` - a custom data value that is included in the `parametervalues` object
* `Project ID` - a custom data value that is included in the `parametervalues` object
* `Expanded Project Name` - a custom data value that is included in the `parametervalues` object

### Explanation:

When querying the `parametervalues` JSON object, each custom data field can be accessed as a column using the following:

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` is the name of the JSON object in the table that is being queried. In the case of custom data, this will always be `parametervalues`.
* `<parameter_name>` is the `parametername` string found in the form configuration tool, although it may not always match this value.

>[!NOTE]
>
>If the name of the parameter is changed in the Workfront form configuration tool, it will be represented as a new column in the JSON object. As such, we recommended not changing the name of a column once it is created in the form configuration tool. However, the label may be changed without affecting the JSON object.
>
>If the text string for the parameter name is incorrect, the column will return a NULL value, rather than an error.

* `<data_type>` converts the value being returned from the JSON object into a data type appropriate for the field. Choosing an incompatible data type for the value being returned will result in a datatype mismatch error. Possible data types include:

    * `text`
    * `varchar`
    * `int`
    * `float`
    * `number(len,precision)` (e.g., `Number(32,4)` would return 1234.0987)
    * `date`
    * `timestamp`

* `<column_name>` is the label you create for each custom data column.

>[!NOTE]
>
>Only parameters that have values assigned to them in the form will be included in the JSON object. If a custom data field is empty on the form, it will not appear.

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
