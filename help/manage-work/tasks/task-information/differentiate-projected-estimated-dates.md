---
filename: differentiate-projected-estimated-dates
content-type: overview
product-area: projects
navigation-topic: task-information
---



# Differentiate between Projected and Estimated Dates  {#differentiate-between-projected-and-estimated-dates}

There are several types of dates that show the timeline of tasks between when they can start and when they can complete.&nbsp;


When the task is first created, the Planned, Projected, and Estimated Dates should typically match. Some exceptions exist.&nbsp;


## Overview of Planned Dates {#overview-of-planned-dates}

The Planned Dates are the dates that the Project Owner defines as the start and the end dates of the tasks.&nbsp;


You or the Project Owner can manually modify the Planned Dates on a task. 


## Overview of Projected and&nbsp;Estimated Dates {#overview-of-projected-and-estimated-dates}

During the life of a project, the Projected and Estimated Dates are more in line with the reality of the project, as they take into account what can influence the actual start and end of a task. This causes them to change from the Planned Dates. 


Consider the following when working with Projected and Estimated Dates on tasks: 



* You cannot manually modify either the Estimated nor the Projected Dates of tasks. They are both calculated by *`Adobe Workfront`*.
*  When you create a task, the Projected and the Estimated dates should be identical and they should illustrate the actual times when the tasks can start or end.  
  Certain updates that you make to tasks directly affect the values of the Projected and Estimated Dates.&nbsp;


  For example, if the user starts or completes a task, the task displays Actual Start and Completion Dates which influence the Projected and Estimated Dates of the task. Also, if an assignee on the task modifies the Commit Date, this date influences the Projected Date of the task.





## Difference between Projected and Estimated Dates {#difference-between-projected-and-estimated-dates}

The difference between Projected and Estimated Dates is:



* Projected Dates are affected by a user making the following updates on the task:
    
    
    * Add a Constraint Date by adding a fixed Task Constraint 
    * Add a Commit Date
    
    
*   Estimated Dates only take into account the real progress on a task in a given point in time. 


  For example, if we have a task that has a Planned Start Date of September 20 and a Planned Completion Date of September 24, and it has Must Finish On Constraint, the Projected Completion Date September 24. This task has a Duration of 4 days. The Estimated Completion Date is calculated based on the current progress of the work on the task. So, if today is September 23 and the task has not started yet, the Estimated Completion Date is September 27 (it should be completed after 4 days, assuming that the work is started today). If the task is 50% completed today, the Estimated Completion Date is on September 25 (it should be completed after 2 days which is half of the Duration of the task). 



Here are some scenarios when the Projected Dates of tasks are changed during the life of a project:&nbsp;



*  When a task is marked as Complete: 


  *Projected Dates = Estimated Dates = Actual Dates* 

*  When a task has an Actual Start Date:


  *Projected Start Date = Estimated Start Date = Actual Start Date* 

*  When a task does not have an Actual Start Date, but there is a forced constraint on the Planned Start Date (Must Start On) that is in the future:


  *Projected Start Date = Constraint Date* 

*  When a task does not have an Actual Start Date and the task does not have a forced constraint date:


  *Projected Start Date = the next available date in the future that falls within working schedule* 

*  When the assignee updates the Commit Date:


  *Projected Completion Date = Commit Date* 

*  When the task does not have an updated Commit Date and the task has a forced constraint (Must Finish On) for the Planned Completion Date that is in the future:


  *Projected Completion Date = Constraint Date* 

*  When a task does not have an updated Commit Date, a forced constraint date in the future, or it has a Constraint Date in the past:


  *Projected Completion Date = system calculation for the Completion Date based on the current progress and the work left to be done* 



In comparison with the scenarios described above for the Projected Dates, the Estimated Dates always reflect the real analysis by the system on when the task will start or complete regardless of the Constraint or Commit Dates.


## What influences the timeline of a task {#what-influences-the-timeline-of-a-task}

The following are some examples of what can influence the real timeline of a task:&nbsp;



* task progress in relation to the Planned Dates and to the current day
* percent complete of the task so far
* predecessor relationship
* predecessor progress
*  user allocation 


  >[!NOTE]
  >
  >User allocation can influence the Estimated Completion&nbsp;Date of a task if they affect the speed with which the task can be completed. For example, if the task Duration Type is Effort Driven, you can make the task complete sooner by adding assignees. As a result, the Estimated Completion Date changes. 





