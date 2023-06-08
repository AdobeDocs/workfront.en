---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Task Constraint overview: Earliest Available Time'
description: Earliest Available Time is a Task Constraint that schedules a task to begin at the earliest available time after considering any predecessor relationships.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
---
# Task Constraint overview: Earliest Available Time

Earliest Available Time is a Task Constraint that schedules a task to begin at the earliest available time after considering any predecessor relationships.

For information about how to update the Task Constraint on a task, see [Update the Task Constraint of a task](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above) </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

   <!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit Task</strong>.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Earliest Available Time</strong>.</p>
   -->

   <!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save Changes</strong>.</li>
   -->

## The difference between Earliest Available Time and As Soon As Possible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

The Earliest Available Time constraint differs from the As Soon As Possible constraint when all of the following criteria exist:

* The project is scheduled From Completion 
* Tasks in the project have a predecessor relationship 
* The predecessor task has a flexible task constraint

In this situation:

* **Earliest Available Time:** Using the Earliest Available Time constraint on the successor task gives priority to the predecessor's flexible constraint.

  **EXAMPLE** 
  
  Task A is a predecessor to Task B. Task B has the Earliest Available Time constraint and Task A has the As Late As Possible constraint. In this situation, Task B is scheduled as close to the completion of the project as possible.

  ![Earliest Available Time constraint when task has the dates close to the project's Completion Date](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **As Soon As Possible:** In this scenario, using the As Soon As Possible constraint on the successor task gives the priority to the successor task.

  **EXAMPLE**
  
  Task A is a predecessor to Task B. Task B has the As Soon As Possible constraint and Task A has the As Late As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.

  ![As Soon As Possible constraint when task has the dates close to the project's Start Date](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
