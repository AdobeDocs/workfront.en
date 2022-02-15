---
filename: task-duration-and-duration-type
content-type: overview
product-area: projects
navigation-topic: task-duration
---



# Overview of Task Duration and Duration Type {#overview-of-task-duration-and-duration-type}

The task Duration is the difference between the Planned Completion Date and the Planned Start Date of the task. The Duration indicates the time frame that is available for the task to get completed.


## Task Duration overview {#task-duration-overview}



>[!NOTE]
>
>When taking into account the Primary Assignee's time off on a project, the planned dates of the task might adjust, but the Duration of the task remains the same. For information about taking into account the time off of the Primary Assignee when planning a project, see ` [Configure system-wide project preferences](set-project-preferences.md)`. 


If the Actual Start and&nbsp;Actual Completion Dates of the task fall outside of the schedule of the project, primary assignee, or the Default Schedule, the task&nbsp;Duration is zero. 


` `**Example: **``If you have a schedule that starts at 9:00&nbsp;AM and ends at 12:00&nbsp;PM and a task that is scheduled to start at 2:00 PM and end at 4:00 PM, the task's Duration is zero. 


The following are two scenarios that exist when calculating duration in  *`Adobe Workfront`*. 



*  If the task is assigned to a user *`Workfront`* uses one of the following schedules, in this exact order to calculate Duration: 

    
    
    1.  *`Workfront`* takes into account the user's schedule. 
    1.  If the user is not associated with a schedule, *`Workfront`* takes into account the project's schedule.
    1.  If the project is not associated with a schedule, *`Workfront`* takes into account the Default Schedule of your system. For information about schedules, see [Create a schedule](create-schedules.md). 
    
    






*  If the task is assigned to multiple users:


  *`Workfront`* takes into account either the schedule of the project or that of the primary assignee. 


  Your *`Workfront administrator`* determines which schedule *`Workfront`* uses when a task is assigned to multiple users. For information, see [Configure system-wide project preferences](set-project-preferences.md). 


  The steps are similar to the first scenario after understanding which schedule *`Workfront`* uses to calculate Duration. 





## Units of time for Task Duration {#units-of-time-for-task-duration}

You can indicate task&nbsp;Duration in both the regular time and the elapsed time between the Planned Start and Planned Completion Dates. 


When updating the Duration of tasks in a list, you can use the following abbreviations for indicating units of time in  *`Workfront`*: 


` `**Example: **`` If you want to indicate that a task's Duration is 3 Elapsed Day, you would type "3 ED" in the Duration field in a task list . `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> You can also select the preferred option for the Duration Unit of Time from the available drop-down menu when editing a task or in the Task&nbsp;Details section. </MadCap:conditionalText>`For information about editing tasks, see [Edit tasks](edit-tasks.md). 


![](assets/duration-elapsed-days-tasks-nwe-350x282.png)


Consider the following when indicating the Duration of a task: 



*  Elapsed time is a unit of time for a task's Duration. It is the time between the Planned Start Date and the Planned Completion Date of a task that includes holidays, weekends, and time off. In other words, elapsed time is the passage of calendar days. 
*  Regular time takes into account holidays, weekends, and time off and excludes them from the Duration of the task. 





*  When you indicate the Duration of a task in weeks, *`Workfront`* calculates the Duration in days and hours based on the Typical work days per week and Typical hours per work day settings set by your *`Workfront administrator`* in the Project&nbsp;Preferences area of Setup.
*  *`Workfront`* uses the default duration of 4 weeks for one month when calculating Duration in months.




## Task Duration Type overview {#task-duration-type-overview}

The Duration Type of a task identifies the relationship between the number of resources assigned to a task, the total effort, and the total Duration of the task. It enables you to set consistent resource assignments based on the needs of the task. 


Duration Type helps to answer the following questions:



* How busy are we going to be?
* How big is the job?
* How long is it going to take?


![duration_type_triangle.png](assets/duration-type-triangle-350x245.png)




## Define Duration Types {#define-duration-types}


