---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Duration Type overview: Simple'
description: The Simple Duration Type is a Duration Type that you can set for a task in Adobe Workfront. For general information about Duration Types in Workfront, see Overview of Task Duration and Duration Type.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
---
# Duration Type overview: Simple

The Simple Duration Type is a Duration Type that you can set for a task in Adobe Workfront. For general information about Duration Types in Workfront, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Overview of the Simple Duration Type

Your Workfront or a group administrator can set the default Duration&nbsp;Type of your system or group as Simple.&nbsp;In this case, all new tasks will be created with this Duration Type. For information about changing your task and issue preferences as part of your system-level or group-level project preferences, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

The following things occur when a task has a Duration Type of Simple:

* Project managers can modify the both the Duration and the Planned Hours of a task when modifying how those hours should be distributed among assignees.

  For information, see [Update the Planned Hours and Duration of a task with a Simple Duration Type](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md).

  >[!IMPORTANT]
  >
  >When you first create a task and assign the Simple Duration Type to it and do not specify a Duration, Workfront calculates the Duration of the task based on the amount of Planned Hours you specify for the task. If you manually modify the Duration of a Simple Duration task, Workfront stops matching the Planned Hours to the Duration because it assumes you want to define them manually yourself.
  >
  >Workfront calculates the duration of tasks whose duration has not been manually modified using the following formula:
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >Your Workfront administrator defines the `Typical hours per work day` in the Project Preferences area of your instance's Setup. 

* Allocation percent is hidden and allocation hours are available to be edited, instead.
* All new customers have the system-level Duration Type set to Simple.

## Change the Duration Type of a task to Simple

For information about changing the Duration Type of a task, see [Update the Duration Type of a task](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
