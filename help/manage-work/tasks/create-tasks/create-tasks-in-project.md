---
filename: create-tasks-in-project
product-area: projects
navigation-topic: create-tasks
title: Create tasks in a project
description: You can create tasks in a project only after you created the project.
---

# Create tasks in a project

You can create tasks in a project only after you created the project.

For example, after creating a project, you might want to add tasks and modify them to organize the project plan. For more information about creating a project, see [Create a project](../../../manage-work/projects/create-projects/create-project.md).

For information about creating personal tasks that are not in a project, see the "Create a personal task" section in the article [Create work items from the Home area](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

This article describes how you create tasks from scratch. You can also create tasks in the following ways:

* By copying or duplicating existing tasks.&nbsp;For information, see [Copy and duplicate tasks](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* By moving tasks from one project to another.&nbsp;For information, see [Move tasks](../../../manage-work/tasks/manage-tasks/move-tasks.md).

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
   <td role="rowheader"> <p role="rowheader"><em>Adobe Workfront</em> license*</p> </td> 
   <td> <p><em>Work</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task in&nbsp;Adobe Workfront</a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2><a name="Create2"></a>Create tasks in a project</h2>
<ol>
<li value="1">Go to the project where you want to create a task.</li>
<li value="2">Click <span class="bold">Tasks</span> in the left panel. </li>
<li value="3"> <p>(Conditional) If you are currently viewing the task list in an agile view, click the <span class="bold">List View</span> icon <img src="assets/list-view-in-agile-view-for-tasks.png"> in the upper-right corner to display the task list. </p> </li>
<li value="4"> <p>(Optional) Click the <span class="bold">Plan Mode</span> icon <img src="assets/nwe-plan-mode-icon-task-list.png"> and select <span class="bold">Manual Save</span>, then select either <span class="bold">Standard</span> or <span class="bold">Timeline Planning</span>. This disables the <span class="bold">Autosave</span> option which is enabled by default. </p> <draft-comment>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-autosave-off-manual-highlighted-350x58.png" style="width: 350;height: 58;"> </p>
</draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-autosave-off-manual-highlighted-350x58.png" style="width: 350;height: 58;"> </p> <note type="tip">
You can reverse your changes when you select Manual Save.
</note> </li>
<li value="5"> <p>Create a new task by doing one of the following: </p>
<ul>
<li> <p>Click <span class="bold">New Task</span> at the top of the task list</p> </li>
<li> <p>Click <span class="bold">Add More Tasks</span> at the bottom of the task list</p> </li>
</ul> <p> <draft-comment>
<img src="assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png" style="width: 350;height: 242;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
</draft-comment><img src="assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png" style="width: 350;height: 242;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="6"> <p>(Conditional)&nbsp;If you clicked <span class="bold">New Task</span> do the following:</p>
<ol>
<li value="1"> <p>Specify any of the fields on the limited list of fields inside the <span class="bold">New Task</span> box, then click&nbsp;<span class="bold">Create Task</span> if you want to quickly create a task.</p> <p>Or</p> <p>To update all fields for the task, click <span class="bold">More Options</span> to open the <span class="bold">Create Task</span> box.</p> <p> <draft-comment>
<img src="assets/nwe-create-task-small-screen-350x272.png" style="width: 350;height: 272;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
</draft-comment><img src="assets/nwe-create-task-small-screen-350x272.png" style="width: 350;height: 272;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The <span class="bold">Create Task</span> box opens. </p> <p> <img src="assets/create-task-larger-box-nwe-350x244.png" style="width: 350;height: 244;"> </p> <p>&nbsp;</p> <note type="note">
Depending on how your
<em>Workfront administrator</em> sets up our Layout Template, the fields in the Create Task box might display different fields in your environment. For information, see
<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md" class="MCXref xref">Customize the Details view using a layout template</a>.
</note> </li>
<li value="2"> <p>Specify information for the following areas in the left panel of the Create Task box:</p>
<ul>
<li> <p>Task Name</p> </li>
<li> <p>Overview</p> </li>
<li> <p>Assignments</p> </li>
<li> <p>Custom&nbsp;Forms</p> </li>
<li> <p>Finance</p> </li>
<li> <p>Settings</p> <p>For information about defining all task-related fields on a task, see <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>. </p> </li>
</ul> </li>
<li value="3"> <p>(Conditional and optional) If you want the task to be recurring, update the <span class="bold">Recurrence Frequency</span> field. For more information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>.</p> </li>
<li value="4"> <p>(Optional) Click <span class="bold">Documents</span> in the left panel to attach a document to the new task, then click <span class="bold">Add or link files</span> to add a document to the task from your computer, another service, or to link documents and folders from your computer or another service.</p> </li>
</ol> </li>
<li value="7"> <p>(Conditional) If you clicked <span class="bold">Add More Tasks</span> in step 5, start entering the task information using in-line editing, then press Enter.</p> <p>We recommend using this option especially when adding multiple tasks to the list. </p> <p> <img src="assets/ctp4-350x26.png" alt="" style="width: 350;height: 26;"> </p> </li>
<li value="8"> <p>(Conditional) Do one of the following:</p>
<ul>
<li> <p>If you clicked <span class="bold">New Task</span> in step 5, click <span class="bold">Create task</span> to save your changes and add the new task to your project..</p> </li>
<li> <p>If you clicked <span class="bold">Add More Tasks</span> in step 5 do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1"> <p>Click anywhere in the browser to submit your changes, or press Enter.</p> </li>
<li value="2"> <p> (Optional) In the task list, select the newly created task, then click <span class="bold">Indent</span>. </p> <p>This makes the new task a child or subtask of the previous task. </p> <p>For more information about children tasks, see <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Tasks overview</a>. </p> </li>
<li value="3"> <p>(Conditional) If you disabled the <span class="bold">Autosave</span> option after pressing <span class="bold">Add More Tasks</span>, you may do the following: </p>
<ul>
<li> <p>Click <span class="bold">Undo</span> at any time to reverse your last change, or <span class="bold">Cancel</span> to reverse all the changes you made to the task list. </p> </li>
<li> <p>If you previously clicked <span class="bold">Undo</span>, click <span class="bold">Redo</span> to re-apply the last change you canceled.</p> </li>
<li>Click <span class="bold">Save</span> to save your changes to the task list. </li>
</ul> </li>
</ol> </li>
</ul> </li>
</ol>
</div>
-->

## Create tasks in a project

<ol> 
 <li value="1">Go to the project where you want to create a task.</li> 
 <li value="2">Click <span class="bold">Tasks</span> in the left panel. </li> 
 <li value="3"> <p>(Conditional) If you are currently viewing the task list in an agile view, click the <span class="bold">List View</span> icon <img src="assets/list-view-in-agile-view-for-tasks.png"> in the upper-right corner to display the task list. </p> </li> 
 <li value="4"> <p>(Optional) Click the <span class="bold">Plan Mode</span> icon <img src="assets/nwe-plan-mode-icon-task-list.png"> and select <span class="bold">Manual Save</span>, then select either <span class="bold">Standard</span> or <span class="bold">Timeline Planning</span>. This disables the <span class="bold">Autosave</span> option which is enabled by default. </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-autosave-off-manual-highlighted-350x58.png" style="width: 350;height: 58;"> </p> <note type="tip">
   You can reverse your changes when you select Manual Save.
  </note> </li> 
 <li value="5"> <p>Create a new task by doing one of the following: </p> 
  <ul> 
   <li> <p>Click <span class="bold">New Task</span> at the top of the task list</p> </li> 
   <li> <p>Click <span class="bold">Add More Tasks</span> at the bottom of the task list</p> </li> 
  </ul> <p> <img src="assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png" style="width: 350;height: 242;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="6"> <p>(Conditional)&nbsp;If you clicked <span class="bold">New Task</span> do the following:</p> 
  <ol> 
   <li value="1"> <p>Specify any of the fields on the limited list of fields inside the <span class="bold">New Task</span> box, then click&nbsp;<span class="bold">Create Task</span> if you want to quickly create a task.</p> <p>Or</p> <p>To update all fields for the task, click <span class="bold">More Options</span> to open the <span class="bold">Create Task</span> box.</p> <p> <img src="assets/nwe-create-task-small-screen-350x272.png" style="width: 350;height: 272;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The <span class="bold">Create Task</span> box opens. </p> <p> <img src="assets/create-task-larger-box-nwe-350x244.png" style="width: 350;height: 244;"> </p> <p>&nbsp;</p> <note type="note">
     Depending on how your 
     <em>Workfront administrator</em> sets up our Layout Template, the fields in the Create Task box might display different fields in your environment. For information, see 
     <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md" class="MCXref xref">Customize the Details view using a layout template</a>.
    </note> </li> 
   <li value="2"> <p>Specify information for the following areas in the left panel of the Create Task box:</p> 
    <ul> 
     <li> <p>Task Name</p> </li> 
     <li> <p>Overview</p> </li> 
     <li> <p>Assignments</p> </li> 
     <li> <p>Custom&nbsp;Forms</p> </li> 
     <li> <p>Finance</p> </li> 
     <li> <p>Settings</p> <p>For information about defining all task-related fields on a task, see <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>. </p> </li> 
    </ul> </li> 
   <li value="3"> <p>(Conditional and optional) If you want the task to be recurring, update the <span class="bold">Recurrence Frequency</span> field. For more information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>.</p> </li> 
   <li value="4"> <p>(Optional) Click <span class="bold">Documents</span> in the left panel to attach a document to the new task, then click <span class="bold">Add or link files</span> to add a document to the task from your computer, another service, or to link documents and folders from your computer or another service.</p> </li> 
  </ol> </li> 
 <li value="7"> <p>(Conditional) If you clicked <span class="bold">Add More Tasks</span> in step 5, start entering the task information using in-line editing, then press Enter.</p> <p>We recommend using this option especially when adding multiple tasks to the list. </p> <p> <img src="assets/ctp4-350x26.png" alt="" style="width: 350;height: 26;"> </p> </li> 
 <li value="8"> <p>(Conditional) Do one of the following:</p> 
  <ul> 
   <li> <p>If you clicked <span class="bold">New Task</span> in step 5, click <span class="bold">Create task</span> to save your changes and add the new task to your project..</p> </li> 
   <li> <p>If you clicked <span class="bold">Add More Tasks</span> in step 5 do the following:</p> 
    <ol style="list-style-type: lower-alpha;"> 
     <li value="1"> <p>Click anywhere in the browser to submit your changes, or press Enter.</p> </li> 
     <li value="2"> <p> (Optional) In the task list, select the newly created task, then click <span class="bold">Indent</span>. </p> <p>This makes the new task a child or subtask of the previous task. </p> <p>For more information about children tasks, see <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Tasks overview</a>. </p> </li> 
     <li value="3"> <p>(Conditional) If you disabled the <span class="bold">Autosave</span> option after pressing <span class="bold">Add More Tasks</span>, you may do the following: </p> 
      <ul> 
       <li> <p>Click <span class="bold">Undo</span> at any time to reverse your last change, or <span class="bold">Cancel</span> to reverse all the changes you made to the task list. </p> </li> 
       <li> <p>If you previously clicked <span class="bold">Undo</span>, click <span class="bold">Redo</span> to re-apply the last change you canceled.</p> </li> 
       <li>Click <span class="bold">Save</span> to save your changes to the task list. </li> 
      </ul> </li> 
    </ol> </li> 
  </ul> </li> 
</ol>

