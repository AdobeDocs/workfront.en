---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect query examples
description: Example queries you can use to familiarize yourself with the syntax and structure of specific kinds of queries.
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/flDonZVaLR3bTF2aZcY9iy2ZnWbfrdhctL7J8esvxng
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
    internal-label: Measurement
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

## Planning: single record type query

This example demonstrates how to query Workfront Planning data for a single record type stored in the Data Connect data lake.

### Scenario

Your organization uses Workfront Planning to track Campaigns. Each Campaign record includes a name, status, start date, end date, and owner. You want to pull a list of all active campaigns and their key details for use in a dashboard.

* Planning record type data is stored in the PLANNINGRECORD_CURRENT view.
* Each row represents a single record, and all field values are stored in a JSON column named FIELD_VALUES.
* The record type is identified by the RECORDTYPEID column.
* The record's workspace is identified by the WORKSPACEID column (or the WORKSPACENAME column for a human-readable filter).

### Query

```sql
SELECT
  recordid,
  FIELD_VALUES:"Name"::text AS campaign_name,
  FIELD_VALUES:"Status"::text AS campaign_status,
  FIELD_VALUES:"Start Date"::date AS start_date,
  FIELD_VALUES:"End Date"::date AS end_date,
  FIELD_VALUES:"Owner"::text AS owner
FROM PLANNINGRECORD_CURRENT
WHERE WORKSPACEID = '<your_campaign_workspace_id>'
AND RECORDTYPEID = '<your_campaign_record_type_id>'
AND FIELD_VALUES:"Status"::text = 'Active'
ORDER BY start_date ASC
```

### Response

The above query returns the following data:

* **recordid**: The unique Planning record ID for the campaign.
* **campaign_name**: The name of the campaign, extracted from the FIELD_VALUES JSON object.
* **campaign_status**: The current status of the campaign.
* **start_date**: The campaign's start date, cast to a date data type.
* **end_date**: The campaign's end date, cast to a date data type.
* **owner**: The name of the user or team assigned as the campaign owner.

### Explanation

Planning records in Data Connect share a single table structure regardless of record type. The RECORDTYPEID column is used to scope the query to a specific record type — in this case, Campaigns. Replace `<your_campaign_record_type_id>` with the ID of the record type you want to query, which can be found in the Workfront Planning record type settings or by querying RECORDTYPE_CURRENT.

Field values are stored as a JSON object in the FIELD_VALUES column and are accessed using the same colon-notation syntax used for custom form data:

```
<field_column>:"<field_name>"::<data_type> AS <alias>
```

Field name references must match exactly the field name defined in the Planning record type field configuration, including capitalization, spacing and emoji.

>[!NOTE]
>
>Planning record type IDs can be found in the URL when viewing a record type in Workfront Planning. It is the path of the URL that begins with "Rt...". Record types can also be found with the following SQL call within Data Connect:
>
>
>```sql
>SELECT
>ID AS recordtypeid,
>DISPLAYNAME AS record_type_name,
>WORKSPACEID
>FROM RECORDTYPE_CURRENT
>ORDER BY record_type_name ASC
>```

## Planning: connected record types query

This example demonstrates how to query data across two connected Planning record types — a parent record type and a record type it is connected to.

### Scenario

Your organization connects Campaign records to Tactic records in Workfront Planning. You want to produce a report that shows each campaign alongside key details from its associated tactics. They specifically want to show the tactic name, strategic priority, and budget allocation so that leadership can review campaign activity organized by tactic.

In Data Connect, connections between native Planning record types are stored directly in the FIELD_VALUES_RAW column of PLANNINGRECORD_CURRENT. For a reference field named "Tactics", the value is a JSON array of connected record objects, each containing an id property with the connected record's RECORDID. Use Snowflake's LATERAL FLATTEN to expand this array into rows and join to the connected record type.

### Query

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  t.FIELD_VALUES:"Name"::text AS tactic_name,
  t.FIELD_VALUES:"Strategic Priority"::text AS strategic_priority,
  t.FIELD_VALUES:"Budget Allocation"::float AS budget_allocation
FROM PLANNINGRECORD_CURRENT c,
INNER JOIN REFERENCE_CURRENT R 
ON r.FROM_REFERENCEID = c.REFERENCE_IDS:"Tactics"::text
INNER JOIN PLANNINGRECORD_CURRENT t
-- Join to the Tactic record using the connected record ID from the array
ON t.RECORDID = r.TO_RECORDID
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
ORDER BY tactic_name, campaign_name
```

### Response

The above query returns the following data:

* **campaign_id**: The unique Planning record ID for the campaign.
* **campaign_name**: The name of the campaign record.
* **campaign_status**: The current status of the campaign.
* **tactic_name**: The name of the connected Tactic record.
* **strategic_priority**: The Strategic Priority field value from the connected Tactic record.
* **budget_allocation**: The Budget Allocation field value from the connected Tactic record, cast as a float.

### Explanation - Modified KP

Connections between native Planning record types are stored in a REFERENCE_CURRENT join table.  The REFERENCE_CURRENT join table is used for joins between RecordType.   When joining between RecordType, the TO_RECORDID field should be used. 

The REFERENCE_ID column in the PLANNINGRECORD view contains a list of all REFERENCEID fields that are applicable to that planning record. You can access the id by utilizing the same JSON notation as a field_value.  

```
<reference_ids>:"<reference_name>"::text

