---
product-area: projects
navigation-topic: use-predecessors
title: Create Predecessor Relationships by Chaining Tasks
description: You can create predecessor relationships in multiple ways in Adobe Workfront. One method is by chaining tasks.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
---
# Create predecessor relationships by chaining tasks

You can create predecessor relationships in multiple ways in Adobe Workfront. One method is by chaining tasks.

For information about predecessor tasks, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

By chaining tasks, you can allow the system to create the predecessor relationships automatically on selected tasks, rather than manually creating a relationship on each task yourself. Different predecessor relationship types can still be used between tasks.

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

<!--Old:
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
   <p>Standard </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Chain tasks to create predecessor relationships

1. Go to the project that contains the tasks that you want to chain. 
1. Click **Tasks** in the left panel.
1. (Conditional) Select **Autosave** in the upper-right corner of the task list, then select the tasks that you want to chain.

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >Chaining tasks in a task list is not possible when you manually save changes to tasks or use the Timeline Planning mode for saving tasks.

1. Right-click the selected tasks, then click **Chain**. 
1. Select from the following dependency types:

   * **Finish-Start**
   * **Finish-Finish**
   * **Start-Start**
   * **Start-Finish**

   For more information about predecessor dependency types, see [Overview of task dependency types](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Optional) Click **Unchain** if some of the tasks have been previously chained.

   >[!CAUTION]
   >
   >Only sequential predecessors are removed by using the unchain option when bulk editing tasks.

   Your selected tasks are now linked by predecessor relationships.
