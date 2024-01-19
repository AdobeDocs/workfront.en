---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Level Resources in the  [!UICONTROL Gantt Chart]
description: Information about how to level resources in the Gantt Chart. 
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
---
# Level Resources in the [!UICONTROL Gantt Chart]

Leveling your resources on a project has two purposes:

* To automatically adjust over-allocation of time for assignees.
* To automatically create a realistic task schedule for a project.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects</p> <p><b>NOTE</b>

If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] access to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Overview of Resource Leveling

If the same resource is assigned to two different tasks, you can use resource leveling to adjust the timeline of the tasks so they will not occur at the same time. 

Consider the following when leveling resources on a project:

* Resource leveling only applies to one project, so [!DNL Adobe Workfront] does not level resources across more than one project at a time.
* If **[!UICONTROL Effort Driven]** is selected as a **[!UICONTROL Duration Type]**, [!DNL Workfront] will not level the resources.
* When multiple users are assigned to the same task, leveling will be canceled.
* Conditions for the type of **[!UICONTROL Task Constraint]** will take precedence over the leveling of resources. For example, if **[!UICONTROL Fixed Dates]** is selected as the [!UICONTROL Task Constraint], resource leveling will not change the task dates.
* Predecessor relationships will take precedence over resource leveling.
* **[!UICONTROL Resource Leveling]** needs to be set to **[!UICONTROL Manual]** for the project in order to adjust leveling in the [!UICONTROL Gantt chart]. If you have Manage permissions to the project, you can can have the system automatically level resources by adjusting this setting on the project and selecting **[!UICONTROL Automatic]** instead of **[!UICONTROL Manual]** in the **[!UICONTROL Edit Project]** box.

   ![](assets/resource-leveling-mode-350x177.png)

* As the project owner, or the task assignee, you can introduce a leveling delay for a task to indicate that there is a great chance that the task might need extra time. For information about adding a leveling delay to a task, see [Update task Leveling Delay](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Apply Resource Leveling in the [!UICONTROL Gantt Chart]

You can use the Task List [!UICONTROL Gantt Chart] to level your resources.

1. Go to the project you want to level.
1. In the **[!UICONTROL Tasks]** area, click the **[!UICONTROL Gantt chart]** icon.

   All changes are saved automatically when the **[!UICONTROL Autosave]** option is enabled. It is enabled by default.

1. (Optional) Click the **[!UICONTROL Plan] mode** icon and select **[!UICONTROL Manual save Standard]** or **[!UICONTROL Timeline Planning]** to save your changes manually.

   >[!TIP]
   >
   >You cannot level resources in the  [!UICONTROL Gantt Chart] when the [!UICONTROL Autosave] option is enabled.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Click the **[!UICONTROL Level Resources]** drop-down menu.

   ![Level_resouces.png](assets/level-resouces.png)

1. Select one of following options:

   * **[!UICONTROL Level Now]**: Applies resource leveling to the selected task.
   * **[!UICONTROL Clear Leveling]**: Removes all resource leveling from the selected task.

   >[!NOTE]
   >
   >Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.

1. (Optional and conditional) If you have disabled the Autosave option, click the **[!UICONTROL Undo]** or&#x200B;**[!UICONTROL Redo]** icons if you want to cancel or duplicate any of the changes.

   >[!TIP]
   >
   >You can use the following keyboard shortcuts to undo or redo changes on the [!UICONTROL Gantt Chart]:
   >
   >* [!DNL Mac]: Use [!UICONTROL Command + Z] to undo and [!UICONTROL Command + Shift + Z] to redo.
   >* Windows: Use [!UICONTROL Ctrl + Z] to undo and [!UICONTROL Ctrl + Y] to redo.


1. Click **[!UICONTROL Save]** in the upper-right corner of the [!UICONTROL Gantt chart].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p>  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
