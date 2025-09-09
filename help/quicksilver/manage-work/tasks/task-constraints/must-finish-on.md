---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Task Constraint Overview: Must Finish On'
description: You can use the Must Finish On (MFO) Task Constraint to schedule a task to end on a specific date.
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
---
# Task Constraint overview: Must Finish On

You can use the Must Finish On (MFO) Task Constraint to schedule a task to end on a specific date. 

The Must Finish On constraint schedules a task to finish exactly at the time and date you specify in the **Planned Completion Date** field.

>[!TIP]
>
>Manually updating a task's Planned Completion Date changes the constraint of the task to Must Finish On.

## Overview of the Must Finish On Task Constraint

Consider the following when scheduling a task with a Must Finish On constraint:

* Predecessor relationships do not force the task to be rescheduled. Adobe Workfront essentially ignores the predecessor relationships.
* The task shows as **At Risk** if the predecessors begin to run behind or are late.

* When you move or copy a task with a MFO constraint to another project, the constraint of the task or the dates of the project might change depending on what the constraint dates are and what the Start and Completion Dates of the project are. The following scenarios exist:

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
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Must Finish On Task Constraint</h2>
<p>To update the Task Constraint to Must Finish On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Finish On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete by this date, and no later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
