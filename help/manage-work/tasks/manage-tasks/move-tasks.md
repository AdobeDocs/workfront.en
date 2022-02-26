---
filename: move-tasks
product-area: projects
navigation-topic: manage-tasks
title: Move tasks
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Move tasks

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

You can move tasks in *Adobe Workfront* between the following objects:

* An ad hoc task to a project.
* A task from a project to another project.
* A task from a project under a different parent in another project. 
* A task within the same project under a different parent.

You can move a task at the task level or you can move a task from a list of tasks.

## Access requirements

You must have the following access to perform the actions in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> licenses*</td> 
   <td> <p><em>Work</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks</p> <p>Contribute or higher permissions to the project with ability to Add Tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Move a task in a list

To move a task displayed in a task list:

<ol> 
 <li value="1">Go to the project that contains the task or tasks that you want to move.</li> 
 <li value="2"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Tasks</span> in the left panel to display the task list.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Tasks</span> in the left panel to display the task list.
  </MadCap:conditionalText> </li> 
 <li value="3"> 
  <div> 
   <p>Ensure that the <span class="bold">Autosave</span> toggle is enabled, then select the task or tasks that you want to move. </p> 
   <p> <img src="assets/autosave-icon-on-highlighted-350x202.png" style="width: 350;height: 202;"> </p> <note type="important">
    You cannot move tasks when the 
    <span class="bold">Autosave</span> toggle is disabled. 
    <br>
   </note> 
  </div> </li> 
 <li value="4"> <p>(Optional and conditional) If you want to move the selected tasks within the same project, click the tasks you selected, drag them and drop them where you want them moved on the project.</p> <p>After you dropped the tasks in the correct place on the project, the changes you made to the task hierarchy are saved immediately. All the information associated with each task is moved with the tasks.</p> </li> 
 <li value="5"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Conditional) Select the task or tasks that you want to move and do one of the following:</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Conditional) Select the task or tasks that you want to move and do one of the following:</p> <draft-comment>
   <ul data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
    <li> <p>Click the More menu <img src="assets/qs-more-menu.png"> at the top of the task list, then click <span class="bold">Move to</span>. </p> </li> 
    <li> <p>Right click the selected tasks, then click <span class="bold">Move to</span>.</p> </li> 
    <li> <p>When selecting one task, click the <span class="bold">More</span> menu <img src="assets/more-icon-task-list.png"> next to the task name in the list, then click&nbsp;<span class="bold">Move to</span>. </p> </li> 
   </ul>
  </draft-comment>
  <ul data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <li> <p>Click the More menu <img src="assets/qs-more-menu.png"> at the top of the task list, then click <span class="bold">Move to</span>. </p> </li> 
   <li> <p>Right click the selected tasks, then click <span class="bold">Move to</span>.</p> </li> 
   <li> <p>When selecting one task, click the <span class="bold">More</span> menu <img src="assets/more-icon-task-list.png"> next to the task name in the list, then click&nbsp;<span class="bold">Move to</span>. </p> </li> 
  </ul> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/move-task-in-list-nwe-350x119.png" style="width: 350;height: 119;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/move-task-in-list-nwe-350x119.png" style="width: 350;height: 119;"> </p> <p>The Move Task box displays</p> </li> 
 <li value="6"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Continue with moving the task, as described in the section <a href="#moving-one-task" class="MCXref xref">Move a task&nbsp;at the task level</a> in this article, starting with Step 4.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Continue with moving the task, as described in the section <a href="#moving-one-task" class="MCXref xref">Move a task&nbsp;at the task level</a> in this article, starting with Step 4.</p> </li> 
</ol>

## Move a task&nbsp;at the task level

In addition to moving tasks from a list of tasks, you can also move a task at the task level, after you have opened it.&nbsp;

