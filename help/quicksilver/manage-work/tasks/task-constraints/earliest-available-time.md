---
filename: earliest-available-time
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: Task Constraint overview: Earliest Available Time
description: Earliest Available Time is a Task Constraint that schedules a task to begin at the earliest available time after considering any predecessor relationships.
---

# Task Constraint overview: Earliest Available Time

Earliest Available Time is a Task Constraint that schedules a task to begin at the earliest available time after considering any predecessor relationships.

For information about how to update the Task&nbsp;Constraint on a task, see [Update the Task Constraint of a task](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
To update the Task Constraint to Earliest Available Time:
-->

   <!--
   Go to a task whose constraint you want to modify.
   -->

1. 

   <!--
   Click Edit Task.
   -->

   <!--
   Click the More icon next to the task name, then click Edit.
   -->

1. 

   <!--
   In the Overview section, expand the Task Constraint drop-down menu.
   -->

1. 

   <!--
   Select Earliest Available Time.
   -->

   <!--
   Click Save Changes.
   -->

## The difference between Earliest Available Time and As Soon As Possible

The Earliest Available Time constraint differs from the As Soon As Possible constraint when all of the following criteria exist:

* The project is scheduled From Completion 
* Tasks in the project have a predecessor relationship 
* The predecessor task has a flexible task constraint

In this situation:

* `Earliest Available Time:` Using the Earliest Available Time constraint on the successor task gives priority to the predecessor's flexible constraint.

  ` `**Example: **`` Task A is a predecessor to Task B. Task B has the Earliest Available Time constraint and Task A has the As Late As Possible constraint. In this situation, Task B is scheduled as close to the completion of the project as possible.

  ![Earliest Available Time constraint when task has the dates close to the project's Completion Date](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* `As Soon As Possible:` In this scenario, using the As Soon As Possible constraint on the successor task gives the priority to the successor task.

  ` `**Example: **``  Task A is a predecessor to Task B. Task B has the As Soon As Possible constraint and Task A has the As Late As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.

  ![As Soon As Possible constraint when task has the dates close to the project's Start Date](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)

