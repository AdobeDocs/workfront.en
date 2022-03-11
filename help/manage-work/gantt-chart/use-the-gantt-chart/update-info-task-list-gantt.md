---
filename: update-info-task-list-gantt
product-area: projects
navigation-topic: use-the-gantt-chart
title: Update information in the task list Gantt Chart
description: The task list Gantt Chart shows details about tasks that are on a project or template.
---

# Update information in the task list Gantt Chart

The task list Gantt Chart shows details about tasks that are on a project or template.

In a template, the task list Gantt Chart reflects updates made in the template's task list at the task level. This Gantt chart is not editable.

In a project, you can update task information directly in the task list Gantt Chart.

You can perform the following actions directly in the Task List Gantt Chart:

* Modify Task Duration
* Create or remove Predecessor relationships
* Change Task Start and End Dates
* Update Percent Complete
* Level Project Resources

## Access requirements

You must have the following to follow the steps in this article:

<table cellspacing="0"> 
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
   <td> <p>Manage access to the project and tasks </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Modify Task Duration

1. Go to the project you want to modify.
1. Click Tasks in the left panel.  
1. Click the Gantt chart icon.  All changes are saved automatically when the `Autosave` option is enabled. It is enabled by default. 
1. (Optional) Click the Plan mode icon and select Manual save Standard or Timeline Planning to save your changes manually.  
1. Hover over the timeline of a task and drag the time line indicator to a different date.
1. Drop the indicator when you have reached the correct new Completion Date for the task. 
1. (Optional and conditional) If you have selected to manually save your changes, click the `Undo` or `Redo` icons if you want to cancel or duplicate any of the changes. 

   ` `**Tip: **`` You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:

  * Mac: Use Command + Z to undo and Command + Shift + Z to redo.
  * Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.

1. Click `Save` in the upper-right corner of the Gantt chart.

## Create or remove Predecessor relationships

<ol> 
 <li value="1">Go to the project you want to modify.</li> In the Tasks area, click the Gantt chart icon. The Autosave option is selected by default, in which case all changes are saved automatically. 
 <li value="3"> (Optional) Click the Plan mode icon and select Manual save Standard or Timeline Planning to save your changes manually.  </li> 
 <br> 
 <li value="4">To create a predecessor relationship, click the start point of a task and drag it to the end point of task. </li> 
 <li value="5"> To delete a predecessor relationship, c lick a predecessor line that connects two tasks to select it, then press <span class="bold">Delete</span> on your keyboard.<br><img src="assets/delete-predecessor-350x152.png" alt="Delete_predecessor.png" style="width: 350;height: 152;"></li> 
 <li value="6"> <p>(Optional and conditional) If you selected to save your changes manually, click the <span class="bold">Undo</span> or<span class="bold"> Redo</span> icons if you want to cancel or duplicate any of the changes. </p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p> 
   <ul> 
    <li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li> 
    <li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.<br></li> 
   </ul> 
  </div> </li> 
 <li value="7">Click <span class="bold">Save</span> .</li> 
</ol>

## Change Task Start and End Dates