<!--
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<ol>
<li value="1">Find a task in your <em>Workfront</em> system by searching for it.</li>
<li value="2">Click the name of the task to open it.&nbsp;</li>
<li value="3"> <p>Click the <span class="bold">More</span> drop-down menu <img src="assets/qs-more-menu.png"> next to the name of the task, then click <span class="bold">Move</span><span class="bold"> to</span>. The Move Task box displays. </p> <p> <img src="assets/move-task-at-task-level-nwe-350x222.png" style="width: 350;height: 222;"> </p> </li>
<li value="4"> <p>(Optional) Update the <span class="bold">Task Name</span>. The task moves with the new name in the new location. <em>Workfront</em> does not record the original name of the task.</p>
<div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
<span class="autonumber"><span><b>Tip: </b></span></span>
<p>This field is dimmed and not editable when selecting to move multiple tasks in <span data-mc-edit-date="2021-11-04T09:17:43.3878352-04:00" data-mc-editor="alinaw" data-mc-comment="keep yellow for preview release 22.1" data-mc-initials="AL" data-mc-creator="alinaw" data-mc-create-date="2021-11-03T15:36:51.6009888-04:00">a</span><span> list. You can hover over the Task Name field and a list of all selected tasks displays.</span></p>
<p> <img src="assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png" style="width: 350;height: 142;"> </p>
</div> </li>
<li value="5"> <p>Type the name of the <span class="bold">Destination Project</span>&nbsp;where you want the task to move&nbsp;in the <span class="bold">Select Destination Project</span> field.&nbsp;</p> <p>If you want to move the task within the same project, type the name of the current project.</p>
<div class="tips" data-mc-autonum="<b>Tips: </b>">
<span class="autonumber"><span><b>Tips: </b></span></span>
<ul>
<li> <p>The name of the project is case sensitive. </p> </li>
<li> <p>You can also start typing the Reference Number or enter the ID of the project. This might help you distinguish between projects with identical names. </p> </li>
<li> <p>Only 100 projects display in the list.</p> </li>
</ul>
</div> </li>
<li value="6"> <p>(Conditional)&nbsp;Click&nbsp;<span class="bold">request access</span> to request access to the project, if you don't have access to the selected project. </p> <draft-comment>
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Continue to move the task on the selected destination project without requesting access if you have access to add tasks to one of the tasks on the destination project. </p>
</draft-comment><p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Continue to move the task on the selected destination project without requesting access if you have access to add tasks to one of the tasks on the destination project. </p> <p> <img src="assets/move-task-request-access-from-project-nwe-350x156.png" style="width: 350;height: 156;"> </p> </li>
<li value="7"> <p>(Optional) Click&nbsp;<span class="bold">Options</span> in the left panel</p> <p>Or </p> <p>Scroll down to the <span class="bold">Options</span> section in the Move Task box, then deselect any of the items listed in the table below to remove&nbsp;them&nbsp;from&nbsp;the moved tasks . All options are selected by default. </p> <note type="important">
Deselecting items in the Options list results in loss of data. Information from the existing task will be removed and cannot be recovered.
</note>
<table cellspacing="0">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Select all</td>
<td>Deselect this option to remove all information from the task when moving it to its new location. </td>
</tr>
<tr>
<td role="rowheader">Constraint</td>
<td> <p>The task constraint is set to As Soon As Possible or As Late As Possible based on the project Schedule Mode setting.</p> <p> When selected, the current constraint of the task transfers with the task. </p> <note type="note">
When moving or copying a task with date-specific constraints to another project and the constraint dates of the task are outside the dates of the new project, either the Task&nbsp;Constraint changes to As Soon as Possible or As Late as Possible or the Planned Start or Planned Completion dates of the projects are adjusted. Some examples of date-specific constraints are Must Start On, Must&nbsp;Finish On, Start No Earlier Than, Start No Later Than, etc. For information about task constraints and how task constraints or project dates can be affected, see
<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a> and look for a specific constraint.
</note> </td>
</tr>
<tr>
<td role="rowheader">Assignments</td>
<td> <p>All the assignments are removed from the task. </p> </td>
</tr>
<tr>
<td role="rowheader">Approval Process</td>
<td>All approval processes are removed from the task.</td>
</tr>
<tr>
<td role="rowheader">Progress</td>
<td>The task status is New. Otherwise, the existing task status is preserved. </td>
</tr>
<tr>
<td role="rowheader">Financial Information</td>
<td>The financial information of the task is removed and the <em>Workfront</em> updates the task&nbsp;Cost Type to No Cost and the task Revenue Type as Not Billable. </td>
</tr>
<tr>
<td role="rowheader">All&nbsp;Predecessors</td>
<td> <p>When selected, the dependency becomes a cross-project predecessor when you move the task to another project. </p> </td>
</tr>
<tr>
<td role="rowheader">Documents</td>
<td> <p>The documents attached to the task are not transferred to the moved task. This includes versions, <em>proofs</em>, and linked documents.</p> <p>This does not include document approvals. Document approvals can never be moved when a task is moved.</p> </td>
</tr>
<tr>
<td role="rowheader">Reminder Notifications</td>
<td>The task reminders do not transfer to the moved task. </td>
</tr>
<tr>
<td role="rowheader">Expenses</td>
<td>The expenses logged on the task do not transfer to the moved task. </td>
</tr>
<tr>
<td role="rowheader">Permissions</td>
<td> <p><em>Workfront</em> removes the names of all the entities displaying in the Sharing list of the task. </p> </td>
</tr>
</tbody>
</table> </li>
<li value="8"> <p>&nbsp;</p> </li>
<li value="9"> <p>(Optional) Click <span class="bold">Select Parent</span> in the left panel</p> <p>Or</p> <p>Scroll to the <span class="bold">Select Parent</span> section, then select the task in the destination project that you want to become the parent of the moved task. </p> <note type="tip">
<span>When selecting to move multiple tasks in a list, all selected tasks become the children of the selected parent.</span>
</note> <p>Select a parent by doing one of the following:</p>
<ul>
<li> <p>In the task list, select one of the parents in the project plan.</p> </li>
<li> <p>Click the search icon <img src="assets/search-icon.png" alt="Search icon"> and search for a parent task by name. </p> </li>
</ul> <p>The task should appear in the list.</p> <p> <img src="assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png" alt="Select parent task when moving a task with search functionality " style="width: 350;height: 110;"> </p> </li>
<li value="10"> <p>Select the radio button for the parent, after you have found it.&nbsp;</p> <p>If you do not select a parent task, the tasks are moved&nbsp;as main tasks rather than subtasks and they&nbsp;will be placed at the end of the task list on the destination project.&nbsp;</p> </li>
<li value="11">
<div>
<p>Click <span class="bold">Move task</span></p>
<p>Or</p>
<p>Click <span class="bold">Move tasks</span> when you select multiple tasks in a list. </p>
</div> <p>The moved&nbsp;tasks are&nbsp;now on the specified project and&nbsp;are either subtasks to a parent task, or the last tasks on the project.<br></p> </li>
</ol>
</div>
-->

