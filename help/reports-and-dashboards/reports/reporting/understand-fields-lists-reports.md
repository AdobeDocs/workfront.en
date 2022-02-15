---
filename: understand-fields-lists-reports
content-type: reference
product-area: reporting
navigation-topic: reporting-navigation-topic
---




# Understand fields in lists and reports {#understand-fields-in-lists-and-reports}



>[!NOTE]
>
>The information in this article has been added to the `Workfront` glossary. This article will be deleted in the near future. For the `Workfront` glossary, see [Glossary of Workfront terminology](workfront-terminology-glossary.md).




>[!IMPORTANT] {type="important"}
>
>This article should be used as a reference to understand the fields that are visible through the report builder in `Workfront`. The fields available in the report builder are listed in the following table in alphabetical order. We are currently&nbsp;updating this information and as a result this table might not be complete. We will remove this disclaimer when we consider this information exhaustive.&nbsp;


`Workfront` fields are available to be configured in the following reporting elements:



* Views
* Filters
* Groupings
* Prompts


For more information about reporting elements, see the article [Reporting elements overview](_reporting-elements-overview.md).


For more information about building reports, see<![CDATA[  ]]> [Create and manage reports](_create-manage-reports.md).


When creating a report, you can select what objects or fields associated with those objects you want to show in your report. Those will become your report columns, groupings, filters, or prompts. You can build standalone views, filters, and groupings for lists of objects, as well, in the same manner you would build them inside the report builder.&nbsp;


![](assets/4.png)




