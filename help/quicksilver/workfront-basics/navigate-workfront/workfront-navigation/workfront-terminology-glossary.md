---
content-type: reference
navigation-topic: workfront-navigation
title: Glossary of Adobe Workfront terminology
description: The Adobe Workfront glossary lists commonly used terms in Adobe Workfront.
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
---
# Glossary of Adobe Workfront terminology

>[!IMPORTANT]
>
>This article should be used as a reference to understand the terms that you may encounter in the Adobe Workfront application, in the Workfront documentation, or when generally speaking about planning and managing work. We are currently updating this information and as a result this table might not be complete. We will remove this disclaimer when we consider this information exhaustive.

The following table is a list of commonly used terms in Adobe Workfront:

## A - C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Object Name</strong></th> 
   <th><strong>Description</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Access Level</td> 
   <td>A user profile that determines how a user can interact with different objects and tools within Workfront.</td> 
  </tr> 
  <tr> 
   <td>Active Task</td> 
   <td>An incomplete task in a current project that is not prevented from being worked on by a predecessor task and does not have a task constraint with a future planned start date. In other words, it can be worked on today.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Activity</td> 
   <td>In Workfront Goals, an activity is a progress indicator for a goal. It can be a progress bar that you update manually, or a project that is associated with the goal. You cannot display activities in a report and you cannot access them through the Workfront API. For information about activities, see <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Get started with results and activities in Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr> 
   <td>Actual Cost</td> 
   <td> <p>For tasks and issues, this is the cost associated with the actual hours logged in relation to the Cost per hour rate of the resource assigned to the task or issue. For projects, this is a total of all Actual Costs from tasks and issues on the project. For information, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Actual Expense Cost</td> 
   <td> <p>The sum of the Actual Amounts for all expenses logged for a project or a task.</p> <b>EXAMPLE </b>
   <p>If you create an expense for Task 1 and enter $600.00 in the Actual Amount field, the Actual Expense Cost for this task is $600.00. </p> 
   <p>For a project, Workfront uses the following formula to calculate Actual Expense Cost:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs)</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Actual Hours</td> 
   <td> <p>In a project, task, or issue report, Actual Hours are the sum of all hours logged on the project, task, or issue.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> If from the Updates tab for Task 1, you click 'Log Time' and enter 25 hours, the Actual Hours of Task 1 = 25 hours. </p> <p>Workfront calculates Actual Hours for parent tasks or projects using the following formulas:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children Actual Hours + Actual Hours on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = Actual Hours logged on the project + Actual Hours logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Actual Labor Cost</td> 
   <td> <p>The Actual Cost associated with the labor invested in a task or a project. </p> <p>For a task, Workfront calculates the Actual Labor Cost using the following formula:</p> <p><code>Task Actual Labor Cost = Number of Actual Hours on the task * User or Job Role Hourly Cost Rate</code> </p> <p>If the task has a Cost Type of User Hourly, Workfront uses the user rate. If the task has a Cost Type of Role Hourly, Workfront uses the job role rate to calculate Actual Labor Cost. </p> <p>For a project, Workfront uses the following formula to calculate the Actual Labor Cost:</p> <p><code>Project Actual Labor Cost = SUM(All Tasks Actual Labor Cost) </code> </p> <p>For more information, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>For example, if a user logs 5 hours for a task with a User Hourly Cost Type and their hourly rate is $100, the Actual Labor Cost is $500.</p></td> 
  </tr> 
  <tr> 
   <td>Actual Revenue </td> 
   <td> <p>The Actual Revenue of a project or a task is the amount of money associated with the Actual Hours of the project or the task. </p> <p>For information about tracking revenue in Workfront, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Actual Start</td> 
   <td>The timestamp when a user changes an object in in-progress on work assigned to them.</td> 
  </tr> 
  <!--<tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>Agile Methodology</td> 
   <td>A type of methodology based on the collaborative evolution of needs and solutions with cross-functional teams. It encourages flexibility and change based on a fixed timeline.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Agile Team</td> 
   <td>Differ from traditional team because they take their prospective work from a backlog and work on it within a set period of time that is called an Iteration.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>All My Teams</td> 
   <td> <p>When this is referenced in filters, this field displays either users that belong to the any of the teams that the logged-in user belongs to, or work items assigned to any of the teams that the logged-in user belongs to. </p> <p>We recommend using this field in a filter to make reports more generic when sharing them with other users. This way, you can build only one report which will display different information depending on who logs in to view it, as the information is always customized for the logged-in user. </p> </td> 
  </tr> 
  <tr> 
   <td>Allocation Date</td> 
   <td> <p>You can find this field in the following types of reports:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>Project (Financial Data)</li> 
     <li>Budgeted Hour</li> 
    </ul> <p>For a<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     --> Project (Financial Data) report: </p> 
    <ul> 
     <li>Build this report when trying to understand <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> the amount of Planned Hours that is assigned to your resources.</li> 
     <li> <p>The Allocation Date is the first day (Sunday) of a week in which the allocation of a Job Role to a task starts. A resource (Job Role) can have as many Allocation Dates as it has weeks during the Duration of the tasks that it is assigned to. If tasks span over multiple months, then the first day of a month can also become an Allocation Date, if it falls within the Duration of the task.</p> <p>For example, you can have a Job Role assigned to a task that spans over 3 weeks and has 90 Planned Hours. These hours are spread evenly during the duration of the task, which makes every day assign 6 Planned Hours to your job role:</p> <p><em> Daily Planned Hours = Total Planned Hours/ Number of Work Days during the Duration of the task </em> </p> <p>As a result, there are three Allocation Dates, one for every Sunday of every week during the Duration of the task, each with a certain number of Planned Hours associated with them.<br>If the task starts in the middle of the last week of a month and ends two weeks after the beginning of a new month, the task will have four Allocation Dates: one for every Sunday of every week during the Duration of the task, and one for the first day of the new month.</p> <p>To make the most use of this information, we recommend that you build a <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Project (Financial Data) report and add a matrix grouping for Allocation Date, then group the results weekly, monthly, quarterly, or yearly for the most accurate data.<br>For information about building a matrix grouping, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Create a matrix report</a>.</p> </li> 
    </ul> <p>Financial information populates in Project (Financial Data) reports only when the data associated with it is less than 5 years old. For example, if a job role was allocated to a task in January 2015 and today is September 2021, a financial filed like the Allocation Date for the job role does not populate in the Project (Financial Data) report. </p> 
    <div> 
     <p>For a Budgeted Hour report:</p> 
     <ul> 
      <li>Build this report when trying to understand the amount of Budgeted Hours that is allocated to your resources or to your projects in the Resource Planner.</li> 
      <li> <p>The Allocation Date is the first day (a Sunday) of the week for which you budgeted the hours in the Resource Planner. </p> <p>Tip:   <p>If a week spans for two months, it will generate two rows in the report: one corresponding to the first day of the week (Sunday of the first week which is during the first month), and the second row displays the first day of the second month. </p> <p>For example, if you budget 8 hours for a user for the week of June 30 (Sunday) - July 6 (Saturday), the two rows show an Allocation Date of June 30, and July 1. </p> </p> <p>For information about budgeting resources in the Resource Planner, see the article <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>.</p> <p>For information about building a Budgeted Hour report, see <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Announcements</td> 
   <td> <p>A way to communicate to users information within the system. This information is often coming from Workfront to the Administrator or from the Administrator to the user. </p> <p>For more information, see <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Send announcements</a></p> </td> 
  </tr> 
  <tr> 
   <td>App Integration</td> 
   <td>An app most commonly represents a connector to a software application, but can also represent special functions that manipulate data.</td> 
  </tr> 
  <tr> 
   <td>Approver Decision</td> 
   <td> <p>In the Proof Approval report, this field displays&nbsp;proof approval decisions for proofs that are no longer active.</p> </td> 
  </tr> 
  <tr> 
   <td>Approver stage</td> 
   <td>In the Proof Approval report, this field displays&nbsp;information about a proofs current stage.</td> 
  </tr> 
  <tr> 
   <td>Approval</td> 
   <td> <p>A given work item, such as a task, document, or timesheet, may require that a supervisor or other user sign off on the work item. This process of signing off is called approval. </p> <p>For more information, see <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Approval process overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Approval date</td> 
   <td>In the Proof Approval report, this field displays the date a proof was approved.</td> 
  </tr> 
  <tr> 
   <td>Approver</td> 
   <td>A user or job role that must sign off on a given work item, or the user that approves hour entries on timesheets.</td> 
  </tr> 
  <tr> 
   <td>Assigned To</td> 
   <td> <p>In a Task or Issue report, this field displays the Owner of the task or the issue, or the Primary Assignee. You can filter or group by this field, as well.</p> </td> 
  </tr> 
  <tr> 
   <td>Assignment</td> 
   <td>A user, job role, or team assigned to an issue or a task . Projects, portfolios, or programs cannot have assignments.</td> 
  </tr> 
  <tr> 
   <td>Assignments</td> 
   <td> <p>In a Task or Issue report, this field displays a list of all entities (users, job roles, teams) that are assigned to the task or issue. You can filter by this field using the fields Assignment Users and Assignment Roles. You can filter by the team assigned to the task or issue using the Team field. You cannot group a report by this field.</p> <p>Work items that have been placed in the Recycle Bin will continue to display in some reports that refer to the Assignment object where an OR filter modifier is used.</p> </td> 
  </tr> 
  <tr> 
   <td>Assignment Roles</td> 
   <td>
   <p>In a Task or Issue report, this field displays information about the job roles assigned to the tasks or issues. This field displays Primary Owners, as well as other job roles assigned to tasks or issues.</p> </td> 
  </tr> 
  <tr> 
   <td>Assignment Status</td> 
   <td> <p>In an assignment, task, or issue report, the Assignment Status displays whether the users assigned to a work item have clicked the Work On It or the Done button to accept or complete the work. The following Assignment Statuses exist:</p> 
    <ul> 
     <li><b>Requested</b>: the user has been assigned to the task or issue, but they have not clicked the Work On It button to start working on it yet.</li> 
     <li><b>Working</b>: the user has clicked the Work On It button and is currently working on the item. </li> 
     <li><b>Done</b>: the user has clicked the Done button and has completed their work on the item. </li> 
    </ul> <p>For more information, see <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">Work On It and Done button overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Assignment Teams</td> 
   <td>
   <p>In a task or issue report, this field displays information about the teams assigned to the tasks or issues. The field displays Primary Owners, as well as other teams assigned to tasks or issues. </p></td> 
  </tr> 
  <tr> 
   <td>Assignment Users</td> 
   <td>
   <p>In a Task or Issue report, this field displays information about the users assigned to the tasks or issues. This field displays Primary Owners, as well as other users assigned to tasks or issues. </p></td> 
  </tr> 
  <tr> 
   <td>Attribute</td> 
   <td>An attribute is a trait of a Workfront object.</td> 
  </tr> 
  <tr> 
   <td>Audit Area</td> 
   <td> <p>Audits are system messages that record an action tha happened in Workfront. The following audit types are recorded:</p> 
    <ul> 
     <li>Scope Change</li> 
     <li>Attachment Action</li> 
     <li>General Edit</li> 
     <li>Status Change</li> 
     <li>Note</li> 
     <li>Combined Entry</li> 
     <li>Error Entry</li> 
     <li>Status Change</li> 
     <li>Subscription Change</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Audit Trail</td> 
   <td>The collection of notes automatically generated by events that are tracked through the Recorded Changes (Audit Areas). Each note records who did the action, what they did, and when they did it.</td> 
  </tr> 
  <tr> 
   <td>Automatic And On Change</td> 
   <td> <p>One of the Project Update types. This will recalculate the Project's Projected and Planned timelines when the nightly recalculation process runs and when any update is made to the Project or Tasks within the Project. </p> <p>For more information, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Automatic Only</td> 
   <td> <p>One of the Project Update types. This will recalculate Projected and Planned timelines when the nightly recalculation process runs.</p> <p>For more information, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>BAU</td> 
   <td>"Business as usual" work that contributes to running the everday primary business goals.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Backlog</td> 
   <td>The area in an agile environment where new issues are kept until they are ready to be worked on.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Baseline</td> 
   <td>A source of data to measure iterations against in an agile environment.</td> 
  </tr> 
  
  <tr data-mc-conditions=""> 
   <td>Billing Record</td> 
   <td> <p>Records the revenue, hours, or expenses that can be billed. This information can be used to create invoices in an external accounting system.</p> <p>For more information, see <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Create billing records</a>. </p> 
   </td> 
  </tr>

 <tr> 
   <td>Billing Record Status</td> 
   <td> <p>In a Billing Record or Hour report, the Status of a billing record indicates whether the billing record has been Billed or Not Billed. You cannot delete a project or edit time associated with a Billed billing record. For more information, see <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Create billing records</a>.</p>  
   </td> 
  </tr>


  <tr> 
   <td>Branding</td> 
   <td>The process of customizing&nbsp;Workfront to give the interface an appearance that mirrors your company by using your colors and logos.</td> 
  </tr> 
  <tr> 
   <td>Breadcrumbs</td> 
   <td> <p>The area at the top of the page that shows the hierarchical location of where the user is in the application.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">For more information, see <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Breadcrumbs overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Budget Status</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>This field shows&nbsp;whether the project was added to the Capacity Planner and if the budget calculation has been completed&nbsp;for it. The Capacity Planner has been removed from&nbsp;Workfront. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;not added to the capacity planner, its value is <i>Not Included</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is <i>Included but not Calculated</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Budgeted Completion Date</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p>
   <p> This field is still visible in project and tasks reports and lists.</p>  </td> 
  </tr> 
  <tr> 
   <td>Budgeted Cost</td> 

   <td> <p>This is the cost associated with budgeting resources for a project. </p>
   <p>The field displays in the following areas of Workfront under the following names:</p>
   <ul>
   <li><strong>Budgeted Cost</strong>: in the Business Case Summary panel</li>
   <li><strong>Cost</strong>: in the Utilization areas when viewing information by Cost</li>
   <li><strong>Project Budgeted Cost</strong>: in lists and reports</li>
   </ul>   
    <p>The Budgeted Cost for the project is calculated using the following formula:</p> 
    <p><code>Project Budgeted Cost (or Budgeted Cost) = Budgeted Expense Cost + Budgeted Labor Cost + Fixed Cost of the project</code> </p> 
    <p>For more information about calculating Budgeted Cost and to understand various names for this concept in Workfront, see <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calculate Project Budgeted Cost</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Budgeted Hours</td> 
   <td> <p>The hours budgeted for resources for the work they need to complete on projects. This field refers to the hours budgeted in the Resource Budgeting area of the Business Case (or in the Resource Planner) for the project or for the project resources.</p> <p>For more information, see <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> For information about budgeting Users in the Resource Planner, see the article <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> 
    <p>The hours budgeted in the Resource Budgeting area of the Business Case or the Resource Planner display in the following areas of Workfront and under the following names:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>Budgeted Hours display name</strong></td> 
        <td><strong>Areas of Workfront</strong></td> 
       </tr> 
       <tr> 
        <td>Hours</td> 
        <td>Resource Budgeting area of the Business Case</td> 
       </tr> 
       <tr> 
        <td>BDG</td> 
        <td>Resource Planner viewed by Hours</td> 
       </tr> 
       <tr> 
        <td>Budgeted Hours</td> 
        <td> <p>Utilization report Hours view</p> <p>For more information about the Utilization report, see the article <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Overview of the Resource Utilization report</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>Bud. Hours</td> 
        <td> <p>Budgeted Hour report</p><p>The Budgeted Hour object in the Budgeted Hour report refers to information related to a deprecated resource management tool. Only the "Bud. Hours" field in this report refers to the hours budgeted in the Resource Planner or the Resource Budgeting area of the project's Business Case. </p> <p>For more information about creating a report, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>Resource Planner Budgeted Hours </td> 
        <td> <p>Found in the following reports:</p>
        <ul>
        <li>Project report
        <li>Project (Financial Data) report
        <li>Task report
        <li>Issue report
        <li>Budgeted Hour report</li>
        </ul>
         <p>For more information about creating a report, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Any other mention of Budgeted Hours in Adobe Workfront refers to hours budgeted using deprecated features that have been removed from Workfront . These are view-only fields and do not update with current information when you use current resource budgeting tools. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the&nbsp;Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial&nbsp;Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>Budgeted Labor Cost</td> 
   <td> <p>This is the cost associated with the hours that you, as the Resource Manager, budget for your job roles for the work they need to complete on projects. </p> <p>The Budgeted Labor Cost in a project report is calculated using the following formula:</p> <p><code style="font-style: normal;">Budgeted Labor Cost = SUM(Job Role Cost per Hour * Budgeted Hours per Job Role)</code> </p> <p>This field  may refer to the following:</p> 
    <ul> 
     <li> <p>Labor costs displayed in the Resource Budgeting area of the Business Case or in the Resource Planner that are associated with the cost of job roles on a project. For information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Labor costs displayed in the Resource Budgeting area of the Business Case that reflect the People Costs estimated in an initiative linked to the project from the Scenario Planner when you use the Scenario Planner to budget your project resources. For information about initiatives, see <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Initiatives overview in the Scenario Planner</a>. </p> <p>The Scenario Planner requires an additional license. For information about the Workfront Scenario Planner, see <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The Scenario Planner overview</a>. </p> </li> 
     <p>It displays in the following areas of  under the following names:</p>
   <ul>
   <li><strong>Budgeted Labor Cost</strong>: in the Resource Budgeting area of the Business Case.
   <li><strong>Budgeted Cost</strong>: in the Utilization report Cost view
   <p>For more information, see <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">View resource utilization information </a>.</p>
   <li><strong>BDG</strong>: in the Resource Planner Project or Role views, when viewing by Cost
   <li><strong>Resource Planner Budgeted Labor Cost</strong>: in the following reports: 
   <ul>
    <li>Project report</li>
    <li>Project (Financial Data) report</li>
    <li>Task report</li>
    <li>Issue report</li>
    <li>Budgeted Hour report</li> 
    </ul>
    <p>For more information about creating a report, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;.&nbsp;</p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>Budgeted Start Date</td> 
  <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated.</p>
  <p>These areas have been removed from Workfront. </p> 
  <p>The field is still visible in project and task reports and lists.</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Burndown Chart</td> 
   <td>A line chart that provides a visual representation of completed and remaining work.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Business Case</td> 
   <td> <p>A tool used to evaluate whether a project should be moved forward from the Idea status to the Planning status. In other words, a business case helps the organization decide whether it is worthwhile to launch and complete the project or not, especially when comparing projects with others in a portfolio.</p> <p>For more information, see <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Create a Business Case for a project </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Business Case Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated.</p> <p>This field is still visible in project and task lists and reports. </td> 
  </tr> 
  <tr> 
   <td>Calculated Assignment</td> 
   <td> <p>One of the task Duration Types. This will calculate the percentage of an 8-hour work day that the user assigned to the task will be allocated to the task, based on the Duration of the task and the Work Required.</p> <p>For more information, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Calculated Work</td> 
   <td> <p>One of the task Duration Types. This will calculate the WOrk Required on a task, given the Duration and the user Assignment percentages (which are based on an 8-hour work day).</p> <p>For more information, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Calendar</td> 
   <td> <p>There are two types of calendars in Workfront: the Home Calendar and calendar reports.</p> <p>The Home Calendar is a personal calendar that allows a user to manage their workload against their available hours in Workfront. The user can also integrate their Home Calendar with Outlook (Google and Microsoft integration to come). </p> <p>For more information about the Home Calendar, see <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">Home Calendar view</a>.</p> <p>A calendar report is a dynamic report in which users can view the date and other important details of an event, including the due date, status of work, and the user to whom the event is assigned.</p> <p> For more information about calendar reports, see <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Calendar reports overview</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>Can Start</td> 
   <td> <p>This field indicates whether a task is ready to start to be worked on. If the start is ready to be worked on the Can Start field on the task is set to True. </p> <p>For more information, see <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">"Can Start" overview for tasks</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;</li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;</li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    --> <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    --> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  --> 
  <tr> 
   <td> <p>Category</p> </td> 
   <td> <p>A category is a custom form. You can build reports for this object and you can show it in other object reports, as well. Not all objects can have a custom form, or category. The following objects can have a custom form:&nbsp;<br></p> 
    <ul> 
     <li>Project</li> 
     <li>Task</li> 
     <li>Issue</li> 
     <li>Portfolio</li> 
     <li>Document</li> 
     <li>Expense</li> 
     <li>Program</li> 
     <li>User</li> 
     <li>Company</li> 
    </ul> <p>Iteration</p> </td> 
  </tr> 
  <tr> 
   <td>Category&nbsp;Name</td> 
   <td> <p>When added as a column to the view of any of the following objects it displays a list of all custom forms associated with these objects:</p> 
    <ul> 
     <li>Project</li> 
     <li>Task<br></li> 
     <li>Issue<br></li> 
     <li>Portfolio<br></li> 
     <li>Document<br></li> 
     <li>Expense<br></li> 
     <li>Program<br></li> 
     <li>User<br></li> 
     <li>Company</li> 
     <li>Iteration</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Change Management</td> 
   <td>A practice area focused on defining, understanding, and adapting planned work to changes in scope, schedule, cost, and resource factors.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Change Order</td> 
   <td>A type of issue raised against a project that outlines a requested change to the agreed scope.</td> 
  </tr> 
  <tr> 
   <td>Change Only</td> 
   <td>One of the Project Update Types. It only updates Project Projected and Planned timelines when Updates are made to Tasks or edits are performed on the Project or Tasks.</td> 
  </tr> 
  <tr> 
   <td>Change Order</td> 
   <td> <p>One of the Issue types, usually indicating that an unplanned amount of work must be done before the project can be completed.</p> <p>For more information on Issue types, see the section "Default issue types" in the article <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Customize default issue types</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Child Task</td> 
   <td>A task that is a Subtask of a Parent Task (Summary Task).</td> 
  </tr> 
  <tr> 
   <td>Children</td> 
   <td>The collection of Subtasks to a Parent Task (Summary Task).</td> 
  </tr> 
  <tr> 
   <td>Coaching and Training</td> 
   <td>Learning modules, certifications, standards, or a community of practice.</td> 
  </tr> 
  <tr> 
   <td>Commit</td> 
   <td>A communication tool for users to set expectations regarding task deliverables.</td> 
  </tr> 
  <tr> 
   <td>Commit Date</td> 
   <td>A communication tool for user's to set expectations around task deliverables.</td> 
  </tr> 
  <tr> 
   <td>Communication and Reporting</td> 
   <td>Standards to review the exceptions and health of a project, program, or portfolio</td> 
  </tr> 
  <tr> 
   <td>Company</td> 
   <td> <p>A Company is an organizational unit in Workfront. </p> 
   <p> You can associate a user or a project with one company. For more information, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Create and edit companies</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>Completion date</td> 
   <td> <p>The date that a project, task, or issue is set to be completed. There are several types of Completion dates in Workfront:</p> 
    <ul> 
     <li>Actual Completion Date. For more information, see <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Overview of the project Actual Completion Date </a>.</li> 
     <li>Planned Completion Date. For more information, see <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Set the project Planned Completion Date</a> and <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overview of the task Planned Completion Date</a>.</li> 
     <li>Projected Completion Date. For more information, see <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Overview of the Projected Completion Date for projects, tasks, and issues</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Completion Day</td> 
   <td>The day, relative to the start of the Template, that a Template Task or a Template is supposed to be complete.</td> 
  </tr> 
  <tr> 
   <td>Completion Mode</td> 
   <td> <p>This indicates how a project will be marked as Complete. It can have two values:</p> 
    <ul> 
     <li>Manual: A user must change the project status to Complete.</li> 
     <li>Automatic: The project status will automatically change to Complete when all of the tasks in the project are 100% Complete and all of the issues are closed.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Condition</td> 
   <td> <p>This is a visual representation of the progress of a task, issue or project.</p> <p>For projects, the condition can be manually set by the project owner or it can be automatically set by Workfront, based on the progress status of the project. </p> <p>The possible values for the project condition are:</p> 
    <ul> 
     <li>On Target</li> 
     <li>At Risk</li> 
     <li>In Trouble</li> 
    </ul> <p>For more information about project condition, see the article <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Overview of Project Condition and Condition Type</a>.</p>
     <p>You can associate task and issue conditions with a number that can display in reports. The lists below display the default names and numbers for task and issue conditions. Your system administrator can update the names of conditions and they can add new conditions with different numbers. After a number is associated with a condition, it cannot be edited.  </p> 
     <p>For tasks, the condition is set manually by the task owner. The possible values for the task condition are:</p> 
    <ul> 
     <li>Going Smoothly (0)<br></li> 
     <li> Some Concerns (1)<br></li> 
     <li>Major Roadblocks (2)</li> 
    </ul> <p>For more information about task condition, see the article <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Update Condition for tasks and issues</a>.</p> <p>For issues, the condition is set manually by the issue owner. The possible values for the task condition are:<br></p> 
    <ul> 
     <li>Going Smoothly (0)<br></li> 
     <li>Some Concerns (1)<br></li> 
     <li>Major Roadblocks (2)</li> 
    </ul> 
   <p><b>NOTE</b></p>
    <p>When the Condition field is tracked in Journal Entry reports, the New and Old Number Values display the number associated with the condition instead of its name. If a condition is originally not defined for a task or an issue and you later update it, the journal entry that captures the update will display the Old Number Value of the Condition field as -2,147,483,648. See also "New Number Value", "Old Number Value", and "Journal Entry" in this article. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>Condition Update</td> 
   <td> <p>This field shows the current condition of tasks, projects or issues. This option shows the most recent updates that the owners of tasks, projects or issues have provided in the Update Status field, along with the new condition.</p> <p>Comments made on condition updates are not displayed in the Condition Update column; only the main update is displayed.</p> </td> 
  </tr> 
  <tr> 
   <td>Constraint Date</td> 
   <td> <p>If you are using a Task Constraint that is tied to a specific date, such as Must Start On, then that specific date becomes the Constraint Date of the task.</p> <p>The following task constraints update the Constraint Date field:</p> 
    <ul> 
     <li>Must Start On</li> 
     <li>Must Finish On</li> 
     <li>Start No Later Than</li> 
     <li>Start No Earlier Than</li> 
    </ul> <p>Tip:   
     <ul> 
      <li> <p>A task with a Constraint of Fixed Dates has no Constraint Date. </p> </li> 
      <li> <p> Constraint Date is only viewable in a report or customized view.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td>Constraint Day</td> 
   <td> <p>If you are using a Task Constraint in a template task that is tied to a specific day, such as Must Start On, then that specific day becomes the Constraint Day of the template task.</p> <p>The following task constraints update the Constraint Day field:</p> 
    <ul> 
     <li>Must Start On</li> 
     <li>Must Finish On</li> 
     <li>Start No Later Than</li> 
     <li>Start No Earlier Than</li> 
    </ul> <p>Tip:   Constraint Day is only viewable in a report or customized view. </p> </td> 
  </tr> 
  <tr> 
   <td>Constraint Type</td> 
   <td> <p>The scheduling tendency of a Task. For example, As Soon as Possible will schedule a Task to begin as soon as possible, and Finish No Later Than will schedule a Task to finish by the Constraint Date and no later.</p> <p>For more information, see <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Contextual Menu</td> 
   <td>A menu, located on the left side of the screen, on which the items change to correlate with the active content. For example, when a user is viewing a Project, the Contextual Menu will display links to Project-related information and tools.</td> 
  </tr> 
  <tr> 
   <td>Converted Issue Originator</td> 
   <td>A field in a project or task report that displays information about the user who is the Primary Contact of an issue when the issue is converted into a project or task. The field also displays in the Project Details  section  where it displays the name of the Primary Contact of the converted issue. See also "Primary Contact" in this article.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Cost</td> 
   <td> <p>The monetary amount that you must spend when completing a project, task, or issue. </p> <p>You can track various types of costs for labor, expenses, risks that relate to the project.For information about tracking costs in Workfront see <a href="../../../manage-work/projects/project-finances/track-costs.md">Track costs</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>Cost Type</td> 
   <td>For a task, the Cost Type determines how the task will accrue costs. Some examples include Fixed Hourly, User Hourly, and User Hourly plus Fixed. </td> 
  </tr> 
  <tr> 
   <td>Cross-Project Dependencies</td> 
   <td> <p>A task of one project is dependent on a task from a different project.</p> <p>For more information, see <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Create cross-project predecessors</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Custom Data</td> 
   <td> <p>Data that is unique to an organization. Organizations can customize the Workfront application by creating custom forms and custom fields. This custom information can drive reporting for KPIs, auditing, and demand mix. </p> <p>Custom Data can be linked to:</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Users</li> 
     <li>Companies</li> 
     <li>Issues</li> 
     <li>Documents</li> 
     <li>Expenses</li> 
     <li>Portfolios</li> 
     <li>Programs</li> 
     <li>Iterations</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Custom Data Type</td> 
   <td>The option to specify if a Custom Data Field is stored in the database as Text, a Date, a Number, or Currency.</td> 
  </tr> 
  <tr> 
   <td>Custom Display Type</td> 
   <td>The field display type of a custom field. Examples include Drop-Down, Text Field, Text Area, Radio Buttons, etc.</td> 
  </tr> 
  <tr> 
   <td>Custom Field</td> 
   <td>For Custom data that allow the user to select from several options, these are the values from which a User can select. Custom Options are only valid on Drop-Down, Multi-Select Drop-Down, Radio Buttons, and Checkboxes.</td> 
  </tr> 
  <tr> 
   <td>Custom Form Label</td> 
   <td>When using a Custom Display Type with Custom Options, this is the User Interface text that will display in the Drop-Down menu, the Checkboxes, or the Radio Buttons for that Custom Option.</td> 
  </tr> 
  <tr> 
   <td>Custom Value</td> 
   <td>When using a Custom field with Custom Options, this is the value that will be store in the database for a particular Option.</td> 
  </tr> 
  <tr> 
   <td>Custom View</td> 
   <td>A definition of the data fields, or columns, that are displayed for each object in a list.</td> 
  </tr> 
  <tr> 
   <td>Customer</td> 
   <td>An organization that uses an instance of Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## D - F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Name</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Dashboards</td> 
   <td> <p> You can add this field in a report or a list of the report object, to display the dashboards on which the report is listed in a list. </p> <p> You can use this field to filter for reports that are listed on a specific dashboard, as well. </p> <p> For more information about including dashboard information on report object reports, see the "Understanding What Reports Are Listed on Dashboards" section in the article <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Access and organize reports</a></p> </td> 
  </tr> 
  <tr> 
   <td>Data Type</td> 
   <td>See "Custom Data Type".</td> 
  </tr> 
  <tr> 
   <td>Days Late</td> 
   <td> <p>This field shows a date difference between Planned Start and Today if the Actual Completion Date is missing.</p> <p>Also&nbsp;shows a date difference between Actual Completion and Planned Completion, when an Actual Completion Date is present.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Default Schedule</td> 
   <td> <p>Customizable default working hours to be assigned to users and projects within an organization. </p> <p>Schedules are used to calculate the planned, start, and completion dates of tasks that are assigned to users.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Deliverable</td> 
   <td>Quantifiable goods or services that must be provided upon the completion of a project.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Demand Management</td> 
   <td>Scoring and prioritization of the intake processes.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Department Goals</td> 
   <td>Goals unique to a specific department that focus on improving operational metrics within the department.</td> 
  </tr> 
  <tr> 
   <td>Dependency</td> 
   <td>The link between two tasks that require one task to change status before the other task can also change status.</td> 
  </tr> 
  <tr> 
   <td>Dependency Type</td> 
   <td> <p>The type of scheduling relationship between a task and its predecessor(s). One example is Finish-Start, which requires that the fist task must Finish before the second task can Start.</p> <p>For more information, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Document</td> 
   <td>Any file that is attached to an object within Workfront.</td> 
  </tr> 
  <tr> 
   <td>Document Version</td> 
   <td> <p>Each time the same document is uploaded to the same object, it is assigned a version number. Users can view and change several options for a previous version of a document.</p> <p>For more information, see <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Manage document versions</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Duration</td> 
   <td> <p>The window of time allocated for completion of a task issue, or project (as determined by the number of days between the Planned Start and the Planned Completion).</p> 
    <ul> 
     <li>For tasks, the Duration is an editable field if the Duration Type of the task is not Simple. If the Duration Type of the task is Simple, or if the Task Constraint is Fixed Dates, the Duration is a calculation performed by Workfront.</li> 
     <li>For issues, the Duration is always an editable field and it should represent an estimate of a number of days that would require the issue to be resolved.</li> 
     <li>For projects, the Duration is a calculation performed by Workfront and it represents the difference in days between the Planned Start of the earliest task and the Planned Completion of the latest task on the project.</li> 
    </ul> <p>For more information about the difference between Duration and Planned Duration for tasks, see the article <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Difference between Planned Duration and Duration for tasks</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Duration in Minutes</td> 
   <td>This field displays the same information as the Duration field in minutes instead of days. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>Duration per Occurrence</td> 
   <td> <p>This displays in the Task&nbsp;Details and the Edit Task boxes of a parent of recurring tasks. It displays the duration of each recurring task. For information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>. </p> <p> <span>Durations modified in individual recurring tasks do not display the value indicated in this field.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Duration Type</td> 
   <td> <p>A task field that indicates how the work required to complete the task is allocated to the assignees across the task duration. It represents the relationship between the Duration of the task, the Work Required, and the amount of time, or Allocation, the assigned resources should spend on the task to complete it. </p> <p>This field appears on the Details tab of a task. </p> <p>Option are:</p> 
    <ul> 
     <li>Calculated assignment</li> 
     <li>Calculated Work</li> 
     <li>Effort Driven</li> 
     <li>Simple</li> 
    </ul> <p>For more information, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>Duration Unit</td> 
   <td>The unit that is used to measure time in a power search.</td> 
  </tr> 
  <tr> 
   <td>Effort Driven</td> 
   <td>The relationship between the number of users and the amount of time the task will take to complete. As you add more users, the total time scheduled for the task to complete decreases, but the duration of the task stays the same. For example if a task is shelling a barrel of peanuts, adding more people will decrease the time scheduled, but the duration in person-days will remain the same.</td> 
  </tr> 
  <tr> 
   <td>Elapsed Time</td> 
   <td> <p>Elapsed time is a unit of time for a task's Duration. It is the time between the Planned Start Date and the Planned Completion Date of a task that includes holidays, weekends, and time off. In other words, elapsed time is the passage of calendar days. </p> <p>Workfront supports the following elapsed time units for task duration:</p> 
    <ul> 
     <li> <p>Elapsed Minutes</p> </li> 
     <li> <p>Elapsed Hours</p> </li> 
     <li> <p>Elapsed Days</p> </li> 
     <li> <p>Elapsed Weeks</p> </li> 
     <li> <p>Elapsed Months</p> </li> 
    </ul> <p>For more information about task duration, including elapsed time, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>End Date</td> 
   <td> <p> In a Rate report, this is the date when a new billing rate for a job role at the project level ends. The hours associated with the project that are before this date are multiplied by this billing rate to calculate the revenue on the project. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>Engagement</td> 
   <td>The Work Performance Indicator (WPI) that indicates when commitment and belief in the task, project, team, or organization is waning. This indicates that you need to act to revive that belief and commitment. WPI would be measured by asking the simple questions, "Did you understand what was expected of you? Did the work you were assigned make a difference to the organization? Did you do great work?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Enterprise Goals</td> 
   <td>Cross-functional goals that contribute to the metrics of the company goals.</td> 
  </tr> 
  <tr> 
   <td>Event</td> 
   <td>Any change in a project or task.</td> 
  </tr> 
  <tr> 
   <td>Event Handler</td> 
   <td>Automated tasks that occur when Events take place. A common example is an automated email notification.</td> 
  </tr> 
  <tr> 
   <td>Event notification</td> 
   <td>Email that is generated from an event handler.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Expenses</td> 
   <td>A non-labor cost on tasks or projects.</td> 
  </tr> 
  <tr> 
   <td>External</td> 
   <td> <p>Typically, a license type, or a user with such a license, which only has the ability to review information in the system.</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>External System</td> 
   <td>Any services or software that is stored and governed outside the designated system of record.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Filter</td> 
   <td> <p>One of the main building blocks of a report or a list element that defines what information displays on the screen. For more information about reporting elements, see <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Reporting elements: filters, views, and groupings</a>.</p> <p>The Filter determines the results that display in a report or on an Workfront panel listing, like projects, tasks, or issues.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Financial Work Management</td> 
   <td>Process to manage labor costs, expenses, and revenue data in Workfront.</td> 
  </tr> 
  <tr> 
   <td>Fixed Cost</td> 
   <td>You can define a fixed amount of cost for a project. This is part of the Planned Cost of the project which represents the amount of money that you need to complete the project. For information about costs, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>. </td> 
  </tr> 
  <tr> 
   <td>Fixed&nbsp;Revenue</td> 
   <td>You can define a fixed amount of revenue for a project. This is part of the Planned Revenue of the project which represents the amount of money that you might obtain if you complete the project. For information about revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>. </td> 
  </tr> 
  <tr> 
   <td>Flags</td> 
   <td> <p> This is the same field as Status Icons, but it is only available for the following views: </p> 
    <ul> 
     <li> Templates </li> 
     <li> Expenses </li> 
    </ul> <p> For more information, see the article <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Built-in Status Icons in Views</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder</td> 
   <td>Folders are used to organize documents or reports associated with an object.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Integrated"> 
    <td>FTE</td> 
    <td>The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours.</td> 
   </tr>
  --> 
 </tbody> 
