---
product-area: projects
navigation-topic: use-predecessors
title: Enforce Predecessors
description: Predecessors are tasks on which other tasks are dependent for completion. Predecessor relationships affect the Start and Completion Dates of the tasks and ultimately impact the timeline of the project.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/GRkH39mvpwOvxVqlDdiB9vgz5tMfhv5nTlsEK4iY6jM
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
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Enforce predecessors

<!-- Audited: 11/2025 -->

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
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p></td> 
  </tr> 
 </tbody> 
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

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
-->

## Enforce a predecessor at the task level

1. Go to the successor task whose predecessor you want to enforce.
1. Click **Predecessors** in the left panel, then click **Add Predecessor**. 
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

   ![Predecessor enforced list](assets/predecessor-enforced-in-list-350x308.png)

   The information about the predecessor being enforced is immediately saved.
