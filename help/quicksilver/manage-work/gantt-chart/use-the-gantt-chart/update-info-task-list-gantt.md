---
product-area: projects
navigation-topic: use-the-gantt-chart
title: Update information in the task list Gantt Chart
description: The task list Gantt Chart shows details about tasks that are on a project or template.
feature: Work Management
---

# Update information in the task list Gantt Chart

The task list Gantt Chart shows details about tasks that are on a project or template.

In a template, the task list Gantt Chart reflects updates made in the template's task list at the task level. You cannot edit the Gantt chart associated with a template.

In a project, you can update task information directly in the task list Gantt Chart.

This article describes the following actions that you can perform directly in the Task List Gantt Chart:

* Modify Task Duration
* Create or remove Predecessor relationships
* Change Task Start and End Dates
* Update Percent Complete
* Level Project Resources

## Access requirements

You must have the following to follow the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the project and tasks </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Modify Task Duration

1. Go to the project you want to modify.
1. Click **Tasks** in the left panel.

   ![](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. Click the **Gantt chart** icon.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   All changes are saved automatically when the **Autosave** option is enabled. It is enabled by default. 

1. (Optional) Click the **Plan mode** icon and select **Manual save Standard** or **Timeline Planning** to save your changes manually.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Hover over the timeline of a task and drag the time line indicator to a different date.
1. Drop the indicator when you have reached the correct new Completion Date for the task. 
1. (Optional and conditional) If you have selected to manually save your changes, click the **Undo** or**Redo** icons if you want to cancel or duplicate any of the changes.

   >[!TIP]
   >
   >You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:
   >
   >   
   >   
   >   * Mac: Use Command + Z to undo and Command + Shift + Z to redo.
   >   * Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.
   >   
   >

1. Click **Save** in the upper-right corner of the Gantt chart.

## Create or remove predecessor relationships

1. Go to the project you want to modify.
1. In the **Tasks** area, click the **Gantt chart** icon.

   The **Autosave** option is selected by default, in which case all changes are saved automatically.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (Optional) Click the **Plan mode** icon and select **Manual save Standard** or **Timeline Planning** to save your changes manually.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. To create a predecessor relationship, click the start point of a task and drag it to the end point of task. 
1. To delete a predecessor relationship, c lick a predecessor line that connects two tasks to select it, then press **Delete** on your keyboard.  
   ![Delete_predecessor.png](assets/delete-predecessor-350x152.png)

1. (Optional and conditional) If you selected to save your changes manually, click the **Undo** or**Redo** icons if you want to cancel or duplicate any of the changes.

   >[!TIP]
   >
   >You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:
   >
   >   
   >   
   >   * Mac: Use Command + Z to undo and Command + Shift + Z to redo.
   >   * Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.  
   >   
   >

1. Click **Save** .

## Change Task Start and End Dates

1. Go to the project you want to modify. 
1. In the **Tasks** area, click the **Gantt chart** icon.

   All changes are saved automatically when the **Autosave** option is enabled. It is enabled by default.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (Optional) Click the **Plan mode** icon and select **Manual save Standard** or **Timeline Planning** to save your changes manually.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Hover over the center of the task and locate the multi-directional arrow.
1. Click and drag the task to the desired date.

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. If you change the task date in a way that affects the task constraint, click **Accept** to acknowledge the task constraint change.

   >[!NOTE]
   >
   >If the task has one of the following constraints, the system updates the Task Constraint to Start No Earlier Than if the project is scheduled from the Start Date or Finish No Later Than if the project is scheduled from the Completion Date:
   >
   >   
   >   
   >   * As Soon As Possible
   >   * As Late As Possible
   >   * Earliest Available Time
   >   * Latest Available Time
   >   
   >   
   >In some cases, the predecessor relationships might prevent the tasks from starting earlier, and the task move is not allowed.

1. (Optional and conditional) If you have selected to save your changes manually, click the **Undo** or**Redo** icons if you want to cancel or duplicate any of the changes.

   >[!TIP]
   >
   >You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:
   >
   >   
   >   
   >   * Mac: Use Command + Z to undo and Command + Shift + Z to redo.
   >   * Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.  
   >   
   >

1. Click **Save**.

## Update Percent Complete

1. Go to the project you want to modify.
1. In the **Tasks** area, click the **Gantt chart** icon.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   All changes are saved automatically when the **Autosave** option is enabled. It is enabled by default. 

1. (Optional) Click the **Plan mode** icon and select **Manual save Standard** or **Timeline Planning** to save your changes manually.
1. Double-click the percent number inside of the task and enter the number.

   >[!IMPORTANT]
   >
   >You must have % Complete selected in the Options dialog in order to update percent complete. To do this, click the **Options** icon and select **% Complete**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >
   >

1. (Optional and conditional) If you selected to save your changes manually, click the **Undo** or**Redo** icons if you want to cancel or duplicate any of the changes.

   >[!TIP]
   >
   >You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:
   >
   >   
   >   
   >   * Mac: Use Command + Z to undo and Command + Shift + Z to redo.
   >   * Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.  
   >   
   >

1. Click **Save** in the upper-right corner of the Gantt chart.

## Level project resources

You can use the Task List Gantt Chart to level your resources.

For information on about leveling resources in the Gantt chart, see [Level Resources in the Gantt Chart](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this is drafted because I moved the whole content to the article linked above)</p>
<ol>
<li value="1">Go to the project you want to level.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> In the <strong>Tasks</strong> area, click the <strong>Gantt chart</strong> icon.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">All changes are saved automatically when the <strong>Autosave</strong> option is enabled. It is enabled by default. </p> </li>
<li value="3">
<div>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <strong>Plan mode</strong> icon and select <strong>Manual save Standard</strong> or <strong>Timeline Planning</strong> to save your changes manually.</p> <note type="tip">
You cannot level resources in the Gantt chart when the Autosave option is enabled.
</note>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p>
</div> </li>
<li value="4"> <p>Click the <strong>Level Resources</strong> drop-down menu.</p> <p> <img src="assets/level-resouces.png" alt="Level_resouces.png"> </p> </li>
<li value="5">Select one of following options:
<ul>
<li><strong>Level Now</strong>: Applies resource leveling to the selected task.</li>
<li><p><strong>Clear Leveling</strong>: Removes all resource leveling from the selected task.</p></li>
</ul><note type="note">
Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.
</note></li>
<li value="6"> <p>(Optional and conditional) If you have disabled the Autosave option, click the <strong>Undo</strong> or<strong>Redo</strong> icons if you want to cancel or duplicate any of the changes. </p> <note type="tip">
<p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p>
<ul>
<li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li>
<li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.</li>
</ul>
</note> </li>
<li value="7">Click <strong>Save</strong> in the upper-right corner of the Gantt chart.</li>
</ol>
</div>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"> </h2>
-->