<ol> 
 <li value="1"> Go to the project you want to modify. </li> In the Tasks area, click the Gantt chart icon. All changes are saved automatically when the Autosave option is enabled. It is enabled by default. 
 <li value="3"> (Optional) Click the Plan mode icon and select Manual save Standard or Timeline Planning to save your changes manually.  </li> 
 <li value="4">Hover over the center of the task and locate the multi-directional arrow.</li> 
 <li value="5"> <p>Click and drag the task to the desired date.</p> <p> <img src="assets/change-start-end-date.png" alt="Change_start_end_date.png"> </p> </li> 
 <li value="6"> <p>If you change the task date in a way that affects the task constraint, click <span class="bold">Accept</span> to acknowledge the task constraint change.</p> <note type="note"> 
   <p>If the task has one of the following constraints, the system updates the Task Constraint to Start No Earlier Than if the project is scheduled from the Start Date or Finish No Later Than if the project is scheduled from the Completion Date:</p> 
   <ul> 
    <li>As Soon As Possible</li> 
    <li>As Late As Possible</li> 
    <li>Earliest Available Time</li> 
    <li>Latest Available Time</li> 
   </ul> 
   <p>In some cases, the predecessor relationships might prevent the tasks from starting earlier, and the task move is not allowed. </p> 
  </note> </li> 
 <li value="7"> <p>(Optional and conditional) If you have selected to save your changes manually, click the <span class="bold">Undo</span> or<span class="bold"> Redo</span> icons if you want to cancel or duplicate any of the changes. </p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p> 
   <ul> 
    <li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li> 
    <li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.<br></li> 
   </ul> 
  </div> </li> 
 <li value="8">Click <span class="bold">Save</span>. </li> 
</ol>

## Update Percent Complete

<ol> 
 <li value="1">Go to the project you want to modify.</li> 
 <li value="2"> In the Tasks area, click the Gantt chart icon.  All changes are saved automatically when the Autosave option is enabled. It is enabled by default. </li> 
 <li value="3"> (Optional) Click the Plan mode icon and select Manual save Standard or Timeline Planning to save your changes manually. </li> 
 <li value="4"> <p>Double-click the percent number inside of the task and enter the number. </p> <note type="important"> 
   <p> You must have % Complete selected in the Options dialog in order to update percent complete. To do this, click the <span class="bold">Options</span> icon and select <span class="bold">% Complete</span>.</p> 
   <p> <img src="assets/update-percent-complete-350x175.png" alt="update_percent_complete.png" style="width: 350;height: 175;"> </p> 
  </note> </li> 
 <li value="5"> <p>(Optional and conditional) If you selected to save your changes manually, click the <span class="bold">Undo</span> or<span class="bold"> Redo</span> icons if you want to cancel or duplicate any of the changes. </p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p> 
   <ul> 
    <li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li> 
    <li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.<br></li> 
   </ul> 
  </div> </li> 
 <li value="6">Click <span class="bold">Save</span> in the upper-right corner of the Gantt chart.</li> 
</ol>

## Level Project Resources

