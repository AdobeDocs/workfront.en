---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overview of The task Planned Start Date
description: The Planned Start Date of a task is the date when you, as the task creator, decide that the work on the task should start. Planned task dates influence the dates and the timeline on the project. For information about the project Planned Start Date, see Overview of the project Planned Start Date.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
---
# Overview of the task Planned Start Date

<!-- Audited: 6/2025 -->

The Planned Start Date of a task is the date when you, as the task creator, decide that the work on the task should start. Planned task dates influence the dates and the timeline on the project. For information about the project Planned Start Date, see [Overview of the project Planned Start Date](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## The Planned Start Date of a task

You can either specify the task's Planned Start Date or you can leave it up to Adobe Workfront to calculate it depending on certain criteria.&nbsp;

* [Manually set the Planned Start Date of a task](#manually-set-the-planned-start-date-of-a-task) 
* [How the Planned Start Date is calculated for a task](#how-the-planned-start-date-is-calculated-for-a-task)

### Manually set the Planned Start Date of a task {#manually-set-the-planned-start-date-of-a-task}

Setting a task's Planned Start Date depends on the type of Task Constraint you assign to the task.&nbsp;

You can manually set the Planned Start Date&nbsp;when creating a task. For more information, see [Create tasks in a project](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

You can manually specify the Planned Start Date when you select any of the following Task Constraints:&nbsp;

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Task Constraint Type</strong> </p> </th> 
   <th> <p><strong>Effect of Manually Changing the Planned Completion Date</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Must Start On</p> <p>Start No Earlier Than</p> <p>Start No Later Than</p> </td> 
   <td> <p><span class="s1">The Planned Completion Date is adjusted in order to keep the Duration the same.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fixed Dates</p> </td> 
   <td> <p>The Duration is adjusted in order to keep the Planned Completion Date the same.</p> </td> 
  </tr> 
 </tbody> 
</table>

### How the Planned Start Date is calculated for a task {#how-the-planned-start-date-is-calculated-for-a-task}

When it is calculated automatically by the system, the following can influence the Planned Start Date of a task:

* The Start&nbsp;Date preference setting in the Tasks & Issues area in Setup

  Your Workfront or group administrator can determine whether a new task starts on the same date as the project's Planned Start&nbsp;Date or on the day you create the task.

  For information about Tasks &&nbsp;Issues preferences, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Task Constraint

  For more information about Task Constraints, see [Task Constraint overview](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Task predecessor relationship

  For more information about task predecessors, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Project Start Date, when the project is scheduled from Start Date.
* The time off schedule of the task's Primary&nbsp;Assignee.

  When the Primary Assignee has time off scheduled during the task duration, the planned dates of the task adjust accordingly when the Consider user time off in task durations setting is selected for the User Time Off field. New projects inherit this setting from the Project&nbsp;Preferences area, but you can edit the setting at the project level.

  For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 1 marked for time off, the task Planned Start Date becomes June 2.

  For information about the User Time Off preference, see  [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) or [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

When set automatically, the Planned Start Date&nbsp;is determined based on the following calculation:&nbsp;

```
Planned Start Date = Planned Completion Date - Task Duration
```

For example, if your task has a Completion Date of September 16 and a duration of 10 days, the Planned Start Date is September 6.

>[!NOTE]
>
>&nbsp;The Update Type for the project must also be&nbsp;set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically&nbsp;adjusted.   
>For more information about the Update Type, see [Select the project Update Type](../../../manage-work/projects/manage-projects/select-project-update-type.md).
