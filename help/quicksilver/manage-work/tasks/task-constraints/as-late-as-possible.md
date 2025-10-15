---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Task Constraint Overview: As Late As Possible'
description: As Late As Possible (ALAP) is a Adobe Workfront Task Constraint which places the completion time of the task as close to the end of the project as possible.
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
---
# Task Constraint overview: As Late As Possible

As Late As Possible (ALAP) is a Adobe Workfront Task Constraint which places the completion time of the task as close to the end of the project as possible.

Using this constraint may cause predecessor or dependent Tasks to be rescheduled.

For more information about predecessor relationships, see [Use task predecessors: article index](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

As Late as Possible is the default constraint if a project uses a schedule mode of Schedule from Completion Date and system or group default for the Start Date of a task is Based on the Project Planned Date.

For information about where to set the default Constraint for a new task, refer to [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

For information about how to update the Task Constraint on a task, see [Update the Task Constraint of a task](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## The difference between Latest Available Time and As Late As Possible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

The Latest Available Time constraint differs from the As Late As Possible constraint when the following criteria exist:

* The project is scheduled From Start Date
* Tasks in the project have a predecessor relationship 
* The successor task has a flexible task constraint

In this situation:

* **Latest Available Time:** Using the Latest Available Time constraint on the predecessor task gives priority to flexible constraint of the successor.

  **Example:** For example, Task A is a predecessor to Task B. Task A has the Latest Available Time constraint and Task B has the As Soon As Possible constraint. In this situation, Task A is scheduled as close to the start of the project as possible.

  ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **As Late As Possible:** In this scenario, using the As Late As Possible constraint on the predecessor task gives the priority to the predecessor task.

  **Example:** For example, Task A is a predecessor to Task B. Task A has the As Late As Possible constraint and Task B has the As Soon As Possible constraint. In this situation, Task A is scheduled as close to the end of the project as possible.

  ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

 

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest Available Time constraint differs from the As Late As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
