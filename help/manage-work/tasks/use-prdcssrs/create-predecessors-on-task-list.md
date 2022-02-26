---
filename: create-predecessors-on-task-list
product-area: projects
navigation-topic: use-predecessors
title: Create a predecessor relationship on the task list
description: You can use predecessor tasks (or just predecessors) to link tasks that depend on other tasks to start or complete. For example, you would not want to host a party (dependent task) before you send out the invitations (predecessor task).
---

# Create a predecessor relationship on the task list

You can use predecessor tasks (or just predecessors) to link tasks that depend on other tasks to start or complete. For example, you would not want to host a party (dependent task) before you send out the invitations (predecessor task).

This article shows you how to create predecessors on the task list.

You can view the predecessors of tasks in the following areas of *Adobe Workfront*:

* In the task list in the Predecessors column. 
* In the Gantt chart
* In the Predecessors 

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  section
  </MadCap:conditionalText>
  -->

  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section </MadCap:conditionalText>`of a dependent task

For more information, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Create a predecessor

1. Go to a project. 
1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Tasks</span> in the left panel. </p>
   -->

   Click `Tasks` in the left panel. 

1. Ensure that your current view displays the `Predecessor` column.

   If the view doesn't display the Predecessors column, change to a view that does, or add the column to your view. 

1. Select the task that you want to designate as the dependent task. 
1. Click inside the `Predecessors` column.
1. Type the task number that you want to designate as the predecessor of the selected task, then press `Enter`.

   The predecessor icon turns green when the predecessor task is marked complete. This signals that the dependent task is ready for work.

   For more information about the relationship types available in the Predecessors column, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## View predecessor details

You can quickly view details about the predecessor from the task list.

<ol> 
 <li value="1"> <p>On the task list, mouse over the predecessor number in the <span class="bold">Predecessors</span> column.</p> <p>A box with the details of the predecessor displays. </p> <p> <img src="assets/cpr4-350x175.png" alt="" style="width: 350;height: 175;"> </p> <p>The following details are displayed:</p> <p><span class="bold">Predecessor name:</span> The name of the predecessor that is being referenced. In the above example, the predecessor is Market Research.</p> <p><span class="bold">Project name:</span> The name of the project where the predecessor resides. In the above example, the project name is Target Markets.</p> <p><span class="bold">Number of predecessors (left of details box):</span> The number of predecessors for the predecessor being referenced. In the above example, the predecessor being referenced has 0 predecessors.</p> <p><span class="bold">Requested:</span> The date when the predecessor task was requested.</p> <p><span class="bold">Due Date:</span> The date when the predecessor task is due.</p> <p><span class="bold">Number of successors (right of details box):</span> The number of successor (or dependent) tasks for the predecessor being referenced. In the above example, the predecessor being referenced has 1 successor.</p> </li> 
</ol>

