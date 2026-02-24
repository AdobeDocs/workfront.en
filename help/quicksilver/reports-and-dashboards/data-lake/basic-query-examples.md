---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect query examples
description: Example queries you can use to familiarize yourself with the syntax and structure of specific kinds of queries.
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
---
# Workfront Data Connect query examples

To help you better utilize your Workfront Data Connect data, this page contains basic example queries you can use to familiarize yourself with the syntax and structure of specific kinds of queries.

## Custom data query

This example demonstrates how you can compose a query to return your custom data in Workfront, such as custom forms and custom fields. 

### Scenario

Your organization utilizes a custom form named Finance Integration. The form is attached to every project, and contains the following fields:

* **Business Unit**: A custom field that contains a string.
* **ProjectID**: A custom field that contains a numerical string.
* **Expanded Project Name**: A calculated custom data field that concatenates the values of Business Unit, ProjectID, and the native Workfront project name into a single string.

You need to include this information in the response for a query against Data Connect. Custom data values for a record in the data lake are contained in a column titled `parametervalues`. This column is stored as a JSON object.

### Query

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

### Response

The above query returns the following data:

* `projectid`: The native Workfront project ID.
* `parametervalues`: A column storing a JSON object.
* `name`: The native Workfront project name.
* `Business Unit`: A custom data value that is included in the `parametervalues` object.
* `Project ID`: A custom data value that is included in the `parametervalues` object.
* `Expanded Project Name`: A custom data value that is included in the `parametervalues` object.

### Explanation

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

## Time in status query 

This example demonstrates how to measure the time a project spent in previously assigned statuses. It can easily be adapted to measure task or issue time in a status, or it can be adapted to measure how long an object had any other attribute (including custom data values) applied to it. 

### Scenario

Your organization leadership believes you are spending too much time in each stage of your work lifecycle. Before making recommendations to improve the process, you want to create a baseline measurement of how often a project status changes over time and how many days a project stays in any given status. 

You're going to use the PROJECTS_EVENT data view to pull in a list of each status change against the project object. You'll compare the new status to the previous status, grab the effective time range for the previously assigned status, and then calculate the days spent in that status. 

Using this raw output of time spent in each status per project, you can start to build visualizations or aggregate the data further to build status duration averages by status, project type, or time of year. This baseline is then used to set a benchmark you can measure against to meet your leadership's expectations. 

The following query uses the Data Connect PROJECTS_EVENTS data view to compare each project status change event and display the time in status. 

### Query

```
-- Calculate the begin/end effective timestamp and duration in days 

SELECT 

    projectid, 
    name as project_name, 
    prev_status as previous_status, 
    status, 
    status_change_date as status_begin_effective_timestamp, 
    case 
        when status_change_date is null then NULL
        else
            nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp) 
    end as status_end_effective_timestamp, 
    datediff('DAYS',status_change_date, nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp)) as status_duration_days 

FROM 
    ( -- Filter to just the records that have changed 
     SELECT projectid, 
        name, 
        prev_status, 
        status, 
        begin_effective_timestamp as status_change_date    
     FROM 
        (  -- Calculate records where previous status is different 
          SELECT DISTINCT  
           pe.projectid, 
           pe.name AS name, 
           pe.STATUS, 
           nvl(lag(pe.STATUS) over (partition by pe.projectid order by pe.BEGIN_EFFECTIVE_TIMESTAMP), status) prev_status, 
           begin_effective_timestamp 

          FROM projects_event pe 
         -- Set any WHERE conditions to limit the results as needed 
         --WHERE 
            -- pe.PROJECTID = '5ebe…c1e1' 
        ) 
        WHERE prev_status != status 
    ) 
    order by status_change_date; 
```
 
### Response

The above query returns the following data: 

* `PROJECTID`: The Workfront project ID associated with the status change event. 
* `PROJECT_NAME`: The Workfront project name. 
* `PREVIOUS_STATUS`: The project's status immediately before the change. 
* `STATUS`: The project's status after the change. 
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP`: The change event timestamp when the previous status was set. 
* `STATUS_END_EFFECTIVE_TIMESTAMP`: The change event timestamp when the updated status value was set. 
* `STATUS_DURATION_DAYS`: The difference (in days) between the end effective timestamp and the begin effective timestamp. 

### Explanation

The query uses Data Connect's change event tracking capabilities.  It determines the date an event that had a new status value different from the previous event was triggered.  

Examining the query from the inside out:  

1. Calculate records where previous status is different:  
    * For every change event, use the lag() function to identify the previous value of status.  

2. Filter to just the records that have changed:  

    * Select records from calculation in step 1 where previous status != current status.  

3. Calculate the begin/end effective timestamp and duration in days:  

    * `<status_begin_effective_timestamp>`: Calculated in step 2.  

    * `<status_end_effective_timestamp>`: Calculated based on the next (lead()). `<status_begin_effective_timestamp>`: Only display the status if `<status_begin_effective_timestamp>` is NOT NULL.  
    * `<status_duration_days>`: Data difference between `<status_begin_effective_timestamp>` and `<status_end_effective_timestamp>`.  

>[!NOTE]
>
>It's recommended you use this query as its own "View" in PowerBI or Tableau.  If you want to bring in other fields from the `<object>_event view`, join the output from this query back to the `<object>_event view`.  The join fields would be the following:  <br>
>For projects_event:  
>`From projects_event p`
>`Join <above query> c on c.projectid = p.projectid  `
>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`

 

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
