---
filename: enforced-predecessors
product-area: projects
navigation-topic: use-predecessors
title: Enforce predecessors
description: Predecessors are tasks on which other tasks are dependent for completion. Predecessor relationships affect the Start and Completion Dates of the tasks and ultimately impact the timeline of the project.
---

# Enforce predecessors

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

## Enforce a predecessor at the task level

<ol> 
 <li value="1">Go to the successor task whose predecessor you want to enforce.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Predecessors</span> in the left panel, then click <span class="bold">Add Predecessor</span>. You might need to click <span class="bold">Show More</span>, then <span class="bold">Predecessors</span>. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Predecessors</span> in the left panel, then click <span class="bold">Add Predecessor</span>. You might need to click <span class="bold">Show More</span>, then <span class="bold">Predecessors</span>. </p> </li> <draft-comment>
  <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Conditional) If you want to add a cross-project predecessor, remove the name of the project in the <span class="bold">Parent Project</span> field and replace it with another project. </li>
 </draft-comment>
 <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Conditional) If you want to add a cross-project predecessor, remove the name of the project in the <span class="bold">Parent Project</span> field and replace it with another project. </li> 
 <li value="4">Specify the name of the predecessor task or tasks in the <span class="bold">Tasks</span> field. </li> 
 <li value="5"> <p>Specify the <span class="bold">Dependency Type</span> between these two tasks.</p> <p>The default <span class="bold">Dependency Type</span> is <span class="bold">Finish-Start</span>.</p> <p> <img src="assets/ep-350x408.png" alt="" style="width: 350;height: 408;"> </p> </li> 
 <li value="6">Select the <span class="bold">Enforced</span> field to enforce the predecessor.</li> 
 <li value="7">Click <span class="bold">Save</span>.</li> 
</ol>

## Enforce a predecessor in a task list

<ol> 
 <li value="1">Go to a task list on a project.</li> 
 <li value="2">From the <span class="bold">View</span> drop-down menu, select the <span class="bold">Standard View</span>. </li> 
 <li value="3">Make a mental note of the number of task which you are going to designate as the predecessor.</li> 
 <li value="4">Find the successor task whose predecessor you want to enforce. </li> 
 <li value="5">In the <span class="bold">Predecessors</span> column, start entering the number of the predecessor task followed by "e". For example, type "1e" to add task number 1 as a predecessor to the selected task. </li> 
 <li value="6"> <p>Click Enter to save your predecessor information for the task. </p> <p> <img src="assets/predecessor-enforced-in-list-350x308.png" alt="predecessor_enforced_in_list.png" style="width: 350;height: 308;"> </p> </li> 
</ol>

