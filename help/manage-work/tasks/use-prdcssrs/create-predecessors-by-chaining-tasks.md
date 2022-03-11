---
filename: create-predecessors-by-chaining-tasks
product-area: projects
navigation-topic: use-predecessors
title: Create predecessor relationships by chaining tasks
description: You can create predecessor relationships in multiple ways in Adobe Workfront. One method is by chaining tasks.
---

# Create predecessor relationships by chaining tasks

You can create predecessor relationships in multiple ways in Adobe Workfront. One method is by chaining tasks.

For information about predecessor tasks, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

By chaining tasks, you can allow the system to create the predecessor relationships automatically on selected tasks, rather than manually creating a relationship on each task yourself. Different predecessor relationship types can still be used between tasks.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
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
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Chain tasks to create predecessor relationships

<ol> 
 <li value="1">Go to the project that contains the tasks that you want to chain. </li> 
 <li value="2"> <p> Click Tasks in the left panel.</p> </li> 
 <li value="3"> <p>(Conditional) Select <span class="bold">Autosave</span> in the upper-right corner of the task list, then select the tasks that you want to chain. </p>  <note type="important">
   Chaining tasks in a task list is not possible when you manually save changes to tasks or use the Timeline Planning mode for saving tasks. 
  </note> </li> 
 <li value="4"> <p>Right-click the selected tasks, then click <span class="bold">Chain</span>. </p> </li> 
 <li value="5">Select from the following dependency types: 
  <ul>
   <li><span class="bold">Finish-Start</span></li>
   <li><span class="bold">Finish-Finish</span></li>
   <li><span class="bold">Start-Start</span></li>
   <li><span class="bold">Start-Finish</span></li>
  </ul> For more information about predecessor dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>.</li> 
 <li value="6"> <p>(Optional) Click <span class="bold">Unchain</span> if some of the tasks have been previously chained. </p> <p class="warning" data-mc-autonum="<b>Warning: </b>"><span class="autonumber"><span><b>Warning: </b></span></span> Only sequential predecessors are removed by using the unchain option when bulk editing tasks. </p> <p>Your selected tasks are now linked by predecessor relationships. </p> </li> 
</ol>

