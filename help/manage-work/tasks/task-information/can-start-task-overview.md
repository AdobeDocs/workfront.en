


# Task&nbsp;Can Start overview {#task-can-start-overview}

When a task is ready to start, *`Adobe Workfront`* adds a Can Start indicator to the task to easily identify that it's safe for you to start working on the task. You can view this indicator in the view of a task list or report. 


When the start is ready to be worked on, the Can Start field on the task is set to True. 


## Task Can Start overview {#task-can-start-overview-1}

*`Workfront`* checks for the following things before it marks a task as True for the Can Start field:  




*  If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;
*   It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;


  For information about task predecessors, see [Overview of task predecessors](predecessors-overview.md).





## Considerations about identifying tasks that are ready to start {#considerations-about-identifying-tasks-that-are-ready-to-start}




*  If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see [Overview of task dependency types](task-dependency-types.md). 
*  If a task has a cross-project predecessor, the completion of the predecessor does not trigger the Can Start indicator to apply to the successor automatically. You must recalculate the timeline of the successor's project before the successor task displays as a Can&nbsp;Start task. 


  For information about cross-project predecessors, see [Create cross-project predecessors](cross-project-predecessors.md).


  For information about recalculating project timelines, see [Recalculate project timelines](recalculate-project-timeline.md).



