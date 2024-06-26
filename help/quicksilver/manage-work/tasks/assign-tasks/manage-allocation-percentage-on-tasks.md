---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Manage user or role allocation percentage on tasks
description: Allocation percentage represents the amount of time an assigned resource is planned to work on a task in a day. It is the percent of a work day (according to the user or project schedule) at which a resource is allocated throughout the duration of the task.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
---
# Manage user or role allocation percentage on tasks

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Allocation percentage represents the amount of time an assigned resource is planned to work on a task in a day. It is the percent of a work day (according to the user or project schedule) at which a resource is allocated throughout the duration of the task.

>[!NOTE]
>
>When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks and issues. For information about schedules, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
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
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the task</p> <p>Edit permissions to update allocation percentage in the Edit Task box</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations about modifying percent allocations for tasks

* Users are allocated an equal percentage of time to tasks they are assigned to, by default. 
* You can manually modify the allocation percentage for users and job roles assigned to tasks only when the Duration Type of the task is Calculated Work or Effort Driven.

  For information, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). 

* You cannot modify the percent allocation for teams assigned to tasks.
* You cannot modify the percentage allocation for users and job roles assigned to issues.

## Modify the user or role percent allocation for a task

1. Go to a task for whose resources you are changing the percent allocation.
1. Click the **More** menu ![](assets/qs-more-icon-on-an-object.png) next to the name of the task, then click **Edit**.

   Or

   Click the **Assignments** area in the task header, then click&nbsp;**Advanced**.

1. Ensure that the **Duration Type** of the task is one of the following:

   * Calculated Work
   * Effort Driven

   >[!TIP]
   >
   >* For the Calculated Assignment Duration Type, Workfront uses the following formula to calculate the allocation percentage of each assignee: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* For the Simple Duration Type, you can estimate the hours assigned to each resource, not the allocation percentage. 

1. Click **Assignments**, then modify the **Allocations** for each task assignee.

   You can only modify the allocation percentage for user and job role assignments.

   You cannot modify the allocation percentage for a team assigned to a task.

   Sample image in the Production environment:
   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

   <span class="preview">Sample image in the Preview environment:</span>
   ![Modify allocation percentage](assets/advanced-assignments-allocation-percentage.png)

1. Click **Save**.
