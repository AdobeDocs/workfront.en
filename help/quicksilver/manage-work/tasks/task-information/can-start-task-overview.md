---
content-type: overview
product-area: projects
navigation-topic: task-information
title: '`Can Start` overview for tasks'
description: When a task is ready to start, Adobe Workfront adds a Can Start indicator to the task to easily identify that it's safe for you to start working on the task. You can view this indicator in the view of a task list or report.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
---
# "Can Start" overview for tasks

When a task is ready to start, Adobe Workfront adds a Can Start indicator to the task to easily identify that it's safe for you to start working on the task. You can view this indicator in the view of a task list or report.

When the task is ready to be worked on, the Can Start field on the task is set to True.

## How Workfront marks a task as "Can Start"

Workfront checks for the following things before it marks a task as True for the Can Start field:

* Whether the value of Can Start for the parent it set to True, if the task has a parent. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.
* Whether the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.
* Whether the task dependency type is either Start-Start or Start-Finish. If the dependency type is Start-Start or Start-Finish, the dependent task will have the "Can start" flag set to True after the predecessor task is in progress (or after the percent complete of the predecessor task is greater than 1%). 

  For information about task predecessors, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Considerations about identifying tasks that are ready to start

* If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see [Overview of task dependency types](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md). 
* If a task has a cross-project predecessor, the completion of the predecessor does not trigger the Can Start indicator to apply to the successor automatically. You must manually recalculate the timeline of the successor's project or Workfront must automatically recalculate it, before the successor task displays as a Can&nbsp;Start task. For more information about recalculating project timelines, see [Recalculate project timelines](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

  For information about cross-project predecessors, see [Create cross-project predecessors](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
