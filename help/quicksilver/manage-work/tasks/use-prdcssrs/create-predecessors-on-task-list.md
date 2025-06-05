---
product-area: projects
navigation-topic: use-predecessors
title: Create a predecessor relationship on the task list
description: You can use predecessor tasks (or just predecessors) to link tasks that depend on other tasks to start or complete. For example, you would not want to host a party (dependent task) before you send out the invitations (predecessor task).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
---
# Create a predecessor relationship on the task list

<!-- Audited: 5/2025 -->

You can use predecessor tasks (or just predecessors) to link tasks that depend on other tasks to start or complete. For example, you would not want to host a party (dependent task) before you send out the invitations (predecessor task).

This article shows you how to create predecessors on the task list.

You can view the predecessors of tasks in the following areas of Adobe Workfront:

* In the task list in the Predecessors column. 
* In the Gantt chart.
* In the Predecessors section of a dependent task.

For more information, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

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
   <td> <p>New: Standard </p><p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

 +++

## Create a predecessor

{{step1-to-projects}}

1. Select a project on the **Projects** page.
1. Click **Tasks** in the left panel. 
1. In the **Views** drop-down, select a view that displays the **Predecessor** column, or add the column to your current view. 

1. Select the task that you want to designate as the dependent task. 
1. Click inside the task's **Predecessors** column.
1. Type in the task number you want to designate as the predecessor of the selected task, then press **Enter**.

   >[!TIP]
   >
   >To add a cross-project predecessor, do the following:
   >
   >1. Click the **Plan Mode** icon and choose **Autosave**. 
   >
   >1. Type in the Reference Number of the project of the predecessor followed, by a colon and the number of the task. For example, typing in *765021:12* indicates that the Reference Number of the predecessor's project is 765021 and the predecessor is task number 12 on the project. 
   >
   >1. Add the dependency type for this predecessor. For more information, see [Create cross-project predecessors](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md). 
   >
   >1. Press **Enter**.
   >
   >**IMPORTANT**
   >
   >You can't add a cross-project predecessor when the task list displays in Manual save mode. 

   The predecessor icon turns green when the predecessor task is marked complete. This signals that the dependent task is ready for work.

   For more information about the relationship types available in the Predecessors column, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## View predecessor details

You can quickly view details about the predecessor from the task list.

1. On the task list, hover over the predecessor number in the **Predecessors** column. A box with the predecessor details displays.

   ![Predecessor details](assets/predecessor-details-in-task-list.png)

   The following details are displayed:

   **Predecessor name:** The name of the predecessor that is being referenced. The task number of the predecessor is included. Click the task name to open it.

   **Project name:** The name of the project where the predecessor resides. The project is identified as the current project if the predecessor belongs to the same projects as the task, or as a cross project, if the predecessor belongs to a different project. For more information about cross-project predecessors, see [Create cross-project predecessors](../../tasks/use-prdcssrs/cross-project-predecessors.md). 

   You can expand the project details to see the project's planned start and end dates, condition, status, percent complete, and owner. For a cross project, you can then click **See Project** to open the project.

   **ID:** The Reference number of the project where the predecessor is located. 

   **Planned Start:** The Planned Start Date of the predecessor task.

   **Planned End:** The Planned Completion Date of the predecessor task.

   **Number of predecessors:** The number of predecessors for the predecessor being referenced. 

   **Number of successors:** The number of successor (or dependent) tasks for the predecessor being referenced. 
