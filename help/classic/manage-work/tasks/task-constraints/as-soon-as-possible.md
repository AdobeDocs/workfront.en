---
filename: as-soon-as-possible
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: Task Constraint overview: As Soon As Possible
description: As Soon As Possible is a task constraint that places the start time of the task as close to the beginning of the project as possible.
---

# Task Constraint overview: As Soon As Possible

As Soon As Possible is a task constraint that places the start time of the task as close to the beginning of the project as possible.

## Considerations for using the As Soon As Possible constraint

* As Soon As Possible is the default constraint if a project uses a Schedule Mode of Schedule from Start Date and if the system default start date for a new task is set to Based on the Project Planned Date.  

* If a project uses a schedule mode of Schedule from Start Date and if the system `or group` default Start Date for a new task is set to Today, then the default Task Constraint is Start No Earlier Than.

  For information about where to set the default Constraint for a new task, refer to [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

For information about how to update the Task&nbsp;Constraint on a task, see [Update the Task Constraint of a task](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
To update the Task Constraint to As Soon As Possible: Go to a task whose Task Constraint you want to update. Click Edit Task. In the Overview section, expand the Task Constraint drop-down menu. Select As Soon As Possible. Click Save Changes.
-->

## The difference between Earliest Available Time and As Soon As Possible

The Earliest Available Time constraint differs from the As Soon As Possible constraint when all of the following criteria exist:

* The project is Scheduled From Completion. 
* Tasks in the project have a predecessor relationship. 
* The predecessor task has a flexible task constraint.

In this situation:

* `Earliest Available Time:` Using the Earliest Available Time constraint on the successor task gives priority to the predecessor's flexible constraint.

  For example, suppose that Task A is a predecessor to Task B. Task B has the Earliest Available Time constraint and Task A has the As Late As Possible constraint. In this situation, the task is scheduled as close to the completion of the project as possible.

* `As Soon As Possible:` In this scenario, using the As Soon As Possible constraint on the successor task gives the priority to the successor task.

  For example, suppose that Task A is a predecessor to Task B. Task B has the As Soon As Possible constraint and Task A has the As Late As Possible constraint. In this situation, the task is scheduled as close to the start of the project as possible.

