---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Duration Type Overview: Effort Driven'
description: Effort Driven is a duration type that you can set for a task in Adobe Workfront. For general information about Duration Types in Workfront, see Overview of Task Duration and Duration Type.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
---
# Duration Type overview: Effort Driven

Effort Driven is a duration type that you can set for a task in Adobe Workfront. For general information about Duration Types in Workfront, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Overview of the Effort Driven Duration Type

Your Workfront or a group administrator can set the default Duration&nbsp;Type of your system or group as Effort Driven.&nbsp;In this case, all new tasks will be created with this Duration Type. For information about changing your task and issue preferences as part of your system-level or group-level project preferences, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

In this scenario, there is a risk of arbitrarily shortening the project plan, unless you, as the project manager, take the time to consider whether the task is actually an Effort Driven task.

Use Effort Driven to:

* Determine the Planned Duration based on the number of resources available to work on the task. Duration is equal to Planned Hours. Planned Duration is equal to Planned Hours divided by the number of assignees.

  The level of effort applied to the task determines the division of labor and Duration.

* Track the total number of hours spent on a task when multiple resources are assigned.

  As resources are added, the Planned Duration of the task decreases. (The principle of "many hands make light work" illustrates the effect that this Duration Type has on the Planned Duration of a task.)

The following sections provide more detailed information about how Workfront calculates the Planned Duration of an Effort Driven task and the effect that adding resources has to the task with this Duration Type.

## Overview of the Effort Driven Duration Type formula

The formula for calculation the Planned Duration for a task with a Duration Type of Effort Driven depends on the allocation percentage of each resource assigned to the task. In the case of an Effort Driven task, Workfront calculates the Planned Hours of the task and they are always the same as the Duration of the task:

```
Planned Hours (in hours) = Duration (in days)
```

You can manually adjust the Duration of the task.

Workfront assumes that there are 8 working hours in a working day. Your Workfront or group administrator defines the hours per workday with the Typical Hours per Work Day setting in the Project Preferences in Setup. For more information about changing your task and issue preferences as part of your system-level project preferences, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront considers the Schedule for each resource assigned to the task to determine the percent of allocation for each resource for the task. For information about creating and assigning schedules to users, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Consider the following scenarios:

* [Resources are allocated 100% to the task](#resources-are-allocated-100-to-the-task) 
* [Resources are allocated for various percentages of time to the task](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### Resources are allocated 100% to the task {#resources-are-allocated-100-to-the-task}

This formula assumes that all resources are allocated 100% to the task.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

This calculation assumes that the number of hours in a normal work day is 8. The equation includes this value so the Planned Duration displays in days.

### Resources are allocated for various percentages of time to the task {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Because each assigned resource can have a unique level of allocation, the actual formula takes these allocation values into account:

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

This calculation assumes that the number of hours in a normal work day is 8. The equation includes this value so the Planned Duration displays in days.

## The effect of adding more resources to a task

When adding or removing assignees to a task with the Effort Driven Duration Type, Duration and Planned Hours do not change. However, the Planned Duration does change.

In the following example, the Typical Hours per Work Day is set to 8 in the Project Preferences in your system setup. Because the duration is 3 days, the Planned Hours is set to 24 (3 days x 8 hours per work day = 24 Planned Hours).

>[!NOTE]
>
>When using the Fixed Dates Task Constraint, the Planned Duration remains the same when you add or remove assignees, and instead the Duration and Planned Hours are adjusted. When using any Task Constraint other than Fixed Dates, the Planned Duration is adjusted.

The following table illustrates how the Planned Duration changes with adding resources to the task:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>Number of Assignees (each 100% allocated)</strong> </p> </th> 
   <th> <p><strong>Duration</strong> </p> </th> 
   <th> <p><strong>Planned Hours</strong> </p> </th> 
   <th><strong>Planned Duration</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 Days</p> </td> 
   <td> <p>24 Hours</p> <p>(3 Days x 8 Hours per Work Day = 24 Planned Hours)</p> </td> 
   <td> <p>3 Days</p> <p>(24 Planned Hours / 1 Assignee = 3 Days)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 Days</p> </td> 
   <td> <p>24 Hours</p> <p>(3 Days x 8 Hours per Work Day = 24 Planned Hours)</p> </td> 
   <td> <p>1.5 Days</p> <p>(24 Planned Hours / 2 Assignees = 12 Hours, or 1.5 Days)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 Days</p> </td> 
   <td> <p>24 Hours</p> <p>(3 Days x 8 Hours per Work Day = 24 Planned Hours)</p> </td> 
   <td> <p>1 Day</p> <p>(24 Planned Hours / 3 Assignees = 8 Hours, or 1 Day)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Change the Duration Type of a task to Effort Driven

For information about changing the Duration Type of a task, see [Update the Duration Type of a task](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Effort Driven</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong><strong>Changes</strong>.</li>
</ol>
-->
