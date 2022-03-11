---
filename: level-resources-in-gantt
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Level Resources in the Gantt Chart
description: Leveling your resources on a project has two purposes:
---

# Level Resources in the Gantt Chart

Leveling your resources&nbsp;on a project&nbsp;has two purposes:

* To automatically adjust&nbsp;over-allocation of time for assignees.
* To automatically create a realistic task schedule for a&nbsp;project.&nbsp;

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Overview of Resource Leveling

If the same resource is assigned to two different tasks, you can use resource leveling to adjust the timeline of the tasks so they will not occur at the same time.&nbsp;

Consider the following when leveling resources on a project:

<ul> 
 <li> <p>Resource leveling only applies to one project, so Adobe Workfront does not level resources across more than one project at a time.</p> </li> 
 <li> <p>If <span class="bold">Effort Driven</span> is selected as a <span class="bold">Duration Type</span>, Workfront will not level the resources.</p> </li> 
 <li> <p>When multiple users are assigned to the same task, leveling will be canceled.</p> </li> 
 <li> <p>Conditions for the type of <span class="bold">Task Constraint</span>&nbsp;will take precedence over the leveling of resources. For example,&nbsp;if <span class="bold">Fixed Dates</span> is selected as the Task Constraint, resource leveling will not change the task dates.</p> </li> 
 <li> <p>Predecessor relationships will take precedence over resource leveling.</p> </li> 
 <li> <p><span class="bold">Resource Leveling</span> needs to be set to <span class="bold">Manual</span> for the project in order to adjust leveling in the Gantt chart. Users can have the system automatically level resources by adjusting this setting on the project and selecting <span class="bold">Automatic</span> instead of <span class="bold">Manual</span>.</p> <p> <img src="assets/resource-leveling-mode.png"> </p> </li> 
 <li> <p>As the project owner, or the task assignee, you can introduce a leveling delay for a task to indicate that there is a great chance that the task might need extra time. For information about adding a leveling delay to a task, see <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">Update task Leveling Delay</a>. <br></p> </li> 
</ul>

## Apply Resource Leveling in the Gantt Chart

<ol> 
 <li value="1">Navigate to a project.</li> 
 <li value="2">Select the <span class="bold">Tasks</span> area.</li> 
 <li value="3"> <p>Click the <span class="bold">Gantt</span> icon.<br></p> </li> 
 <li value="4"> <p>Disable the <span class="bold">Autosave</span> option. </p> <note type="tip">
   You cannot level resources in the Gantt chart when the Autosave option is enabled. 
  </note> </li> 
 <li value="5">Click the <span class="bold">Resource Leveling</span> drop-down menu and select <span class="bold">Level Now</span>.<br><img src="assets/new-gantt-resource-leveling.png" alt="new_gantt_resource_leveling.png"></li> 
 <li value="6">(Optional) Select <span class="bold">Clear Leveling</span>, to remove all resource leveling from the project.<br><note type="note">
    Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.
  </note></li> 
 <li value="7">Click <span class="bold">Save</span>.&nbsp;</li> 
</ol>

<!--
Overview of Leveling Delay At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts. To manually add a Leveling Delay to a task: Navigate to a task for which you want to add a Leveling Delay. Click the More icon to the right of the task name, then click Edit. Click Settings. Specify the Leveling Delay, in hours. This is the time that the resource will be delayed starting the task due to resource conflicts. Click Save Changes.
-->

