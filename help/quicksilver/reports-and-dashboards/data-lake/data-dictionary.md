---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Data Lake data dictionary
description: This page contains information about the structure and content of the data in Workfront data lake.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
---
# Workfront data lake data dictionary

This page contains information about the structure and content of the data in Workfront data lake. 

>[!NOTE]
>
>The data in Workfront data lake refreshes every four hours, so recent changes may not be immediately reflected.

## Table types

There are a number of table types you can utilize to view your Workfront data in a way that provides the most insight.

### Current table

The Current table reflects data similarly to how it exists in Workfront, every object and its current state. However, it can be navigated with much lower latency than within Workfront.

### Event table

The Event table tracks every change record in Workfront: that is, every time an object changes state, a record is created that shows when the change happened, who made the change, and what was changed. Therefore, this table is useful for point-in-time comparisons. This table only includes records from the past three years. 

### Daily History table

The Daily History table offers an abbreviated version of the Event table, in that it shows the state of each object on a daily basis rather than when each individual event occurred. As such, this table is useful for trend analysis.

<!-- Custom table -->

## Terminology table

The following table correlates the object names in Workfront (as well as their names in the interface and API) with their equivalent name in the data lake.

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
    <td>ASSIGNMENTS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ASSIGNMENTS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>Condition, Priority, Severity,&nbsp;&nbsp;&nbsp;Status</td>
    <td>CSTEM | Custom Enum</td>
    <td>CUSTOMENUMS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CUSTOMENUMS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CUSTOMENUMS_EVENT</td>
    <td>The type of record is identified&nbsp;&nbsp;&nbsp;through the `enumClass` property. The following are the expected types:<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CONDITION_OPTASK<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CONDITION_PROJ<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CONDITION_TASK<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PRIORITY_OPTASK<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PRIORITY_PROJ<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PRIORITY_TASK<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;SEVERITY_OPTASK<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;STATUS_OPTASK<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;STATUS_PROJ<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;STATUS_TASK</td>
  </tr>
  <tr>
    <td>Document</td>
    <td>Document</td>
    <td>DOCU | Document</td>
    <td>DOCUMENTS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;DOCUMENTS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;DOCUMENTS_EVENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;DOCUMENTS_CUSTOM_VALUE_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>DocumentVersion</td>
    <td>Document Version</td>
    <td>DOCV | Document Version</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;DOCUMENTVERSIONS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Group</td>
    <td>Group</td>
    <td>GROUP | Group</td>
    <td>GROUPS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;GROUPS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Hour</td>
    <td>Hour</td>
    <td>HOUR | Hour</td>
    <td>HOURS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HOURS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HOURS_EVENT</td>
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
    <td>MILESTONES_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MILESTONES_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MILESTONES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>MilestonePath</td>
    <td>Milestone Path</td>
    <td>MPATH | Milestone Path</td>
    <td>MILESTONEPATHS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MILESTONEPATHS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Note</td>
    <td>Note</td>
    <td>NOTE | Note</td>
    <td>NOTES_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;NOTES_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>Issue, Request</td>
    <td>OPTASK | Issue</td>
    <td>OPTASKS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;OPTASKS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;OPTASKS_EVENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;OPTASKS_CUSTOM_VALUE_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Portfolio</td>
    <td>Portfolio</td>
    <td>PORT | Portfolio</td>
    <td>PORTFOLIOS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PORTFOLIOS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PORTFOLIOS_EVENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PORTFOLIOS_CUSTOM_VALUE_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PORTFOLIOS_CUSTOM_VALUE_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PORTFOLIOS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Program</td>
    <td>Program</td>
    <td>PRGM | Program</td>
    <td>PROGRAMS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PROGRAMS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PROGRAMS_EVENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PROGRAMS_CUSTOM_VALUE_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Project</td>
    <td>Project</td>
    <td>PROJ | Project</td>
    <td>PROJECTS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PROJECTS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PROJECTS_EVENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PROJECTS_CUSTOM_VALUE_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Role</td>
    <td>Job Role</td>
    <td>ROLE | Job Role</td>
    <td>ROLES_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ROLES_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Schedule</td>
    <td>Schedule</td>
    <td>SCHED | Schedule</td>
    <td>SCHEDULES_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;SCHEDULES_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Task</td>
    <td>Task</td>
    <td>TASK | Task</td>
    <td>TASKS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TASKS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TASKS_EVENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TASKS_CUSTOM_VALUE_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Team</td>
    <td>Team</td>
    <td>TEAMOB | Team</td>
    <td>TEAMS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TEAMS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Timesheet</td>
    <td>Timesheet</td>
    <td>TSHET | Timesheet</td>
    <td>TIMESHEETS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TIMESHEETS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>User</td>
    <td>User</td>
    <td>USER | User</td>
    <td>USERS_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;USERS_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;USERS_EVENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;USERS_CUSTOM_VALUE_CURRENT<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;USERS_CUSTOM_VALUE_DAILY_HISTORY<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