<table style="width: 717px;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" border="1" cellspacing="15" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th style="width: 143px;" scope="row" class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Duration Type </th> 
   <th style="width: 294.5px;" scope="col" class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Function</span> </p> </th> 
   <th style="width: 276.5px;" scope="col" class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p><span class="bold">How Resources Affect It</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <th style="width: 143px;" scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><span class="bold">Calculated Assignment</span> </p> </th> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Calculates the allocation percentage for each assignee on a task. </p> <p>When you choose this Duration Type, you can input individual Duration and Planned Hours for the task. <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> divides the Planned Hours by the number of hours inside the Duration of the task, then by the number of resources assigned to the task to calculate the allocation for each assignee.</p> <p>For more detailed information, see <a href="calculated-assignment.md" class="MCXref xref">Duration Type overview: Calculated Assignment</a>.</p> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Duration and Planned Hours do not change when adding or removing assignees to the task. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <th style="width: 143px;" scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span class="bold">Calculated Work</span> </p> </th> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Determines the Planned Hours (amount of effort) required for the task to be completed.</p> <p>Normally used when the resources assigned to the task are allocated for the entire Duration of the task.</p> <p>When you choose this Duration Type, you have the ability to input an individual Duration for the task. <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates the Planned Hours for the task by multiplying the number of days in the Duration by the number of work hours in the schedule and by the number of assignees to the task. </p> <p>You have the ability to manually change the allocation percentage of each assignee to the task which will shorten the amount of the Planned Hours.</p> <p>For more detailed information, see <a href="calculated-work.md" class="MCXref xref">Duration Type overview: Calculated Work </a>.</p> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Planned Hours increase when assignees are added to the task. </p> <p>Planned Hours decrease when assignees are removed from the task.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <th style="width: 143px;" scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Effort Driven</p> </th> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Determines the Planned Hours based on the number of resources.</p> <p>When you choose this Duration Type, you have the ability to input an individual Duration for the task. <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates the Planned Hours for the task by multiplying the number of days in the Duration by the number of work hours in the schedule and dividing that by the number of assignees to the task. </p> <p>You have the ability to manually change the allocation percentage of each assignee to the task, but the number of Planned Hours remains the same.</p> <p>For more detailed information, see <a href="effort-driven.md" class="MCXref xref">Duration Type overview: Effort Driven </a>.</p> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Planned hours increase when assignees are removed from the task.</p> <p>Planned hours decrease when assignees are added to the task. </p> <p>The Duration does not change, regardless of changes in the number of assignees or their schedule. </p> <p>Duration is equal to Planned Hours. Planned Duration is equal to Planned Hours divided by the number of assignees.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <th style="width: 143px;" scope="col" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p><span class="bold">Simple</span> </p> </th> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>Determines the Planned Hours and the Duration (which are the same, for this Duration Type) based on the number of hours each assignee is allocated for. </p> <p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates the Planned Hours by adding up the planned allocated hours for each assignee. </p> <p>You have the ability to manually change the amount of hours that each assignee is allocated for, and the number of Planned Hours and the amount of the Duration changes accordingly. If you choose a total number of allocated hours for all the assignees, that number is divided equally between each assignee.</p> <p>For more detailed information, see <a href="simple-duration-type.md" class="MCXref xref">Duration Type overview: Simple </a>.</p> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Hours are distributed evenly among assignees if you choose a total number of allocated hours. However, as the project manager, you can manually adjust the hours for each assignee. </p> <p>You can either edit Planned Hours and Duration of a task with a Simple Duration Type inline or at the task level. </p> <p>If an agile team is assigned to a task, the Duration Type is automatically set to Simple and cannot be changed. The task duration for an agile team must be greater than 0 minutes.</p> </td> 
  </tr> 
 </tbody> 
</table>



##  The Duration&nbsp;Type of new tasks {#the-duration-type-of-new-tasks}

The Duration Type of a new task matches the Duration Type set up in your system. The default Duration Type is Calculated Assignment. Your *`Workfront administrator`* `or a *`group administrator`*` can update the default Duration Type for your system `or for the group associated with the project`.&nbsp;For information, see [Configure system-wide task and issue preferences](set-task-issue-preferences.md). 


## Change the Duration Type of a task {#change-the-duration-type-of-a-task}

For information about changing the Duration Type of a task, see [Update the Duration Type of a task](update-duration-type-of-task.md).