The following table is a list of commonly used objects and fields that you can display in reports and lists. Not all fields are available on all objects:&nbsp;&nbsp;

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 219px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 797px;"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Object Name</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Actual Hours</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In a project, task, or issue report, Actual Hours are the sum of all hours logged on the project, task, or issue.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Allocation Date</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>You can find this field in the following types of reports:</p> 
    <ul> 
     <li value="1">Resource Estimates</li> 
     <li value="2">Project (Financial Data)</li> 
     <li value="3">Budgeted Hour</li> 
    </ul> <p>For a Resource Estimates or Project (Financial Data) report: </p> 
    <ul> 
     <li value="1">Build these reports when trying to understand how resources are budgeted for work, or the amount of Planned Hours that is assigned to your resources.</li> 
     <li value="2"> <p>The Allocation Date is the first day (Sunday) of a week in which the allocation of a Job Role to a task starts. A resource (Job Role) can have as many Allocation Dates as it has weeks during the Duration of the tasks that it is assigned to. If tasks span over multiple months, then the first day of a month can also become an Allocation Date, if it falls within the Duration of the task.&nbsp;</p> <p>For example, you can have a Job Role assigned to a task that spans over 3 weeks and has 90 Planned Hours. These hours are spread evenly during the duration of the task, which makes every day assign 6 Planned Hours to your job role:</p> <p><em> Daily Planned Hours = Total Planned Hours/ Number of Work Days during the Duration of the task </em> </p> <p>As a result, there are three Allocation Dates, one for every Sunday of every week during the Duration of the task, each with a certain number of Planned Hours associated with them.<br>If the task starts in the middle of the last week of a month and ends two weeks after the beginning of a new month, the task will have four Allocation Dates: one for every Sunday of every week during the Duration of the task, and one for the first day of the new month.</p> <p>To make the most use of this information, we recommend that you build a Resource Estimates or a Project (Financial Data) report and add a matrix grouping for Allocation Date, and group the results weekly, monthly, quarterly, or yearly for the most accurate data.<br>For information about building a matrix grouping, see the article <a href="create-matrix-report.md" class="MCXref xref">Create a matrix report</a>.</p> </li> 
    </ul> 
    <div> 
     <p>For a Budgeted Hour report:</p> 
     <ul> 
      <li value="1">Build this report when trying to understand the amount of Budgeted Hours that is allocated to your resources or to your projects in the Resource Planner.</li> 
      <li value="2"> <p>The Allocation Date is the first day (a Sunday) of the week for which you budgeted the hours in the Resource Planner. </p> 
       <div class="tips" data-mc-autonum="<b>Tips: </b>">
        <span class="autonumber"><span><b>Tips: </b></span></span> 
        <p>If a week spans for two months, it will generate two rows in the report: one corresponding to the first day of the week (Sunday of the first week which is during the first month), and the second row displays the first day of the second month. </p> 
        <p>For example, if you budget 8 hours for a user for the week of June 30 (Sunday) - July 6 (Saturday), the two rows show an Allocation Date of June 30, and July 1. </p> 
       </div> <p>For information about budgeting resources in the Resource Planner, see the article <a href="budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and&nbsp;Role views</a>.</p> </li> 
     </ul> 
    </div> <p> &nbsp; </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Approver Decision</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In the Proof Approval report, displays&nbsp;<span class="WFVariablesproof-sing-n">proof</span> approval decisions for <span class="WFVariablesproof-plur-n">proofs</span> that are no longer active.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Assigned To</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>In a Task or Issue report, this field displays the Owner of the task or the issue, or the Primary Assignee. You can filter or group by this field, as well.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Assignments</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In a Task or Issue report, this field displays a list of all entities (users, job roles, teams) that are assigned to the task or issue. You can filter by this field only in a text mode filter. You cannot group the&nbsp;report by this field.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Assignment Users</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">In a Task or Issue report, this field displays information about the users assigned to the tasks or issues.&nbsp;This field displays Primary&nbsp;Owners, as well as other users assigned to tasks or issues. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Assignment Roles</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">In a Task or Issue report, this field displays information about the job roles assigned to the tasks or issues.&nbsp;This field displays Primary&nbsp;Owners, as well as other job roles assigned to tasks or issues. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Budget Status</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Shows&nbsp;whether the project is currently added to the capacity planner and if the budget calculation has been completed&nbsp;for it.</p> <p>If the project is&nbsp;not added to the capacity planner, its value is "Not Included."&nbsp;</p> <p>If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is "Included but not Calculated."&nbsp;</p> <p> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is "Included and Calculated." </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Budgeted Completion Date</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This is a deprecated field that shows the date when the budgeting of resources ends, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner. The field is available in project and task reports.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Budgeted Cost or Project Budgeted Cost</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The Budgeted Cost for the project is calculated using the following formula:<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost + Fixed Cost of the project</code> </p> <p>The Budgeted Labor Cost in the calculation above refers to both labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner), and hours budgeted in the Resource Budgeting area of the Business Case (or in the Resource Planner). </p> <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates areas are currently deprecated and will be removed from&nbsp;<span class="WFVariablesProdNameWF">Workfront</span>.</p> <p>You can locate the Budgeted Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;<span class="WFVariablesProdNameWF">Workfront</span>: </p> 
    <ul> 
     <li value="1">Business Case Summary</li> 
     <li value="2">Portfolio Optimizer (in the Cost field)</li> 
     <li value="3"> <p>In the following reports, in the Project Budgeted Cost field: </p> 
      <ul> 
       <li value="1">Resource Estimates report</li> 
       <li value="2">Budgeted Hour report </li> 
       <li value="3">Project report</li> 
       <li value="4">Project (Financial&nbsp;Data)</li> 
       <li value="5">Task&nbsp;report</li> 
       <li value="6">Issue report</li> 
      </ul> </li> 
    </ul> <p>You can locate the Budgeted Cost field based on the hours budgeted in the Capacity Planner in the following areas and reports in&nbsp;<span class="WFVariablesProdNameWF">Workfront</span>: </p> 
    <ul> 
     <li value="1">Resource Estimates report</li> 
     <li value="2">Budgeted Hour report </li> 
     <li value="3">Project report</li> 
     <li value="4">Project (Financial Data)</li> 
     <li value="5">Task&nbsp;report</li> 
     <li value="6">Issue report</li> 
    </ul> <p>For more information about calculating Budgeted Cost, see the article <a href="budgeted-cost.md" class="MCXref xref">Calculate Budgeted Cost</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Budgeted Hours or Bud. Hours or Pln. Bud. Hours</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>These are the hours that you, as the Resource Manager, budget for your resources for the work they need to complete on projects. This field refers to both hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner), and hours budgeted in the Resource Budgeting area of the Business Case (or in the Resource Planner). </p> <p>You can locate the Budgeted Hours from the Resource Planner in the following areas and reports in&nbsp;<span class="WFVariablesProdNameWF">Workfront</span>: </p> 
    <ul> 
     <li value="1">Resource Planner Hours view (in the BDG column)</li> 
     <li value="2">Utilization report Hours view</li> 
     <li value="3">Resource Budgeting area of the Business Case (in the Hours field)</li> 
     <li value="4">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li> 
    </ul> <p>You can locate the Budgeted Hours from the&nbsp;Capacity Planner in the following areas and reports in&nbsp;<span class="WFVariablesProdNameWF">Workfront</span>: </p> 
    <ul> 
     <li value="1">Capacity Planner</li> 
     <li value="2">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li> 
     <li value="3">Resource Estimates report (in the Bud. Hours field)</li> 
     <li value="4">Budgeted Hour report (in the Budgeted Hours field)</li> 
     <li value="5">Project report</li> 
     <li value="6">Project (Financial&nbsp;Data)</li> 
     <li value="7">Task&nbsp;report</li> 
     <li value="8">Issue report</li> 
    </ul> <p>The Capacity Planner and Legacy&nbsp;Resource Estimates areas are currently deprecated and will be removed from <span class="WFVariablesProdNameWF">Workfront</span>. For information about budgeting Users in the Resource Planner, see the article <a href="budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and&nbsp;Role views</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Budgeted Labor Cost or Resource Planner Budgeted Cost </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This is the cost associated with the hours that you, as the Resource Manager, budget for your resources for the work they need to complete on projects. </p> <p>The Budgeted Labor Cost in a project report is calculated using the following formula:</p> <p><code style="font-style: normal;">Budgeted Labor Cost = SUM(Job Role Cost per Hour * Budgeted Hours per Job Role)</code> </p> <p>This field refers to both labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner), and hours budgeted in the Resource Budgeting area of the Business Case (or in the Resource Planner). </p> <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates areas are currently deprecated and will be removed from&nbsp;<span class="WFVariablesProdNameWF">Workfront</span>.</p> <p>You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;<span class="WFVariablesProdNameWF">Workfront</span>: </p> 
    <ul> 
     <li value="1">Resource Planner Cost view (in the BDG column)</li> 
     <li value="2">Utilization report Cost view (in the Budgeted Cost column)</li> 
     <li value="3">Resource Budgeting area of the Business Case </li> 
     <li value="4"> <p>In the following reports, in the Resource Planner Budgeted Labor Cost field: </p> 
      <ul> 
       <li value="1">Resource Estimates report</li> 
       <li value="2">Budgeted Hour report </li> 
       <li value="3">Project report</li> 
       <li value="4">Project (Financial&nbsp;Data)</li> 
       <li value="5">Task&nbsp;report</li> 
       <li value="6">Issue report</li> 
      </ul> </li> 
    </ul> <p>You can locate the Budgeted Labor Cost based on the hours budgeted in the Capacity Planner in the following areas and reports in&nbsp;<span class="WFVariablesProdNameWF">Workfront</span>: </p> 
    <ul> 
     <li value="1">Capacity Planner</li> 
     <li value="2">Legacy&nbsp;Resource Estimates area of the Business Case (in the Legacy Budgeted Labor Cost field)</li> 
     <li value="3">Resource Estimates report</li> 
     <li value="4">Budgeted Hour report </li> 
     <li value="5">Project report</li> 
     <li value="6">Project (Financial Data)</li> 
     <li value="7">Task&nbsp;report</li> 
     <li value="8">Issue report</li> 
    </ul> <p>For more information about calculating the Budgeted Labor Cost, see the article <a href="budgeted-labor-cost.md" class="MCXref xref">Calculate Budgeted Labor Cost </a>&nbsp;&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Budgeted Start Date</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This is a deprecated field that shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.&nbsp;The field is available in project and task reports.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Completion Day</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">In a template or template task report, this is the day in the timeline of the template when the template task or the template completes. By default, the template has a Completion Day of 0 before you start adding template tasks to it. After adding the template tasks, the tasks and the template show a Completion Day of 1 because <span class="WFVariablesProdNameWF">Workfront</span> assumes a Duration of 1 Day for each new template task. When you start adding Task&nbsp;Constraints, Duration, or dependencies to your template tasks, the Completion Day might change to reflect these changes.<p>For more information about the Completion&nbsp;Day in a template, see <a href="edit-templates.md" class="MCXref xref">Edit project templates</a>.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Can Start</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Shows if a task is ready to start to be worked on. &nbsp;The system checks for the following things before it marks a task as "True" for the "Can Start" field:<br></p> <p>- If the task has a parent, it checks to see if the value of "Can Start" for the parent it set to "True". If the value for the parent is "False", then all the subtasks have the value of "Can Start" set to "False", as well.&nbsp;</p> <p>- It also checks to see if the predecessors of the task are complete. If they are complete, the "Can Start" value for the task is set to "True". If any of the predecessors is not complete, or has a status of "Complete - Pending Approval", then the "Can Start" value for the task is set to "False".&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Category</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>A category is a custom form. You can build reports for this object and you can show it in other object reports, as well. <br>Not all objects can have a custom form, or category. <br>The following objects can have a custom form:&nbsp;<br>- Project<br>- Task<br>- Issue<br>- Portfolio<br>- Document<br>- Expense<br>- Program<br>- User<br>- Company<br>- Iteration</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Category&nbsp;Name</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>When added as a column to the view of any of the following objects it displays a list of all custom forms associated with these objects:</p> <p>- Project<br>- Task<br>- Issue<br>- Portfolio<br>- Document<br>- Expense<br>- Program<br>- User<br>- Company<br>- Iteration</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Condition</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>It is a visual representation of the progress of a task, issue or project.&nbsp;</p> <p>For projects, the condition can be manually set by the project owner or it can be automatically set by <span class="WFVariablesProdNameWF">Workfront</span>, based on the progress status of the project. For more information about project condition, see the article <a href="project-condition-and-condition-type.md" class="MCXref xref">Overview of Project Condition and Condition Type</a>.</p> <p>The possible values for the project condition are:<br>- On Target<br>- At Risk<br>- In Trouble</p> <p>For tasks, the condition is set manually by the task&nbsp;owner.<br>The possible values for the task condition are:<br>- Going Smoothly<br>- Some Concerns<br>- Major Roadblocks</p> <p>For more information about task condition, see the article <a href="update-condition-for-tasks-and-issues.md" class="MCXref xref">Update Condition for tasks and issues</a>.</p> <p>For issues, the condition is set manually by the issue&nbsp;owner.<br>The possible values for the task condition are:<br>- Going Smoothly<br>- Some Concerns<br>- Major Roadblocks</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Condition Update</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Shows the current condition of tasks, projects or issues.</p> <p>This option&nbsp;shows the most recent&nbsp;updates&nbsp;that the owners of tasks, projects or issues&nbsp;have provided in the 'Update Status' field, along with the new condition.&nbsp;</p> <p>Comments made on condition updates are not displayed in the 'Condition Update' column; only the main update is displayed.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Constraint Date</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>If you are using a Task Constraint that is tied to a specific date, such as Must Start On, then that specific date becomes the Constraint Date of the task.<br><br>The following task constraints update the Constraint Date field:</p> 
    <ul> 
     <li value="1">Must Start On</li> 
     <li value="2">Must Finish On</li> 
     <li value="3">Start No Later Than</li> 
     <li value="4">Start No Earlier Than</li> 
    </ul> <p>Note:  Constraint Date is only viewable in a report or customized view.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Constraint Day</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>If you are using a Task Constraint in a template task that is tied to a specific day, such as Must Start On, then that specific day becomes the Constraint Day of the template task.&nbsp;</p> <p>The following task constraints update the Constraint Day field:</p> 
    <ul> 
     <li value="1">Must Start On</li> 
     <li value="2">Must Finish On</li> 
     <li value="3">Start No Later Than</li> 
     <li value="4">Start No Earlier Than</li> 
    </ul> <p>Note:  Constraint Day is only viewable in a report or customized view.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Dashboards</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> You can add this field in a report or a list of the report object, to display the dashboards on which the report is listed in a list. </p> <p> You can use this field to filter for reports that are listed on a specific dashboard, as well. </p> <p> For more information about including dashboard information on report object reports, see the “Understanding What Reports Are Listed on Dashboards” section in the article <a href="access-organize-reports.md" class="MCXref xref">Access and organize reports</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Days Late</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Shows a date difference between Planned Start and Today if the Actual Completion Date is missing.</p> <p>Also&nbsp;shows a date difference between Actual Completion and Planned Completion, when an Actual Completion Date is present.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Duration</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This field appears on projects, tasks and issues. It is the number of days between the Planned Start and the Planned Completion Date of the object.&nbsp;</p> <p>For tasks, the Duration is an editable field if the Duration Type of the task is not Simple. If the Duration Type of the task is Simple, or if the Task Constraint is Fixed Dates, the Duration is a calculation performed by <span class="WFVariablesProdNameWF">Workfront</span>.&nbsp;</p> <p>For issues, the Duration is always an editable field and it should represent an estimate of a number of days that would require the issue to be resolved.&nbsp;</p> <p>For projects, the Duration is a calculation performed by <span class="WFVariablesProdNameWF">Workfront</span> and it represents the difference in days between the Planned Start of the earliest task and the Planned Completion of the latest task on the project.&nbsp;</p> <p>For more information about the difference between Duration and Planned Duration for tasks, see the article <a href="planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Difference between Planned Duration and Duration for tasks</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>End Date</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> In a Rate report, this is the date when a new billing rate for a job role at the project level ends. The hours associated with the project that are before this date are multiplied by this billing rate to calculate the revenue on the project. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Flags</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> This is the same field as Status Icons, but it is only available for the following views: </p> 
    <ul> 
     <li value="1"> Templates </li> 
     <li value="2"> Expenses </li> 
    </ul> <p> For more information, see the article <a href="built-in-status-icons-views.md" class="MCXref xref">Built-in Status Icons in Views</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Group Administrator</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> In a Group report, this field displays the names of the users designated as Group Administrators in the Group. For more information, see <a href="group-administrators.md" class="MCXref xref">Group Administrators</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Group with Administration Access</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> In a Layout Template, Timesheet Profile, or Schedule report, this field displays the Groups whose Group Administrators have access to modify the template. You can also filter this report by this field. For more information about Group with Administration Access, see the article <a href="create-and-manage-layout-templates.md" class="MCXref xref">Create and manage Layout Templates</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Handoff Date</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The date when a task becomes available for work. The Handoff Date is a calculation and cannot be set manually. <br>For more information about the Handoff Date, see the article <a href="handoff-task-date.md" class="MCXref xref">Overview of the Handoff Date of a task </a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>(Hour) Owner</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>In an Hour report, the&nbsp;Hour Owner is the user to whom the hours are attributed. This is different than the user who is actually logging the time. These two entities can sometimes be two different users. <br>For more information about logging time for another user, see the article <a href="log-time.md" class="MCXref xref">Log Time</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Kanban Flag</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In a Task Report or Issue Report,&nbsp;the Kanban Flag field displays the flag status that is set on the story on the Kanban board. Possible values are On Track, Ready to Pull, and Is Blocked.</p> <p>For more information about setting flag status on stories on the Kanban story board, see&nbsp; the article <a href="use-flags-on-stories.md" class="MCXref xref">Use flags on stories on the Kanban board</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Last 10 Viewers</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>In a report list, it displays the names of up to 10 users who have viewed the report most recently.<br>For more information about usage information in report lists, see the article <a href="view-report-usage.md" class="MCXref xref">View report usage</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Last Condition Note</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Displays the update last entered on an object by the&nbsp;owner of the object.<br>This field is helpful to display the owner's most recent activity or interaction on an object.</p> <p>The Last Condition Note column is&nbsp;empty if the note text of the last note of an object has been deleted. When a new note is entered on the object, it becomes the last note and it displays again in the column.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Last Note</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Displays the update last entered on an object by any user.<br>This field is helpful to display the most recent activity or interaction on an object.</p> <p>The Last Note column is empty if the text of the last note of an object has been deleted. When a new note is entered on the object, it becomes the last note and it displays again in the column.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Last Viewed By</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In a report list, it displays information about the user who viewed the report last.<br>For more information about usage information in report lists, see the article <a href="view-report-usage.md" class="MCXref xref">View report usage</a>.<br></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Last Viewed Date</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>In a report list, it displays the date on which the report was displayed last.<br>For more information about usage information in report lists, see the article <a href="view-report-usage.md" class="MCXref xref">View report usage</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Legacy Resource Pool</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. For more information about Legacy Resource Planning, see the article <a href="_resource-planning-overview.md">Resource Planning</a>. This is a deprecated field. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>License Type Limit: Planner Limit</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>In a Group view or report, this shows the maximum number of Plan licenses that can be assigned to users who have the respective group designated as their Home Group.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>License Type Limit: Worker Limit</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In a Group view or report, this shows the maximum number of Work licenses that can be assigned to users who have the respective group designated as their Home Group.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Note Text</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Displays the text of an update entered by an user on any object.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Parameter</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>A parameter is a custom field. You can build a report for all parameters, or custom fields in your system.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Percent Complete</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>A project, task, or issue field that shows what percentage of the work associated with the task, project, or issue is completed.</p> <p>You can update this field manually for issues and working tasks. </p> <p>For projects and parent tasks, this field is a roll-up from all the working tasks and you cannot update it manually. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planned Budgeted Hours</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In a Budgeted Hour report, this displays the amount of hours budgeted for Projects or Job Roles in the Resource Planner. </p> <p>For information about budgeting Projects or Roles in the Resource Planner, see the article <a href="budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and&nbsp;Role views</a>. For information about the Budgeted Hours report, see the article <a href="report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Planned Completion Date</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>You can manually set the Planned Completion Date to a date of your choosing. If you do not set the Planned Completion Date, <span class="WFVariablesProdNameWF">Workfront</span>&nbsp;sets it automatically. When set automatically, the Planned Completion Date is:&nbsp;Planned Start Date + Duration</p> <p>For more information, see the article <a href="project-planned-completion-date.md" class="MCXref xref">Overview of the project Planned Completion Date </a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Planned Cost</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>A total of the Planned Labor Cost&nbsp;and the Planned Expense Cost of the project. This does not include the Planned Risk Cost on the project.&nbsp;&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Planned Duration</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>A task's Planned Duration is usually the same as the task's Duration. It represents the difference in days between the Planned Start and the Planned Completion Dates of the task.&nbsp;</p> <p>When the task has a Duration Type of Effort Driven, the Planned Duration can differ from the Duration of the task, based on how many resources you assign to the task.&nbsp;</p> <p>For example, if a task with a Duration Type of Effort Driven has a Duration of 3 days and you assign one resource with a full time schedule to the task, the Planned Duration is 3 days, as well. If you assign three resources with a full time schedule to the same task, the Duration stays 3 days, but the Planned Duration becomes 1 day. The Planned Duration also changes the Planned Start and Planned Completion dates of the task, to reflect the new Planned Duration. As a result, the timeline of the project is affected as well.&nbsp;</p> <p>For more information about the difference between Duration and Planned Duration for tasks, see the article <a href="planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Difference between Planned Duration and Duration for tasks</a>.</p> <p>Projects and issues don't have a Planned Duration.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Planned Duration Minutes</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The Planned Duration Minutes of a project or an issue is the Duration of the project or issue in minutes.&nbsp;</p> <p>Tasks don't have a Planned Duration Minutes field.&nbsp;</p> <p>Template Tasks have a Planned Duration Minutes field which displays the Planned Duration of the task in minutes.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Planned Expense Cost</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Total&nbsp;of the Planned Amounts&nbsp;of all the expenses on the project.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Planned Hours</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This field appears on projects, tasks, and issues.&nbsp;</p> <p>It shows the amount of hours that the Project Owner estimates that each task or issue should take to complete. </p> <p>For tasks, you can manually update this field when the Duration Type of the task is Calculated Assignment. This field is calculated by <span class="WFVariablesProdNameWF">Workfront</span> when the Duration Type of the task is Calculated Work, Effort Driven, or Simple.<br>For information about Task Duration, see the article <a href="task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.<br>Planned Hours are distributed equally to all the days within the duration of each task. They are stored in minutes in the <span class="WFVariablesProdNameWF">Workfront</span> database.<br></p> <p><span class="WFVariablesProdNameWF">Workfront</span> calculates the Planned Hours of a Project by adding all Planned Hours from all the tasks on the project. </p> <p>You can manually update this field for Issues.&nbsp;Issue Planned Hours are not added to the Project Planned Hours.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><a name="Planned-Labor-Cost"></a>Planned Labor Cost</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>For a task, the hourly rate of the user or role, multiplied by the number of hours assigned to the user or role.&nbsp;</p> <p>For a project, it is a total of all Planned Labor Costs of all the tasks.&nbsp;&nbsp;</p> <p>Whether the rate of the user or role is used depends on the Cost Type that is selected for the given task, as described in the section <a href="track-costs.md#modifying-cost-types-for-individual-tasks">Modifying Cost Types for Individual Tasks</a> in&nbsp; the article <a href="track-costs.md" class="MCXref xref">Track costs </a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Planned Risk Cost</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The total of the Potential Cost of all the risks on the project. This amount is not included in the Planned Cost of the project.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Project Budgeted Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">See Budgeted&nbsp;Cost</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Proof Deadline</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In reports that contain the Document Version object (such as a Document Version report and Proof Approval report), displays the day of the week, date, time of day, and year of the <span class="WFVariablesproof-sing-n">proof</span> deadline.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Proof Decision</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>In reports that contain the Document Version object (such as a Document Version report&nbsp; and Proof Approval report), displays the decision status of the <span class="WFVariablesproof-sing-n">proof</span> (pending, changes required, or approved)</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Proof Name</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In reports that contain the Document Version object (such as a Document Version report and Proof Approval report), displays the <span class="WFVariablesproof-sing-n">proof</span> name.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Proof Pages</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>In reports that contain the Document Version object (such as a Document Version report and Proof Approval report), displays the number of pages included in the <span class="WFVariablesproof-sing-n">proof</span>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Proof Progress</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In reports that contain the Document Version object (such as a Document Version report and Proof Approval report), displays the progress status of the <span class="WFVariablesproof-sing-n">proof</span> (Sent, Opened, Commented, Decision Made).</p> <p>For more information, see the section <a href="view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Understand proof progress</a> in the article <a href="view-progress-status-proof.md" class="MCXref xref">View progress and status of a proof</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Rank</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>In an Access Level report, you can manually indicate a Rank of the Access Level. This helps you, as the <span class="WFVariablesAdminWF">Workfront administrator</span>, to visually identify the level of complexity associated with each Access Level. For example, you can give lower numbers for more complex (Plan-level) Access Levels, and higher numbers for less complex (Requestor-level) Access Levels. You cannot rank the standard Access Levels.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Ready</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This is a field on a task report which indicates whether&nbsp;an Agile task has been marked as "Ready" on the backlog. This flag only applies to Agile tasks, which are tasks assigned to an Agile team.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Rejection&nbsp;Issue</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">In a project or a task report, this is the issue that is created when the approval for the project or the task is rejected. For information about rejection issues, see the article <a href="create-approval-processes.md" class="MCXref xref">Create and edit approval processes</a>. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Resolve Issue/ Project/ Task</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In an issue report, use this field in views or filters to refer to the issue, the project, or the task that resolves the issue. </p> <p>For information about displaying resolving objects in reports, see the section <a href="resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a> in the article <a href="resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Resource Managers</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Resource Managers can perform resource scheduling actions on a project.&nbsp;</p> <p>When you use this in a report, a list of resource managers is displayed, with each resource manager on the project separated by a comma (there can be up to 10 resource managers on a given project).</p> <p>For more information, see the article <a href="designate-resource-managers-for-projects-and-templates.md" class="MCXref xref">Designate Resource Managers for a project or template </a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Resource Manager IDs</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Use this option &nbsp;when creating a filter to find a specific resource manager.</p> <p>Begin typing the name of the resource manager that you want to use in the filter, then click the name when it appears in the drop-down list.</p> <p>Resource Managers can perform resource scheduling actions on a project.</p> <p>For more information, see the article <a href="designate-resource-managers-for-projects-and-templates.md" class="MCXref xref">Designate Resource Managers for a project or template </a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Resource Planner Budgeted Labor&nbsp;Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">See Budgeted Labor&nbsp;Cost. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Resource Pool</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>A collection&nbsp;of job roles associated with a project or a user. The functionality of the Resource Pools is displayed in the tools available in the Resource Planning tab of the People area in the Production environment.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Resource Pools</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>In project reports, Resource Pools show all the pools associated with a project. &nbsp;Resource Pools are collections of users that can be associated with a project.&nbsp;This object cannot be used in a grouping. <br>For more information about the functionality of Resource Pools see the&nbsp;section <a href="_resource-planning-overview.md">Resource Planning</a>.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Resource Scope</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">A task-level field that is applicable only when using a Task Constraint of Fixed Dates. For more information about the Fixed Dates Task Constraint, see the article <a href="fixed-dates.md">Fixed Dates</a>. The value of the Resource Scope on a task is intended to prevent other tasks from being assigned to the same user during the time frame of the task. For more information about Resource Scope, see the article <a href="resource-scope.md">Understanding Resource Scope</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Scheduled Report</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>When you build a report of reports, you can display&nbsp;information about the schedules of the report, if the report is scheduled for delivery using the Scheduled Report field. This field shows multiple values, one for each schedule of each report, in a bulleted list. For more information about scheduling reports, see the article <a href="set-up-report-deliveries.md" class="MCXref xref">Set up report deliveries</a>.</p> <p>Because this field shows multiple values, it cannot be used in a grouping. You can access it only in a filter or a view.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Source</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Indicates the parent object of another object. For example, a document attached to a task has the name of the task in the Source field of a Document report or view; an issue logged under a project has the name of the project in the Source field of an Issue report or view.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Start Date</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> In a Rate report, this is the date when a new billing rate for a job role at the project level starts. The hours associated with the project that are after this date are multiplied by this billing rate to calculate the revenue on the project. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Start Day</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In a template or template task report, this is the day in the timeline of the template when the template task or the template starts. By default, the template and any template tasks indicate a Start Day of 0. When you start adding Task&nbsp;Constraints, Duration, or dependencies to your template tasks, the Start Day might change to reflect these changes. </p> <p>For more information about the Start Day in a template, see <a href="edit-templates.md" class="MCXref xref">Edit project templates</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Status</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Shows the most recent status of tasks. This is&nbsp;the 'New,' 'In Process,' and 'Complete' statuses that users can select when updating a task.</p> <p>For more information about task status, see the article <a href="update-task-status.md" class="MCXref xref">Update task status</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Status Icons</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>You can add the built-in Status Icons field as a column in your views to enhance visibility into key points about your objects, like:</p> 
    <ul> 
     <li value="1">An object has documents attached</li> 
     <li value="2">An object is associated with an approval process</li> 
     <li value="3">An object has additional notes associated with it</li> 
     <li value="4">An expense is billable or reimbursable&nbsp;</li> 
     <li value="5">A task is on a critical path</li> 
     <li value="6">A user belongs to a company, a team, or is located in a different time zone&nbsp;</li> 
    </ul> <p>You can add the Status Icons field in the views of the following objects:&nbsp;</p> 
    <ul> 
     <li value="1">Tasks</li> 
     <li value="2">Issues</li> 
     <li value="3">Projects</li> 
     <li value="4">Template Tasks</li> 
     <li value="5">Templates</li> 
     <li value="6">Expenses</li> 
     <li value="7">Documents</li> 
     <li value="8">Users</li> 
    </ul> <p>For more information, see the article <a href="built-in-status-icons-views.md" class="MCXref xref">Built-in Status Icons in Views</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Status Update</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Shows the most recent status update&nbsp;on&nbsp;tasks.&nbsp;</p> <p>This option&nbsp;shows the most recent status updates&nbsp;that users have provided in the 'Update Status' field.&nbsp;&nbsp;</p> <p>(To show the 'New,' 'In Process,' and 'Complete' statuses, use the Status column.)</p> <p>Comments made on&nbsp;status&nbsp;updates are not displayed in the 'Status Update' column; only the main update is displayed.</p> <p>For more information on statuses, see the article <a href="update-task-status.md" class="MCXref xref">Update task status</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Subscribers</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Lists the subscribers to projects, tasks, or issues.</p> <p>When you use this field in a report, a list of subscribers displays, with each subscriber separated by a comma.</p> <p>For more information, see the article <a href="subscribe-to-items-in-workfront.md" class="MCXref xref">Subscribe to items in Workfront</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span>Time Off</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">You can build a Time Off report to view when users have indicated time off in their profile. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Total Hours</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In a project report, Total Hours display&nbsp;the rounded sum of all hours on the project, the last time the project finances were calculated.</p> <p>Actual Hours reflect the exact hours logged on the project. Typically, the Actual Hours should match the Total Hours.</p> <p>If the Total Hours appears significantly different than the Actual Hours field, you must Recalculate Finances on the project.<br>For more information about recalculating project finances, see the article <a href="recalculate-project-finances.md" class="MCXref xref">Recalculate project finances</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Thumbnail / Large Thumbnail&nbsp;</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> In a Document list or report, it displays a preview of the document in a thumbnail. </p> <p> Do one of the following: </p> 
    <ul> 
     <li value="1"> Select <b>Thumbnail</b> &nbsp;to view a 33-66 pixel-wide thumbnail in the report. </li> 
     <li value="2">Select <b>Large Thumbnail </b>to view a 400 pixel-wide thumbnail in the report.</li> 
    </ul> <p>The size of the thumbnail adjusts when you modify the width of the column in a list or report.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>View Icons</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> This is the same field as Status Icons, but it is only available for the following views: </p> 
    <ul> 
     <li value="1"> Documents </li> 
    </ul> <p> For more information, see the article <a href="built-in-status-icons-views.md" class="MCXref xref">Built-in Status Icons in Views</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Views Last Month/ Quarter/ Year</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>In a report list, it displays the number of times the report has been viewed during the last month, quarter, or year.<br>For more information about usage information in report lists, see the article <a href="view-report-usage.md" class="MCXref xref">View report usage</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Views This Month/ Quarter/ Year</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>In a report list, it displays the number of times the report has been viewed during this month, quarter, or year.<br>For more information about usage information in report lists, see the article <a href="view-report-usage.md" class="MCXref xref">View report usage</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

