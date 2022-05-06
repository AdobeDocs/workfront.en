---
filename: critical-path
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Overview of the project Critical Path
description: Determining the Critical Path of a project is an automatic way for Adobe Workfront to flag a sequence of tasks in a project that have the potential to impact the timeline of the project. Tasks that can impact the timeline of the project are flagged as being Critical Path tasks.
---

# Overview of the project Critical Path

Determining the Critical Path of a project is an automatic way for Adobe Workfront to flag a sequence of tasks in a project that have the potential to impact the timeline of the project. Tasks that can impact the timeline of the project are flagged as being Critical Path tasks.

The following features can impact the Critical Path of a project:

* The Work Breakdown Structure of the project.

  For more information about Work Breakdown Structure, see [Determine Work Breakdown Structure in a project](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* The time (duration) that each task will take to complete.
* The dependencies between the tasks.

  Consider the following:

   * When a task on the Critical Path has a predecessor relationship, its predecessors and successors are also on the Critical Path if the changes on dates of the predecessors or the successors directly impact their dependents.

     >[!TIP]
     >
     >When the date of the successor of a task does not directly impact the date of their dependent tasks and it does not impact the dates of the project, the successor task is not on the Critical Path. 
     >
     >
     >![](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * When a subtask is identified as a Critical Path task, the parent task is also identified as a Critical Path task, if the Projected Start Date and time of the parent is the same as that of the subtask.

Taking these features into consideration, the system calculates the Critical Path by using the longest path between the earliest task and the task that determines the end of the project. The Critical Path Calculation takes into account what is the earliest and latest time that each task can start and finish by without making the project longer. This process determines which tasks are "critical" (and belong to the longest path) and which ones have "total float" (can be delayed without making the project longer).

Any delay in the activity of a task on the Critical Path directly impacts the Projected Completion Date of the project (there is no float on the critical path).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on a task </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## View the Critical Path

You can view the tasks that belong to the Critical Path in the following areas of the Workfront application:

* [View the Critical Path in the Gantt chart](#view-the-critical-path-in-the-gantt-chart) 
* [View the Critical Path in a task list or report](#view-the-critical-path-in-a-task-list-or-report)

### View the Critical Path in the Gantt chart {#view-the-critical-path-in-the-gantt-chart}

To view tasks on the Critical Path in the Gantt chart:

1. Go to a project for which you want to view the Critical Path.
1. Click **Tasks** in the left panel.
1. Click the **Gantt Chart** icon in the upper-right corner of the task list.

   ![gantt_chart_icon__1_.png](assets/gantt-chart-icon--1-.png)

1. Expand the **Options** menu, then enable the **Critical Path** option.

   The tasks that are on the Critical Path have a red line above their timeline in the Gantt chart.

   ![crtitical_path_on_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### View the Critical Path in a task list or report {#view-the-critical-path-in-a-task-list-or-report}

To view which tasks are on the critical path in a list of tasks:

1. Go to a project for which you want to view the Critical Path.
1. Click **Tasks** in the left panel. 
1. From the **View** drop-down menu, select **Status**.

   The tasks that are on the Critical Path have a **Critical Path** flag in the **Flags** column of the list.

   You can apply the same view to a task report.

   For more information about creating reports, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   Or

   From the **Filter** drop-down menu, select **New Filter**.

1. Click **Add Filter Rule** and start typing **Is Critical** in the **Only show me Tasks in which the ...** field. 

1. Select it when it appears in the list.
1. Click **Save Filter**.

   The list should only display tasks that are on the Critical Path.

