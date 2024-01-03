---
product-area: projects
navigation-topic: use-predecessors
title: Create cross-project predecessors
description: A Cross-Project Predecessor is a task that another task (called a successor task) in another project depends on. The predecessor is the task that takes priority over the dependent (successor) task. For example, you can create a dependency that requires that the predecessor task be marked Complete before the dependent task can start.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
---
# Create cross-project predecessors

<!--Audited: 12/2023-->

A cross-project predecessor is a task that another task (called a successor task) in another project depends on. The predecessor is the task that takes priority over the dependent (successor) task. For example, you can create a dependency that requires that the predecessor task be marked Complete before the dependent task can start.

Adobe Workfront allows for tasks to be dependent on tasks in other projects, just as it allows predecessors within a single project.

>[!INFO]
>
>For example, an excavating company has only one backhoe, and two projects have tasks that require the use of the backhoe. The project manager can make the task in the first project a predecessor to the task in the second project. This shows that the second project can begin using the backhoe when the first project is finished with it.

When linking projects through cross-project predecessors, the dates of the primary project (the one that has the predecessor task) will impact the secondary project (the one that has the successor task).

>[!TIP]
>
>You must recalculate timelines for the projects in order to see dates updated for the secondary project. For more information on recalculating timelines, see [Configure timeline recalculations for projects](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

For more information about predecessor relationships, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Access requirements

<!--drafted - replace table for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
  <td> <p>New: Standard </p>
 <p>or</p> 
<p>Current: Plan </p> 
</td> 
 </tr>   <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Create a cross-project predecessor

1. Go to the task that will be your successor (dependent task). 
1. Click **Predecessors** in the left panel. 
1. Click **Add Predecessor.**
1. In the **Parent Project** field, begin typing the name of the project that contains the task that you want to be the predecessor to your current task.
1. Click the name when it appears in the drop-down list.
1. In the **Tasks** field, begin typing the name of the task that you want to be the predecessor to your current task.
1. Specify the following information for defining the relationship between the predecessor and dependent task:

   * **Dependency Type:** Select the relationship that you want the predecessor task to have with the dependent task. The default relationship is "Finish-Start," meaning that the predecessor task must finish before the dependent task can start. For more information about the various dependency types, see [Overview of task dependency types](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)
   
   * **Lag:** Specify the amount of time that must pass after the completion of an enforced predecessor until the dependent task can begin. For more information about the various types of lag, see [Lag Types overview](../../../manage-work/tasks/use-prdcssrs/lag-types.md).
   
   * **Enforced:** When this option is selected, dependency relationship between the two tasks cannot be circumvented by users beginning tasks early. For example, if you enforce a relationship between Task A and Task B, Task B cannot be started until Task A is complete. For more information about enforcing predecessors, see [Enforce predecessors](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     When this option is not selected, the dependency is treated like a suggestion to users. For example, users are able to start Task B before Task A is complete.

1. Click **Save**.

   Tasks that have a cross-project predecessor display the reference number of the project the predecessor belongs to and the number of the task, separated by a colon, in the Predecessors column on a task list.

   ![Cross-project predecessor](assets/cross-project-predecessor-in-list-view.png)

   The predecessor icon turns green when the predecessor task is marked complete. This signals that the dependent task is ready for work.

   Hover over this value to get more information on the predecessor, the project, and the dates. Click the cross-project predecessor in the details box to open the task.

   Click near the top of the hover window to see more information about the predecessor's project.

   Click **See Project** to open the predecessor's project.

   ![Cross-project predecessor details](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   The **See Project** option displays only when viewing a cross-project predecessor. 

