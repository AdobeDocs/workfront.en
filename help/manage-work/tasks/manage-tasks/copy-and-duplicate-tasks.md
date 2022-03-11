---
filename: copy-and-duplicate-tasks
product-area: projects
navigation-topic: manage-tasks
title: Copy and duplicate tasks
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Copy and duplicate tasks

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

You can copy a task from a project to another project, or you can duplicate a task within the same project.

You can copy or duplicate one or several tasks or parent tasks at a time.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Work</span> or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task </p> <p>Contribute or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Considerations for copying tasks

Consider the following when copying a task:

* Issues are not copied with the task.
* Milestones are transferred to the copied task and removed from the original task.

You can copy a task in the following areas of the `Adobe Workfront` web application:

<ul> 
 <li> At the task level, from the More icon to the left of the task name. <p>For information, see the <a href="#copy" class="MCXref xref">Copy a task&nbsp;at the task level</a> section in this article.</p> </li> 
 <li> <p>In a task list, by doing one of the following:</p> 
  <ul> 
   <li> <p>Right-click the name of a task.</p> </li> 
   <li> <p>Select the task (or tasks) and expand the More icon at the top of the task list.</p> </li> 
   <li> <p>Select a task and expanding the <span class="bold">More</span> icon <img src="assets/more-icon-task-list.png"> next to the task name.</p> <p>This option is not available when selecting multiple tasks. </p> </li> 
  </ul> <p>For information, see the <a href="#copy2" class="MCXref xref">Copy tasks in a list</a> section in this article.</p> </li> 
</ul>

## Copy tasks in a list

<ol> 
 <li value="1"> <p>Go to the project that contains the task or tasks that you want to copy.</p> <p>Or</p> <p>Go to a task report. </p> </li> 
 <li value="2"> Click Tasks in the left panel. </li> 
 <li value="3"> Click the Plan mode menu , then Autosave. <note type="important">
   You can copy tasks in a list only when automatically saving your changes. For information about saving options when editing tasks, see 
   <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Edit tasks in a list</a>.
  </note> </li> 
 <li value="4"> Select the task or tasks that you want to copy and do one of the following: Click the More menu at the top of the task list, then click Copy to. Right click the selected tasks, then click Copy to. When selecting one task, click the More menu next to the task name in the list, then click Copy to.  </li> 
 <li value="5"> Continue with copying the task, as described in the section Copy a task at the task level starting with Step 4. </li> 
</ol>

## Copy a task&nbsp;at the task level

