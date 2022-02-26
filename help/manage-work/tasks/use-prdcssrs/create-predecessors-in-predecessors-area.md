---
filename: create-predecessors-in-predecessors-area
product-area: projects
navigation-topic: use-predecessors
title: Create a predecessor relationship using the Predecessors area
description: You can use predecessor tasks (or just predecessors) to link tasks that depend on other tasks to start or complete. For example, you would not want to host a party (dependent task) before you send out the invitations (predecessor task).
---

# Create a predecessor relationship using the Predecessors area

You can use predecessor tasks (or just predecessors) to link tasks that depend on other tasks to start or complete. For example, you would not want to host a party (dependent task) before you send out the invitations (predecessor task).

This article shows how you can set predecessors using the Predecessors tab within a task.

For information about setting predecessors in a list of tasks, see [Create a predecessor relationship on the task list](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

You can view the predecessors of tasks in the following areas of *Adobe Workfront*:

* In the Predecessors 

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  section
  </MadCap:conditionalText>
  -->

  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section </MadCap:conditionalText>`of the dependent tasks

* In the Gantt Chart
* In the task list in the Predecessors column

For information about predecessors, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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

## Create a predecessor for a task

<ol> 
 <li value="1"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Go to a task that you want to designate as a dependent task, then click <span class="bold">Predecessors</span> in the left panel. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Go to a task that you want to designate as a dependent task, then click <span class="bold">Predecessors</span> in the left panel. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You might need to click <span class="bold">Show More</span>, then <span class="bold">Predecessors</span>. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You might need to click <span class="bold">Show More</span>, then <span class="bold">Predecessors</span>. </p> </li> 
 <li value="2"> <p>Click <span class="bold">+Add Predecessor</span>. </p> </li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) To add a cross-project predecessor, replace the name of the project in the <span class="bold">Parent Project</span> field with another project, then type the name of the task or tasks that you want as the predecessors. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) To add a cross-project predecessor, replace the name of the project in the <span class="bold">Parent Project</span> field with another project, then type the name of the task or tasks that you want as the predecessors. </p> <p>For information about adding cross-project predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Create cross-project predecessors</a>.</p> </li> 
 <li value="4"> <p>Type in the name of the task or tasks that you want to designate as the predecessors. </p> <p> <draft-comment>
    <img src="assets/add-predecessor-box-nwe-350x465.png" style="width: 350;height: 465;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/add-predecessor-box-nwe-350x465.png" style="width: 350;height: 465;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="5"> <p>Select a <span class="bold">Dependency Type</span>.</p> <p>For information about task Dependency Types, see a <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>.</p> </li> 
 <li value="6"> <p>Specify a <span class="bold">Lag</span> amount in days. </p> <p>For information about Lag Types, see ​<a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Overview of Lag Types</a>.</p> </li> 
 <li value="7"> <p>Select <span class="bold">Enforced</span> if you want to enforce the predecessor relationship between the two tasks. </p> <p>For information about enforcing predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">Enforce predecessors</a>.</p> </li> 
 <li value="8"> <p>Click <span class="bold">Save</span>. </p> </li> 
</ol>

