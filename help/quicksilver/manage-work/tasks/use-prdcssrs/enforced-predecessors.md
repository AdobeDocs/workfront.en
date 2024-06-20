---
product-area: projects
navigation-topic: use-predecessors
title: Enforce predecessors
description: Predecessors are tasks on which other tasks are dependent for completion. Predecessor relationships affect the Start and Completion Dates of the tasks and ultimately impact the timeline of the project.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
---
# Enforce predecessors

<!-- Audited: 2/2024 -->

Predecessors are tasks on which other tasks are dependent for completion. Predecessor relationships affect the Start and Completion Dates of the tasks and ultimately impact the timeline of the project.

For information about predecessors, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

By setting predecessor relationships between tasks, you define how the start or finish of a dependent task depends upon the start or finish of their predecessor tasks. This is done by using different Dependency Types.

For information about Dependency Types, see [Overview of task dependency types](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Overview of enforced predecessors

>[!IMPORTANT]
>
>You must enforce predecessors to require that predecessor relationships are respected. Without enforcing the predecessors, dependent tasks can start and finish independently from the start and finish of their predecessors, regardless of their Dependency Types.

You can enforce the predecessor relationship when setting predecessors on a project.

If a predecessor is enforced, the successor task cannot start before the predecessor completes. For example, enforcing a Finish-Start relationship between Task A and Task B means that Task B cannot start (the Status must remain New, and the Percent Complete must remain 0%) until Task A is marked as completed. Enforcing relationships apply to all predecessor types.

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
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
      <p>New: Standard</p> 
      <p>OR</p>
      <p>Current: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td><p>Manage permissions to the tasks and the project</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Enforce a predecessor at the task level

1. Go to the successor task whose predecessor you want to enforce.
1. Click **Predecessors** in the left panel, then click **Add Predecessor**. You might need to click **Show More**, then **Predecessors**. 
1. (Conditional) If you want to add a cross-project predecessor, remove the name of the project in the **Parent Project** field and replace it with another project. 
1. Specify the name of the predecessor task or tasks in the **Tasks** field. 
1. Specify the **Dependency Type** between these two tasks.

   The default **Dependency Type** is **Finish-Start**.

1. Select the **Enforced** field to enforce the predecessor.
1. Click **Save**.

## Enforce a predecessor in a task list

1. Go to a task list on a project.
1. From the **View** drop-down menu, select the **Standard View**. 

1. Make a mental note of the number of task which you are going to designate as the predecessor.
1. Find the successor task whose predecessor you want to enforce. 
1. In the **Predecessors** column, start entering the number of the predecessor task followed by "e". For example, type "1e" to add task number 1 as a predecessor to the selected task. 
1. Click Enter to save your predecessor information for the task.

   ![predecessor_enforced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
