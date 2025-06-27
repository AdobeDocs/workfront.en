---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Duration Type overview: Calculated Assignment'
description: Calculated Assignment is a Duration Type that you can set for a task in Adobe Workfront. For general information about Duration Types in Workfront, see Overview of Task Duration and Duration Type.
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
---
# Duration Type overview: Calculated Assignment

<!-- Audited: 5/2025 -->

Calculated Assignment is a Duration Type that you can set for a task in Adobe Workfront. For general information about Duration Types in Workfront, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Overview of the Calculated Assignment Duration Type

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* When you use a Calculated Assignment Duration Type, you must specify both a Duration and a number of Planned Hours for the task. Workfront then divides the amount of Planned Hours by the amount of hours in the Duration, then by the number of resources assigned to the task to calculate the allocation percentage (calculates the assignment) for each resource. Each resource will equally have the same value for their allocation percentage. In this case, you can't modify the allocation values for each resource.
* Your Workfront or a group administrator can set the default Duration&nbsp;Type of your system or group as Calculated Assignment.&nbsp;In this case, all new tasks will be created with this Duration Type. For information about changing your task and issue preferences as part of your system-level or group-level project preferences, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  In this case, the task has a default of a one-day Duration and a default of 0 hours of Planned Hours. Unless the project manager sets a more accurate Duration and populates the Planned Hours field with a realistic estimate, then resources appear underallocated.

Calculated Assignment is the preferred Duration Type in the following situations:

* When assignments have a window of activity but don't take the entire Duration allotted to complete their work. For example, you are assigned to deliver a report to your supervisor by the end of the week. You have a five-day duration, but it will only take you 10 hours to draft the document.
* When a single resource is assigned to a task because the project manager can estimate the planned Duration and planned amount of effort independent of each other.

  You can use the Calculated Work Duration Type for the same result, but the project manager must input a percentage allocation for the resource in order to affect the calculated value for Planned Hours. This makes project planning more difficult and time-consuming.

The allocation percentage for each resource is calculated as follows:

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

For example, in the scenario outlined below, each task has a Duration of 3 days. The project manager manually enters both the Duration (3 days or 24 hours) and Planned Hours, and as a result, the allocation percentage (or assignment percentage) is calculated:

![](assets/calcassign-350x80.png)

## Change the Duration Type of a task to Calculated Assignment

For information about changing the Duration Type of a task, see [Update the Duration Type of a task](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Assignment</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
