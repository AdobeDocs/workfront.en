---
filename: start-no-earlier-than
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
---



# Task Constraint overview: Start No Earlier Than {#task-constraint-overview-start-no-earlier-than}

Use the Start No Earlier Than (SNET) Task Constraint to schedule a task to start after the date you specify.



## Overview of the Start No Earlier Than Task Constraint {#overview-of-the-start-no-earlier-than-task-constraint}

Consider the following when using the Start No Earlier Than Task Constraint: 



* You should use the Start No Earlier Than constraint when the project is scheduled From Start Date. In this case, you can provide a soft constraint on a task before it forces other dependent tasks to show as At Risk.
* Start No Earlier Than is the default constraint if a project is scheduled From Start Date and if the system `or group` default start date for a new task is set to Today. For information about configuring defaults for tasks, see [Configure system-wide task and issue preferences](set-task-issue-preferences.md).

* If you schedule the project From Start Date and the system default start date for a new task is set to Based on the Project Planned Date, the default constraint for a new task is As Soon As Possible. 
*  If you schedule the project From Completion Date project and the system default start date for a new task is set to Today, then the Start No Earlier Than constraint schedules the task as it would an As Late As Possible task. 
* When you move or copy a task with a SNET constraint to another project, the constraint of the task or the dates of the project might change depending on what the constraint dates are and what the Start and Completion Dates of the project are. The following scenarios exist: 
    
    
    * When the destination project is scheduled From Start:    
        
        
        * When the constraint date of the task is earlier than the project Planned Start Date, the task constraint changes to As Soon As Possible. 
        * When the constraint date of the task is later than the project Planned Completion Date, the project Planned Completion Date changes to match the completion constraint date of the task. 
        
        

    
        
        
        * When the destination project is scheduled From Completion:        
            
            
            * When the constraint date of the task is later than the Project Completion Date, the task constraint changes to As Late As Possible. 
            * When the constraint date of the task is earlier than the Planned Start Date of the project, the project Planned Start Date changes to match the start constraint date of the task. 
            
            
        * Regardless of the schedule of the project, when the constraint date of the task is within the Start and Completion Dates of the project, there are no changes to the Task Constraint or the project dates. 
        
        
    
    
    
  For information about moving tasks, see [Move tasks](move-tasks.md). For information about copying tasks, see [Copy and duplicate tasks](copy-and-duplicate-tasks.md). 



For information about how to update the Task&nbsp;Constraint on a task, see [Update the Task Constraint of a task](update-task-constraint-of-task.md). 
