---
filename: latest-available-time
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: Task Constraint overview: Latest Available Time
description: Latest Available Time (LAT) is a type of Task Constraint in Adobe Workfront.
---

# Task Constraint overview: Latest Available Time

Latest Available Time (LAT) is a type of Task Constraint in Adobe Workfront.

## Use the Latest Available Time Task Constraint

You can use the LAT constraint when you want to schedule a task to begin at the latest available time after considering predecessor-successor relationships in the project.

This constraint differs from As Soon As Possible in that it will not force predecessors or successors to be rescheduled. Rather, it will only affect the schedule of the task it is associated with, setting it to the latest available time based on its relationship to other tasks.

For information about how to update the Task&nbsp;Constraint on a task, see [Update the Task Constraint of a task](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
To update the Task Constraint to Latest Available Time: Go to a task whose Task Constraint you want to update. Click Edit Task. In the Overview section, expand the Task Constraint drop-down menu. Select Latest Available Time. Click Save Changes.
-->

## The difference between Latest Available Time and As Late As Possible

The Latest Available Time constraint differs from the As Late As Possible constraint when the following criteria exist:

* The project is scheduled From Completion 
* Tasks in the project have a predecessor relationship 
* The predecessor task has a flexible task constraint

In this situation:

* `Latest Available Time:` Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.

  For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.

* `As Late As Possible:` In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.

  For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the end of the project as possible.

