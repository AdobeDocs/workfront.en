---
filename: task-progress-status
content-type: overview
product-area: projects
navigation-topic: task-information
---



# Task Progress Status overview {#task-progress-status-overview}

*`Adobe Workfront`* determines the Progress Status of a task by looking at the progression of the task across its timeline. You can configure *`Workfront`* to determine the Condition of a project based on the value of the Progress Status of the tasks. For more information about configuring the Condition of the project, see the article [Overview of Project Condition and Condition Type](project-condition-and-condition-type.md). 


## Criteria that determine the Progress Status of tasks {#criteria-that-determine-the-progress-status-of-tasks}

For information about the Progress Status of a project, see [Project Progress Status overview](project-progress-status.md). 


For information about tracking the progress of your tasks, see [Task Tracking Mode overview](task-tracking-mode.md).


The following criteria determine the Progress Status of a task: 

<table style="width: 719px;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" border="0" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Progress Status</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p><span class="bold">Determining Criteria</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top" class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>&nbsp;</p> <p><span class="bold"><br>On Time</span> </p> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>A task is considered <span class="bold">On Time</span> when all the Planned Dates match the Projected Dates. This Progress Status could also mean that the project is ahead of schedule and the Projected Dates could be before the Planned Dates.</p> <p>For more information about Projected Dates, see <a href="project-projected-completion-date.md" class="MCXref xref">Overview of the Projected Completion Date for projects, tasks, and issues</a>.</p> <p>For more information about Planned Dates, see <a href="project-planned-completion-date.md" class="MCXref xref">Overview of the project Planned Completion Date </a>.</p> </td> 
  </tr> 
  <tr valign="top" class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>&nbsp;</p> <p><span class="bold">At Risk</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>A task is considered <span class="bold">At Risk</span> when the Estimated Completion Date is later than the Planned Completion Date and later than the Projected Completion Date. This can happen when a task has a constraint of <span class="bold">Must Finish On</span> or <span class="bold">Must Start On</span> but the percent complete or the predecessor relationships of the task show that it cannot finish or start on the specified dates. </p> <p> Setting the Task Constraint to <span class="bold">Must Finish On</span> manually sets the Planned Completion Date to a specific date. The Projected Completion Date in this case matches the Planned Completion Date. In the case of this constraint, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> analyzes the task to calculate when it will finish based on the percent completed. This calculation is stored as the Estimated Due Date. If the Estimated Due Date is after the Projected Completion Date, the task is considered at risk of being late. </p> <p> Setting the Task Constraint to <span class="bold">Must Start On</span> manually sets the Planned Start Date to a specific date. The Projected Start Date in this case matches the Planned Start Date. In the case of this constraint, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> analyzes the task to calculate when it will start based on its predecessor relationships. This calculation is stored as the Estimated Start Date. If there is an enforced predecessor that will not allow the task to start on the specified Start Date, then the Estimated Start Date can be after the Projected Completion Date. The task is considered at risk of being late. </p> <p>Note:  Typically, Estimated Dates match Projected Dates except for when <span class="bold">Must Start On</span> or <span class="bold">Must Finish On</span> are used. In these cases, Estimated Dates continue to calculate based on percent complete and other factors (predecessor relationships), while the Projected Dates are forced to match the Planned Dates which have been set manually.</p> </td> 
  </tr> 
  <tr valign="top" class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><span class="bold"><br>Behind</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>A task is considered to be <span class="bold">Behind</span> when the Estimated Completion Date is later or equal than the Planned Completion Date and sooner than the Projected Completion Date.</p> <p>The Projected Completion Date is a real-time view of when the task will be completed based on prior progress. Though the task was started late, it is not considered late yet, because the Planned and Projected Completion Dates are still in the future, and the task might still be completed on time.</p> <p>Note:  The <span class="bold">Behind</span> and <span class="bold">At Risk</span> Progress Statuses are almost identical. However, <span class="bold">At Risk</span> indicates there are some forced Task Constraints (Must Finish On, Must Start On, Fixed Dates) on one or both of the Planned Dates. If there are no forced constraints on the task, the Projected Dates are the same as the Estimated Dates and reflect the system calculation of the Completion Date based on the current progress of the task. The task is not considered late yet, because the Planned and Projected Completion Dates are still in the future, and the task might still be completed on time.<br>For more information about the Projected and the Estimated Dates, see <a href="differentiate-projected-estimated-dates.md" class="MCXref xref">Differentiate between Projected and Estimated Dates </a>.</p> </td> 
  </tr> 
  <tr valign="top" class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p><span class="bold">Late</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>A task is <span class="bold">Late</span> when the Planned Completion Date is before today's date.<br></p> </td> 
  </tr> 
 </tbody> 
</table>



## How task Progress Status updates over time {#how-task-progress-status-updates-over-time}

The different date types in our projects tell us how tasks are progressing over time: 



*  On Time


  ![](assets/on-time-progress-status-350x233.png)



*  At Risk


  ![](assets/at-risk-progress-status-350x233.png)



*  Behind


  ![](assets/behind-progress-status-350x233.png)



*  Late


  ![](assets/late-progress-status-350x233.png)





