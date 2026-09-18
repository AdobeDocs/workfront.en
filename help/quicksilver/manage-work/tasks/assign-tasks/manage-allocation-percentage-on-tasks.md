---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Manage User or Role Allocation Percentage on Tasks
description: Allocation percentage represents the amount of time an assigned resource is planned to work on a task in a day. It is the percent of a work day (according to the user or project schedule) at which a resource is allocated throughout the duration of the task.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/tpBEkOgTsJSJ-dk-gKZ6uLyCk4j4vP4nMIQ5-ciHMAI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Manage user or role allocation percentage on tasks

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->


Allocation percentage represents the amount of time an assigned resource is planned to work on a task in a day. It is the percent of a work day (according to the user or project schedule) at which a resource is allocated throughout the duration of the task.

You can modify the allocation percentage when you make advanced assignments on a task. 

>[!NOTE]
>
>When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks and issues. For information about schedules, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td> <p>Standard</p>
   <p>Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>Edit access to Tasks</td> 
  </tr> 
  <tr> 
   <td>Object permissions</td>
   <td><p>Contribute or higher permissions to the task</p>
   <p>Edit permissions to update allocation percentage in the Edit Task box.</p>
   <!--
   Not true anymore: 
   <p><b>NOTE</b></p>
   <p> You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a>.</p>
   -->
   </td>
  </tr>
 </tbody>
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations about modifying percent allocations for tasks

* Users are allocated an equal percentage of time to tasks they are assigned to, by default. 
* You can manually modify the allocation percentage for users and job roles assigned to tasks only when the Duration Type of the task is Calculated Work or Effort Driven.

  For information, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). 

* You cannot modify the percent allocation for teams assigned to tasks.
* You cannot modify the percentage allocation for users and job roles assigned to issues.

## Modify the user or role percent allocation for a task

1. Go to a task for whose resources you are changing the percent allocation.
1. Click the **Assignments** area in the task header, then click **Advanced**.

1. Ensure that the **Duration Type** of the task is one of the following:

   * Calculated Work
   * Effort Driven

   >[!TIP]
   >
   >* For the Calculated Assignment Duration Type, Workfront uses the following formula to calculate the allocation percentage of each assignee: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* For the Simple Duration Type, you can estimate the hours assigned to each resource, not the allocation percentage. 

1. Modify the **Allocations** field for each task assignee.

   You can only modify the allocation percentage for user and job role assignments.

   You cannot modify the allocation percentage for a team assigned to a task.

   You may see one of these screens depending on your organization's Workfront or Workflow package.

   ![Modify allocation percentage](assets/advanced-assignments-allocation-percentage.png)

   ![Modify allocation percentage](assets/new-aa-allocation-by-percentage.png)

1. Click **Save**.