In addition to copying tasks in a list of tasks, you can also copy a task after you have opened it.&nbsp;
Find a task in your Workfront system by searching for it. Click the name of the task to open it. Click the More drop-down menu next to the name of the task, then click Copy to. The Copy Task box displays. (Optional) Update the Task Name. Tip: This field is dimmed and not editable when selecting to copy multiple tasks in a list. You can hover over the Task Name field and a list of all selected tasks displays. Type the name of the Destination Project where you want to copy the task in the Select Destination Project field. Tips: The name of the project is case sensitive. You can also start typing the Reference Number or enter the ID of the project. This might help you distinguish between projects with identical names. Only 100 projects display in the list. The current project name displays by default. If you want to copy the task within the same project, leave this field unchanged. (Conditional) Click request access to request access to the project, if you don't have access to the selected project. Continue to copy the task on the selected destination project without request access if you have access to add tasks to one of the tasks on the destination project. Tip: Similar messages display if the project selected is in pending approval or completed or dead, when the Workfront administrator prevents adding tasks to these projects. For more information, see Configure system-wide project preferences. Click Options in the left panel, then deselect the task attributes that you do not want to copy with the task. All options are selected by default. Tip: Selecting then deselecting Select all deselects all the options. Deselect from the following options to not transfer them to the copied task. The following table describes what happens when the options are deselected: Constraint The task constraint is set to As Soon As Possible or As Late As Possible based on the project Schedule Mode setting. When selected, the current constraint of the task transfers to the copied task. Note: When moving or copying a task with date-specific constraints to another project and the constraint dates of the task are outside the dates of the new project, either the Task Constraint changes to As Soon as Possible or As Late as Possible or the Planned Start or Planned Completion dates of the projects are adjusted. Some examples of date-specific constraints are Must Start On, Must Finish On, Start No Earlier Than, Start No Later Than, etc. For information about task constraints and how task constraints or project dates can be affected, see Task Constraint overview and look for a specific constraint. Assignments All the assignments are removed from the task. Approval Process All approval processes are removed from the task. Progress The task status is New. Otherwise, the copied task keeps the status of the existing task. Financial Information The financial information of the task is removed. All Predecessors This means that the dependencies will not carry over to the copied tasks. When selected, the predecessors within the group of copied tasks are preserved, others are deleted. Documents The documents attached to the task are not transferred to the copied task. This includes versions, proofs, and linked documents. This does not include document approvals. Document approvals can never be copied when a task is copied. Reminder Notifications The task reminders do not transfer to the copied task. Expenses The expenses logged on the task do not transfer to the copied task. Permissions Workfront removes the names of all the entities displaying in the Sharing list of the task. Custom Data The values for the custom fields are cleared and the custom forms are transferred to the copied task. When selected, both the forms and the values for the custom fields transfer to the copied task. (Optional) Click Select Parent in the left panel, then select the task in the destination project that you want to become the parent of the copied task. Tip: When selecting to copy multiple tasks in a list, all selected tasks become the children of the selected parent. Select a parent by doing one of the following: In the task list, select one of the parents in the project plan. Click the search icon and search for a parent task by name. The task should appear in the list. Select the radio button for the parent, after you have found it. If you do not select a parent task, the tasks are copied as main tasks rather than subtasks and they will be placed at the end of the task list on the destination project. Click Copy task Or Click Copy tasks when you select multiple tasks in a list. The copied tasks are now on the specified project and are either subtasks to the selected parent task, or the last tasks on the project.  

## Duplicate tasks

You can quickly duplicate a task in a task list, if you need an identical task on the same project.

* [Considerations for duplicating tasks](#consider) 
* [Duplicate tasks](#duplicat)

### Considerations for duplicating tasks

* You can duplicate a task in a task list only when the list is sorted by task number.

* The new task will have the same name as the original task.
* You cannot select what information is duplicated to the new task. Almost all the information from the original task will be transferred to the duplicated task, including parent relationship, by default. 
* The following items are not transferred to the new task:

  * Logged hours
  * Notes
  * Issues
  * Only the predecessors which are in the same group of copied tasks are also copied with their successor tasks.

    ` `**Example: **``For example, if you copy Task 2 and its predecessor, Task 1, at the same time, then you have a copy of Task 2 and a copy of Task 1. The copy of Task 1 will be the predecessor of the copy of Task 2. But if you copy just Task 2 without copying its predecessor, then its copy will have no predecessor.

* When you duplicate a parent task, all children tasks are also duplicated, even when the children tasks are not selected. 
* You can duplicate multiple tasks as the same time.

  However, you cannot duplicate multiple tasks that are not sequential at the same time. 

* Milestones are moved to the new task and removed from the original task.

### Duplicate tasks

1. Go to the project that contains the task or tasks that you want to duplicate.
1. Click Tasks in the left panel. 
1. 
   Do one of the following:

  * (Conditional) Click the Plan mode menu > Autosave, select the tasks you want to duplicate, then click the More menu > Duplicate.

  * (Conditional) Click the Plan mode menu > Manual save > Standard or Timeline Planning, then do the following: 
  * `<li value="1">Select the task or tasks you want to duplicate, and click <span class="bold">Duplicate</span>. </li>` `<li value="2">(Optional) Click <span class="bold">Undo</span> to reverse your changes and not duplicate the tasks.</li>` `<li value="3">(Optional and conditional) Click <span class="bold">Redo</span> if you had previously clicked <span class="bold">Undo</span>, to keep the changes and duplicate the tasks.</li>` `<li value="4">Click <span class="bold">Save</span> to save your changes.</li>`

  1. Edit tasks in a list