<ol> 
 <li value="1">Find a task in your <em>Workfront</em> system by searching for it.</li> 
 <li value="2">Click the name of the task to open it.&nbsp;</li> 
 <li value="3"> <p>Click the <span class="bold">More</span> drop-down menu <img src="assets/qs-more-menu.png"> next to the name of the task, then click <span class="bold">Move</span><span class="bold"> to</span>. The Move Task box displays. </p> <p> <img src="assets/move-task-at-task-level-nwe-350x222.png" style="width: 350;height: 222;"> </p> </li> 
 <li value="4"> <p>(Optional) Update the <span class="bold">Task Name</span>. The task moves with the new name in the new location. <em>Workfront</em> does not record the original name of the task.</p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>This field is dimmed and not editable when selecting to move multiple tasks in <span data-mc-edit-date="2021-11-04T09:17:43.3878352-04:00" data-mc-editor="alinaw" data-mc-comment="keep yellow for preview release 22.1" data-mc-initials="AL" data-mc-creator="alinaw" data-mc-create-date="2021-11-03T15:36:51.6009888-04:00">a</span><span> list. You can hover over the Task Name field and a list of all selected tasks displays.</span></p> 
   <p> <img src="assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png" style="width: 350;height: 142;"> </p> 
  </div> </li> 
 <li value="5"> <p>Type the name of the <span class="bold">Destination Project</span>&nbsp;where you want the task to move&nbsp;in the <span class="bold">Select Destination Project</span> field.&nbsp;</p> <p>If you want to move the task within the same project, type the name of the current project.</p> 
  <div class="tips" data-mc-autonum="<b>Tips: </b>">
   <span class="autonumber"><span><b>Tips: </b></span></span> 
   <ul> 
    <li> <p>The name of the project is case sensitive. </p> </li> 
    <li> <p>You can also start typing the Reference Number or enter the ID of the project. This might help you distinguish between projects with identical names. </p> </li> 
    <li> <p>Only 100 projects display in the list.</p> </li> 
   </ul> 
  </div> </li> 
 <li value="6"> <p>(Conditional)&nbsp;Click&nbsp;<span class="bold">request access</span> to request access to the project, if you don't have access to the selected project. </p> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Continue to move the task on the selected destination project without requesting access if you have access to add tasks to one of the tasks on the destination project. </p> <p> <img src="assets/move-task-request-access-from-project-nwe-350x156.png" style="width: 350;height: 156;"> </p> </li> 
 <li value="7"> <p>(Optional) Click&nbsp;<span class="bold">Options</span> in the left panel</p> <p>Or </p> <p>Scroll down to the <span class="bold">Options</span> section in the Move Task box, then deselect any of the items listed in the table below to remove&nbsp;them&nbsp;from&nbsp;the moved tasks . All options are selected by default. </p> <note type="important">
   Deselecting items in the Options list results in loss of data. Information from the existing task will be removed and cannot be recovered. 
  </note> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Select all</td> 
     <td>Deselect this option to remove all information from the task when moving it to its new location. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Constraint</td> 
     <td> <p>The task constraint is set to As Soon As Possible or As Late As Possible based on the project Schedule Mode setting.</p> <p> When selected, the current constraint of the task transfers with the task. </p> <note type="note">
       When moving or copying a task with date-specific constraints to another project and the constraint dates of the task are outside the dates of the new project, either the Task&nbsp;Constraint changes to As Soon as Possible or As Late as Possible or the Planned Start or Planned Completion dates of the projects are adjusted. Some examples of date-specific constraints are Must Start On, Must&nbsp;Finish On, Start No Earlier Than, Start No Later Than, etc. For information about task constraints and how task constraints or project dates can be affected, see 
       <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a> and look for a specific constraint.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Assignments</td> 
     <td> <p>All the assignments are removed from the task. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Approval Process</td> 
     <td>All approval processes are removed from the task.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Progress</td> 
     <td>The task status is New. Otherwise, the existing task status is preserved. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Financial Information</td> 
     <td>The financial information of the task is removed and the <em>Workfront</em> updates the task&nbsp;Cost Type to No Cost and the task Revenue Type as Not Billable. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">All&nbsp;Predecessors</td> 
     <td> <p>When selected, the dependency becomes a cross-project predecessor when you move the task to another project. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Documents</td> 
     <td> <p>The documents attached to the task are not transferred to the moved task. This includes versions, <em>proofs</em>, and linked documents.</p> <p>This does not include document approvals. Document approvals can never be moved when a task is moved.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Reminder Notifications</td> 
     <td>The task reminders do not transfer to the moved task. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Expenses</td> 
     <td>The expenses logged on the task do not transfer to the moved task. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Permissions</td> 
     <td> <p><em>Workfront</em> removes the names of all the entities displaying in the Sharing list of the task. </p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="8"> <p>&nbsp;</p> </li> 
 <li value="9"> <p>(Optional) Click <span class="bold">Select Parent</span> in the left panel</p> <p>Or</p> <p>Scroll to the <span class="bold">Select Parent</span> section, then select the task in the destination project that you want to become the parent of the moved task. </p> <note type="tip">
   <span>When selecting to move multiple tasks in a list, all selected tasks become the children of the selected parent.</span> 
  </note> <p>Select a parent by doing one of the following:</p> 
  <ul> 
   <li> <p>In the task list, select one of the parents in the project plan.</p> </li> 
   <li> <p>Click the search icon <img src="assets/search-icon.png" alt="Search icon"> and search for a parent task by name. </p> </li> 
  </ul> <p>The task should appear in the list.</p> <p> <img src="assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png" alt="Select parent task when moving a task with search functionality " style="width: 350;height: 110;"> </p> </li> 
 <li value="10"> <p>Select the radio button for the parent, after you have found it.&nbsp;</p> <p>If you do not select a parent task, the tasks are moved&nbsp;as main tasks rather than subtasks and they&nbsp;will be placed at the end of the task list on the destination project.&nbsp;</p> </li> 
 <li value="11"> 
  <div> 
   <p>Click <span class="bold">Move task</span></p> 
   <p>Or</p> 
   <p>Click <span class="bold">Move tasks</span> when you select multiple tasks in a list. </p> 
  </div> <p>The moved&nbsp;tasks are&nbsp;now on the specified project and&nbsp;are either subtasks to a parent task, or the last tasks on the project.<br></p> </li> 
</ol>

