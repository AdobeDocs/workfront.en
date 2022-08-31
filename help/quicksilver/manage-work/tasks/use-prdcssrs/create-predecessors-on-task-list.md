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

{{highlighted-preview}}

You can use predecessor tasks (or just predecessors) to link tasks that depend on other tasks to start or complete. For example, you would not want to host a party (dependent task) before you send out the invitations (predecessor task).

This article shows you how to create predecessors on the task list.

You can view the predecessors of tasks in the following areas of Adobe Workfront:

* In the task list in the Predecessors column. 
* In the Gantt chart
* In the Predecessors section of a dependent task

For more information, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Create a predecessor

1. Go to a project. 
1. Click **Tasks** in the left panel. 
1. Ensure that your current view displays the **Predecessor** column.

   If the view doesn't display the Predecessors column, change to a view that does, or add the column to your view. 

1. Select the task that you want to designate as the dependent task. 
1. Click inside the **Predecessors** column.
1. Type the task number that you want to designate as the predecessor of the selected task, then press **Enter**.

   The predecessor icon turns green when the predecessor task is marked complete. This signals that the dependent task is ready for work.

   For more information about the relationship types available in the Predecessors column, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## View predecessor details (available only in the Preview environment)

<span class="preview">You can quickly view details about the predecessor from the task list.</span>

1. <span class="preview">On the task list, hover over the predecessor number in the **Predecessors** column.</span>

   <div class="preview">

   A box with the details of the predecessor displays.

   ![Predecessor details](assets/cpr4-350x175.png)

   The following details are displayed:

   **Predecessor name:** The name of the predecessor that is being referenced. The task number of the predecessor is included. For cross-project predecessors, you can click the task name to open it in a new browser window. In the above example, the predecessor is Market Research.

   **Project name:** The name of the project where the predecessor resides. The project is identified as the current project or a cross project. In the above example, the project name is Target Markets.

   You can expand the project details to see the project's start and end dates, condition, status, percent complete, and owner. For a cross project, you can then click See project to open the project in a new browser window.

   **Start:** The date when the predecessor task was requested.

   **End Date:** The date when the predecessor task is due.

   **Number of predecessors:** The number of predecessors for the predecessor being referenced. In the above example, the predecessor being referenced has 0 predecessors.

   **Number of successors:** The number of successor (or dependent) tasks for the predecessor being referenced. In the above example, the predecessor being referenced has 1 successor.

   </div>
