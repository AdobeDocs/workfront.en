---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overview of the Task Planned Completion Date
description: The Planned Completion Date of a task is the date by which the task is set to complete.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
---
# Overview of the task Planned Completion Date

The Planned Completion Date of a task is the date by which the task is set to complete. 

You can either specify the Planned Completion Date of a task, or you can leave it up to Adobe Workfront to calculate it depending on certain criteria. 

The Planned Completion Dates of tasks on a project determine the Planned Completion Date of a project when the project is scheduled from Start Date. For more information about the project Planned Completion Date, see [Set the project Planned Completion Date](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>The Planned Completion Date of a task differs from the Commit Date of the task or the Projected Completion Date of the task in the following ways:
>
>* The Commit Date is the date by which the person assigned to the task manually estimates that they will have completed the task. For more information see the following articles:
>
>   * [Commit Date overview](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md) 
>   * [Interactions between the Commit Date and the Planned Completion Date](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* The Projected Completion Date is a date calculated by Workfront and takes into account task delays, timelines of the task or their predecessors , and other factors to determine a real-life date for when the task can be realistically completed. For more information, see [Overview of the Projected Completion Date for projects, tasks, and issues](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Manually set the Planned Completion Date of a task

You must have Edit access to Tasks and Manage permissions on the task to be able to update the Planned Completion Date of the task.

Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task. 

You can manually set the Planned Completion Date in the following areas of Workfront:

* In the Edit Task box, when creating or editing a task. For information, see [Edit tasks](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* In the Task Details area. For information, see [Manage task information in the Task Details Overview area](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* In the Home area if the Planned Completion Date displays when viewing a task in the Summary panel. For information, see [Update or edit a work item in the Home area](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* In the task header. For information, see [New object headers](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In a task list or report when the Planned Completion Date field displays in the view.

  For information, see [Edit tasks in a list](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

You can manually specify the Planned Completion Date when you select any of the following Task Constraints: 

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
   <td> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td> 
   <td> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fixed Dates</p> </td> 
   <td> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td> 
  </tr> 
 </tbody> 
</table>

## How Workfront automatically calculates the Planned Completion Date for a task

When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:

* Task Constraint

  For more information about Task Constraints, see the article [Task Constraint overview](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Task predecessor relationship

  For more information about task predecessors, see the article [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Project Completion Date, when the project is scheduled from Completion Date.
* The time off schedule of the Primary Assignee of the task.

  When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the **Consider user time off in task durations** setting is selected for the **User Time Off** field. New projects inherit this setting from the Project Preferences area, but you can edit the setting at the project level.

  For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4.

  For information about the **User Time Off** preference, see the articles [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) or [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

* The amount of time associated with Approval Settings if the task is associated with an approval. For more information, see [Configure global approval settings](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

When set automatically, the Planned Completion Date is determined based on the following calculation: 

```
Planned Completion Date = Planned Start Date + Duration
```

For example, if your task has a start date of September 16 and a Duration of 10 days, the Planned Completion Date is September 26.

>[!NOTE]
>
> The Update Type for the project must be set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically adjusted.   
>For more information about the Update Type, see the article [Select the project Update Type](../../../manage-work/projects/manage-projects/select-project-update-type.md).
