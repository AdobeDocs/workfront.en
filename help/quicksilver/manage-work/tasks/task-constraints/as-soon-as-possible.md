---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Task Constraint Overview: As Soon As Possible'
description: As Soon As Possible is a task constraint that places the start time of the task as close to the beginning of the project as possible.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
---
# Task Constraint overview: As Soon As Possible

As Soon As Possible is a task constraint that places the start time of the task as close to the beginning of the project as possible.

## Considerations for using the As Soon As Possible constraint

* As Soon As Possible is the default constraint if a project uses a Schedule Mode of Schedule from Start Date and if the system default start date for a new task is set to Based on the Project Planned Date.  

* If a project uses a schedule mode of Schedule from Start Date and if the system or group default Start Date for a new task is set to Today, then the default Task Constraint is Start No Earlier Than.

  For information about where to set the default Constraint for a new task, refer to [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

For information about how to update the Task&nbsp;Constraint on a task, see [Update the Task Constraint of a task](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Soon As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Soon As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## The difference between Earliest Available Time and As Soon As Possible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

The Earliest Available Time constraint differs from the As Soon As Possible constraint when all of the following criteria exist:

* The project is Scheduled From Completion. 
* Tasks in the project have a predecessor relationship. 
* The predecessor task has a flexible task constraint.

In this situation:

* **Earliest Available Time:** Using the Earliest Available Time constraint on the successor task gives priority to the predecessor's flexible constraint.

  For example, suppose that Task A is a predecessor to Task B. Task B has the Earliest Available Time constraint and Task A has the As Late As Possible constraint. In this situation, the task is scheduled as close to the completion of the project as possible.

* **As Soon As Possible:** In this scenario, using the As Soon As Possible constraint on the successor task gives the priority to the successor task.

  For example, suppose that Task A is a predecessor to Task B. Task B has the As Soon As Possible constraint and Task A has the As Late As Possible constraint. In this situation, the task is scheduled as close to the start of the project as possible.
