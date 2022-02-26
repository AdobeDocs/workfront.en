---
filename: edit-tasks-in-a-list
product-area: projects
navigation-topic: manage-tasks
title: Edit tasks in a list
description: You can edit task information in a list of tasks by editing the fields displayed in the list. For information about other ways to edit tasks, see Edit tasks.
---

# Edit tasks in a list

You can edit task information in a list of tasks by editing the fields displayed in the list. For information about other ways to edit tasks, see [Edit tasks](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p><em>Work</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and&nbsp;Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the task and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Considerations about editing tasks in a list

Editing tasks in a list is a fast way to make changes to multiple tasks simultaneously, with a clear view of how your changes might affect the project timeline.

Consider the following when editing tasks in a list:

<ul> 
 <li>Unlike needing Manage permissions to the task when editing it in the Edit Box, you can edit a task in a list only with Contribute permissions to the task. This allows you to edit the following limited information for the task: 
  <ul> 
   <li>Description</li> 
   <li>Status</li> 
   <li>Percent Complete</li> 
   <li><p>Custom&nbsp;Form information</p><note type="note">
     You can edit a task custom field in a list only if you have permissions to update the field.
    </note></li> 
   <li>Log hours</li> 
   <li>Modify Assignments</li> 
   <li>View finance information </li> 
   <li><p>Add expenses, tasks, or issues</p></li> 
  </ul></li> 
 <li>You can edit a task in the following lists: 
  <ul> 
   <li>The Tasks <draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       section 
     </MadCap:conditionalText>
    </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      section 
    </MadCap:conditionalText> of the project</li> 
   <li>The Subtasks <draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       section 
     </MadCap:conditionalText>
    </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      section 
    </MadCap:conditionalText> of the project</li> 
   <li><p>A task report</p><note type="note">
     By default, 
     <em>Workfront</em> automatically saves your changes to tasks in the Subtasks 
     <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
        section 
      </MadCap:conditionalText>
     </draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       section 
     </MadCap:conditionalText>or in a task report. 
    </note></li> 
  </ul></li> 
 <li> <p>You can control when <em>Workfront</em> saves the changes you make to the tasks in a list. Your changes can be saved automatically or you can manually save them. </p> <p>For information about configuring when <em>Workfront</em> saves changes you make to tasks in a list, see the <a href="#selectin" class="MCXref xref">Select a save option when editing tasks in a list</a> section in this article. </p> </li> 
</ul>

## Select a save option when editing tasks in a list

You can decide where the changes you make to tasks in a list are saved automatically, as they occur, or if you want to manually save each change.

>[!IMPORTANT]
>
>Depending on whether you save the tasks automatically or manually, you might overwrite someone else's information as you are editing tasks in a list. For information about how *Workfront* saves changes on tasks that you make concurrently with other users, see [Overview of saving concurrent changes within a task list](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

When you save your changes in a list for a project that has either Automatic or Automatic and On Change selected as the Update Type, *Workfront* updates the project timeline, along with all in-project and cross-project dependencies. Timeline calculations can take a long time if the project is large or if there are a lot of dependencies. Some methods of editing a task list can be faster than others, depending on the method you select to save your changes.

You can control when *Workfront* saves the changes you make to the tasks in a list. The following scenarios exist:&nbsp;

* You can have *Workfront* automatically save the changes, after each update.

  For information, see the section [Edit tasks in a list and automatically save changes](#autosave) in this article. 

* You can have control over when you apply multiple changes at a time by manually using a Save button.

  For information, see the section [Edit tasks in a list and manually save changes](#save) in this article.

### Edit tasks in a list and automatically save changes

>[!TIP]
>
>Saving your changes and all the project dependencies might be slower if your project has more than 2000 tasks or if it has a lot of dependencies.

Consider the following when saving your task list changes automatically:

* You can apply a custom view to the task list and edit any task-related fields that you have access to update. 
* You cannot reverse auto-saved changes. This is the default setting. 
* *Workfront* recalculates the timeline of the project and all the in-project and cross-projects dependencies automatically after every change, when the project Update Type is Automatic or Automatic and On Change. For information about the project Update Type, see [Select the project Update Type](../../../manage-work/projects/manage-projects/select-project-update-type.md).

To edit tasks in a list and save changes automatically:

<ol> 
 <li value="1">Go to the project, then click the <span class="bold">Tasks</span> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     section 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    section 
  </MadCap:conditionalText>.</li> <draft-comment>
  <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <div> 
    <p>Click the <span class="bold">Plan mode menu</span> <img src="assets/qs-list-mode-or-save-mode-icon-small.png"> at the top of the list and make sure that the <span class="bold">Autosave</span> option is selected. </p> 
    <p><img src="assets/autosave-setting-enabled-quicksilver-task-list-350x308.png" style="width: 350;height: 308;"></p> 
   </div></li>
 </draft-comment>
 <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
  <div> 
   <p>Click the <span class="bold">Plan mode menu</span> <img src="assets/qs-list-mode-or-save-mode-icon-small.png"> at the top of the list and make sure that the <span class="bold">Autosave</span> option is selected. </p> 
   <p><img src="assets/autosave-setting-enabled-quicksilver-task-list-350x308.png" style="width: 350;height: 308;"></p> 
  </div></li> 
 <li value="3"><p>Edit any field that you have permissions to update manually.</p><p><img src="assets/inline-editing-a-task-350x26.png" style="width: 350;height: 26;"></p></li> 
 <li value="4"><p>(Optional) Press <span class="bold">Escape</span> to cancel your changes.</p></li> 
 <li value="5"><p>Press Enter to save your changes to the tasks and to the project timeline. </p></li> 
 <li value="6"><p>(Optional) Right click a task you want to modify.</p><p>Or</p><p>Click the <span class="bold">More</span> menu <img src="assets/more-icon-task-list.png"> to the right of the task name. </p></li> 
 <li value="7"><p>(Optional) Select from the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Open in a new tab</span></td> 
     <td>Opens the task in a new browser tab. </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Edit</span></td> 
     <td><p>Opens the <span class="bold">Edit Task</span> box, where you can edit the task.</p><p>For information about editing a task, see <a href="#top" class="MCXref xref">Edit tasks in a list</a>.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Delete</td> 
     <td><p>Deletes the task.</p><p>For information about deleting tasks, see <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Delete tasks</a>.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Indent</td> 
     <td><p>Indents the task by one level. </p><p>This option displays only on stand-alone tasks.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Outdent</td> 
     <td><p>Outdents the task by one level. </p><p>This option displays only on children tasks. </p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Insert Task Above</td> 
     <td>Inserts a task above the selected task.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Insert Task Below</td> 
     <td>Inserts a task under the selected task</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Duplicate</td> 
     <td><p>Creates a duplicate version of the task within the same project. </p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Copy To</td> 
     <td><p>Copies the task to another project.</p><p>For information about copying and duplicating tasks, see <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copy and duplicate tasks</a>.</p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Move To</td> 
     <td><p>Moves the task to another project.</p><p>For information about moving tasks, see <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Move tasks</a>.</p></td> 
    </tr> 
   </tbody> 
  </table><p>Changes are saved automatically and you cannot reverse them. </p></li> 
</ol>

### Edit tasks in a list and manually save changes

You can manually save changes you make to tasks in a list. When you save changes this way, you have the flexibility to reverse them before saving. 

` `**Tips: **``

* You cannot reverse changes you make to tasks in a list when you are editing them in the Subtasks 

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  section
  </MadCap:conditionalText>
  -->

  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  section </MadCap:conditionalText>` or in a task report.

* There are no limitations on how many changes you can reverse. You can reverse all of them one by one until you reach the original state of the tasks.

Consider the following when saving changes in a task list manually:

* In order to save task list changes manually, you need permissions to Manage both the tasks and the project. 
* You cannot edit the project. The option to edit the project is disabled.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">You cannot update information in the header of the project. You can only do the following when manually saving the changes in the task list:
  <ul> <draft-comment>
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">Subscribe to the project.</li>
  </draft-comment>
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">Subscribe to the project.</li> <draft-comment>
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">Add the project to your list of favorites. </li>
  </draft-comment>
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">Add the project to your list of favorites. </li> <draft-comment>
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">Open a task by clicking the its name in the list.</li>
  </draft-comment>
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">Open a task by clicking the its name in the list.</li>
  </ul></li>
  -->

* You cannot update information in the header of the project. You can only do the following when manually saving the changes in the task list:

  * Subscribe to the project.
  * Add the project to your list of favorites. 
  * Open a task by clicking the its name in the list.

* dit the tasks in bulk. The Edit icon is disabled when selecting multiple tasks. 
* *Workfront* triggers notifications about the changes you make to the tasks only after you save your changes.

There are two ways to manually save changes to tasks in a list. These two ways are described below.

* 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><a href="#save3" class="MCXref xref">Save changes in a task list manually when you select the Manual save Standard option</a> </p>
  -->

  [Save changes in a task list manually when you select the Manual save Standard option](#save3)

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"><a href="#save5" class="MCXref xref">Save changes in a task list manually when you select the Manual save Timeline Planning option</a> </li>
  -->

* [Save changes in a task list manually when you select the Manual save Timeline Planning option](#save5)

<!--
<h4 data-mc-conditions="QuicksilverOrClassic.Quicksilver"><a name="Save3"></a>Save changes in a task list manually when you select the Manual save Standard option</h4>
-->

#### Save changes in a task list manually when you select the Manual save Standard option

>[!TIP]
>
>If your project has more than 2000 tasks, or if it has a lot of dependencies, it might take a while to visually identify the changes you make to your tasks and how these changes affect all the project dependencies. In this case, saving your changes might take longer if your project has more than 2000 tasks or if it has a lot of dependencies.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Consider the following when updating tasks in a list after selecting the Manual save Standard option:</p>
-->

Consider the following when updating tasks in a list after selecting the Manual save Standard option:

* You can apply a custom view to the task list and edit any task-related fields that you have permissions to Manage in that view.
* *Workfront* calculates the timeline of the project and all the in-project and cross-project dependencies after you click Save, when the project Update Type is Automatic or Automatic and On Change. For information about the project Update Type, see [Select the project Update Type](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">To edit tasks in a list when selecting the Manual save Standard option:</p>
-->

To edit tasks in a list when selecting the Manual save Standard option:

<ol> 
 <li value="1">Go to a project, then click the <span class="bold">Tasks</span> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     section 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    section 
  </MadCap:conditionalText>.</li> 
 <li value="2"> <draft-comment>
   <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
    <p>Click the <span class="bold">Plan mode menu</span> <img src="assets/qs-list-mode-or-save-mode-icon-small.png"> at the top of the list and select <span class="bold">Manual save</span>, then click <span class="bold">Standard</span> > <span class="bold">Apply</span>. </p> 
    <p> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p> 
    <p>A toolbar setting displays with options to undo, redo, and save your changes.</p> 
    <p> <img src="assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png" style="width: 350;height: 65;"> </p> 
   </div>
  </draft-comment>
  <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <p>Click the <span class="bold">Plan mode menu</span> <img src="assets/qs-list-mode-or-save-mode-icon-small.png"> at the top of the list and select <span class="bold">Manual save</span>, then click <span class="bold">Standard</span> > <span class="bold">Apply</span>. </p> 
   <p> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p> 
   <p>A toolbar setting displays with options to undo, redo, and save your changes.</p> 
   <p> <img src="assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png" style="width: 350;height: 65;"> </p> 
  </div> </li> 
 <li value="3"> <p>Click inside any field that you have permissions to update manually. The field becomes editable and you can make your changes. </p> <p> <img src="assets/inline-editing-a-task-350x26.png" style="width: 350;height: 26;"> </p> </li> 
 <li value="4">Press Enter to temporarily save the changes you made.</li> 
 <li value="5"> <p>(Optional) Click the <span class="bold">Undo icon</span> <img src="assets/undo-icon-on-task-list.png"> to reverse a change and return a field to its original state.</p> </li> 
 <li value="6">(Optional and conditional) Click the <span class="bold">Redo icon</span> <img src="assets/redo-icon-on-task-list.png"> to restore the change you reversed. </li> 
 <li value="7"> <p>(Optional) Right-click a task you want to modify.</p> <p>Or</p> <p>Click the <span class="bold">More</span> menu <img src="assets/more-icon-task-list.png">. </p> </li> 
 <li value="8"> <p>(Optional) Select from the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Open in a new tab</span> </td> 
     <td>Opens the task in a new browser tab. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Delete</td> 
     <td>For information about deleting tasks, see <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Delete tasks</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Indent</td> 
     <td> <p>Indents the task by one level. </p> <p>This option displays only on stand-alone tasks.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Outdent</td> 
     <td> <p>Outdents the task by one level. </p> <p>This option displays only on children tasks. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Insert Task Above</td> 
     <td>Inserts a task above the selected task.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Insert Task Below</td> 
     <td>Inserts a task under the selected task</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Duplicate</td> 
     <td> <p>Creates a duplicate version of the task within the same project. </p> <p>For information about copying and duplicating tasks, see <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copy and duplicate tasks</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <p><em>Workfront</em> updates all in-project and cross-project dependencies when you make changes to the timeline of tasks. </p> 
 <li value="9"> <p>Click <span class="bold">Save</span> when you want to keep your task changes permanently and save the timeline of the project. </p> </li> 
</ol>

<!--
<h4 data-mc-conditions="QuicksilverOrClassic.Quicksilver"><a name="Save5"></a>Save changes in a task list manually when you select the Manual save Timeline Planning option</h4>
-->

#### Save changes in a task list manually when you select the Manual save Timeline Planning option

Saving your changes and all the project dependencies is faster. This is not available for projects with more than 2000 tasks.

>[!IMPORTANT]
>
>We recommend that you use this option when editing a large list of tasks of more than a few hundred that have a lot of dependencies. Using this option allows you to visually identify your changes much faster than using the Manual save option.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Consider the following when using the Manual save Timeline Planning option in a task list: </p>
-->

Consider the following when using the Manual save Timeline Planning option in a task list:

* You cannot apply 

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  Manual save
  </MadCap:conditionalText>
  -->

  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  Manual save </MadCap:conditionalText>` Timeline Planning option to projects that have more than 2000 tasks. 

* You cannot apply a custom view, filter, or grouping to the task list. The View, Filter, and Grouping drop-down menus, as well as the Agile view icon, are disabled. The view that is applied by default contains a limited number of fields. 
* The timeline of the project and all the in-project dependencies are calculated automatically after each change when the project Update Type is Automatic or Automatic and On Change. 
* The cross-project dependencies are calculated after you click Save, when the project Update Type is Automatic or Automatic and On Change. For information about the project Update Type, see [Select the project Update Type](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">To edit tasks in a list when using the Manual save Timeline Planning option:</p>
-->

To edit tasks in a list when using the Manual save Timeline Planning option:

<ol> 
 <li value="1">Go to a project, then click the <span class="bold">Tasks</span> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     section 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    section 
  </MadCap:conditionalText>. </li> 
 <li value="2"> <draft-comment>
   <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
    <p> Click the <span class="bold">Plan mode menu </span> <img src="assets/qs-list-mode-or-save-mode-icon-small.png"> at the top of the list and select <span class="bold">Manual save</span>, then click <span class="bold">Timeline Planning</span>> <span class="bold">Apply</span>.</p> 
    <p>This option is dimmed for projects with more than 2000 tasks. </p> 
    <p> <img src="assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png" style="width: 350;height: 490;"> </p> 
   </div>
  </draft-comment>
  <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <p> Click the <span class="bold">Plan mode menu </span> <img src="assets/qs-list-mode-or-save-mode-icon-small.png"> at the top of the list and select <span class="bold">Manual save</span>, then click <span class="bold">Timeline Planning</span>> <span class="bold">Apply</span>.</p> 
   <p>This option is dimmed for projects with more than 2000 tasks. </p> 
   <p> <img src="assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png" style="width: 350;height: 490;"> </p> 
  </div> <note type="tip">
   When you navigate away from this page, 
   <em>Workfront</em> re-enables the Autosave option.
  </note> <p>Notice the following changes in the list:</p> 
  <ul> 
   <li>The View, Grouping, and Filter drop-down menus are removed and the view is replaced by the following fields:<p> 
     <ul> 
      <li>Task Number</li> 
      <li>Task Name</li> 
      <li>Constraint Type</li> 
      <li>Duration</li> 
      <li>Planned Start Date</li> 
      <li>Planned Completion Date</li> 
      <li>Predecessors</li> 
      <li>Assignments</li> 
      <li>Status</li> 
      <li>Percent Complete</li> 
     </ul></p></li> 
   <li>The Agile view icon is removed. </li> 
   <li> <p>A toolbar setting displays with options to undo, redo, and save your changes.</p> <p> <img src="assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png" style="width: 350;height: 65;"> </p> </li> 
  </ul> </li> 
 <li value="3"> <p>Edit any field that you have permissions to update manually.</p> <p> <img src="assets/inline-editing-a-task-350x26.png" style="width: 350;height: 26;"> </p> </li> 
 <li value="4">Press Enter to temporarily save the changes you made.</li> 
 <li value="5"> <p>(Optional) Click the <span class="bold">Undo icon</span> <img src="assets/undo-icon-on-task-list.png"> to reverse a change and return a field to its original state.</p> </li> 
 <li value="6">(Optional and conditional) Click the <span class="bold">Redo icon</span> <img src="assets/redo-icon-on-task-list.png"> to reinstate the change you reversed. </li> 
 <li value="7"> <p>(Optional) Right click a task you want to modify</p> <p>Or</p> <p>Click the <span class="bold">More</span> menu <img src="assets/more-icon-task-list.png">. </p> </li> 
 <li value="8"> <p>Select from the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Open in a new tab</span> </td> 
     <td>Opens the task in a new browser tab. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Delete</td> 
     <td>For information about deleting tasks, see <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Delete tasks</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Indent</td> 
     <td> <p>Indents the task by one level. </p> <p>This option displays only on stand-alone tasks.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Outdent</td> 
     <td> <p>Outdents the task by one level. </p> <p>This option displays only on children tasks. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Insert Task Above</td> 
     <td>Inserts a task above the selected task.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Insert Task Below</td> 
     <td>Inserts a task under the selected task</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Duplicate</td> 
     <td> <p>Creates a duplicate version of the task within the same project. </p> <p>For information about copying and duplicating tasks, see <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copy and duplicate tasks</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <p><em>Workfront</em> updates all in-project and cross-project dependencies when you change the timeline of a task. </p> 
 <li value="9"> <p>Click <span class="bold">Save</span> when you want to keep your task changes permanently and save the timeline of the project. </p> </li> 
</ol>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Quicksilver"><a name="Editing2"></a>Edit a task in a list using the Summary</h2>
-->

## Edit a task in a list using the Summary

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Go to the project containing tasks you want to edit.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Go to the project containing tasks you want to edit.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click<span class="bold">Tasks</span> in the left panel. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click<span class="bold">Tasks</span> in the left panel. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The list of tasks on the project displays. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The list of tasks on the project displays. </p> </li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the More menu <img src="assets/more-icon-task-list.png"> after the task name, then click <span class="bold">Open Summary</span>. Select the task you want to <span data-mc-edit-date="2020-02-25T16:39:34.7933088-05:00" data-mc-editor="alinawilson" data-mc-comment=" preview highlighted for the Summary icon story (Orion)" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2020-02-25T16:38:26.4957329-05:00">edit,</span> then click the <span class="bold">Open Summary icon</span> <img src="assets/qs-open-summary-icon-in-new-toolbar-small.png"> in the upper-right corner of the list.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the More menu <img src="assets/more-icon-task-list.png"> after the task name, then click <span class="bold">Open Summary</span>. Select the task you want to <span data-mc-edit-date="2020-02-25T16:39:34.7933088-05:00" data-mc-editor="alinawilson" data-mc-comment=" preview highlighted for the Summary icon story (Orion)" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2020-02-25T16:38:26.4957329-05:00">edit,</span> then click the <span class="bold">Open Summary icon</span> <img src="assets/qs-open-summary-icon-in-new-toolbar-small.png"> in the upper-right corner of the list.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <span class="bold">Summary</span> opens.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <span class="bold">Summary</span> opens.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/qs-task-right-panel-in-a-task-list-350x328.png" style="width: 350;height: 328;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/qs-task-right-panel-in-a-task-list-350x328.png" style="width: 350;height: 328;"> </p> </li> 
 <li value="4"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <span class="bold">X icon</span> in the upper-right of the Summary to close the panel and edit the tasks inline. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <span class="bold">X icon</span> in the upper-right of the Summary to close the panel and edit the tasks inline. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Follow the steps about editing a task in a list to inline edit the task. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Follow the steps about editing a task in a list to inline edit the task. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">For information about editing the task in a list, see <a href="#editing" class="MCXref xref">Considerations about editing tasks in a list</a> in this article. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">For information about editing the task in a list, see <a href="#editing" class="MCXref xref">Considerations about editing tasks in a list</a> in this article. </p> </li> <draft-comment>
  <li value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Type an update for the task in the <span class="bold">Updates</span> area. </li>
 </draft-comment>
 <li value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Type an update for the task in the <span class="bold">Updates</span> area. </li> 
 <li value="6"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click any of the following icons or areas to go to the task and edit information at the task level:</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click any of the following icons or areas to go to the task and edit information at the task level:</p> <draft-comment>
   <table cellspacing="0" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
    <col> 
    <col> 
    <tbody> 
     <tr> <draft-comment>
       <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Documents</span> </td>
      </draft-comment>
      <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Documents</span> </td> <draft-comment>
       <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Click here to add</span> to add documents to the task.</td>
      </draft-comment>
      <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Click here to add</span> to add documents to the task.</td> 
     </tr> 
     <tr> <draft-comment>
       <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Details</span> </td>
      </draft-comment>
      <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Details</span> </td> <draft-comment>
       <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click to update information about the task.</td>
      </draft-comment>
      <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click to update information about the task.</td> 
     </tr> 
     <tr> <draft-comment>
       <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Custom Forms</span> </td>
      </draft-comment>
      <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Custom Forms</span> </td> <draft-comment>
       <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click to add or remove Custom Forms or update information on the forms. </td>
      </draft-comment>
      <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click to add or remove Custom Forms or update information on the forms. </td> 
     </tr> 
     <tr> <draft-comment>
       <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Hours</span> </td>
      </draft-comment>
      <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Hours</span> </td> <draft-comment>
       <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click to log hours.</td>
      </draft-comment>
      <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click to log hours.</td> 
     </tr> 
     <tr> <draft-comment>
       <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Approvals</span> </td>
      </draft-comment>
      <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Approvals</span> </td> <draft-comment>
       <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click to add task approvals. </td>
      </draft-comment>
      <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click to add task approvals. </td> 
     </tr> 
    </tbody> 
   </table>
  </draft-comment>
  <table cellspacing="0" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Documents</span> </td> 
     <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Click here to add</span> to add documents to the task.</td> 
    </tr> 
    <tr> 
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Details</span> </td> 
     <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click to update information about the task.</td> 
    </tr> 
    <tr> 
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Custom Forms</span> </td> 
     <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click to add or remove Custom Forms or update information on the forms. </td> 
    </tr> 
    <tr> 
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Hours</span> </td> 
     <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click to log hours.</td> 
    </tr> 
    <tr> 
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span style="font-weight: bold;">Approvals</span> </td> 
     <td data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click to add task approvals. </td> 
    </tr> 
   </tbody> 
  </table> </li> <draft-comment>
  <li value="7" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the back button on your browser to return to the task list when you finish updating the task. </li>
 </draft-comment>
 <li value="7" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the back button on your browser to return to the task list when you finish updating the task. </li> 
</ol>

## Edit tasks in bulk

You can edit multiple tasks all at once. Ensure you have manage permissions to the tasks to be able to edit them.

<ol> 
 <li value="1">Go to a project containing tasks you want to edit in bulk. </li> 
 <li value="2"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click 
    <span class="bold">Tasks</span> in the left panel. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
   <span class="bold">Tasks</span> in the left panel. 
  </MadCap:conditionalText></li> 
 <li value="3"> <p>Ensure that the <span class="bold">Autosave</span> option is selected. </p> <note type="important">
   You cannot edit tasks in bulk when saving tasks manually. 
  </note> <p>For more information about ways of saving changes to tasks in a list, see the section <a href="#editing" class="MCXref xref">Considerations about editing tasks in a list</a> in this article. </p> </li> 
 <li value="4">Select several tasks in the tasks list. </li> 
 <li value="5"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Edit icon</span> <img src="assets/qs-edit-icon.png">. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Edit icon</span> <img src="assets/qs-edit-icon.png">. </p> <p>The <span class="bold">Edit Tasks</span> dialog box opens.</p> </li> 
 <li value="6"> <p> Specify the information you want to change for all the tasks you selected.</p> <p>Editing the information on all tasks is identical to editing information on one task. If you want to edit task Duration, the tasks selected must have the same Task Constraint; otherwise, the <span class="bold">Duration</span> field does not populate.</p> <p>For more information about editing a task, see <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> <note type="note">
    The information you are changing on all the tasks selected will override the existing information on individual tasks, except for the 
   <span class="bold">Assignments</span> field. Adding a new assignee in bulk edit will add that assignee to all the selected tasks. If other assignees are assigned to the selected tasks, they will remain assigned in addition to the one added through bulk edit. 
  </note> </li> 
 <li value="7"> <p>Click <span class="bold">Custom Forms</span> to edit the custom forms attached to all the tasks selected. Only active custom forms display in the list.</p> <p>If the tasks selected do not have any common custom forms, no forms are listed in this section.</p> <p>You can edit only the fields on the forms that are attached to all tasks selected and which you have permissions to edit. </p> </li> 
 <li value="8">(Optional) In the Custom Forms section, select the <span class="bold">Recalculate Custom Expressions</span> option to ensure that all Calculated Custom Fields that are on the custom forms attached to the tasks selected are up to date. </li> 
 <li value="9"> <p>Click <span class="bold">Save Changes</span>. </p> <p>All changes you made are now visible on all the selected tasks. </p> </li> 
</ol>

For information about bulk editing custom forms, see the section "Edit multiple Custom Forms when bulk-editing objects" in [Manage custom forms attached to objects in Adobe Workfront](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
