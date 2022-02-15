---
filename: calculated-work
content-type: overview
product-area: projects
navigation-topic: task-duration
---



# Duration Type overview: Calculated Work  {#duration-type-overview-calculated-work}

Calculated Work is a Duration Type that you can set for a task in *`Adobe Workfront`*.


## Overview of the Calculated Work Duration Type {#overview-of-the-calculated-work-duration-type}

Calculated Work determines the amount of effort (Planned Hours) needed for the task to be completed. We recommend that you use the Calculated Work Duration Type when the resources assigned to the task are allocated for the entire duration of the task.


Your *`Workfront`* `or a *`group administrator`*` can set the default Duration&nbsp;Type of your system or group as Calculated Work.&nbsp;In this case, all new tasks will be created with this Duration Type. For information about changing your task and issue preferences as part of your system-level or group-level project preferences, see [Configure system-wide task and issue preferences](set-task-issue-preferences.md).


As resources are added to a task, a project manager can expect to see the planned effort increase. To illustrate, a one-hour planning meeting with three resources represents three total hours of work required, and a one-hour planning meeting with ten resources represents ten hours of work required. This assumes that each resource is allocated to the task with 100% allocation. 


## Review the formula for calculating the Work Required when using the Calculated Work Duration Type {#review-the-formula-for-calculating-the-work-required-when-using-the-calculated-work-duration-type}

When you use the Calculated Work Duration Type on a task, *`Workfront`* calculates the amount of Work for each task using the following two formulas. The formulas differ depending on what percentage of time each resource is allocated to the task and how many resources you have assigned to each task: 



* Simplified formula: Assuming you have one resource assigned to the task and they are allocated to the task for 100% of their available time, the Work Required value for each task is calculated using the following formula: 




```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```





* Complex formula: If you assign each resource with various allocations, the formula takes these allocations into account and accounts for these variations: 




```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```




## Review the effect of adding or removing resources from the task {#review-the-effect-of-adding-or-removing-resources-from-the-task}

When adding or removing assignees to a task with the Calculated Work duration type, Duration can be manually edited. As assignees are added or removed from the task, the Planned Hours change.


In the following example, the Typical Hours per Work Day is set to 8 in the Project Preferences in Setup. Each task has a Duration of 1 day. As the number of assignees changes, the Planned Hours changes based on the number of assignees on a given task:

<table style="width: 718px;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" border="1" cellspacing="15" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Number of Assignees (each 100% allocated)</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Duration</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p><span class="bold">Planned Hours</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>1</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>1 Day</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>8 Hours</p> <p>(1 Day x 8 Hours per Work Day x 1 Assignee = 8 Planned Hours)</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>2</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>1 Day</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>16 Hours</p> <p>(1 Day x 8 Hours per Work Day x 2 Assignees = 16 Planned Hours)</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>3</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>1 Day</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>24 Hours</p> <p>(1 Day x 8 Hours per Work Day x 3 Assignees = 24 Planned Hours)</p> </td> 
  </tr> 
 </tbody> 
</table>

In this case, each assignee is 100% allocated to the Calculated Work task.


![](assets/calcwork-350x71.png)




## Change the Duration Type of a task to Calculated Work {#change-the-duration-type-of-a-task-to-calculated-work}

For information about changing the Duration Type of a task, see [Update the Duration Type of a task](update-duration-type-of-task.md). 
