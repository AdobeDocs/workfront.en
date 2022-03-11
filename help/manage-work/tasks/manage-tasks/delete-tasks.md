---
filename: delete-tasks
product-area: projects
navigation-topic: manage-tasks
title: Delete tasks
description: You can delete tasks that might be duplicates, or have been created in error.
---

# Delete tasks

##  

You can delete tasks that might be duplicates, or have been created in error.

For tasks that have historical information (updates, changes of schedule, status, or other fields), we recommend that you close them or mark them Dead, instead of deleting them.&nbsp;This helps you keep the historical information for your projects.

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
   <td> <p><span>Work</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects with access to&nbsp;Delete</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task in&nbsp;Adobe Workfront</a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Understand the process of deleting tasks

* [Limitations for deleting tasks](#access-and-permissions-needed) 
* [The impact of deleting tasks](#the-impact-of-deleting-tasks)

### Limitations for deleting tasks

* When a project has a status of Complete you can delete tasks only if your `Workfront administrator` `or a `group administrator`` has allowed this in your Project Preferences area. For information about setting up project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* If the task has logged hours, the `Workfront` ` `or `group administrator``` must allow the deletion of these tasks by configuring the Task & Issue Preferences in your `Workfront` instance. This also applies when you try to delete projects that have tasks with hours logged on them.

  For more information about enabling the deletion of tasks where hours are logged, see the "Deletion" section in [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### The impact of deleting tasks

When you delete a task, you impact other objects linked to the task.

The following objects attached to a task are also deleted when you delete a task:

* Documents

  You cannot delete a task that has a document which has been checked out attached to it. For more information about checking out documents, see [Check out documents](../../../documents/managing-documents/check-out-documents.md).

* Issues
* Subtasks
* Notes
* Approvals

Depending on how your `Workfront administrator` configures the Project, Task, or Issue Deletion Preferences in the Timesheet & Hour Preferences of your `Workfront` instance, hours logged for the tasks are handled in one of the following ways when deleting a task:

* Move to the project and will not be restored on the task, if the task is later restored.
* Are deleted and will be restored on the task, if the task is later restored.
  This also applies when you try to delete projects that have tasks with hours logged on them. 

  For more information about configuring the deletion preferences for hours logged on issues, see [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Expenses on the task will move to the project.

* The users assigned to the task or to the task approval remain on the project team.

  For more information about project teams, see [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Delete tasks

* [Delete multiple tasks in a project simultaneously](#delete-tasks-in-a-project-task-list) 
* [Delete a single task](#delete-a-task)

### Delete multiple tasks in a project simultaneously

<ol> 
 <li value="1"> Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>.</li> 
 <li value="2"> Click Projects.</li> 
 <li value="3">Click the project name that contains the tasks you want to delete.</li> 
 <li value="4"> Click Tasks in the left panel. </li> 
 <li value="5">Do one of the following: 
  <ol>
   <ul>
    <li>(Conditional) When the <span class="bold">Autosave</span> toggle is enabled: 
     <ol>
      <li value="1"> Select the tasks you want to delete, then click <span class="bold">More</span></li>
      <li value="2"><p>Click <span class="bold">Delete</span>, then <span class="bold">Yes, Delete It</span> to confirm the deletion. </p><p>The tasks are deleted. </p></li>
     </ol></li>
    <li>(Conditional) Click the Plan Mode icon and select Manual save if you want to reverse the changes you make to the task list.<p>Do the following: </p>
     <ol style="list-style-type: lower-alpha;">
      <li value="1">Select the tasks you want to delete. </li>
      <li value="2">Click <span class="bold">Delete</span>.</li>
      <li value="3"><p>(Optional) Click <span class="bold">Undo</span> to reverse your change and not delete the tasks.</p></li>
      <li value="4"> Click <span class="bold">Redo</span> if you want to keep the change and delete the task.</li>
      <li value="5"><p>Click <span class="bold">Save</span> to delete the tasks.</p><p>Tasks are deleted only after you save your changes. </p></li>
     </ol></li>
   </ul>
  </ol></li> 
</ol>

### Delete a single task

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>.</li> 
 <li value="2"> Click Projects. </li> 
 <li value="3">Click the project name that contains the task you want to delete.</li> 
 <li value="4"> Click Tasks in he left panel.</li> 
 <li value="5">Click the name of the task you want to delete.</li> 
 <li value="6"> <p> Click the More icon in the upper-right corner. </p>  </li> 
 <li value="7">Click <span class="bold">Delete Task</span>.</li> 
 <li value="8"> <p>If the deletion is allowed, click <span class="bold">Yes, Delete it</span>.</p> <p>Your <span>Workfront administrator</span> <span>or <span>group administrator</span></span> might not allow the deletion of tasks where hours are logged. </p> <p>For more information about the access and permissions needed to delete a task, see the section <a href="#access-and-permissions-needed" class="MCXref xref">Limitations for deleting tasks </a> in this article.</p> </li> 
</ol>

## Restore deleted tasks

A `Workfront` or `group administrator` can restore tasks within 30 days after they are deleted, as described in [Restore deleted items](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