You can use the Task List Gantt Chart to level your resources. For information on about leveling resources in the Gantt chart, see [Level Resources in the Gantt Chart](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

<ol> 
 <li value="1">Go to the project you want to level.</li> 
 <li value="2"> In the Tasks area, click the Gantt chart icon. All changes are saved automatically when the Autosave option is enabled. It is enabled by default. </li> 
 <li value="3"> 
  <div> (Optional) Click the Plan mode icon and select Manual save Standard or Timeline Planning to save your changes manually.  
  </div> </li> 
 <li value="4"> <p>Click the <span class="bold">Level Resources</span> drop-down menu.</p> <p> <img src="assets/level-resouces.png" alt="Level_resouces.png"> </p> </li> 
 <li value="5">Select one of following options: 
  <ul>
   <li><span class="bold">Level Now</span>: Applies resource leveling to the selected task.</li>
   <li><span class="bold">Clear Leveling</span>: Removes all resource leveling from the selected task.</li>
  </ul></li> 
 <li value="6"> <p>(Optional and conditional) If you have disabled the Autosave option, click the <span class="bold">Undo</span> or<span class="bold"> Redo</span> icons if you want to cancel or duplicate any of the changes. </p> <note type="tip"> 
   <p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p> 
   <ul> 
    <li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li> 
    <li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.</li> 
   </ul> 
  </note> </li> 
 <li value="7">Click <span class="bold">Save</span> in the upper-right corner of the Gantt chart.</li> 
</ol>

<!--
Editing the Task List in Gantt Chart Edit Mode
-->

<!--
You can keep the edit mode enabled mode in the Gantt chart to preview changes made in the task list before saving. This allows you to try out what-if scenarios to understand how changes can affect your project timeline. If the Gantt chart is not in edit mode, inline edits are permanent.
-->

<!--
Note: When making changes affecting the timeline (such as dates and durations), the system performs timeline calculations and provides a new state of the project as if the change is actually committed. However, the changes are not permanently applied to the project until they are saved. Undoing the action should change the project timeline back to the previous state.
-->

<!--
In the Preview environment, you can edit the task list with or without the Gantt Chart enabled.
-->

<!--
If you want to reverse the changes you make to the task list in the Preview environment, you must disable the Autosave icon.
-->

<!--
For information about editing the task list in the Preview environment, see Editing tasks.
-->

<!--
You can perform the following actions directly in the task list while the Gantt chart is in edit mode in the Production environment:
-->

  <!--
  Add or Remove Tasks
  -->

  <!--
  Edit Task Fields
  -->

<!--
Add or Remove Tasks
-->

<!--
To preview how adding or removing tasks impacts the project timeline:
-->

   <!--
   Go to a project for which you want to edit tasks.
   -->

1. 

   <!--
   On the Tasks tab, click the Gantt chart icon in the upper-right corner.
   -->

   <!--
   All changes are saved automatically when the Autosave option is enabled. It is enabled by default.
   -->

1. 

   <!--
   (Optional) Disable the Autosave toggle.
   -->

   <!--

   -->

   <!--
   To add tasks to the task list: If you have no tasks in the task list, click Start Adding Tasks. If you need to add tasks , click Add More Tasks.
   -->

   <!--
   To remove a task, select the task, then click Delete.
   -->

1. 

   <!--
   (Optional and conditional) If you have disabled the Autosave option, click the Undo or Redo icons if you want to cancel or duplicate any of the changes.
   -->

   <!--

   -->

   ` `**Tip: **`` 

   <!--
   You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:
   -->

    <!--  
    Mac: Use Command + Z to undo and Command + Shift + Z to redo.  
    -->

    <!--  
    Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.  
    -->

   <!--
   To commit the changes to the project, click Save. Or To discard the changes, click the Cancel icon.
   -->

<!--
Edit Task Fields
-->

<!--
To preview how editing task fields impacts the project:
-->

<ol> <!--
  Go to a project for which you want to edit tasks.
 --> 
 <li value="2"> <!--
   On the Tasks tab, click the Gantt chart icon in the upper-right corner.
  --> <!--
   In the Tasks tab, click the Gantt chart icon in the upper-right corner.
  --> <!--
   All changes are saved automatically when the Autosave option is enabled. It is enabled by default.
  --> </li> 
 <li value="3"> 
  <div> <!--
    (Optional) Disable the Autosave toggle.
   --> <!--
   --> 
  </div> </li> 
 <li value="4"> <!--
   You can update any inline editable fields that display in the task list. The fields displayed vary depending on what View you select for your task list.
  --> <note type="note"> 
   <!--
    The ability to edit the Duration, Planned Hours, Planned Start Date, and Completion Date of the tasks depends on the Task Constraint and Duration Type. Not all Task Constraints and Duration Types allow for these fields to be edited.
   --> 
   <!--
    For more information about Task Constraint, see Task Constraint overview.
   --> 
   <!--
    For more information about Task Duration Type, see Overview of Task Duration and Duration Type.
   --> 
  </note> </li> 
 <li value="5"> <!--
   (Optional and conditional) If you have disabled the Autosave option, click the Undo or Redo icons if you want to cancel or duplicate any of the changes.
  --> <!--
  --> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> <!--
    You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:
   --> 
   <ul> <!--
     Mac: Use Command + Z to undo and Command + Shift + Z to redo.
    --> <!--
     Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.
    --> 
   </ul> 
  </div> </li> <!--
  To officially commit the changes to the project, click Save. Or To discard the changes, click the Cancel icon.
 --> 
</ol>

