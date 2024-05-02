---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Manage user and role allocation hours on tasks
description: When assigning users or roles to a task, they are allocated to work a certain number of hours to complete the task. You can manually modify the amount of hours that each user or job role is allocated when they are assigned to a task, when the task Duration Type is Simple.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
---
# Manage user and role allocation hours on tasks

{{highlighted-preview}}

When assigning users or roles to a task, they are allocated to work a certain number of hours to complete the task. You can manually modify the amount of hours that each user or job role is allocated when they are assigned to a task, when the task&nbsp;Duration&nbsp;Type is Simple.

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
   <td> <p>Contribute or higher permissions to the task</p> <p>Edit permissions to update allocation hours in the Edit Task box</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations for modifying the allocation hours for a task

>[!IMPORTANT]
>
>After you manually modify the allocations for each assignment on tasks, the Planned Hours of the tasks might update accordingly. For more information, see the section [Update task Planned Hours when managing user allocations](../../../manage-work/tasks/task-information/planned-hours.md#update) in the article [Planned Hours overview](../../../manage-work/tasks/task-information/planned-hours.md).

* The total of hours allocated to individual resources assigned to the task represents the Planned Hours of the task. 
* If there is one user or role assignment to a task, the amount of hours allocated to the user or role matches the Planned Hours of the task.
* In the case of multiple assignments, each user or job role is assigned an equal amount of hours to work on the task, by default, if the task Duration Type is Simple. For more information, see the following articles:

   * [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) 
   * [Duration Type overview: Simple](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* When the task has a Simple Duration&nbsp;Type, you can manually change the amount of allocated hours for each user or job role to indicate that some of the task assignees might have more time to work on a task than others. 
* You cannot modify the amount of hours allocated to teams assigned to tasks.
* You cannot manually modify the user or job role allocation for issues. 
* You can also manage daily, weekly, or monthly allocations of users to tasks or issues by using the Workload Balancer. For more information, see [Manage user allocations in the Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modify the user or role allocation hours for a task

1. Go to a task for whose assignments you want to change the allocation hours.
1. Click the **More** menu ![](assets/qs-more-icon-on-an-object.png) next to the name of the task, then click **Edit**, then **Assignments**.

   Or

   Click the **Assignments** area in the task header, then click&nbsp;**Advanced**.

1. Ensure that the **Duration Type** of the task is **Simple**.
1. Modify the **Allocations** for each task assignee. These are overall allocations for each assignment to this task, for the entire duration of the task. This might also update the overall Planned Hours of the task.

   Sample image in the Production environment:
   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

   <span class="preview">Sample image in the Preview environment:</span>
   ![Modify allocations](assets/advanced-assignments-duration-type-allocations.png)

1. Click **Save**.
