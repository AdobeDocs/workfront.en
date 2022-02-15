---
filename: track-costs
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
---



# Track costs {#track-costs}

You can track costs for projects, tasks, and issues in *`Adobe Workfront`*. 


*`Workfront`* also calculates a number of cost performance indexes for projects so they can be tracked for cost efficiency.  
For more information about calculating cost-performance indexes, see:



*  [Calculate Cost Performance Index (CPI)](calculate-cpi.md) 
*  [Calculate Cost Schedule Performance Index (CSI)](calculate-csi.md) 
*  [Calculate Schedule Performance Index (SPI)](calculate-spi.md) 




## How *`Workfront`* tracks costs for tasks and projects {#how-workfront-tracks-costs-for-tasks-and-projects}




* [How Workfront tracks costs](#understa) 
* [How Workfront calculates Planned, Budgeted, and Actual Costs](#understanding-how-planned-and-actual-costs-are-calculated) 
* [How Workfront calculates Cost Types for tasks](#modifying-cost-types-for-individual-tasks) 




### How *`Workfront`* tracks costs  {#how-workfront-tracks-costs}

You can track several types of Costs for tasks and projects in *`Workfront`*. Overall Costs are calculated by the following formula:




```
Costs = Labor Costs + Expense Costs
```





*  `Labor Costs` are associated with the hours on tasks and projects and the Cost per Hour rates of the resources associated with tasks. Generally, *`Workfront`* calculates the following labor costs:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStylesheets/Standard.css');" class="TableStyle-Standard" cellspacing="3"> 
 <col class="TableStyle-Standard-Column-Column1"> 
 <col class="TableStyle-Standard-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Planned Labor Costs</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray"> <p>They are calculated using the following formula:</p><pre>Planned Labor&nbsp;Costs = Planned Hours * Cost per Hour rate</pre> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: bold;">Budgeted Labor&nbsp;Costs</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray"> <p>They are calculated using the following formula:</p><pre>Budgeted Labor&nbsp;Costs = Budgeted Hours * Cost per Hour rate</pre> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyB-Column1-LightGray" style="font-weight: bold;">Actual Labor Costs</td> 
   <td class="TableStyle-Standard-BodyA-Column1-LightGray"> <p>They are calculated using the following formula:</p><pre>Actual Labor&nbsp;Costs = Actual Hours * Cost per Hour rate</pre> </td> 
  </tr> 
 </tbody> 
</table>

  For more information, see the [How Workfront calculates Planned, Budgeted, and Actual Costs](#understanding-how-planned-and-actual-costs-are-calculated) section in this article. 

* `Expense Costs` are associated with Expenses on projects and tasks.  
  When you create a project, you can set planned expenses for the entire project. Additionally, you can associate expenses with new or existing tasks. For information, see [Manage project expenses](manage-project-expenses.md). 

*  **Fixed Costs** are defined as a fixed amount of cost for a project. This is part of the Planned Cost of the project which represents the amount of money that you need to complete the project.


  >[!TIP] {type="tip"}
  >
  >When attaching a template to a project, the Fixed Cost of a template is added to the Fixed Cost of the project. For information, see [Overview of attaching a template to a project](attach-template-to-project-overview.md). 







### How *`Workfront`* calculates Planned, Budgeted, and Actual Costs {#how-workfront-calculates-planned-budgeted-and-actual-costs}

*`Workfront`* calculates the Planned Cost and the Actual Cost for each individual task in a project. *`Workfront`* uses these calculations for individual tasks to calculate the Planned Cost and the Actual Cost for the project.



* [Planned Cost](#planned) 
* [Budgeted Cost](#budgeted) 
* [Actual Cost](#actual) 




#### Planned Cost {#planned-cost}

The Planned Cost of a project is the cost associated with the planned work (Planned Hours) on the project.


The Planned Cost of a project is calculated by the following formula:




```
Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project
```

* * 


For example, you have the following expenses in the Expenses tab of a task: a $100 Marketing expense and a $50 Administrative expense. In the Finance tab, you select the User Hourly cost type. A user is assigned to the task, and the user's hourly rate is $15. The user is assigned to work 5 hours on this task. In the Expenses tab of the project, you have a $100 Planned Cost for an expense called Consulting. You also have a $200 Fixed Cost for the project. 


The Planned Cost of the project is calculated as follows:




```
$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense)+$15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost)= $525
```




#### Budgeted Cost {#budgeted-cost}

The Budgeted Cost of a project is the cost associated with the budgeted work (Budgeted Hours) on the project.


The Budgeted Cost of the project is the same as the Planned Cost of the project if the following two conditions are met:



*   The Planned Hours of the tasks on the project match the Budgeted Hours (in the *`Resource Planner`*)
*  The task Billing Type is Role Hourly. 


The Budgeted Cost of the project is calculated using the formula below if the following conditions are met:



*  The Planned Hours of the tasks on the project do not match the Budgeted Hours (in the *`Resource Planner`*)
*  The Billing Type of the tasks is Role Hourly.


When the above conditions are met, *`Workfront`* calculates the Budgeted Cost of the project using the following formula: 
`<pre>Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project</pre>` 

#### Actual Cost {#actual-cost}

The Actual Cost of a project is the cost associated with the actual work (Hours logged) on the project.


Actual Cost is calculated using the following formula:




```
Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project
```

.


For example, you have the following expenses in the Expenses tab of a task: a Marketing expense with an Actual Cost of $110, and an Administrative expense with an Actual Cost of $40. You select the Role Hourly cost type and assign the Consultant job role to the task. The consultant job role’s rate is $15 per hour, and there are 6 hours logged on the task for the Consultant job role. There is also a Consulting expense associated with the project (in the Expenses tab), with an Actual Cost of $100 and a user with a Cost per Hour rate of $20 in their user profile logs 10 hours on the project.


The Actual Cost of the project is calculated as follows:




```
$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project)= $540
```




>[!NOTE]
>
>When logging time on a project, the following scenarios exist when calculating Actual Labor Cost for the project:
>
>
>
>* By default, *`Workfront`* uses the Cost per Hour rate of the user to calculate Actual Labor Cost.
>* If the user logging the time is not associated with any cost, then *`Workfront`* uses the Cost per Hour rate of the user's Primary Role.
>* If your *`Workfront administrator`* enabled the `Assign Job Roles to hour entries manually` setting in the Timesheets & Hours Preferences area, and the user logging time on the project selects a different role to associate with this time, the Actual Cost of the project calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article [Configure timesheet and hour preferences](timesheet-and-hour-preferences.md).
>
>
>





### How *`Workfront`* calculates Cost Types for tasks {#how-workfront-calculates-cost-types-for-tasks}

The Planned and Actual Cost of the tasks and their Labor Costs are determined by the Cost Type of each task. 


You can configure the Cost Type for individual tasks within the project. Each cost type affects the Planned Cost and Actual Cost values.


For information about how to modify the Cost Type of a task, see [Update task Cost Type](update-task-cost-type.md). 

The following table describes the available task Cost Types in  *`Workfront`*: 

<table border="1" style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Task Cost Type</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p><span class="bold">Description</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>User Hourly</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This is the default Cost Type when you create a task.</p> <p><span class="bold">Planned Cost </span>is calculated by the following formula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Where the Planned Labor Cost is calculated by:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Note:  <p>Consider the following impacts of using the User Hourly Cost Type and calculating Planned Cost:</p> 
     <ul> 
      <li>If you assign multiple resources to a task, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> adjusts calculations for Planned Cost based on the percentage of the task assigned to each resource.</li> 
      <li>The value of the Planned Cost field can differ depending on whether you view the Planned Cost from the task itself or from the Utilization report.<br><span class="bold">When viewing Planned Cost from the task itself:</span> The Planned Cost field takes into consideration the Cost/Hr field set at the Job Role level (when the Cost/Hr field has not been set at the user level).<br><span class="bold">When viewing Planned Cost from the Utilization report on the project:</span> The Planned Cost field does not take into consideration the Cost/Hr field set at the Job Role level. Instead, if you want the Utilization report to take into consideration the Cost/Hr field set at the Job Role level, you must set the Cost Type on the task to Role Hourly. </li> 
     </ul> </p> <p><span class="bold">Actual Cost </span>is calculated by the following formula: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Where the Actual Labor Cost is calculated by:</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>For example, a user has a Cost per Hour rate of $20 in their profile. When they log 5 hours for a task, the Actual Labor Cost is $100 for that task. If the user does not have a Cost per Hour rate associated with them, the Actual Cost calculates based on the Cost per Hour rate of their Primary Job Role. If they do not have a job role or the Cost per Hour rate of their job role is not defined, then the Actual Cost of the task is zero. </p> <p>Note:  Actual Costs are calculated based on the Cost per Hour rate for the user who is logging the time, regardless of who is assigned to the task. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Role Hourly</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><span class="bold">Planned Cost </span>is calculated by the following formula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Where the Task Planned Labor Cost is calculated by:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Note: If you assign multiple resources to a task, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> adjusts calculations for Planned Hours based on the percentage of the task assigned to each resource.</p> <p><span class="bold">Actual Cost </span>is calculated by the following formula: </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Where the Task Actual Labor Cost is calculated by:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>For example, a task is assigned to a job role or a user with a job role for which the Cost per Hour rate is $20. When a user logs 5 hours for a task, the Actual Labor Cost is $100 for that task. If the user assigned to the task does not have a job role associated with them on the task, the Actual Cost calculates based on the Cost per Hour rate of their Primary Job Role. If they do not have a job role or the Cost per Hour rate of their job role is not defined, then the Actual Cost of the task is zero. </p> <p>Note:  <p> The Actual Hours of a Role Hourly task calculate based on the job roles of the users associated with the task, not on the roles associated with the user who is logging the time.</p> <p>If your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> enabled the <span class="bold">Assign Job Roles to hour entries manually</span> setting in the Timesheets &amp; Hours Preferences area, and the user logging time on the task selects a different role to associate with this time, the Actual Cost of a Role Hourly task calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article <a href="timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Fixed Hourly</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p><span class="bold">Planned Cost</span> is calculated by the following formula:<span class="bold"> </span></p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Where the Task Labor Cost is calculated by:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><span class="bold">Actual Cost</span> is calculated by the following formula: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Where the Actual Task Labor Cost is calculated by:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>This cost type does not take individual users or job roles into account.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>No Cost</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>This Cost Type does not affect Costs. If a parent task has this Cost Type, subtasks with another Cost Type calculate according to their individual Cost Types, and the Cost of the parent task is affected accordingly. </p> <p>When a user with No Access to Financial Data or a user with no financial permissions on a template creates a project from that template, this is the default Cost Type for the tasks on the project.</p> <p>For information about access to Financial Data, see the article <a href="grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> <p>For information about financial permissions on objects, see the article <a href="share-financial-permissions-object.md" class="MCXref xref">Share financial permissions on an object in Adobe Workfront</a>.</p> <p>For information about creating projects from templates, see the article <a href="create-project-from-template.md" class="MCXref xref">Create a project using a template</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## How *`Workfront`* tracks costs for issues {#how-workfront-tracks-costs-for-issues}

Issues do not have and do not affect the following types of costs on a project:



* Planned Cost
* Budgeted Cost


Issues, can, however, have an `Actual Cost` which also affects the Actual Cost of the project. 


The following table explains how Actual Cost is calculated for issues, depending on the type of assignment on the issue:

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 102px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1" style="height: 57px;"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1" colspan="4">Issue Actual Cost</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>User Assignment</p> <p> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" colspan="3"> <p><span class="bold">Actual Cost</span> is calculated by the following formula:</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>The Cost per Hour rate of the user who is logging the time is taken into account here, regardless of who is assigned to the issue. </p> <p>If the user who logs the time does not have a Cost per Hour rate in their profile, the Cost per Hour rate of their Primary Job Role calculates the Actual Cost of the issue. If the user who is logging the time has no role in their profile or no rate associated with it, the Actual Hours are calculated using the Cost per Hour rate of the Primary Job Role of the Primary Assignee on the issue. If that role has no rate defined, the Actual Cost of the issue is zero. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Role Assignment</p> <p> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" colspan="3"> <p><span class="bold">Actual Cost</span> is calculated by the following formula:</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>The Cost per Hour rate of the user logging the time on the issue is taken into account here, regardless of what role is assigned to the issue. </p> <p>If the user logging the time does not have a Cost per Hour rate associated with them, the Cost per Hour rate of their Primary Role calculates the Actual Cost of the issue.<br>If the user who is logging the time has no role in their profile or no rate associated with it, the Actual Cost of the issue is zero. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>No Assignment</p> <p> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" colspan="3"> <p><span class="bold">Actual Cost</span> is calculated by the following formula:</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>If the user who logs the time does not have a Cost per Hour rate associated with their profile, the Cost per Hour rate of their Primary Job Role calculates the Actual Cost of the issue. </p> <p>If the user who is logging the time has no job role associated with their profile or their Primary Job Role does not have a Cost per Hour rate defined, the Actual Cost of the issue is zero. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" colspan="4"> 
    <div> <MadCap:conditionalText data-mc-conditions="">
      If your 
      <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> enabled the 
      <span class="bold">Assign Job Roles to hour entries manually</span> setting in the Timesheets &amp; Hours Preferences area, and the user logging time on the issue selects a different role to associate with this time, the Actual Cost of the issue calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article 
      <a href="timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>.
     </MadCap:conditionalText> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

