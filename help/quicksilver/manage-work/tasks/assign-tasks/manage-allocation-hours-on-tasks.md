---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Manage User and Role Allocation Hours on Tasks
description: When assigning users or roles to a task, they are allocated to work a certain number of hours to complete the task. You can manually modify the amount of hours that each user or job role is allocated when they are assigned to a task, when the task Duration Type is Simple.
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Jx-D1MY9dopkps0UqnE7Mgu4vlYevFjzRjRGWXDaWQQ
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
# Manage user and role allocation hours on tasks

<!--Audited: 10/2025-->

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->


<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->

Allocation hours represent the total amount of time an assigned resource is planned to work on a task. The hours represent the time that a user is allocated on one given day or weekday, week, or month throughout the duration of the task.

You can modify the allocation hours when you make advanced assignments on a task. 

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
   <p>Edit permissions to update allocation hours in the Edit Task box.</p> 
   <!--
   Not true anymore:
   <p><b>NOTE</b></p>
   <p>
   You can no longer manage allocation hours in the Edit task box when editing tasks in the new experience.</p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a>.</p>
   -->
   </td>
  </tr>
 </tbody>
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations for modifying the allocation hours for a task

>[!IMPORTANT]
>
>After you manually modify the allocations for each assignment on tasks, the Planned Hours of the tasks might update accordingly. For more information, see the section [Update task Planned Hours when managing user allocations](../../../manage-work/tasks/task-information/planned-hours.md#update) in the article [Planned Hours overview](../../../manage-work/tasks/task-information/planned-hours.md).

* The total of hours allocated to individual resources assigned to the task represents the Planned Hours of the task. 
* If there is one user or role assignment to a task, the amount of hours allocated to the user or role matches the Planned Hours of the task.
* In the case of multiple assignments, each user or job role is assigned an equal amount of hours to work on the task, by default, if the task Duration Type is Simple. For more information, see the following articles:

   * [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) 
   * [Duration Type overview: Simple](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* When the task has a Simple Duration Type, you can manually change the amount of allocated hours for each user or job role to indicate that some of the task assignees might have more time to work on a task than others. 
* You cannot modify the amount of hours allocated to teams assigned to tasks.
* You cannot manually modify the user or job role allocation for issues. 
* You can also manage daily, weekly, or monthly allocations of users to tasks or issues by using the Workload Balancer. For more information, see [Manage user allocations in the Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modify the user or role allocation hours for a task

1. Go to a task for whose assignments you want to change the allocation hours.
1. Click the **Assignments** area in the task header, then click **Advanced**.
1. Ensure that the **Duration Type** of the task is **Simple**.
1. Modify the **Allocations** field for each task assignee. These are overall allocations for each assignment to this task, for the entire duration of the task. This might also update the overall **Planned Hours** of the task.

   You may see one of these screens depending on your organization's Workfront or Workflow package.

   ![Modify allocations](assets/advanced-assignments-duration-type-allocations.png)

   ![Modify allocations](assets/new-aa-allocation-by-hour.png)

1. Click **Save**.
