---
product-area: projects
navigation-topic: use-predecessors
title: Create a Predecessor Relationship Using the Predecessors Area
description: You can use predecessor tasks (or just predecessors) to link tasks that depend on other tasks to start or complete.
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
TQID: https://experienceleague.adobe.com/BOZkyUl3TKCzpbjbLnUcMQZjM-1laW-TSsVptvBP-0U
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
# Create a predecessor relationship using the Predecessors area

<!-- Audited: 5/2025 -->

You can use predecessor tasks (or just predecessors) to link tasks that depend on other tasks to start or complete. For example, you wouldn't want to host a party (dependent task) before you send out the invitations (predecessor task).

This article shows how you can set predecessors using the Predecessors tab within a task.

For information about setting predecessors in a list of tasks, see [Create a predecessor relationship on the task list](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

You can view the predecessors of tasks in the following areas of Adobe Workfront:

* In the Predecessors section of the dependent tasks
* In the Gantt Chart
* In the task list in the Predecessors column

For information about predecessors, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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

## Create a predecessor for a task

Creating a predecessor for a project task using the Predecessors area is similar to creating predecessors for a template task on a template. 

To create a predecessor task for a project task: 

1. Navigate to the task you want to designate as a dependent task.

1. In the left panel, click **Predecessors**.

1. In the **Predecessors** section, click **Add Predecessor**. The **Add Predecessor** dialog box opens. 

1. (Optional) To add a cross-project predecessor, replace the name of the project in the **Parent Project** field with another project.

   For information, see [Create cross-project predecessors](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

   >[!TIP]
   >
   >You cannot create cross-template predecessors for template tasks.


1. In the **Tasks** field, type in the name of the task or tasks you want to designate as the predecessors, then select them when they appear in the drop-down.

1. Select a **Dependency Type**.

   For information, see [Overview of task dependency types](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Enter a **Lag** amount.

   For information, see ​[Lag Types overview](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

    ![Add Predecessor dialog box](assets/add-predecessor-dialog-box.png)

1. Select the **Enforced** checkbox if you want to enforce the predecessor relationship between the two tasks.

   For information, see [Enforce predecessors](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Click **Save**.

1. (Optional) To remove a predecessor, select it from the list of predecessors, then click the **Remove** icon ![Remove icon](assets/remove-or-delete-icon.png).

   The predecessor is removed from the list. The predecessor task is not deleted from its project. 
