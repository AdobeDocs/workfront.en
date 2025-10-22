---
content-type: overview
product-area: projects
navigation-topic: task-information
title: View Actual Hours
description: The hours you log on your work items in Adobe Workfront are considered Actual Hours. Actual Hours represent the actual time that it took you to complete a task, issue, or a project.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
---
# View Actual Hours

<!-- Audited: 5/2025 -->

The hours you log on your work items in Adobe Workfront are considered Actual Hours.

Actual Hours represent the actual time that it took you to complete a task, issue, or a project.

We recommend that hours should be logged on work items, which are tasks and issues. However, as a Workfront administrator, you can allow users to also log time on projects depending on your organization's workflows.

For more information about how to set up your system to allow users to log time on projects, see [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Standard<p>
   <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks, Projects, or Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a task, a project, or an issue</p></td> 
  </tr> 
 </tbody> 
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

 <!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks,&nbsp;Projects, or Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a task, a project, or an issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Actual Hours vs Legacy Actual Hours

Depending on what area of Workfront you access the actual hours from, they could refer to one of the following logged hours:

* In project, tasks, and issue reports and lists: 

  * **Actual Hours**: Hours logged for project, tasks, or issues after May 2021. They are stored in the Workfront database in hours and their valuefield is `actualWorkRequiredDouble`.
  * **Legacy Actual Hours**: Hours logged for projects, tasks, or issues any time, including before May 2021. They are stored in the Workfront database as minutes and their valuefield is `actualWorkRequired`. 
  
    >[!IMPORTANT]
    >
    >The Actual Cost of the project uses Legacy Actual Hours to calculate. 

* In the project, task, or issue Details area, actual hours could display in the following fields:

  * **Actual Hours**: In the Details tab, these are hours logged for projects, tasks, or issues after May 2021. They are stored in the Workfront database in hours and their valuefield is `actualWorkRequiredDouble`.
  * **Actual Hours**: In a project, task, or issue custom form, when they are accessed using a Native field reference custom field that references the Actual Hours native field. These are hours logged for projects, tasks, or issues after May 2021. They are stored in the Workfront database in hours and their valuefield is `actualWorkRequiredDouble`.

>[!NOTE]
>
>It is recommended to use the Actual Hours field whenever possible, because the Legacy Actual Hours field could display inaccurate hours due to the way that increments are rounded.

## Actual Hours on tasks and issues vs. Actual Hours on projects

The Actual Hours on tasks and issues represent the number of hours logged directly on the tasks and issues.

Actual Hours from children tasks roll up to the Actual Hours on the parent task. The following formula applies for the Actual Hours on a parent task:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Actual Hours for Projects represent a total of Actual Hours from all the project's tasks (including hours logged directly on parent tasks), all the project's issues, and the Actual Hours logged on the project itself.

The following formula applies for the Actual Hours on a project:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Find Actual Hours

Finding the value for Actual Hours for an item is identical for tasks, projects, and issues.

### Actual Hours in the Details section {#actual-hours-in-the-details-section}

Finding Actual Hours in the Details section is identical for projects, tasks, and issues.

To locate Actual Hours in Task Details:

1. Go to a task you want to review the Actual Hours for. 
1. In the left panel, click **Task Details**. The **Overview** section displays.
1. Locate the **Actual Hours** value in the **Working time** section. This is the total of hours logged on this task.
1. (Optional and conditional) If the Actual Hours native field reference was added to a project, task, or issue custom form, go to the custom form and locate the Actual Hours in the custom field. This is the total of hours logged for the object. 

### Actual Hours in the Hours section {#actual-hours-in-the-hours-section}

Finding Actual Hours in the Hours section is identical for projects, tasks, and issues.

To locate Actual Hours in the Hours section of a task:

1. Go to a task you want to review the Actual Hours for. 

1. In the left panel, click **Hours**. A list of hour entries logged on the task displays, with the **Hours** column showing the total number of Actual Hours for the task.

1. Ensure that the **Standard** view and the **Project** grouping are applied to this list.
1. The Actual Hours for the task displays in the grouping line for the **Actual Hours** column. 

### Actual Hours and Legacy Actual Hours in reports

When building tasks, issues, or projects reports, you can show the Actual Hours and the Legacy Actual Hour values for each task, issue, or project in the report.

For information about the difference between Actual Hours and Legacy Actual Hours see the section [Actual Hours vs Legacy Actual Hours](#actual-hours-vs-legacy-actual-hours) in this article. 

To show Actual Hours and Legacy Actual Hours in a task report:

{{step1-to-reports}}

1. On the **Reports** page, click **New Report**, then choose **Task** as your object.
1. In the bottom-right corner of the page, click **Add Column**.
1. In the **Show in this column** drop-down field, start typing **Actual Hours**, then select the field when it appears in the list.
1. Repeat the step above to add the **Legacy Actual Hours** field to the report.

1. In the bottom-left corner of the page, click **Save + Close** to save the report.

1. In the **Name this Report to Save It** dialog box, enter a new report name, then click **Apply**.
1. Repeat the same steps for a project or issue report. 

### Actual Hours in Resource Management tools {#actual-hours-in-resource-management-tools}

If you want to see the progress of the work your users are doing on their assigned tasks and issues, you can view them in the following Resource Management tools:

* The Utilization Report.  
  For information, see [Overview of the Resource Utilization report](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* The Resource Planner.

  For information, see [View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).


### Actual Hours in the Workfront  API

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

Most Workfront fields that store hours are saved in the Workfront database in minutes. For example, the name of the Planned Hours field of a task is `workRequired` in the Workfront database and it is stored in minutes. 

You must account for the conversion from minutes to hours when accessing these fields in API calls or in calculated custom fields or columns. 

The Actual Hours logged for projects, tasks, or issues are currently stored in the Workfront database as minutes and their valuefield is `actualWorkRequired`.

With the following version of the Workfront API scheduled to release later in 2025, Actual Hours are stored in the following fields and units in the database: 

* **Actual Hours**: Hours logged for project, tasks, or issues after May 2021. They are stored in the Workfront database in hours and their valuefield is `actualWorkRequiredDouble`.
* **Legacy Actual Hours**: Hours logged for projects, tasks, or issues any time, including before May 2021. They are stored in the Workfront database as minutes and their valuefield is `actualWorkRequired`.

For information about API versions, see [API versioning and support schedule](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

  >[!IMPORTANT]
  >
  >The Actual Cost of the project uses Legacy Actual Hours to calculate. 

  For information about using Actual Hours in calculated columns or fields, see [Report FAQs](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md). 

## Log time

You can log time on tasks, issues, and projects in multiple ways.

For more information, see [Log time](../../../timesheets/create-and-manage-timesheets/log-time.md).
