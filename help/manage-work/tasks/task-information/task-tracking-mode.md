---
filename: task-tracking-mode
content-type: overview
product-area: projects
navigation-topic: task-information
title: Task Tracking Mode overview
description: You can adjust the Tracking Mode setting of a task when creating or editing a task to control how and when the Progress Status indicators of a task display. Adobe Workfront displays Progress Status flags when you configure certain settings for tracking progress on tasks.
---

# Task Tracking Mode overview

You can adjust the Tracking Mode setting of a task when creating or editing a task to control how and when the Progress Status indicators of a task display. *Adobe Workfront* displays Progress Status flags when you configure certain settings for tracking progress on tasks.

For more information about Progress Status of tasks, see [Task Progress Status overview](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="setting-tracking-mode"></a>Set Tracking Mode for tasks</h2>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <draft-comment>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<span class="bold">Edit</span>.</p>
</draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<span class="bold">Edit</span>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the&nbsp;<span class="bold">Settings</span> section, use the&nbsp;<span class="bold">Tracking Mode</span> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click&nbsp;<span class="bold">Save Changes.</span></li>
</ol>
</div>
-->

## Set Tracking Mode for tasks

To set the tracking mode:

<ol> 
 <li value="1">Go to the task you want to set the tracking mode for.</li> 
 <li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<span class="bold">Edit</span>.</p> <p>The Edit Task dialog box opens. </p> </li> 
 <li value="3"> <p>In the&nbsp;<span class="bold">Settings</span> section, use the&nbsp;<span class="bold">Tracking Mode</span> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li> 
 <li value="4">Click&nbsp;<span class="bold">Save Changes.</span></li> 
</ol>

## Tracking Mode options

As a task owner or a project manager, you can select how *Workfront* indicates the progress status on each task. For information about how to set&nbsp;Tracking Mode on your tasks, see [Set Tracking Mode for tasks](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

You can select from the following options:

* [User Must Update](#user-must-update) 
* [Assume On Time](#assume-on-time) 
* [Ignore Late Warnings](#ignore-late-warnings) 
* [Auto Complete](#auto-complete) 
* [Predecessor](#predecessor)

### User Must Update

When this option is selected, *Workfront* uses the task's Percent Complete and Actual Hours logged to determine the Progress Status of the task. This is the default option.

### Assume On Time

*Workfront* assumes a task will be completed on time regardless of the current completion status. If it does not, then *Workfront* automatically assumes a Planned Completion Date of the next working day. You must still indicate when the task completes. Use this option when users will not be regularly updating their tasks.

### Ignore Late Warnings

The Progress Status of a task will be On Time until it becomes Late. For example, if you schedule a task to take 10 days and on the day it is to be completed the task shows a Percent Complete of 60%, then *Workfront* updates the Projected Completion Date by adding four days and the Progress Status of the task becomes Late.

### Auto Complete

*Workfront* assumes tasks will be completed as scheduled and marks them as complete on their Due or Planned Completion Dates. Until then, *Workfront* uses Percent Complete and Actual Hours logged to determine the Progress Status. However, regardless of the Progress Status before the scheduled completion date, *Workfront* still marks the task completed.

>[!IMPORTANT]
>
>Selecting to have tasks auto complete marks the task Complete when the project time is recalculated. If the Update Type of the project is set to Automatic or Automatic and On Change, the project timeline is calculated daily. For information about timeline recalculations on projects, see [Recalculate project timelines](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md). 
>
>The time of the Actual Completion Date is midnight of the day when the timeline is automatically calculated. The time used to generate this time stamp is your system's Time&nbsp;Zone as defined by your *Workfront administrator* in the Customer Info section of Setup. For information about setting your system's Time Zone, see [Configure basic information for your system](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Predecessor

*Workfront* estimates the Projected Completion Date of a task according to its predecessor relationship. The Progress Status of a task is&nbsp;determined based on this estimation. For example, Task B has a Duration of 1 Day and is scheduled to complete two days after its predecessor, Task A,&nbsp;which should take five days. A user then updates Task B to 50% complete, but the predecessor, Task A, has not yet started. *Workfront*&nbsp;schedules the dependent Task B for completion six days after the start date of the predecessor task, allowing 5 days for Task A and&nbsp;1 day for Task B.