</table>

## G - I

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Name</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Gantt Chart</td> 
   <td> <p>A visual timeline of the project dates in a calendar view based on the planned or projected dates as the tasks of the project are currently scheduled.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Goal</td> 
   <td><p>There are two concepts of goals in Workfront: </p> 
    <ul> 
     <li> <p><b>Project goals</b>: A set of business objectives agreed to by the relevant stakeholders of a project. Project goals are part of the Business Case of a project. </p> <p>You cannot display project goals in lists or reports but you can access them through the API. </p> <p>For information about Business Case project goals, see <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Create Business Case goals </a>. </p> </li> 
     <li> <p><b>Strategic goals</b>: A strategic goal is an objective that you create to plan your work strategy for a specific time-period. You can create these types of goals using Workfront Goals. Your organization must purchase an additional license and you must have access to this feature to be able to create strategic goals. Workfront Goals are available only with an additional license.</p> 
     <p>For more information, see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">Adobe Workfront Goals overview </a>. </p> 
     <p>You can display strategic goals in a goal or a project report and access them through the API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Goal Hierarchy</td> 
   <td> <p>In Goal and Project reports, this is a collection field that displays the goals in the hierarchy that a strategic goal belongs to when it aligns to other goals. The goals are separated by a ▸ delimiter. </p> <p>Only the parents of the goal and the goal display in this field. Children goals do not display. </p> <p>For information about aligning goals in Workfront Goals, see <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Goal alignment overview in Workfront Goals</a>. </p> 
   <p>This field is visible only if your organization has purchased Workfront Goals. For information about managing strategic goals using Workfront Goals, see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">Adobe Workfront Goals overview </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Goal Success Score</td> 
   <td> In a Project report this field used to refer to project-level goals associated with the Business Case. Currently, this is a deprecated field and is not associated with any functionality.</td> 
  </tr> 
  <tr> 
   <td>Goals </td> 
   <td> <p>In a Project report, this is a collection field that displays all the strategic goals that are associated with a project. The goals are separated by commas.</p> <p>This field is visible only if your organization has purchased Workfront Goals. For information about managing strategic goals using Workfront Goals, see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">Workfront Goals overview</a>. For more information about strategic goals and project goals in Workfront, see "Goal" in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Global Interface Preferences</td> 
   <td>Interface settings that affect all users. Global Interface Preferences can be overwritten by the User Interface Preferences.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Group</td> 
   <td> <p>A collection of users (possibly from the same department or business unit) that have access to the same objects. In addition to users, groups can be associated with portfolios, programs, projects,<span> project templates,</span> companies, teams, schedules, layout templates, and timesheet profiles.</p> <p>You can also grant permissions to objects by group. For more information, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> <p>In a list or report of objects of one of the following types, you can use the Group field to list which objects of that type are associated with a particular group: user, portfolio, program, project, <span>project template</span>, company, team, schedule, layout template or timesheet profile.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Group Administrator</td> 
   <td> <p>Users who manage the objects, access, and users of designated user groups.</p> <p> In a Group report, this field displays the names of the users designated as Group Administrators in the Group. For more information about Group Administrators, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Group with Administration Access</td> 
   <td> <p> In a Layout Template, Timesheet Profile, or Schedule report, this field displays the Groups whose Group Administrators have access to modify the template. You can also filter this report by this field. </p> <p> For more information, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Grouping</td> 
   <td> <p>A reporting element used to categorize information in a list by a common criterion.</p> <p>For more information, see the "Groupings" section in the article <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Reporting elements: filters, views, and groupings</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Handoff Date</td> 
   <td> <p>The date when a task becomes available for work. The Handoff Date is a calculation and cannot be set manually. <br>For more information about the Handoff Date, see the article <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">Task Handoff Date overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Help Desk</td> 
   <td>The portion of Workfront that holds all issue queues. The Help Desk can be used to process customer support tickets, project requests, help desk tickets, etc. This is the same as the Requests area.</td> 
  </tr> 
  <tr> 
   <td>Owner</td> 
   <td>In an Hour report, the&nbsp;Owner is the user to whom the hours are attributed. This is different than the user who is actually logging the time. These two entities can sometimes be two different users. <br>For more information about logging time for another user, see the article <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Log time</a>.</td> 
  </tr> 
  
  <tr> 
   <td>Hour Status</td> 
   <td> <p>An attribute set by Workfront for the Actual Hours that users log for tasks, issues, or projects. </p>
   
   Hour entries can have one of the following statuses in Workfront:
   <ul>
   <li><b>Submitted</b>: the hours have been logged on a project, task, or issue. They are either part of a billing record or not added to a billing record yet.</li>
   <li><b>Approved</b>: the hours have been logged and they have been approved by the Project Owner. They are either part of a billing record or not added to a billing record yet.</li> 
   <li><b>Not Approved</b>: the hours have been logged and rejected by the Project Owner. They are either part of a billing record or not added to a billing record yet.</li>
   <li><b>Billed</b>: the hours have been logged, added to a billing record, and the billing record status has been marked as Billed. They did not require to be approved by the Project Owner.</li>
   <li><b>Billed and Approved</b>: the hours have been logged, approved by the Project Owner, and the billing record status has been marked as Billed.</li>
   </ul> 


   <p>When hours are part of a billing record, the Hour Status indicates whether the hours have been approved or if the Billing Record they belong to has been billed. The Hour Status of an hour entry is only visible in an hour list or report. </p>

   <p>For more information about adding hours to billing records, see the section "Add Hours to billing records" in the article <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Create billing records</a>.</p>

   <p>For more information about approving time on projects, see <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Require time to be approved for a project</a>.</p>
   
   <p><b>TIP</b></p>
   
   <p>General Hours that are not logged directly on work items do not display an Hour Status. </p> </td> 
  </tr>


  
  <tr> 
   <td>Hour Type</td> 
   <td> <p>An attribute that can be set for Actual Hours that users log for tasks, issues, or projects. This is also an attribute for the hours logged that are not directly linked to work, such as Vacation and Time Off.</p> <p>For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Manage hour types</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>ID</td> 
   <td> <p>The ID is an alphanumeric indicator associated with every object in&nbsp;Workfront. It uniquely identifies each object in the Workfront database. You can view the ID of any object in a report or a list for each object. </p> <p>Tip:   <p>You can also view the ID in the URL of the object's page. For example, the ID of a project might look something like the number outlined in the following URL, when you access the Project&nbsp;Details page:</p> <p><code>https://&lt;your domain&gt;.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Individual Goals</td> 
   <td>Individual goals which contribute to the metrics of the team goals, but not related to personal or career development.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Inherited Access</td> 
   <td>Sharing function that allows access to propagate from object to another. For example, project user's inherit access defined in program and portfolio records.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Initiative</td> 
   <td> <p>In&nbsp;the Workfront Scenario Planner, you can divide a plan into several initiatives to make it easier to manage the plan. <span>You can build an Initiative report and you can access Initiative information in a Project report.</span></p> <p>The Scenario Planner requires an additional license. For information about the Workfront Scenario Planner, see <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The Scenario Planner overview</a>. </p> <p>The Initiative report is not visible in your Workfront instance unless your company has purchased a Workfront Scenario Planner license. You cannot access Initiatives through the API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Initiative Job Role</span> </td> 
   <td> <p><span>The Initiative Job Role report type displays information about the job roles associated with a plan initiative in the Workfront Scenario Planner.</span> </p> <p>The Scenario Planner requires an additional license. For information about the Workfront Scenario Planner, see <a href="../../../scenario-planner/scenario-planner-overview.md">The Scenario Planner overview</a>. </p> <p><span>This report type is not visible in your Workfront instance unless your company has purchased a Workfront Scenario Planner license.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Initiative Job&nbsp;Role Hours</span> </td> 
   <td> <p><span> In an Initiative Job&nbsp;Role report, this displays the number of hours associated with a job role in an initiative.</span> </p> <p>The Scenario Planner requires an additional license. For information about the Workfront Scenario Planner, see <a href="../../../scenario-planner/scenario-planner-overview.md">The Scenario Planner overview</a>. </p> <p>This field and the Initiative Job Role report type are not visible in your Workfront instance unless your company has purchased a Workfront Scenario Planner license.</p> </td> 
  </tr> 
  <tr> 
   <td>Initiative Job Role Count</td> 
   <td> <p>In an Initiative Job Role report, this displays the number of a specific job role associated with an initiative.</p> <p>The Scenario Planner requires an additional license. For information about the Workfront Scenario Planner, see <a href="../../../scenario-planner/scenario-planner-overview.md">The Scenario Planner overview</a>. </p> <p>This field and the Initiative Job Role report type are not visible in your Workfront instance unless your company has purchased a Workfront Scenario Planner license.</p> </td> 
  </tr> 
  <tr> 
   <td>Initiative Last Published Date</td> 
   <td> <p>A field in an Initiative, Initiative Job Role, and Project reports that displays the date that a plan initiative was last published to a project. You can publish initiatives to create projects or to update projects linked to the initiatives.</p> <p>The Scenario Planner requires an additional license. For information about the Workfront Scenario Planner, see <a href="../../../scenario-planner/scenario-planner-overview.md">The Scenario Planner overview</a>. </p> <p><span>For information about publishing initiatives, see</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publish scenarios to create and update projects in the Workfront Scenario Planner</a>. This field is not visible in your Workfront instance unless your company has purchased a Workfront Scenario Planner license.</p> </td> 
  </tr> 
  <tr> 
   <td>Inline Search</td> 
   <td>A search performed, in the process of completing a form, to find possible entries for one specific field.</td> 
  </tr> 
  <tr> 
   <td>Interface Setup</td> 
   <td>The area of the application that allows defining Custom Views, Filters, Groupings, List Controls, etc.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Is Company Goal</p></td> 
   <td> <p>In goal reports, this displays a "True/ False" value for each strategic goal to indicate whether your organization is assigned to the goal as its owner. </p> 
   <p>This field is visible only if your organization has purchased Workfront Goals. For information about managing strategic goals using Workfront Goals, see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">Adobe Workfront Goals overview </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Issue</td> 
   <td> <p>An unplanned work item that usually indicates that there is a problem preventing the completion of a task or project. It is triaged and evaluated for further work effort consideration</p> <p>An Issue can also be a Help&nbsp;Desk request. Change Orders, Requests, and Bugs are also Issues.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Issue Management</td> 
   <td> <p>The process and rules governing the definition of issue types and the routing, triage, or traffic process associated with each type.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Issue Owner</td> 
   <td>The team or users responsible for triaging and completing an issue.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>Iteration</td> 
   <td>A period of time in which a team produces a pre-defined set of deliverables.</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Name</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Job Role</td> 
   <td> <p>Used to identify a user's day-to-day job functions and responsibilities. Job roles can be assigned to work items to identify the required skill needed to complete a work process without assigning it to a specific user. </p> <p>A user can have more than one role. Examples include Graphic Designer or Consultant.</p> <p>For more information, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Journal Entry</p> </td> 
   <td> <p>A reportable object that tells you information about system updates for tracked fields that appear in the Updates area of projects, tasks, issues, and other objects.</p> <p>To learn more, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Report on the Updates area</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Kanban Flag</td> 
   <td> <p>In a Task Report or Issue Report,&nbsp;the Kanban Flag field displays the flag status that is set on the story on the Kanban board. Possible values are On Track, Ready to Pull, and Is Blocked.</p> <p>For more information about setting flag status on stories on the Kanban story board, see&nbsp; the article <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Use flags on stories on the Kanban board</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPIs</td> 
   <td>A measurable value that demonstrates how effectively a company is achieving key business objectives.</td> 
  </tr> 
  <tr> 
   <td>Lag</td> 
   <td>Amount of time that must pass after the predecessor task's Planned Completion Date has passed until the dependent task can begin.</td> 
  </tr> 
  <tr> 
   <td>Lag Types</td> 
   <td> <p>The method of calculating the Lag. It can be:</p> 
    <ul> 
     <li>Days (work days)</li> 
     <li>Calendar Days (ignore holidays)</li> 
     <li>Percent</li> 
     <li>Day of Week</li> 
    </ul> <p>For more information, see the section "Lag Types overview" in <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Overview of Lag Types</a></p> </td> 
  </tr> 
  <tr> 
   <td>Large Thumbnail</td> 
   <td> <p> In a Document list or report, it displays a preview of the document in a thumbnail. </p> <p>Select <strong>Large Thumbnail</strong> to view a 400 pixel-wide thumbnail in the report.</p> <p>The size of the thumbnail adjusts when you modify the width of the column in a list or report.</p> <p>See also "Thumbnail" in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Last 10 Viewers</td> 
   <td> <p>In a report list, this field displays the names of up to 10 users who have viewed the report most recently.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Last Condition Note</td> 
   <td> <p>This field displays the update last entered on an object by the&nbsp;owner of the object, This is the owner's most recent activity or interaction on an object.</p> <p>The Last Condition Note column is&nbsp;empty if the note text of the last note of an object has been deleted. When a new note is entered on the object, it becomes the last note and it displays again in the column.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Last Finance Update Date</td> 
   <td>In a project report, this field captures the date and the time when the project finances were last calculated and updated. For information about project finances, see <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Project finances overview</a>. </td> 
  </tr> 
  <tr> 
   <td>Last Note</td> 
   <td> <p>This field displays the update last entered on an object by any user. This is the most recent activity or interaction on an object.</p> <p>The Last Note column is empty if the text of the last note of an object has been deleted. When a new note is entered on the object, it becomes the last note and it displays again in the column.</p>
   <p>When this field is added to a Task report, any updates left on child objects — such as issues, subtasks, documents, etc. — of the task do not display in this column.</p> </td> 
  </tr> 
  <tr> 
   <td>Last Viewed By</td> 
   <td> <p>In a report list, this field displays information about the user who viewed the report last.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>Last Viewed Date</td> 
   <td> <p>In a report list, this field displays the date on which the report was displayed last.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Layout Template</td> 
   <td>Defined by the System Administrator or Group Administrator to identify the tabs and reports that display in a given user's workspace.</td> 
  </tr> 
  <tr> 
   <td>Layout Type</td> 
   <td>In conjunction with Custom Views, the Layout Type specifies the type of Custom View. Currently, only List is available. In the future, Detail (the Detail view of an object) may become available.</td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there&nbsp;are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.&nbsp; 
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.&nbsp;</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;&nbsp;</p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>Library Task</td> 
   <td>A template for a single task that is used to provide consistent naming of Tasks and Template Tasks across the application.</td> 
  </tr> 
  <tr> 
   <td>License Type</td> 
   <td>The type of license allocated to an Access Level. It is either Full User, Limited User, or Requester.</td> 
  </tr> 
  <tr> 
   <td>License Limit Plan</td> 
   <td> <p>In a Group view or report, this field shows the maximum number of Plan licenses that can be assigned to users who have the respective group designated as their Home Group.</p> </td> 
  </tr> 
  <tr> 
   <td>License Limit Work</td> 
   <td> <p>In a Group view or report, this field shows the maximum number of Work licenses that can be assigned to users who have the respective group designated as their Home Group.</p> </td> 
  </tr> 
  <tr> 
   <td>Limited User</td> 
   <td>A License Type that allows creation of an Access Level that contains view-only privileges, with the ability to submit issues, enter notes, and upload documents.</td> 
  </tr> 
  <tr> 
   <td>List Controls</td> 
   <td> <p>A part of Interface Setup that allows linking custom Filters, Views, and Groupings to individual Users or globally to all Users.</p> <p>For more information, see <a href="../../../administration-and-setup/manage-workfront/configure-reports/edit-list-controls-filters-views-groupings.md" class="MCXref xref">Edit list controls: filters, views, and groupings</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Name</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Manual Only</td> 
   <td> <p>One of a Project's Update Types. This setting allows Project Projected and Planned timelines to be updated only when "Recalculated Timelines" is clicked. Projects set up this way will be ignored during the lightly recalculation process and when the Project or Task in the Project are updated.</p> <p>For more information, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Me</td> 
   <td> <p>This refers to the currently logged-in user. </p> <p>We recommend using this field in a filter to make reports more generic when sharing them with other users. This way, you can build only one report which will display different information depending on who logs in to view it, as the information is always customized for the logged-in user. </p> </td> 
  </tr> 
  <tr> 
   <td>Max Users</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>In previous releases of Workfront, you could update this field when creating or editing a job role. It displayed the total number of users that can be associated with a role on each project. A value of zero allowed for an unlimited number of users that can be assigned on a project. </p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Milestone</td> 
   <td> <p>A marker that you can associate with a task to indicate that a key point in the Project has been achieved when the task is completed. You generally can use milestones to show a significant event such as the completion of a phase of the project or a set of critical activities. Milestones are typically associated with parent tasks. You must create the milestones before you can attach them to tasks. For information about milestones, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Create a milestone path</a> and <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Associate milestones with tasks</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Milestone Path</td> 
   <td>A collection of milestones. Milestone Paths are used on Projects to distinguish Projects with certain types of Milestones from Projects with a different set of Milestones.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Milestone Task</td> 
   <td>A task flagged to indicate a reportable event to measure.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Module</td> 
   <td>A single step within a scenario that performs some function based upon the associated app.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>My Primary Role</td> 
   <td> <p>When this is referenced in filters, this displays either users that have the same Primary Role as the logged-in user, or work items assigned to the Primary Role of the logged-in user.</p> <p>We recommend using this field in a filter to make reports more generic when sharing them with other users. This way, you can build only one report which will display different information depending on who logs in to view it, as the information is always customized for the logged-in user. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>My&nbsp;Home Team</td> 
   <td> <p>When this is referenced in filters, this field displays either users that belong to the Home Team of the logged-in user, or work items assigned to the Home Team of the logged-in user. </p> <p>We recommend using this field in a filter to make reports more generic when sharing them with other users. This way, you can build only one report which will display different information depending on who logs in to view it, as the information is always customized for the logged-in user. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Naming convention</td> 
   <td>An organization-wide set of rules that uses data to create names of projects, tasks, and deliverables.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Native Integration</td> 
   <td>An integration that requires no manual coding or API configuration. Also referred to as an "out-of-the-box" integration.</td> 
  </tr> 
  <tr> 
   <td>Navigation Menu</td> 
   <td>The top-center panel of the application that has links to main areas of Workfront.</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>New Number Value</td> 
   <td>In a Journal Entry report, this displays the updated value of a field that replaces the Old Number Value.
   For more information, see "Old Number Value" in this article.</td> 
  </tr>
  <tr> 
   <td>Non Work Day</td> 
   <td>A day that is not allocated to the completion of any assignments. This is usually a vacation day, holiday, or weekend.</td> 
  </tr> 
  <tr> 
   <td>Note</td> 
   <td>A comment or update made on a Workfront object.</td> 
  </tr> 
  <tr> 
   <td>Note Text</td> 
   <td> <p>This displays the text of an update entered by an user on any object.&nbsp;</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Number of Linked Goals</td> 
   <td> <p>In a Project report, this is the number of strategic goals that are associated with the project. For information about associating projects with strategic goals, see <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Overview of connecting projects to goals in Workfront Goals</a>.</p> 
   <p>For information about strategic goals, also see "Goal" in this article.</p> 
   <p>This field is visible only if your organization has purchased Workfront Goals. For information about managing strategic goals using Workfront Goals, see <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Workfront Goals overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Object</td> 
   <td> <p>An organization's work items and reports, as well as the groups of users that manage them in Workfront. Objects can be:</p> 
    <ul> 
     <li>Portfolios</li> 
     <li>Programs</li> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues</li> 
     <li>Documents</li> 
     <li>Dashboards</li> 
     <li>Reports</li> 
     <li>Groups</li> 
     <li>Teams</li> 
     <li>Users</li> 
     <li>Companies</li> 
    </ul> <p>For more information, see <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Object Types</td> 
   <td>If you create a report or list containing all of your custom forms, you can use this field as a view or filter to see which object types are associated with each form. </td> 
  </tr> 
 <tr> 
   <td>Old Number Value</td> 
   <td>In a Journal Entry report, this displays the original value of a field before it was updated. Once a field's value is updated, it will display as the New Number Value in a Journal Entry report. For more information, also see "New Number Value".</td> 
  </tr>
  <tr> 
   <td>On Change Only</td> 
   <td> <p>One of the Project Update Types. When this is selected, the Project Projected and Planned timelines update only when an update or change is made to the Project or to a Task within the Project. It does not update the project every night.</p> <p>For more information, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Op Task</td> 
   <td> <p>The name for Issue in the Workfront database, used in text mode reports or calculated custom data.</p> </td> 
  </tr> 
  <tr> 
   <td>Open</td> 
   <td>An Issue or Task that is not complete, but being worked on.</td> 
  </tr> 
  <tr> 
   <td>Org Chart</td> 
   <td>Short for Organizational Chart. This is a chart showing the hierarchy of an organization. It is also on the Tab on the User detail screen that displays and allows setting the User's Company and Reporting relationships.</td> 
  </tr> 
  <tr> 
   <td>Organizational Setup</td> 
   <td>This defines Companies, Groups, and Security Profiles for your organization.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Other Groups</td> 
   <td> <p>In a report or view that lists users, this field displays all the groups where each user is a member. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Override Currency</span> </td> 
   <td> 
    <div> 
     <p>In a Job Role report, this is the currency associated with a job role. It is an override of the Base Currency as established in the Setup area by the Workfront administrator. </p> 
     <p>For more information, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Override Currency Billing/ Hour</span> </td> 
   <td> 
    <div> 
     <p>In a Job Role report, this is the billing per hour rate of the job role using the selected Override Currency of the job role.</p> 
     <p> For more information, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Override Currency Cost/ Hour</span> </td> 
   <td> 
    <div> 
     <p>In a Job Role report, this is the cost per hour rate of the job role using the selected Override Currency of the job role. </p> 
     <p>For more information, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Owner</td> 
   <td>The user responsible for the completion of the designated object.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Owner Type</span> </td> 
   <td> 
    <div> 
     <p>In a Goal report, this displays the type of owner that is assigned to a strategic goal. The following are the goal owner types:</p> 
     <ul> 
      <li> <p>User</p> </li> 
      <li> <p>Team </p> </li> 
      <li> <p>Group</p> </li> 
     </ul> 
     <p>No value displays in this field when the goal owner is your organization. </p> 
     <p>This requires an additional license. For information about Workfront Goals, see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront Goals overview</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Name</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Parameter</td> 
   <td> <p>A parameter is a custom field. You can build a report for all parameters, or custom fields in your system.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Parent</td> 
   <td>In a report, this field shows information about the parent of the object. For example, in an issue report, it might show information about the task or project that the issue is logged under; in a task report, it might show information about the direct parent task or about the project. For more information about what objects might have parents in Workfront, see the "Interdependency and hierarchy of objects" section in the article <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. </td> 
  </tr> 
  <tr> 
   <td>Parent Lag</td> 
   <td>The amount of time that must pass between the Parent Task start and the Subtask Start.</td> 
  </tr> 
  <tr> 
   <td>Parent Task</td> 
   <td>Also known as a Summary Task. This is a task that has Subtasks (also called Children Tasks). The Duration, Work Required, and Percent Complete of the Parent Task is calculated from the Subtasks.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Part-Time Resources</td> 
   <td>A licensed user who has less capacity than the default schedule defined in the system.</td> 
  </tr> 
  <tr> 
   <td>Percent Complete</td> 
   <td> <p>A project, task, or issue field that shows what percentage of the work associated with the task, project, or issue is completed.</p> <p>You can update this field manually for issues and working tasks. </p> <p>For projects and parent tasks, this field is a roll-up from all the working tasks and you cannot update it manually. </p> <p>For more information, see <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Project Percent Complete overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Permission</td> 
   <td> <p>Rights that are granted to a user on an object, typically given so they can complete work on the item or view the item. You can grant permissions to:</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues</li> 
     <li>Portfolios</li> 
     <li>Programs</li> 
     <li>Reports</li> 
     <li>Dashboards</li> 
     <li>Documents</li> 
     <li>Custom Forms</li> 
     <li>Views</li> 
     <li>Filters</li> 
     <li>Groupings</li> 
    </ul> <p>For more information, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Plan</td> 
   <td> <p>This is a full license type in the Workfront system. Users must have this to access all of the features in Workfront.</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Plan (in the Scenario Planner)</td> 
   <td> <p>A plan is the main object when working with the Workfront Scenario Planner. You can outline the strategy for your company's near and long-term future and identify each high-level outcome and add it as a plan to the Workfront Scenario Planner. </p> <p>You cannot display Scenario Planner plans in a report and you cannot access them through the Workfront API. </p> <p>The Scenario Planner requires an additional license. For information about the Workfront Scenario Planner, see <a href="../../../scenario-planner/scenario-planner-overview.md">The Scenario Planner overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Planned</td> 
   <td> <p>The time frame within which something is scheduled to occur. When you create projects, tasks, or issues in Workfront, you establish the planned start and end dates, as well as the planned timeframe during which they occur. These values represent your original intention or estimate of how long a work time should take to complete. </p></td> 
  </tr> 
  <tr> 
   <td>Planned Benefit</td> 
   <td>This is a manual entry for the Project Manager to estimate whether completing a project would bring any monetary benefit to the organization. Specifying this value can be part of putting together a Business Case for the project. You must have Manage permissions to the project to update this value.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Planned Budgeted Hours</td> 
   <td> <p>In a Budgeted Hour report, this displays the amount of hours budgeted for Projects or Job Roles in the Resource Planner. </p> <p>For information about budgeting Projects or Roles in the Resource Planner, see the article <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. For information about the Budgeted Hours report, see the article <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Planned Completion Date</td> 
   <td> <p>You can manually set the Planned Completion Date to a date of your choosing. If you do not set the Planned Completion Date, Workfront&nbsp;sets it automatically. When set automatically, the Planned Completion Date is:&nbsp;Planned Start Date + Duration</p> <p>For more information, see the following articles:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overview of the task Planned Completion Date</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Set the project Planned Completion Date</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Planned Cost</td> 
   <td> <p>A total of the Planned Labor Cost and the Planned Expense Cost of the project. This does not include the Planned Risk Cost on the project.&nbsp;&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Planned Duration</td> 
   <td> <p>A task's Planned Duration is usually the same as the task's Duration. It represents the difference in days between the Planned Start and the Planned Completion Dates of the task.&nbsp;</p> <p>When the task has a Duration Type of Effort Driven, the Planned Duration can differ from the Duration of the task, based on how many resources you assign to the task.&nbsp;</p> <p>For example, if a task with a Duration Type of Effort Driven has a Duration of 3 days and you assign one resource with a full time schedule to the task, the Planned Duration is 3 days, as well. If you assign three resources with a full time schedule to the same task, the Duration stays 3 days, but the Planned Duration becomes 1 day. The Planned Duration also changes the Planned Start and Planned Completion dates of the task, to reflect the new Planned Duration. As a result, the timeline of the project is affected as well.&nbsp;</p> <p>For more information about the difference between Duration and Planned Duration for tasks, see the article <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Difference between Planned Duration and Duration for tasks</a>.</p> <p>Projects and issues don't have a Planned Duration.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Planned Duration Minutes</td> 
   <td> <p>The Planned Duration Minutes of a project or an issue is the Duration of the project or issue in minutes.&nbsp;</p> <p>Tasks don't have a Planned Duration Minutes field.&nbsp;</p> <p>Template Tasks have a Planned Duration Minutes field which displays the Planned Duration of the task in minutes.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Planned Expense Cost</td> 
   <td> <p>The sum of the Planned Amounts for all expenses logged for a project or a task.</p> <p><b>EXAMPLE</b></p>
   <p>If you create an expense for Task 1 and enter $600.00 in the Planned Amount field, the Planned Expense Cost for this task is $600.00. </p> 
   <p>For a project, Workfront uses the following formula to calculate Planned Expense Cost:</p> <p><code>Project Planned Expense Cost = SUM (All Project Planned Expense Costs) + SUM (All Tasks Planned Expense Costs)</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>Planned Hours</td> 
   <td> <p>This field appears in the projects, tasks, and issues areas, reports for projects, tasks, or issues, and resource management tools like the Resource Planner, Workload Balancer and the Utilization report. </p> <p>It shows the amount of hours that the Project Owner estimates that each task or issue should take to complete. For projects, it is generally a roll-up of the Planned Hours from the tasks on the project. </p> <p>The Planned Hours field might display different information depending on where you view it from. For information about Planned Hours, see <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Planned Hours overview</a>.</p> <p>Planned Hours are stored in minutes in the Workfront database. When writing calculations using this field, ensure you account for the fact that the hours display as minutes.<br></p> <p>By default, Planned Hours are distributed equally to all the days within the duration of a work item and also equally for all resources assigned to the task. Users can update the daily amount of Planned Hours for a work item or the individual Planned Hours for each assignee.</p> <p>Updating this field differs for projects, tasks, and issues: </p> 
    <ul> 
     <li> <p>For issues, you can manually update this field.&nbsp;Issue Planned Hours are not added to the Project Planned Hours.&nbsp;</p> <p>Tip: In an issue report, one of the Planned Hours fields is replaced by the Work field.&nbsp;The field displays the number of Planned Hours on the issue. For more information, see the "work" or "Work" fields in this table. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>For tasks, you can manually update this field when the Duration Type of the task is Calculated Assignment or Simple. This field is calculated by Workfront when the Duration Type of the task is Calculated Work or Effort Driven.<br>For information about Task Duration, see the article <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>For projects, Workfront calculates the Planned Hours by adding all Planned Hours from all the tasks on the project. </p> </li> 
    </ul> <p><b>TIP</b></p> <p>You can display Planned Hours in project, task, or issues reports also by using text mode and reference additional fields. For more information, see the "<code>work</code>", "Work", and "<code>workRequiredExpression</code>" fields in this table. </p> </td> 
  </tr> 
  <tr> 
   <td>Planned Labor Cost</td> 
   <td> 
    <p>For a task, the hourly rate of the user or role multiplied by the number of hours assigned to the user or role.</p> <p>For a project, it is a total of all Planned Labor Costs of all the tasks.</p> <p>Whether the rate of the user or role is used depends on the Cost Type that is selected for the given task. </p> <p>For more information, see <a href="../../../manage-work/projects/project-finances/track-costs.md">Track costs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Planned Revenue</td> 
   <td> <p>Tasks and projects can display a value for Planned Revenue in Workfront. Planned Revenue represents the amount of money associated with the Planned Hours of the tasks on the project. For projects, it can also include the Fixed Revenue of the project. </p> <p>For tasks, this is the revenue associated with the Planned Hours of tasks. The Planned Hours from all tasks roll up to the Planned Hours of the project to contribute to the calculation of the project Planned Hours. </p> 
   <p>Workfront calculates Planned Revenue for tasks and projects using the following formulas:</p> 
   <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code> </p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) + Fixed Revenue</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>The project Planned Revenue that displays in the Project Details area and in project reports differs from the Planned Revenue that displays in the Utilization report. </p> <p>The Planned Revenue in the Project Details area reflects the task revenue as well as the Fixed Revenue of the project. The Planned Revenue in the Utilization Report displays Planned Revenue associated only with the tasks in the project. </p> 
     <p><b>EXAMPLE</b></p>  
      <p>If the project has 1 task with 10 hours, assigned to a Consultant with $20 hourly rate, and the project has $100 Fixed Revenue, the Utilization report displays $200 for Planned Revenue (the Planned Revenue associated with the hours on the task). The Project&nbsp;Details section displays $300 (the Planned Revenue from the task and the Fixed Revenue for the project.) </p> 
    <p>For information about tracking revenue in Workfront see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Overview of Billing and Revenue</a>. </p> 
    <p>For information about Planned Revenue calculations in the Utilization report, see <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">View resource utilization information </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>Planned Risk Cost</td> 
   <td> <p>The total of the Potential Cost of all the risks on the project factoring in their Probability of occurring. This amount is not included in the Planned Cost of the project.</p> <p>The Planned Risk Cost of a project is calculated by the following formula:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Portal Profile</td> 
   <td>An administrator-defined collection of Tabs and Portal Sections that appears on the Workfront Application Home and other Dashboards.</td> 
  </tr> 
  <tr> 
   <td>Portal Section</td> 
   <td>One component of a Tab on a Dashboard or Portal Page. Usually a single Report, Chart, Calendar, or list of key information.</td> 
  </tr> 
  <tr> 
   <td>Portal Tab</td> 
   <td>A Tab on a Portal or Dashboard that contains up to three Portal Sections.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Portfolio</td> 
   <td> <p>A collection of projects that have unifying characteristics. Those projects usually compete for the same resources, budget, or time slot. You can divide Portfolios into Programs and associate the projects with the Programs before they are added to a Portfolio.</p> <p>For more information about portfolios, see <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Portfolio overview in Adobe Workfront</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Portfolio Management</td> 
   <td>A practice area focused on managing a collection or related programs and project efforts.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Portfolio Optimizer</td> 
   <td>A Workfront tool to assist in assessing and prioritizing projects within a portfolio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Portfolio Owner</td> 
   <td>The stakeholder responsible for the prioritization and budget for a portfolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Potential Risk Cost</td> 
   <td>This is a project field that you can locate in lists and reports. It shows the potential cost for the risks associated with the project, should they occur. For more information see <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calculate Potential Risk Cost </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Predecessor</td> 
   <td> <p>A Task that must be complete prior to the completion of a Dependent Task. Also a Task that is marked as a Dependency for another Task. Predecessors allow the planner to set sequence-dependency logic, such as to start a task after another task finishes.</p> <p>For More information, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Primary Company</td> 
   <td>The Company that the user belongs to as designated in their user settings. Companies can also be associated with Projects.</td> 
  </tr> 
  <tr> 
   <td>Primary Contact</td> 
   <td><p>The Primary Contact is the creator of an issue and it is automatically designated by Workfront when the someone creates the issue. You can manually update this field if you have Manage permissions to the issue. An issue can have only one Primary Contact.</p> 
   <p>If you change the Primary Contact, the user originally designated as the primary contact still has Manage access to the issue.</p>
   <p>When converting an issue to a task or a project, the user designated as the Primary Contact of the becomes the Converted Issue Originator of the project or task. If the Primary Contact of the issue is updated after the issue was converted, the Converted Issue Originator will be preserved as the Primary Contact of the issue at the moment when the conversion happened. See also "Converted Issue Originator" in this article.</p> 
   </td> 
  </tr>
  <tr> 
   <td>Priority</td> 
   <td>A value that can be assigned to a Task, Issue or Project to designate how important it is. </td> 
  </tr> 
  <tr> 
   <td>Private</td> 
   <td>On a Note or Document, this option makes that object hidden to most viewers. For a Private Help Desk Queue, only Users on the Queue Team can submit issues to that Queue through the Help Desk Area.</td> 
  </tr> 
  <tr> 
   <td>Profile</td> 
   <td>All information about a user account.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Program</td> 
   <td> <p>A subset within a portfolio, where similar projects can be grouped together in order to achieve a well-defined benefit.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Program Management</td> 
   <td>Management of cross-project dependencies, risks, issues, requirements, and solutions to keep the program healthy and achieve the defined program benefit.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Program Owner</td> 
   <td>The stakeholder responsible for supervising and organizing activities to ensure that project goals align with the company objectives.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Progress</span> </td> 
   <td> <p>In a Goal report, this displays the percent of how close a strategic goal is to completing. The percent of progress displays as a number. For information about strategic goals, also see "Goal" in this table.</p> <p>This field is visible only if your organization has purchased Workfront Goals. For information about managing strategic goals using Workfront Goals, see <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Workfront Goals overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Progress Status</td> 
   <td> <p>In a Project, Task, and Goal report, this field displays the Progress Status of projects, tasks, or strategic goals. For more information, see the following articles:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Project Progress Status overview</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Task Progress Status overview</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Calculate Goal Progress in Workfront Goals</a> </p>
     <p>The Goal report and the Progress Status for goals field are visible only if your organization has purchased Workfront Goals. For information about strategic goals in Workfront Goals, see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">Workfront Goals overview</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>Project</td> 
   <td> <p>A large amount of work that must be completed within a specific timeframe and must use a specific budget and number of resources. To make it manageable, you divide the project into a series of tasks. Completing all the tasks results in the completion of the project. For information about planning a project, see <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Plan a project overview</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>Project Assignment Planned Hours</td> 
   <td> <p>In an Initiative Job Role report, this displays the number of Planned Hours associated with a job role assigned to tasks or issues in the project. This field and the Initiative Job Role report type do not display in your Workfront instance unless your company has purchased a Workfront Scenario Planner license. For information about the Workfront Scenario Planner, see <a href="../../../scenario-planner/scenario-planner-overview.md">The Workfront Scenario Planner overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Project Details</td> 
   <td>The details of the current status of a Project.</td> 
  </tr> 
  <tr> 
   <td>Project Budgeted Cost</td> 
   <td> <p> This is the Budgeted Cost of a project as it displays in lists and reports.</p><p>See also "Budgeted Cost" in this article.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Project Management</td> 
   <td>A set of policies that governs the thresholds for project creation, categorization, and naming of the projects.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Project Overhead</td> 
   <td>In an Hour report, this field is reserved for financial information tied to the hours logged with the hour type of Project Time. Projects can have their own Billing Rates and if an hour is logged directly on a project, then those rates will be used in calculations. Based on the project settings, projects can also have different currencies and there can be a currency conversion for those hours. The Project Overhead object allows Workfront to get that information.</td> 
  </tr> 
  <tr> 
   <td>Project Owner</td> 
   <td>The user responsible for managing the scope, timeline, and assignments of a project. The default approver for change orders, financial changes, and deliverables.</td> 
  </tr> 
  <tr> 
   <td>Project Planning</td> 
   <td>Processes to develop and maintain the project schedule.</td> 
  </tr> 
  <tr> 
   <td>Project Sponsor</td> 
   <td>A designated stakeholder profile that each of your user's should relate to. In Workfront, these are designated as Access Levels</td> 
  </tr> 
  <tr> 
   <td>Project Teams</td> 
   <td> <p>The collection of Users or Roles assigned to a Project</p> <p>For more information, see <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Project Team overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Project tracking</td> 
   <td>The data used to measure the health and scope of a project</td> 
  </tr> 
  <tr> 
   <td>Projected</td> 
   <td> <p>An estimate of the timestamp of when the work will be completed based on the planned hours and percentage complete of a task, issue, or project.</p> <p>This refers to dates or the Duration of tasks, issues, or projects. Usually, it designates dates and durations that are more true to the life of the work items, after some work has already been completed or some time has passed. </p> <p>For example, the Projected Completion Date of a task is the date when Workfront estimates that the task will complete, based on how much work has been done on it so far, how many people are assigned to it, and how much time has passed since the start date.</p> </td> 
  </tr> 
  <tr> 
   <td>Proof Deadline</td> 
   <td> <p>In reports that contain the Document Version object (such as a Document Version report and Proof Approval report), This field displays the day of the week, date, time of day, and year of the proof deadline.</p> </td> 
  </tr> 
  <tr> 
   <td>Proof Decision</td> 
   <td> <p>In reports that contain the Document Version object (such as a Document Version report&nbsp; and Proof Approval report), this field displays the decision status of the proof (pending, changes required, or approved)</p> </td> 
  </tr> 
  <tr> 
   <td>Proof Name</td> 
   <td> <p>In reports that contain the Document Version object (such as a Document Version report and Proof Approval report), this field displays the proof name.</p> </td> 
  </tr> 
  <tr> 
   <td>Proof Pages</td> 
   <td> <p>In reports that contain the Document Version object (such as a Document Version report and Proof Approval report), this field displays the number of pages included in the proof.</p> </td> 
  </tr> 
  <tr> 
   <td>Proof Progress</td> 
   <td> <p>In reports that contain the Document Version object (such as a Document Version report and Proof Approval report), displays the progress status of the proof (Sent, Opened, Commented, Decision Made).</p> <p>For more information, see <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Proof progress overview</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Proof progress and status overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Proofing</td> 
   <td>A review process where one or more users mark and comment on content that should be changed in an image, a text document, a video, or interactive web content.</td> 
  </tr> 
  <tr> 
   <td>Public</td> 
   <td>On a Note or Document, this option makes that object accessible to other users, or even people from outside Workfront. For a Help Desk Queue, Public means that all users that can submit Issues can submit Issues through the Help Desk Area.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Quality</td> 
   <td>The perception of work quality within the organization.</td> 
  </tr> 
  <tr> 
   <td>Queue</td> 
   <td>Also called Help Desk Queue. This is a Project that has been published to the Help Desk area to allow users to submit Issues to it. Usually Queues are created for particular topics, such as Bugs, Project Requests, etc.</td> 
  </tr> 
  <tr> 
   <td>Queue Properties</td> 
   <td>These settings define Issue submission rules for a Project that is being published to the Help Desk.</td> 
  </tr> 
  <tr> 
   <td>Queue Topic</td> 
   <td> <p>A property on a Help Desk Queue that allows users submitting an Issue to select a Topic. Topics can:</p> 
    <ul> 
     <li>Be associated with a Custom Data Form.</li> 
     <li>Assign the Issue automatically to a User, Role, or Team through the Routing Rule set on the selected Topic.</li> 
     <li>Move the issue to a different Project or Queue through the routing rule set on the selected topic.</li> 
    </ul> <p>For more information, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Create Queue Topics</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Rank</td> 
   <td> <p>In an Access Level report, you can manually indicate a Rank of the Access Level. This helps you, as the Workfront administrator, to visually identify the level of complexity associated with each Access Level. For example, you can give lower numbers for more complex (Plan-level) Access Levels, and higher numbers for less complex (Requester-level) Access Levels. You cannot rank the standard Access Levels.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Ready</td> 
   <td> <p>This field on a task report indicates whether&nbsp;an Agile task has been marked as Ready on the backlog. This flag only applies to Agile tasks, which are tasks assigned to an Agile team.&nbsp;</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Recurrence Frequency</td> 
   <td> <p>A field that displays in the Task Details or the Edit Task box of a parent of recurring tasks. It is the frequency with which the tasks in the recurrence occur. For information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Reference Number</td> 
   <td> <p>Projects, tasks, and issues are automatically associated with a unique reference number as they are created. You can view the Reference Number in the Details page of projects, tasks, or issues, or in a list or report. </p> <p><b>TIP</b><p><br>You can defer to reference numbers when two items have the same name, as reference numbers are always unique. </p> <p>Workfront automatically generates sequential reference number at the system level. Each project, task, or issue gets the next available number in the sequence. <br></p> <p>For example, if User A creates a task, Workfront might automatically assign the task the Reference Number of 100. If User B creates an issue right after this, Workfront assigns the issue the Reference Number of 101. You cannot manually edit Reference Numbers. </p> </td> 
  </tr> 
  <tr> 
   <td>Rejection&nbsp;Issue</td> 
   <td>In a project or a task report, this is the issue that is created when the approval for the project or the task is rejected. For information about rejection issues, see the article <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>. </td> 
  </tr> 
  <tr> 
   <td>Remaining Risk&nbsp;Cost</td> 
   <td> <p>A project field that shows the difference between the Planned Risk&nbsp;Cost of a project and the total of all&nbsp;Actual&nbsp;Costs of all risks on the project. </p> <p>The Remaining Risk&nbsp;Cost for a project is calculated using on the following formula:</p> <p><code>Remaining Risk&nbsp;Cost = Project Planned Risk Cost - SUM(Actual Cost for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Replanning</td> 
   <td>Changing the dates of a Project to repair or overcome problems. For example, a project that has been on hold for several months would need to be replanned to reflect accurate dates.</td> 
  </tr> 
  <tr> 
   <td>Report</td> 
   <td>A chart or table containing information about one given Workfront object and its related attributes.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Request</td> 
   <td> <p>A type of issue that is triaged in a single centralized queue and is unrelated to an ongoing work effort.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Request Queue</td> 
   <td>The backlog of issues that is managed by a traffic and triage process.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Request velocity</td> 
   <td>Total work cycle time to intake and complete a request.</td> 
  </tr> 
  <tr> 
   <td>Requester</td> 
   <td>Typically a license type. A user with a Requester license can submit requests for new work to occur in the system.</td> 
  </tr> 
  <tr> 
   <td>Reserved Time</td> 
   <td>Days specified on a User's Personal Time, indicating that the User will not be available for work. See "Non Work Days".</td> 
  </tr> 
  <tr> 
   <td>Resolve Issue</td> 
   <td> <p>In an issue report, use this field in views or filters to refer to the issue that resolves the issue. </p> <p>For information about displaying resolving objects in reports, see <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">View Resolvable and Resolving Object information in a report</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Resolve Project</td> 
   <td> <p>In an issue report, use this field in views or filters to refer to the project that resolves the issue. </p> <p>For information about displaying resolving objects in reports, see <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">View Resolvable and Resolving Object information in a report</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Resolve Task</td> 
   <td> <p>In an issue report, use this field in views or filters to refer to the task that resolves the issue. </p> <p>For information about displaying resolving objects in reports, see <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">View Resolvable and Resolving Object information in a report</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Resource</td> 
   <td>User(s) and/or Role(s) existing in the system and assigned to Project Teams and Tasks.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>Resource Management</td> 
   <td> <p>Resource Management is an enterprise set of tool that allows you to accurately forecast the use of your resources based on their availability so that the work that must be done is completed on time and on budget.&nbsp;</p> <p>With Resource Management tools you can plan long term capacity and short term scheduling needs for your resources. </p> <p>For information about Resource Management in Workfront, see <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Get started with Resource Management</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Resource Manager IDs</td> 
   <td><p>In a project report, you can use this option when creating a filter to find a specific resource manager. </p></td> 
  </tr> 
  <tr> 
   <td>Resource Managers</td> 
   <td> <p>In a project report or list view, this is an informational field that displays users designated to perform resource management activities on the project.  When you use "Resource Managers" in a report, a list of resource managers is displayed, with each resource manager on the project separated by a comma. You can designate up to 30 resource managers on a given project.</p> <p>For more information, see the article <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Designate Resource Managers for a project or template </a>.</p> </td> 
  </tr>
  <tr> 
   <td>Resource Planner Budgeted Hours </td> 
   <td>The hours budgeted for the project and the resources associated with it in the Resource Planner. See also "Budgeted Hours" in this article. </td> 
  </tr>  
  <tr> 
   <td>Resource Planner </td> 
   <td>An advanced Workfront tool that lets you view and manage resources across projects, job roles, or users. For information, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
  </tr> 
  <tr> 
   <td>Resource Planner Budgeted Labor Cost</td> 
   <td> <p>These are the cost associated with the hours budgeted for project job roles using the Resource Planner. </p> <p>See also "Budgeted Labor Cost" in this article. </p> </td> 

  </tr> 
  <tr> 
   <td>Resource Pools</td> 
   <td> <p>Resource Pools are collections of users that can be associated with a project.The users in the same Resource Pool usually belong to the same department, have similar or complementary skills, or are funded by the same budget. You can associate multiple Resource Pools to a project or to a user. A resource pool can be assigned exclusively to a project or shared by several projects.</p> 
   <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> 
   <p>In project reports, Resource Pools show all the pools associated with a project. This object cannot be used in a grouping.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>Resource Utilization</td> 
   <td>A Report displaying the number of hours available during a certain time period and the number of hours scheduled for each user in the report. This is also calculated into Average Hours Per Day and an allocation percentage.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Result</td> 
   <td>In Workfront Goals, a result is a progress indicator for a goal. It can be a number, a percentage value, or a currency amount that you update manually. You cannot display results in a report and you cannot access them through the Workfront API. For information about activities, see <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Get started with results and activities in Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Revenue</td> 
   <td>A billable amount for the task or project. The amount can be hourly, fixed, or a combination of both.</td> 
  </tr> 
  <tr> 
   <td>Revenue Type</td> 
   <td>Revenue type determines how the task will accrue revenue. Some examples include Fixed Hourly, Role Hourly, and Role Hourly w/Cap. For information about tracking revenue in&nbsp;Workfront see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</td> 
  </tr> 
  <tr> 
   <td>Reviewer</td> 
   <td>Typically a license type. A User with a Reviewer license has the ability to review and approve work items in the system.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Risk</td> 
   <td> <p>This may refer to the following concepts in&nbsp;Workfront:</p> 
    <ul> 
     <li> <p>A field on a project that indicates how risky a project can be. You can prioritize the execution of your projects based on the level of risk. Projects can have the following levels of risk:</p> <p>- Very Low</p> <p>- Low</p> <p>- Medium</p> <p>- High</p> <p>- Very High</p> <p>The levels of risks you indicate for a project cannot be customized. </p> <p> For information about updating the Risk of a project, see the " Project  Settings" section of the article <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>. You can display the risk field of a project in reports. </p> </li> 
     <li> <p>An event that might occur during the life of a project that identifies a potential impact to the cost, scope, or schedule of the project. You define potential risks to a project and associate a probability of them occurring or a cost as you build the project's Business Case. For information about adding risks to the Business Case of the project, see "Create and edit risks on projects". </p> <p>You cannot display risks defined in the Business Case in reports. You can only display several types of Risk Costs in reports and lists. </p> </li> 
    </ul> </td> 

  </tr> 
  <tr data-mc-conditions=""> 
   <td>Risk Cost</td> 
   <td> <p>The cost associated with the risks on a project. The following are risk costs associated with projects that you can display in reports:</p> 
    <ul> 
     <li> <p>Actual Cost: a field on a risk that shows the actual cost for the risk that has occurred. In addition to reports and lists, you can locate it in the Edit Risk box when editing or creating a risk. </p> <p>For project, task, or issue costs, see "Actual Cost" in this article. </p> </li> 
     <li> <p>Planned Risk Cost: a field on the project that shows a total of all Potential Risk Costs for the project. See also "Planned Risk Cost" in this article. </p> <p>For information about Potential Risk Cost, see <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calculate Potential Risk Cost </a>. </p> </li> 
     <li> <p>Remaining Risk Cost: a field on the project that displays the difference between the total of the Actual Costs of all risks and the Planned Risk Cost. See also "Remaining Risk Cost" in this article. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Risk Management</td> 
   <td>Processes to identify, mitigate, and monitor risk.</td> 
  </tr> 
  <tr> 
   <td>Role</td> 
   <td>See "Job Role" in this article.</td> 
  </tr> 
  <tr> 
   <td>Routing</td> 
   <td>Automatically assigning or moving an Issue, usually due to a Queue Topic or by way of being the Default Route (Routing RUle) for the Queue.</td> 
  </tr> 
  <tr> 
   <td>Routing Rule</td> 
   <td>A setting on Projects and Queues that automatically assigns an Issue to a User, Role, or Team, or moved the Issue to another Project or Queue. Routing Rules are generally used with Help Desk Queues to automatically assign incoming Issues.</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Name</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Saved Search</td> 
   <td>A search for which the search criteria have been saved. Saved Searches make it easy to run the same each again without having to enter the search criteria again.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>Scenario (in&nbsp;Workfront Fusion) </td> 
   <td> <p>A scenario is comprised of a series of steps (modules) that indicate how data should be transferred and transformed between apps/ services.</p> <p>For information about scenarios in Workfront Fusion, see <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">Adobe Workfront Fusion scenario overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Scenario (in the Workfront Scenario Planner) </td> 
   <td> <p>In the Scenario Planner, a scenario is a copy of a plan. </p> <p>The Scenario Planner requires an additional license. For information about the Workfront Scenario Planner, see <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The Scenario Planner overview</a>. </p> <p>For information about creating scenarios, see <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Create and compare plan scenarios in the Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Schedule</td> 
   <td>The weekly work schedule, including working times, combined with Days off (such as Holidays) and exception days (such as a Saturday work day). Schedules can be applied to Projects and Users.</td> 
  </tr> 
  <tr> 
   <td>Schedule Exemption</td> 
   <td>Also knows as a Modified Shift. Days scheduled in contrast to the regular weekly work times as defined by the schedule. For example, a Saturday scheduled to work, when the Schedule is set up to only Work Monday Through Friday, would be a Schedule Exemption.</td> 
  </tr> 
  <tr> 
   <td>Scheduled Report</td> 
   <td> <p>When you build a report of reports, you can display information about the schedules of the report, if the report is scheduled for delivery using the Scheduled Report field. This field shows multiple values, one for each schedule of each report, in a bulleted list. For more information about scheduling reports, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Report delivery overview</a>.</p> <p>Because this field shows multiple values, it cannot be used in a grouping. You can access it only in a filter or a view.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Scope Change</td> 
   <td>An Audit Trail that, if active, generates a note any time a change is made to the Scope of a Project or Task, such as if a Task Duration or Predecessors are changed.</td> 
  </tr> 
  <tr> 
   <td>Section</td> 
   <td>An area on the screen, with its own header, created to organize the Custom Data for display purposes.</td> 
  </tr> 
  <tr> 
   <td>Section Break</td> 
   <td>A gap or border between sections.</td> 
  </tr> 
  <tr> 
   <td>Security</td> 
   <td>The settings that allow a User to interact with certain objects in the system and not others. See also "Access Levels" in this article.</td> 
  </tr> 
  <tr> 
   <td>Setup</td> 
   <td>The area where administrators can set up system configurations and preferences.</td> 
  </tr> 
  <tr> 
   <td>Severity</td> 
   <td> <p>Severity is an indication of how likely an item is to impact the completion of the work. For example, an Issue with high Severity may completely block a Task's completion, but an Issue with low Severity may be merely cosmetic.</p> <p>For more information, see <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Update issue severity</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Severities</td> 
   <td>See "Severity" in this article.</td> 
  </tr> 
  <tr> 
   <td>Sharing</td> 
   <td>The action of allowing other Users to view or edit a specific item in Workfront.</td> 
  </tr> 
  <tr> 
   <td>Slack&nbsp;Date</td> 
   <td>In a task view or report, the Slack Date displays the exact date when a task could definitely impact the Completion Date of the project. For information about the Slack Date of a task, see <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Task Slack Date overview</a>.</td> 
  </tr> 
  <tr> 
   <td>Smart Assignments</td> 
   <td> <p>When assigning Tasks or Issues to Users, Workfront makes recommendations (Smart Assignments) about who the best users are to complete the work, based on the time they have available to complete it and their relationship to the project.</p> <p>For more information , see <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Smart assignments overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Source</td> 
   <td> <p>Indicates the parent object of another object. For example, a document attached to a task has the name of the task in the Source field of a Document report or view; an issue logged under a project has the name of the project in the Source field of an Issue report or view.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Start Date</td> 
   <td> <p>The Date when the work on an item is set to start. There are several Start Dates in Workfront: </p> 
    <ul> 
     <li>Planned</li> 
     <li>Actual</li> 
     <li>Projected </li> 
    </ul> <p>In a Rate report, this is the date when a new billing rate for a job role at the project level starts. The hours associated with the project that are after this date are multiplied by this billing rate to calculate the revenue on the project. </p> </td> 
  </tr> 
  <tr> 
   <td>Status</td> 
   <td> <p>An indicator used to signal a workflow position of a work item or of a strategic goal.</p> <p>For Projects, the Status is a setting on the Project that indicates whether the Project is:</p> 
    <ul> 
     <li>Current</li> 
     <li>On Hold </li> 
     <li>Complete </li> 
     <li>Dead</li> 
    </ul> <p>For more information on Project Status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Access the list of system project statuses</a>.</p>
    <p>For Tasks, the Status is a setting on the Task that indicates whether the Task is:</p> 
    <ul> 
     <li>New</li> 
     <li>In Progress</li> 
     <li>Complete</li> 
    </ul> <p>For more information on Task Status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Access the list of system task statuses</a></p> <p>For Issues, the Status is a setting on the Issue that indicates whether this Issue is:</p> 
    <ul> 
     <li>New</li> 
     <li>In Progress</li> 
     <li>Awaiting Feedback</li> 
     <li>On Hold</li> 
     <li>Resolved</li> 
     <li>Won't Resolve</li> 
     <li>Cannot Duplicate</li> 
     <li>Verified Complete</li> 
     <li>Reopened</li> 
    </ul> <p>For more information on Issue Statuses, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Access the list of system issue statuses</a>.</p> 
    <p>For strategic goals, the Status is a setting on the goal that indicates whether the goal is:</p> 
     <ul> 
      <li>Active</li> 
      <li>Draft</li> 
      <li>Inactive</li> 
      <li>Closed</li> 
     </ul> 
     <p>For more information about strategic goals, also see "Goal" or "Goals" in this article. </p> 
     <p>For strategic goals, this field is visible only if your organization has purchased Workfront Goals. For information about managing strategic goals using Workfront Goals, see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">Workfront Goals overview</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>Status Change</td> 
   <td>An Audit Trail. A note is generated when a User changes the Status of the Project, Task, or Issue.</td> 
  </tr> 
  <tr> 
   <td>Status Icons</td> 
   <td> <p>You can add the built-in Status Icons field as a column in your views to enhance visibility into key points about your objects, like:</p> 
    <ul> 
     <li>An object has documents attached</li> 
     <li>An object is associated with an approval process</li> 
     <li>An object has additional notes associated with it</li> 
     <li>An expense is billable or reimbursable&nbsp;</li> 
     <li>A task is on a critical path</li> 
     <li>A user belongs to a company, a team, or is located in a different time zone&nbsp;</li> 
    </ul> <p>You can add the Status Icons field in the views of the following objects:&nbsp;</p> 
    <ul> 
     <li>Tasks</li> 
     <li>Issues</li> 
     <li>Projects</li> 
     <li>Template Tasks</li> 
     <li>Templates</li> 
     <li>Expenses</li> 
     <li>Documents</li> 
     <li>Users</li> 
    </ul> <p>For more information, see <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Built-in Status Icons in Views</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Status Update</td> 
   <td> <p>This field shows the most recent status update&nbsp;that users have provided in the 'Update Status' field.&nbsp;Comments made on&nbsp;status&nbsp;updates are not displayed in the Status Update column.</p> <p>To show the 'New,' 'In Process,' and 'Complete' statuses, use the Status column.</p> <p>Comments made on&nbsp;status&nbsp;updates are not displayed in the Status Update column.</p> <p>For more information on statuses, see the article <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Update task status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Statuses</td> 
   <td>See "Status" in this article.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>Storyboard</td> 
   <td>A chart that represents the status of stories (tasks in the agile methodology) and how they are progressing toward completion.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>Story Hours</td> 
   <td>A metric used to measure the difficulty or complexity of a Story. Agile teams can choose whether to use Hours or Points.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>Story Points</td> 
   <td>A metric used to measure the difficulty or complexity of a Story. Agile teams can choose whether to use Hours or Points.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Strategic</td> 
   <td>Long-term work that changes the organization or how the organization works.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>Strategic Alignment</td> 
   <td>Measuring and aligning company goals across portfolios and programs.</td> 
  </tr> 
  <tr> 
   <td>Subscribers</td> 
   <td> <p>Users that subscribe to Projects, Tasks, or Issues.</p> <p>When you use this field in a report, a list of subscribers displays, with each subscriber separated by a comma.</p> <p>For more information, see the article <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Subscribe to items in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Summary Task</td> 
   <td>See "Parent Task" in this article.</td> 
  </tr> 
  <tr> 
   <td>Subtask</td> 
   <td>A child task, which is located under a parent task.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>System Governance</td> 
   <td>A set of policies that governs changes and maintenance of a system.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>System Integration</td> 
   <td>The process of linking together different computing systems and software applications physically or functionally in order to act as a coordinated whole.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Task</td> 
   <td> <p>An activity that must be performed as a step toward achieving a final goal (completing the Project).</p> <p>For more information, see <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Tasks overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Task Attribute</td> 
   <td>Other fields or objects that are associated with a Task and indicate certain details about the Task. Some examples are Planned Completion Date and Status.</td> 
  </tr> 
  <tr> 
   <td>Task Constraint</td> 
   <td>See "Constraint Type" and "Constraint Date".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Task Management</td> 
   <td>A set of policies that governs the thresholds for task creation, assignment, closure, and visibility.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Task Owner</td> 
   <td>The team or user responsible for the estimation of effort and completion of the task</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Team</td> 
   <td> <p>A collection of users working toward similar goals or business objectives. These users can be collectively assigned to a work item by assigning the team to the work item.</p> <p>For more information on Teams, see <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Teams overview</a>.</p> <p>Projects can have a Project Team, which contains all the users or roles associated with the work on the project.</p> <p>For more information about Project Teams, see <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Project Team overview</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>Template</td> 
   <td> <p>Project templates are generic outlines of your most repeatable projects. You can define tasks, queue topics, custom forms, attach documents or approvals when you create a project template to save you time when you must create a new project. </p> <p>You can attach templates to existing projects, or you can use them to build new projects. All the information specified on the template transfers to the projects that are created using it. </p> <p>For more information about templates, see <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Project template overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Template Task</td> 
   <td>A Task that is part of a Template. Template Tasks become Tasks in the Project that is created by using the Template.</td> 
  </tr> 
  <tr> 
   <td>Thread</td> 
   <td>A Note and its collection of replies that relate to a particular topic.</td> 
  </tr> 
  <tr> 
   <td>Thumbnail</td> 
   <td> <p> In a Document list or report, it displays a preview of the document in a thumbnail. </p> <p> Select <strong>Thumbnail</strong> &nbsp;to view a 33-66 pixel-wide thumbnail in the report. </p> <p>The size of the thumbnail adjusts when you modify the width of the column in a list or report.</p> <p>See also "Large Thumbnail" in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Time Off</td> 
   <td>You can build a Time Off report to view when users have indicated time off in their profile. </td> 
  </tr> 
  <tr> 
   <td>Timesheet</td> 
   <td> <p>A timecard that allows users to enter actual hours that they spent working on projects, tasks, or issues, or hours they spent for other activities not related to work, like meetings or training. In addition to entering the amount of time you spent working, you can also indicate whether the time is work-related or it amounts to overhead time by using Hour Types to define your time entries. For information about timesheets, see <a href="../../../timesheets/timesheets/timesheets-overview.md">Timesheets overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet Profile</td> 
   <td> <p>A Timesheet Profile is a template that Workfront uses to automatically create timesheets for the users associated with them. </p> <p>You can configure a number of settings that will apply to each timesheet as it is created. Some of these settings are: how often the timesheet should be created (weekly, every other week, twice a month, or monthly), the start day of the timesheet, the timesheet approvers, the available Hour Types that users can associate with recorded hours.</p> </td> 
  </tr> 
  <tr > 
   <td>Top Parent ID </td> 
   <td> <p>This field allows you to identify and filter data about a top-level group and its subgroups in a list or report.</p> </td> 
  </tr> 
  <tr> 
   <td>Top Parent Name </td> 
   <td> <p>This field allows you to identify data about a top-level group and its subgroups in a View for a list or report.</p> <p>You can also do this using the Top Parent ID field.</p> </td> 
  </tr> 
  <tr> 
   <td>Total Hours</td> 
   <td> <p>In a project report, this field displays the rounded sum of all hours on the project, the last time the project finances were calculated. Actual Hours reflect the exact hours logged on the project. Typically, the Actual Hours should match the Total Hours. If the Total Hours appears significantly different than the Actual Hours field, you must Recalculate Finances on the project.</p> <p>For more information about recalculating project finances, see the article <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Recalculate project finances</a>.</p> <p>In a timesheet Standard view, this field refers to the total hours logged for items for the dates displayed on a timesheet. The Total Hours field for timesheets in this built-in view references the "hoursDuration" field which dynamically calculates the difference in hours between the timesheet Start and End dates. This is used to display the Total Hours column in red if the user logs more time than the available hours in the timesheet's time frame. For more information, see <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">View total hours on the timesheet</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Tracking Mode</td> 
   <td> <p>An attribute of a Task. This determined how and then the Projected timelines will be updated for a Task. For example:</p> 
    <ul> 
     <li>User Must Update requires that a Task be updated manually. Otherwise, it will become Behind Schedule, then Late.</li> 
     <li>Auto Complete will automatically complete a Task when the Due Date, or Planned Completion Date, has passed.</li> 
    </ul> <p>For more information, see <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Task Tracking Mode overview</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>Trigger</td> 
   <td>An event that starts a scenario.</td> 
  </tr> 
  <tr> 
   <td>Trouble Task</td> 
   <td>An incomplete Task with a condition of Late, Behind Schedule, or At Risk.</td> 
  </tr> 
  <tr> 
   <td>Unassigned Task</td> 
   <td>A Task that is not assigned to any User, Role, or Team.</td> 
  </tr> 
  <tr> 
   <td>Update Type</td> 
   <td> <p>A setting on the Project that determines when the Project's Projected timeline will be recalculated. Options are:</p> 
    <ul> 
     <li>Automatic and On Change</li> 
     <li>Automatic Only</li> 
     <li>Manual Only </li> 
    </ul> <p>For more information, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User</td> 
   <td>An account created in Workfront to allow a person to log in and interact with the system.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>User Delegation</p> </td> 
   <td> <p>A reportable object that tells you:</p> 
    <ul> 
     <li>Which users have delegated task, issue, and project approvals</li> 
     <li>Which users have had task, issue, and project approvals delegated to them</li> 
     <li>When these delegations start and end</li> 
    </ul> <p>To learn more, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Create a User Delegation report</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User Interface</td> 
   <td>All visual and interactive aspects of the Workfront application.</td> 
  </tr> 
  <tr> 
   <td>User Interface Preferences</td> 
   <td>User Interface Setup. Workfront administrators can change these settings to customize aspects of the user interface.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Utilization</td> 
   <td>The availability for a user or role based on the assigned schedule, PTO, and current workload.</td> 
  </tr> 
  <tr> 
   <td>User Utilization</td> 
   <td> <p>A search combined with a report that shows how Users (Resources) are allocated or over-allocated. See "Resource Utilization" in this article.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Object Name</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Velocity</td> 
   <td>A measure of the total work cycle time (how long it takes to complete a piece of work) and how frequently work is done in the time originally committed (work-to-commit ratio).</td> 
   </tr> 
  <tr> 
   <td>View</td> 
   <td> <p>Views can be used to modify the columns in a Report or in a list of projects, tasks, or issues, or they can be used to indicate a user's right to only view information on an access level or at a permissions sharing level.</p> </td> 
  </tr> 
  <tr> 
   <td>View Icons</td> 
   <td> <p> This is the same field as Status Icons, but it is only available for the following views: </p> 
    <ul> 
     <li> Documents </li> 
    </ul> <p> For more information, see the article <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Built-in Status Icons in Views</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Views Last Month</td> 
   <td> <p>In a report list, it displays the number of times the report has been viewed during the last month.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Views Last Quarter</td> 
   <td>In a report list, it displays the number of times the report has been viewed during the last quarter.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >View report usage</a>.</td> 
  </tr> 
  <tr> 
   <td>Views Last Year</td> 
   <td>In a report list, it displays the number of times the report has been viewed during the last year.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.</td> 
  </tr> 
  <tr> 
   <td>Views This Month</td> 
   <td> <p>In a report list, it displays the number of times the report has been viewed during this month.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Views This Quarter</td> 
   <td>In a report list, it displays the number of times the report has been viewed during this quarter.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.</td> 
  </tr> 
  <tr> 
   <td>Views This Year</td> 
   <td>In a report list, it displays the number of times the report has been viewed during this year.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">View report usage</a>.</td> 
  </tr> 
  <tr> 
   <td><code>work</code> </td> 
   <td> <p>In a project, task, or issue report, using the following statement in text mode displays the Planned Hours of the project, task, or issue:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>For information about using text mode, see <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Text mode syntax overview</a>. </p> 
   <p><b>TIP</b> 
   <p>In an issue report, adding one of the Planned Hours fields adds the <code>work </code>field to the report. </p> </td> 
  </tr> 
  <tr> 
   <td>Work</td> 
   <td> <p>One of the two primary License Types. This has less access than Plan, but can create and make updates in the system. This mas more abilities than External, Reviewer, or Requester License Types.</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> <p>Work might refer to the number of Planned Hours for a project, task, or issue.&nbsp;For more information, see the "work" field in this table. </p> <p>Tip: In an issue report, adding one of the Planned Hours fields adds the <code>work </code>field to the report. </p> </td> 
  </tr> 
  <tr> 
   <td>Work Breakdown Structure</td> 
   <td>A hierarchical structure of the tasks to be executed by the project team based on the parent/ child relationship.</td> 
   </tr> 
  <tr> 
   <td>Work Effort </td> 
   <td> 
    <p>A project manager might decide to use this field instead of Planned Hours to estimate the effort needed to complete a task. This field is visible only when the following conditions are met:</p> 
     <ul> 
      <li> <p>The task has a Simple Duration&nbsp;Type. </p> <p>Tip: If you update the task Duration&nbsp;Type to any other type, this field becomes hidden. </p> </li> 
      <li>The project manager has enabled the Use Work Effort to automatically calculate task Planned Hours field on the project. </li> 
     </ul> 
     <p>For information about using Work Effort instead of Planned Hours to estimate task effort, see <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort overview</a>. </p> 
     <p>You can display this field in task reports and lists.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>Work Item</td> 
   <td> <p>This field refers to either tasks or issues in Workfront. </p> <p>The Work Item report displays information for both tasks and issues. </p> </td> 
  </tr> 
  <tr> 
   <td>Work management mix</td> 
   <td>A Work Performance Indicator(WPI) of the proportion of work allocated to run your business versus change your business. The Mix WPI helps you understand, at an organizational level, whether your strategy has any real work allocation applied to it.</td> 
  </tr> 
  <tr> 
   <td>Work Management Resource</td> 
   <td>A designation of a persona in the system who is eligible to receive work or track time.</td> 
  </tr> 
  <tr> 
   <td>Work Management Role and Responsibilities</td> 
   <td>Defining the owners and stakeholders for managing the scope, execution, and approvals of the designated issue, task, project, program, or portfolio.</td> 
  </tr> 
  <tr> 
   <td>Work management SLA</td> 
   <td>A quantifiable metric agreed upon by all stakeholders.</td> 
  </tr> 
  <tr> 
   <td>Work Management Stakeholder</td> 
   <td>A collection of users with a vested interest in the outcomes of a work request.</td> 
  </tr> 
  <tr> 
   <td>Work management touchpoints</td> 
   <td>Digitized records of communication between stakeholders.</td> 
  </tr> 
  <tr> 
   <td>Work Performance Indicators </td> 
   <td> <p>Mix ratio, capacity, velocity, quality, and engagement.</p> <p>WPI is a common acronym for Work Performance Indicator.</p> </td> 
  </tr> 
  <tr> 
   <td>Work Process</td> 
   <td> <p>The method in which work is received, prioritized, and executed. The way you execute the work is typically called "the workflow" or "project plan" (a list of tasks with dates, predecessor relationships, and so forth). </p> <p>Examples of a work process might be the production of a single asset or the delivery of a multi-asset campaign. </p> </td> 
  </tr> 
  <tr> 
   <td>Workflow template</td> 
   <td>In the Proof Approval report, this field displays any workflow templates attached to a proof. If there are no templates attached, the column is blank.</td> 
  </tr> 
  <tr> 
   <td>Working time</td> 
   <td>The data that makes up your schedules.</td> 
  </tr> 
  <tr> 
   <td><code>workRequiredExpression</code> </td> 
   <td> <p>In a project, task, or issue report, using the following statement in text mode displays the number of Planned Hours of the project, task, or issue followed by the word "Hours":</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>For information about using text mode, see <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Text mode syntax overview</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
