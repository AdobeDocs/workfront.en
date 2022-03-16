---
filename: finish-no-later-than
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: Task Constraint overview: Finish No Later Than
description: Finish No Later Than (FNLT) is a Task Constraint that schedules a task to complete before the date you specify.
---

# Task Constraint overview: Finish No Later Than

Finish No Later Than (FNLT) is a Task Constraint that schedules a task to complete before the date you specify.

## Overview of the Finish No Later Than constraint

Consider the following when using the Finish No Later Than (FNLT) constraint for a task:

* You should use this constraint when the project is scheduled From Start Date. In this case, you can provide a soft constraint on a task before it forces other dependent tasks to show as At Risk.
* When you use the FNLT constraint with a Schedule From Completion Date project, this constraint schedules the task as it would an As Late As Possible task.
* When you move or copy a task with a FNET constraint to another project, the constraint of the task or the dates of the project might change depending on what the constraint dates are and what the Start and Completion Dates of the project are. The following scenarios exist:

  * When the destination project is scheduled From Start:

    * When the constraint date of the task is earlier than the project Planned Start Date, the task constraint changes to As Soon As Possible. 
    * When the constraint date of the task is later than the project Planned Completion Date, the project Planned Completion Date changes to match the completion constraint date of the task.

    * When the destination project is scheduled From Completion:

      * When the constraint date of the task is later than the Project Completion Date, the task constraint changes to As Late As Possible. 
      * When the constraint date of the task is earlier than the Planned Start Date of the project, the project Planned Start Date changes to match the start constraint date of the task.

    * Regardless of the schedule of the project, when the constraint date of the task is within the Start and Completion Dates of the project, there are no changes to the Task Constraint or the project dates.

  For information about moving tasks, see [Move tasks](../../../manage-work/tasks/manage-tasks/move-tasks.md). For information about copying tasks, see [Copy and duplicate tasks](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

For information about how to update the Task&nbsp;Constraint on a task, see [Update the Task Constraint of a task](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
Use the Finish No Later Than constraint To update the Task Constraint to Finish No Later Than: Go to a task whose Task Constraint you want to update. Click the More icon next to the task name, then click Edit. In the Overview section, expand the Task Constraint drop-down menu. Select Finish No Later Than. Specify a Planned Completion Date. You must complete the task on and not later than this date. Click Save Changes.
-->

