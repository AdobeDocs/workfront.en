---
filename: recurring-tasks-overview
content-type: overview
product-area: projects
keywords: recurrent,reoccur,reoccurring
navigation-topic: manage-tasks
title: Recurring tasks overview
description: You can create recurring tasks for activities that you have to repeat as part of a single project.
---

# Recurring tasks overview

You can create recurring tasks for activities that you have to repeat as part of a single project.

This article outlines information and considerations about creating and editing recurring tasks.

For information about how to create recurring tasks in Adobe Workfront, see [Create recurring tasks](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Recurring Tasks overview and considerations

You may choose to create recurring tasks to indicate repeatable work during the life of a project.

For example, during an IT project, software likely needs to be backed up at regular intervals. Creating a recurring task for this activity reduces the time required to set up multiple individual tasks.

Consider the following when creating recurring tasks in Workfront:

* You cannot add recurring tasks to a template. 
* You cannot add a recurrence frequency to an existing task. 
* Recurring tasks appear as subtasks or children for the main occurrence which appears as the parent task. 
* You cannot attach an approval to a parent recurring task. 
* Workfront transfers most fields that you update for the parent recurrence when creating it to the children tasks.&nbsp;The following fields do not transfer to the children tasks when they are created:

   * The Task Constraint of the children tasks automatically changes to:

      * Must Start On for projects that are planned from Start Date. 
      * Must Complete On for projects that are planned from Completion Date.

   * ```<li> <p>Documents attached to the parent do not transfer to the children. </p> </li>```

* The following changes occur on the parent task after you indicate that the task is recurring:

   * The Duration field is renamed to Duration per Occurrence for the parent task. It remains Duration for the children tasks. 
   * Status is disabled on the parent task and it is automatically set to New on the children. The parent task automatically completes and the status updates to&nbsp;Complete when all children are completed. 
   * The only Duration Types available for recurring tasks are:

      * Simple
      * Effort Driven

## Considerations for editing recurring tasks

Some changes you make to a recurring task parent might not update on all existing recurrences. Children tasks that show progress or have been updated individually will not update when you update the parent. Workfront considers that a task shows progress in the following situations:

* Status is updated and the task is no longer New
* The Percent Complete of the task is higher than zero
* The task has predecessor relationships

The following table illustrates whether changes made to the parent trigger updates on the children that have not been individually edited or show progress:

| ```Fields updated on the parent task```  |Updates transfer to unedited children or children with no progress recorded |
|---|---|
| ```Recurrence Frequency*```  |✔ |
| Assignments&#42;&#42; | ✔ |
| Name | ✔ |
| Description | ✔ |
| Priority | ✔ |
| Duration | ✔ |
| Planned Hours | ✔ |
| Cost Type | ✔ |
| Revenue&nbsp;Type | ✔ |
| Resource Leveling | ✔ |
| Leveling Delay | ✔ |
| Task&nbsp;Constraint |Does not update the children |
| Attach or remove Custom&nbsp;Forms |Does not update the children |
| Duration&nbsp;Type |Does not update the children |
| Custom&nbsp;Form information |Does not update the children |

&#42; The following scenarios exist when you update the&nbsp;Recurrence Frequency of a parent task:

* If you change the Recurrence Frequency on an existing parent task, the existing subtasks are deleted and replaced with new subtasks that follow the new recurrence frequency if they don't show any progress and if you have not manually updated them. 
* If you change the Recurrence Frequency on an existing parent task, subtasks that show progress are not deleted. These tasks are considered separate from the recurrence at this point.

&#42;&#42; Assignments made on the parent task are applied to all subtasks in the recurrence. Any changes made to the assignment on the parent task override any individual assignments on the subtask. If the task shows progress, the assignment does not change.

&nbsp;
