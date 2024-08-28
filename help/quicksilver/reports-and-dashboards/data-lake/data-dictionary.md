---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect data dictionary
description: This page contains information about the structure and content of the data in Workfront Data Connect.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
---
# Workfront Data Connect data dictionary

This page contains information about the structure and content of the data in Workfront Data Connect. 

>[!NOTE]
>
>The data in Data Connect refreshes every four hours, so recent changes may not be immediately reflected.

## Table types

There are a number of table types you can utilize in Data Connect to view your Workfront data in a way that provides the most insight.

* **Current table**

  The Current table reflects data similarly to how it exists in Workfront, every object and its current state. However, it can be navigated with much lower latency than within Workfront.

* **Event table**

  The Event table tracks every change record in Workfront: that is, every time an object changes state, a record is created that shows when the change happened, who made the change, and what was changed. Therefore, this table is useful for point-in-time comparisons. This table only includes records from the past three years. 

* **Daily History table**

  The Daily History table offers an abbreviated version of the Event table, in that it shows the state of each object on a daily basis rather than when each individual event occurred. As such, this table is useful for trend analysis.

<!-- Custom table -->

## Entity relationship diagram

Objects in Workfront (and, therefore, in your Data Connect data lake) are defined not only by their individual values, but by their relationships with other objects. The entity relationship diagram below provides a high-level mapping of object relationships in Data Connect. The diagram can be viewed and downloaded using the following link:

[Data Connect entity relationship diagram](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>The entity relationship diagram is a work in progress—as such, it is for reference purposes only and is subject to change.

## Date types

There are a number of date objects that provide information about when specific events occur. 

* `DL_LOAD_TIMESTAMP`: This date is used for internal reference, and reflects when the data was loaded into the Current, Event, or Daily History table. This date should not be used for data analysis, and planned to be removed during the beta phase of Workfront data lake.
* `CALENDAR_DATE`: This date is present only in the Daily History table. This table provides a record of what the data looked like at 11:59 UTC for each date specified in `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP`: This date is present in both Event and Daily History tables, and records exactly when a record changed _to_ the value it has in the current row.
* `END_EFFECTIVE_TIMESTAMP`: This date is present in both Event and Daily History tables, and records exactly when a record changed _from_ the value in the current row to a value in a different row. To allow for between queries on `BEGIN_EFFECTIVE_TIMESTAMP` and `END_EFFECTIVE_TIMESTAMP` this is value is never null, even if there is no new value. In the event a record is still valid (i.e., the value has not changed), `END_EFFECTIVE_TIMESTAMP` will have a value of 2300-01-01.

## Terminology table

The following table correlates object names in Workfront (as well as their names in the interface and API) with their equivalent names in Data Connect.

<table>
<thead>
  <tr>
    <th>Workfront Entity Name</th>
    <th>Interface References</th>
    <th>API Reference | Label</th>
    <th>Data Lake Tables</th>
    <th>Notes</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Assignment</td>
    <td>Assignment</td>
    <td>ASSGN | Assignment</td>
    <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>Condition, Priority, Severity, Status</td>
    <td>CSTEM | Custom Enum</td>
    <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
    <td>The type of record is identified through the `enumClass` property. The following are the expected types:<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
  </tr>
  <tr>
    <td>Document</td>
    <td>Document</td>
    <td>DOCU | Document</td>
    <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br><br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>DocumentVersion</td>
    <td>Document Version</td>
    <td>DOCV | Document Version</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Group</td>
    <td>Group</td>
    <td>GROUP | Group</td>
    <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Hour</td>
    <td>Hour</td>
    <td>HOUR | Hour</td>
    <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Hour Type</td>
    <td>Hour Type</td>
    <td>HOURT | Hour Type</td>
    <td>HOURTYPES_CURRENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Milestone</td>
    <td>Milestone</td>
    <td>MILE | Milestone</td>
    <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>MilestonePath</td>
    <td>Milestone Path</td>
    <td>MPATH | Milestone Path</td>
    <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Note</td>
    <td>Note</td>
    <td>NOTE | Note</td>
    <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>Issue, Request</td>
    <td>OPTASK | Issue</td>
    <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br><br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Portfolio</td>
    <td>Portfolio</td>
    <td>PORT | Portfolio</td>
    <td>PORTFOLIOS_CURRENT<br>PORTFOLIOS_DAILY_HISTORY<br>PORTFOLIOS_EVENT<br><br>PORTFOLIOS_CUSTOM_VALUE_CURRENT<br>PORTFOLIOS_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIOS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Program</td>
    <td>Program</td>
    <td>PRGM | Program</td>
    <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br><br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Project</td>
    <td>Project</td>
    <td>PROJ | Project</td>
    <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br><br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Role</td>
    <td>Job Role</td>
    <td>ROLE | Job Role</td>
    <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Schedule</td>
    <td>Schedule</td>
    <td>SCHED | Schedule</td>
    <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Task</td>
    <td>Task</td>
    <td>TASK | Task</td>
    <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br><br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Team</td>
    <td>Team</td>
    <td>TEAMOB | Team</td>
    <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Timesheet</td>
    <td>Timesheet</td>
    <td>TSHET | Timesheet</td>
    <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>User</td>
    <td>User</td>
    <td>USER | User</td>
    <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br><br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
