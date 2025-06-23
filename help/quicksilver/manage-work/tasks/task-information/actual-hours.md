---
content-type: overview
product-area: projects
navigation-topic: task-information
title: View Actual Hours
description: The hours you log on your work items in Adobe Workfront are considered Actual Hours.
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

You must have the following access to perform the steps in this article:

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
</table>

*For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

 +++

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

### Actual Hours in the Hours section {#actual-hours-in-the-hours-section}

Finding Actual Hours in the Hours section is identical for projects, tasks, and issues.

To locate Actual Hours in Hours section:

1. Go to a task you want to review the Actual Hours for. 

1. In the left panel, click **Hours**. A list of hour entries logged on the task displays, with the **Hours** column showing the total number of Actual Hours for the task.

1. Ensure that the **Standard** view and the **Project** grouping are applied to this list.

### Actual Hours in reports {#actual-hours-in-reports}

When building tasks, issues, or projects reports, you can show the Actual Hours value for each task, issue, or project in the report.

To show Actual Hours in a task report:

{{step1-to-reports}}

1. On the **Reports** page, click **New Report**, then choose **Task** as your object.
1. In the bottom-right corner of the page, click **Add Column**.
1. In the **Show in this column** drop-down field that appears, start typing **Actual Hours**, then select the field when it appears in the list.

1. In the bottom-left corner of the page, click **Save + Close** to save the report.

1. In the **Name this Report to Save It** dialog box, enter a new report name, then click **Apply**.

### Actual Hours in Resource Management tools {#actual-hours-in-resource-management-tools}

If you want to see the progress of the work your users are doing on their assigned tasks and issues, you can view them in the following Resource Management tools:

* The Utilization Report.  
  For information, see [Overview of the Resource Utilization report](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* The Resource Planner.

  For information, see [View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).


### Actual Hours in the Workfront <!--database and the--> API <!--, and custom data-->

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

Most Workfront fields that store hours are saved in the Workfront database in minutes. For example, the name of the Planned Hours field of a task is `workRequired` in the Workfront database and it is stored in minutes. 

You must account for the conversion from minutes to hours when accessing these fields in API calls or in calculated custom fields or columns. 

Depending on how you are accessing Actual Hours, they can be stored in the following fields and units in the database: 

* In the API: With the following version of the Workfront API scheduled to release later in 2025, the `valuefield` for Actual Hours is `actualWorkRequiredDouble` which is stored in hours. The current version stored Actual Hours as `actualWorkRequired` which is stored in minutes. 
* In the Workfront interface (calculated custom field and columns): The `valuefield` for Actual Hours is `actualWorkRequired` which is stored in minutes.

<!--Change the above with this when we fix this for the Workfront UI: 

You must use the following valuefield name for Actual Hours in API calls or calculated custom fields or columns in Workfront: `actualWorkRequiredDouble`. -->

For information about using Actual Hours in calculated columns or fields, see [Report FAQs](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md). 

## Log time

You can log time on tasks, issues, and projects in multiple ways.

For more information, see [Log time](../../../timesheets/create-and-manage-timesheets/log-time.md).
