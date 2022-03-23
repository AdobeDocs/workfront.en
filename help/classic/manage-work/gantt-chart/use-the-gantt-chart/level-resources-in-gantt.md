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

* Resource leveling only applies to one project, so Adobe Workfront does not level resources across more than one project at a time.
* If **Effort Driven** is selected as a **Duration Type**, Workfront will not level the resources.
* When multiple users are assigned to the same task, leveling will be canceled.
* Conditions for the type of **Task Constraint**&nbsp;will take precedence over the leveling of resources. For example,&nbsp;if **Fixed Dates** is selected as the Task Constraint, resource leveling will not change the task dates.
* Predecessor relationships will take precedence over resource leveling.
* **Resource Leveling** needs to be set to **Manual** for the project in order to adjust leveling in the Gantt chart. Users can have the system automatically level resources by adjusting this setting on the project and selecting **Automatic** instead of **Manual**.

  ![](assets/resource-leveling-mode.png)

* As the project owner, or the task assignee, you can introduce a leveling delay for a task to indicate that there is a great chance that the task might need extra time. For information about adding a leveling delay to a task, see [Update task Leveling Delay](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Apply Resource Leveling in the Gantt Chart

1. Navigate to a project.
1. Select the **Tasks** tab .
1. Click the **Gantt** icon.  

1. Disable the **Autosave** option.

   >[!TIP]
   >
   >You cannot level resources in the Gantt chart when the Autosave option is enabled.

1. Click the **Resource Leveling** drop-down menu and select **Level Now**.  
   ![new_gantt_resource_leveling.png](assets/new-gantt-resource-leveling.png)

1. (Optional) Select **Clear Leveling**, to remove all resource leveling from the project.

   >[!NOTE]
   >
   >Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.

1. Click **Save**.&nbsp;

<!--
<a name="resource-leveling-in-gantt"></a>Apply Resource Leveling in the Legacy Gantt Chart
<ol> Navigate to a project. Click <strong>More</strong>, then click <strong>Legacy Gantt</strong>.
<img src="assets/1-350x173.png" alt="" style="width: 350;height: 173;"> Click&nbsp;the <strong>Resource Leveling</strong> drop-down menu.
<img src="assets/2-350x89.png" alt="" style="width: 350;height: 89;"> Select <strong>Level Now</strong>.
<br>Workfront automatically finds the next available time from the schedule of the over-allocated users, and moves over-allocated tasks to another time. By default, Workfront will look at the task ID number to prioritize this adjustment. In general, tasks with lower ID numbers take precedence over tasks with higher ID numbers. (Optional) Select <strong>Clear Leveling</strong>, to remove all resource leveling from the project.
<br><span class="autonumber"><span><b>Note: </b></span></span> Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame. Click <strong>Save</strong>.&nbsp;
</ol>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="leveling-delay"></a>Overview of Leveling Delay</h2>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic&nbsp;schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels&nbsp;the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> Click <strong>Edit Task</strong>.  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>.&nbsp;</li>
</ol>
</div>
-->

