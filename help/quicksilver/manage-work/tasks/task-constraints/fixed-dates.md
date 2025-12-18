---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Task Constraint Overview: Fixed Dates'
description: You can use the Fixed Dates task constraint when you want to be specific about the exact start date and end date of your tasks. For more information about task constraints, see Task Constraint overview.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
---
# Task Constraint overview: Fixed Dates

You can use the Fixed Dates task constraint when you want to be specific about the exact start date and end date of your tasks. For more information about task constraints, see [Task Constraint overview](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## Overview of the Fixed Dates constraint

Consider the following when using the Fixed Dates constraint:

* When you select the Fixed Dates (FIXT) task constraint, you must specify the Planned Start Date and Planned Completion Date of the task. In this case, the predecessor relationship of the task is ignored. 
* The Duration field of the task is not editable when using the FIXT constraint. Duration is calculated as the difference between the Planned Start and Planned Completion Dates of the task. 
* If the Duration Type of the task is Effort Driven, the number of assignees on the task also affect the Duration of the task.
* When you move or copy a task with a FIXT constraint to another project, the constraint of the task or the dates of the project might change depending on what the constraint dates are and what the Start and Completion Dates of the project are. The following scenarios exist:

   * When the destination project is scheduled From Start:

      * When any constraint dates of the task are earlier than the Project Start Date, the task constraint changes to As Soon As Possible. 
      * When any or both constraint dates of the task are later than the Planned Completion Date of the project, the project Planned Completion Date changes to match the completion constraint date of the task.

   * When the destination project is scheduled From Completion:

      * When any constraint dates of the task are later than the Project Completion Date, the task constraint changes to As Late As Possible. 
      * When any or both constraint dates of the task are earlier than the Planned Start Date of the project, the project Planned Start Date changes to match the start constraint date of the task.

   * Regardless of the schedule of the project, when the constraint dates of the task are within the Start and Completion Dates of the project, there are no changes to the Task Constraint or the project dates.

  For information about moving tasks, see [Move tasks](../../../manage-work/tasks/manage-tasks/move-tasks.md). For information about copying tasks, see [Copy and duplicate tasks](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

For information about how to update the Task&nbsp;Constraint on a task, see [Update the Task Constraint of a task](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Fixed Dates</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start on this date. </p> </li>
<li value="6"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete on this date. </p> </li>
<li value="7">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