```

The REFERENCE_CURRENT view contains one or more records where the TO_RECORDID points to other planning `recordId` fields in the PLANNINGRECORD_* views.

To join another REFERENCE field to additional planning records the same pattern of joining to REFERENCE_CURRENT and the PLANNINGRECORD_* views would be added to the above query.


## Planning: record type joined to Workfront Workflow data query

This example demonstrates how to join a Workfront Planning record type to a native Workfront Workflow object — in this case, a Project — using Planning's native connection feature, which stores external object references in the REFERENCE_CURRENT view.

### Scenario

Your organization connects Campaign records in Workfront Planning to Workfront Projects using Planning's native connection feature. You want to produce a combined report showing campaign details alongside live execution data from the linked project — specifically the project's current Percent Complete, Planned Completion Date, and assigned Project Owner — so that campaign managers can track delivery progress without leaving their Planning workspace context.

### Query

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  conn.TO_EXTERNALID AS linked_project_id,
  p.name AS project_name,
  p.percentcomplete AS project_percent_complete,
  p.plannedcompletiondate AS project_planned_completion,
  p.ownerid AS project_owner_id,
  u.name AS project_owner_name
FROM WORKFRONT.PLANNING.PLANNINGRECORD_CURRENT c
-- Join to the references table to find Workfront Project connections
INNER JOIN WORKFRONT.PLANNING.REFERENCE_CURRENT conn
ON conn.REFERENCE_ID = c.REFERENCE_IDS:"ProjectId"::text
-- Join to the Workfront Projects table on the external ID
INNER JOIN WORKFRONT.WF.PROJECTS_CURRENT p
ON p.projectid = conn.TO_EXTERNALID
-- Join to Users to resolve the project owner name
LEFT JOIN WORKFRONT.WF.USERS_CURRENT u
ON u.userid = p.ownerid
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
AND p.completiontype != 'CPL' -- Exclude completed projects
ORDER BY campaign_name
```

### Response

The above query returns the following data:

* **campaign_id**: The unique Planning record ID for the campaign.
* **campaign_name**: The name of the campaign record.
* **campaign_status**: The current status of the campaign, from Planning.
* **linked_project_id**: The Workfront Project ID from REFERENCE_CURRENT.TO_EXTERNALID, identifying the connected Workfront Project.
* **project_name**: The native Workfront project name from PROJECTS_CURRENT.
* **project_percent_complete**: The project's current percent complete value.
* **project_planned_completion**: The planned completion date of the linked Workfront project.
* **project_owner_id**: The Workfront user ID of the project owner.
* **project_owner_name**: The display name of the project owner, resolved by joining to USERS_CURRENT.

### Explanation

Connections from a Planning record type to a native Workfront Workflow object are stored in REFERENCE_CURRENT. Each row in this view represents one directional link: TO_EXTERNALID holds the ID of the connected Workfront object. Rows representing Workfront connections are identified by `TO_EXTERNALCONNECTIONNAME = 'workfront'` and a TO_EXTERNALOBJECTNAME value that corresponds to the Workfront object type's API code — for example, PROJ for Projects.  

The REFERENCE_ID column in the PLANNINGRECORD tables contains a list of all REFERENCEID fields that are applicable to that record.  You can access the id by utilizing the same JSON notation as a field_value.  
A single REFERENCE_ID in the PLANNINGRECORD_CURRENT may contain one or more reference links in the REFERENCE_CURRENT table that link to objects of a specific object type in the Workfront table.

```
<reference_ids>:"<reference_name>"::text

```
Note that Planning views (PLANNINGRECORD_CURRENT, REFERENCE_CURRENT) reside in the WORKFRONT.PLANNING schema, while native Workfront Workflow views (PROJECTS_CURRENT, USERS_CURRENT, etc.) reside in the WORKFRONT.WF schema. Cross-schema joins require fully qualified table names.

The query performs three joins:

1. **Planning records to the references table:** REFERENCE_CURRENT is joined on `TO_RECORDID = c.RECORDID` to find all connections originating from each Campaign record. The filters on `TO_EXTERNALCONNECTIONNAME = 'workfront'` and `TO_EXTERNALOBJECTNAME = 'PROJ'` narrow the results to rows that represent connections to Workfront Projects specifically.
1. **References table to Workfront Projects:** TO_EXTERNALID holds the native Workfront projectid for the connected Project. This is joined directly to `PROJECTS_CURRENT.projectid` to retrieve live project data.
1. **Projects to Users:** A LEFT JOIN to USERS_CURRENT resolves the ownerid foreign key on the project to a human-readable name. A LEFT JOIN is used here so that projects with no assigned owner are still included in results.

>[!NOTE]
>
>When joining to tables that are external to Planning, DO NOT use the TO_RECORDID field in the query.  It is not needed when joining to external tables.
>
>This pattern can be applied to any Workfront Workflow object that Planning supports connecting to — such as Projects, Portfolios, or Programs — by changing the TO_EXTERNALOBJECTNAME filter to the appropriate object API code (for example, PORT for Portfolios or PRGM for Programs) and joining to the corresponding WORKFRONT.WF table. Refer to the Workfront Data Connect data dictionary for the correct table and ID column names for each object type.

To join another REFERENCE field to additional external records the same pattern of joining to REFERENCE_CURRENT and the Workfront Workflow views would be added to the above query.

External and Planningrecord values can be joined in the same query by joining multiple times to the REFERENCE_CURRENT table an using the appropriate join pattern.


<!--
## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.
-->
