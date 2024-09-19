---
content-type: reference
navigation-topic: workfront-navigation
title: Glossary of [!DNL Adobe Workfront] terminology
description: The [!DNL Adobe Workfront] glossary lists commonly-used terms in [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] interface, reports, or you try to understand the meaning of [!DNL Workfront] concepts defined in the [!DNL Workfront] documentation.
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
---

# Glossary of [!DNL Adobe Workfront] terminology

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>This article should be used as a reference to understand the terms that you may encounter in the [!DNL Adobe Workfront] application, in the [!DNL Workfront] documentation, or when generally speaking about planning and managing work. We are currently updating this information and as a result this table might not be complete. We will remove this disclaimer when we consider this information exhaustive.

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
   <td>[!UICONTROL Access Level]</td> 
   <td>A user profile that determines how a user can interact with different objects and tools within Workfront.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Active Task]</td> 
   <td>An incomplete task in a current project that is not prevented from being worked on by a predecessor task and does not have a task constraint with a future planned start date. In other words, it can be worked on today.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Activity]</td> 
   <td>In [!DNL Workfront Goals], an activity is a progress indicator for a goal. It can be a progress bar that you update manually, or a project that is associated with the goal. You cannot display activities in a report and you cannot access them through the [!DNL Workfront] API. For information about activities, see <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Get started with results and activities in Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Cost]</td> 
   <td> <p>For tasks and issues, this is the cost associated with the actual hours logged in relation to the Cost per hour rate of the resource assigned to the task or issue. For projects, this is a total of all [!UICONTROL Actual Costs] from tasks and issues on the project. For information, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Expense Cost]</td> 
   <td> <p>The sum of the [!UICONTROL Actual Amounts] for all expenses logged for a project or a task.</p> <b>EXAMPLE </b>
   <p>If you create an expense for Task 1 and enter $600.00 in the [!UICONTROL Actual Amount] field, the [!UICONTROL Actual Expense Cost] for this task is $600.00. </p> 
   <p>For a project, [!DNL Workfront] uses the following formula to calculate [!UICONTROL Actual Expense Cost]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Hours]</td> 
   <td> <p>In a project, task, or issue report, [!UICONTROL Actual Hours] are the sum of all hours logged on the project, task, or issue.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> If from the [!UICONTROL Updates] tab for Task 1, you click 'Log Time' and enter 25 hours, the Actual Hours of Task 1 = 25 hours. </p> <p>[!DNL Workfront] calculates [!UICONTROL Actual Hours] for parent tasks or projects using the following formulas:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Labor Cost]</td> 
   <td> <p>The [!UICONTROL Actual Cost] associated with the labor invested in a task or a project. </p> <p>For a task, [!DNL Workfront] calculates the [!UICONTROL Actual Labor Cost] using the following formula:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>If the task has a [!UICONTROL Cost Type] of [!UICONTROL User Hourly], [!DNL Workfront] uses the user rate. If the task has a [!UICONTROL Cost Type] of [!UICONTROL Role Hourly], [!DNL Workfront] uses the job role rate to calculate [!UICONTROL Actual Labor Cost]. </p> <p>For a project, [!DNL Workfront] uses the following formula to calculate the [!UICONTROL Actual Labor Cost]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>For more information, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>For example, if a user logs 5 hours for a task with a [!UICONTROL User Hourly] [!UICONTROL Cost Type] and their hourly rate is $100, the [!UICONTROL Actual Labor Cost] is $500.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Revenue] </td> 
   <td> <p>The [!UICONTROL Actual Revenue] of a project or a task is the amount of money associated with the [!UICONTROL Actual Hours] of the project or the task. </p> <p>For information about tracking revenue in [!DNL Workfront], see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Start]</td> 
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
   <td>[!UICONTROL Agile] Methodology</td> 
   <td>A type of methodology based on the collaborative evolution of needs and solutions with cross-functional teams. It encourages flexibility and change based on a fixed timeline.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>Differs from a traditional team because they take their prospective work from a backlog and work on it within a set period of time that is called an [!UICONTROL Iteration].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL All My Teams]</td> 
   <td> <p>When this is referenced in [!UICONTROL filters], this field displays either users that belong to any of the teams that the logged-in user belongs to, or work items assigned to any of the teams that the logged-in user belongs to. </p> <p>We recommend using this field in a filter to make reports more generic when sharing them with other users. This way, you can build only one report which will display different information depending on who logs in to view it, as the information is always customized for the logged-in user. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allocation Date]</td> 
   <td> <p>You can find this field in the following types of reports:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project] (Financial Data)</li> 
     <li>[!UICONTROL Budgeted Hour]</li> 
    </ul> <p>For a<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL Project (Financial Data)] report: </p> 
    <ul> 
     <li>Build this report when trying to understand <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> the amount of [!UICONTROL Planned Hours] that is assigned to your resources.</li> 
     <li> <p>The [!UICONTROL Allocation Date] is the first day (Sunday) of a week in which the allocation of a [!UICONTROL Job Role] to a task starts. A resource ([!UICONTROL Job Role]) can have as many [!UICONTROL Allocation Dates] as it has weeks during the [!UICONTROL Duration] of the tasks that it is assigned to. If tasks span over multiple months, then the first day of a month can also become an [!UICONTROL Allocation Date], if it falls within the [!UICONTROL Duration] of the task.</p> <p>For example, you can have a [!UICONTROL Job Role] assigned to a task that spans over 3 weeks and has 90 [!UICONTROL Planned Hours]. These hours are spread evenly during the duration of the task, which makes every day assign 6 [!UICONTROL Planned Hours] to your job role:</p> <p><em> [!UICONTROL Daily Planned Hours] = [!UICONTROL Total Planned Hours]/ Number of [!UICONTROL Work Days] during the [!UICONTROL Duration] of the task </em> </p> <p>As a result, there are three [!UICONTROL Allocation Dates], one for every Sunday of every week during the [!UICONTROL Duration] of the task, each with a certain number of [!UICONTROL Planned Hours] associated with them.<br>If the task starts in the middle of the last week of a month and ends two weeks after the beginning of a new month, the task will have four [!UICONTROL Allocation Dates]: one for every Sunday of every week during the [!UICONTROL Duration] of the task, and one for the first day of the new month.</p> <p>To make the most use of this information, we recommend that you build a <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Project (Financial Data) report and add a matrix grouping for [!UICONTROL Allocation Date], then group the results weekly, monthly, quarterly, or yearly for the most accurate data.<br>For information about building a matrix grouping, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Create a matrix report</a>.</p> </li> 
    </ul> <p>Financial information populates in [!UICONTROL Project (Financial Data)] reports only when the data associated with it is less than 5 years old. For example, if a job role was allocated to a task in January 2015 and today is September 2021, a financial field like the [!UICONTROL Allocation Date] for the job role does not populate in the [!UICONTROL Project (Financial Data)] report. </p> 
    <div> 
     <p>For a [!UICONTROL Budgeted Hour] report:</p> 
     <ul> 
      <li>Build this report when trying to understand the amount of [!UICONTROL Budgeted Hours] that is allocated to your resources or to your projects in the Resource Planner.</li> 
      <li> <p>The [!UICONTROL Allocation Date] is the first day (a Sunday) of the week for which you budgeted the hours in the [!UICONTROL Resource Planner]. </p> <p><b>TIP</b></p> <p>If a week spans for two months, it will generate two rows in the report: one corresponding to the first day of the week (Sunday of the first week which is during the first month), and the second row displays the first day of the second month. </p> <p>For example, if you budget 8 hours for a user for the week of June 30 (Sunday) - July 6 (Saturday), the two rows show an [!UICONTROL Allocation Date] of June 30, and July 1. </p> </p> <p>For information about budgeting resources in the [!DNL Resource Planner], see the article <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the [!DNL Resource Planner] using the [!UICONTROL Project] and [!UICONTROL Role] views</a>.</p> <p>For information about building a [!UICONTROL Budgeted Hour] report, see <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Announcements]</td> 
   <td> <p>A way to communicate to users information within the system. This information is often coming from [!DNL Workfront] to the Administrator or from the Administrator to the user. </p> <p>For more information, see <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Send announcements</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App Integration]</td> 
   <td>An app most commonly represents a connector to a software application, but can also represent special functions that manipulate data.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver Decision]</td> 
   <td> <p>In the [!UICONTROL Proof Approval] report, this field displays proof approval decisions for proofs that are no longer active.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver stage]</td> 
   <td>In the [!UICONTROL Proof Approval report], this field displays information about a proofs current stage.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>A given work item, such as a task, document, or timesheet, may require that a supervisor or other user sign off on the work item. This process of signing off is called approval. </p> <p>For more information, see <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Approval process overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval date]</td> 
   <td>In the [!UICONTROL Proof Approval] report, this field displays the date a proof was approved.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver]</td> 
   <td>A user or job role that must sign off on a given work item, or the user that approves hour entries on timesheets.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assigned To]</td> 
   <td> <p>In a [!UICONTROL Task or Issue] report, this field displays the Owner of the task or the issue, or the [!UICONTROL Primary Assignee]. You can filter or group by this field, as well.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment]</td> 
   <td>A user, job role, or team assigned to an issue or a task. Projects, portfolios, or programs cannot have assignments.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignments]</td> 
   <td> <p>In a [!UICONTROL Task] or [!UICONTROL Issue] report, this field displays a list of all entities (users, job roles, teams) that are assigned to the task or issue. You can filter by this field using the fields [!UICONTROL Assignment Users] and [!UICONTROL Assignment Roles]. You can filter by the team assigned to the task or issue using the Team field. You cannot group a report by this field.</p> <p>Work items that have been placed in the [!UICONTROL Recycle Bin] will continue to display in some reports that refer to the [!UICONTROL Assignment] object where an [!DNL OR] filter modifier is used.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Roles]</td> 
   <td>
   <p>In a [!UICONTROL Task] or [!UICONTROL Issue] report, this field displays information about the job roles assigned to the tasks or issues. This field displays [!UICONTROL Primary Owners], as well as other job roles assigned to tasks or issues.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Status]</td> 
   <td> <p>In an assignment, task, or issue report, the [!UICONTROL Assignment Status] displays whether the users assigned to a work item have clicked the [!UICONTROL Work On It] or the [!UICONTROL Done] button to accept or complete the work. The following [!UICONTROL Assignment Statuses] exist:</p> 
    <ul> 
     <li><b>[!UICONTROL Requested]</b>: the user has been assigned to the task or issue, but they have not clicked the [!UICONTROL Work On It] button to start working on it yet.</li> 
     <li><b>[!UICONTROL Working]</b>: the user has clicked the [!UICONTROL Work On It] button and is currently working on the item. </li> 
     <li><b>[!UICONTROL Done]</b>: the user has clicked the [!UICONTROL Done] button and has completed their work on the item. </li> 
    </ul> <p>For more information, see <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Work On It] and [!UICONTROL Done] button overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Teams]</td> 
   <td>
   <p>In a [!UICONTROL task] or [!UICONTROL issue] report, this field displays information about the teams assigned to the tasks or issues. The field displays [!UICONTROL Primary Owners], as well as other teams assigned to tasks or issues. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Users]</td> 
   <td>
   <p>In a [!UICONTROL Task] or [!UICONTROL Issue] report, this field displays information about the users assigned to the tasks or issues. This field displays [!UICONTROL Primary Owners], as well as other users assigned to tasks or issues. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribute]</td> 
   <td>An attribute is a trait of a [!DNL Workfront] object.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Area]</td> 
   <td> <p>Audits are system messages that record an action that happened in Workfront. The following audit types are recorded:</p> 
    <ul> 
     <li>[!UICONTROL Scope Change]</li> 
     <li>[!UICONTROL Attachment Action]</li> 
     <li>[!UICONTROL General Edit]</li> 
     <li>[!UICONTROL Status Change]</li> 
     <li>[!UICONTROL Note]</li> 
     <li>[!UICONTROL Combined Entry]</li> 
     <li>[!UICONTROL Error Entry]</li> 
     <li>[!UICONTROL Status Change]</li> 
     <li>[!UICONTROL Subscription Change]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Trail]</td> 
   <td>The collection of notes automatically generated by events that are tracked through the Recorded Changes ([!UICONTROL Audit Areas]). Each note records who did the action, what they did, and when they did it.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatic And On Change]</td> 
   <td> <p>One of the [!UICONTROL Project Update] types. This will recalculate the Project's Projected and Planned timelines when the nightly recalculation process runs and when any update is made to the project or tasks within the Project. </p> <p>For more information, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p> </td> 
  </tr> 
  
  <tr> 
   <td><p>Availability</p></td> 
   <td> <p>This term is used in relation to "user availability" or "resource availability" and it illustrates the amount of time that the resource (user or job role) is available to work. </p> 
   <p>Workfront calculates user availability using several fields and depending on what the settings of the Resource Management preferences are in your system. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. </p>
   <p>For more information about resource availability, see <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Get started with Resource Management</a></p>
   Alternately, "capacity" is also used to refer to resource availability. 
   </td> 
  </tr> 

  <tr> 
   <td>[!UICONTROL Automatic Only]</td> 
   <td> <p>One of the [!UICONTROL Project Update] types. This will recalculate Projected and Planned timelines when the nightly recalculation process runs.</p> <p>For more information, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type</a>.</p> </td> 
  </tr> 
  
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>"Business as usual" work that contributes to running the everyday primary business goals.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>The area in an agile environment where new issues are kept until they are ready to be worked on.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>A source of data to measure iterations against in an agile environment.</td> 
  </tr> 

  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Billable Expense]</td> 
   <td> <p>An expense that is marked as billable to the customer. This can be either a planned expense or an actual expense.</p> <p>The Planned Billable Expense Cost and Actual Billable Expense Cost fields are available for you to add to views and reports. They do not appear on the project or task details pages.</p>
   <p>You can find these fields in the following types of reports:</p>
   <ul>
   <li>Baseline</li>
   <li>Template</li>
   <li>Project (Financial Data)</li>
   </ul>
   <p>For more information about marking an expense as billable, see <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Manage project expenses</a>.</p>
   </td> 
  </tr>
  
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Billing Record]</td> 
   <td> <p>Records the revenue, hours, or expenses that can be billed. This information can be used to create invoices in an external accounting system.</p> <p>For more information, see <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Create billing records</a>. </p> 
   </td> 
  </tr>

 <tr> 
   <td>Billing Record Status</td> 
   <td> <p>In a Billing Record or Hour report, the Status of a billing record indicates whether the billing record has been Billed or Not Billed. You cannot delete a project or edit time associated with a Billed billing record. For more information, see <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Create billing records</a>.</p>  
   </td> 
  </tr>


  <tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>The process of customizing [!DNL Workfront] to give the interface an appearance that mirrors your company by using your colors and logos.</p><p><strong>NOTE</strong><br>If your organization has been onboarded to [!DNL Adobe Experience Cloud], branding is not available.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumbs]</td> 
   <td> <p>The area at the top of the page that shows the hierarchical location of where the user is in the application.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">For more information, see <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Breadcrumbs overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget Status]</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that [!DNL Workfront] has removed and the field cannot be updated. </p> <p>This field shows whether the project was added to the [!UICONTROL Capacity Planner] and if the budget calculation has been completed for it. The [!UICONTROL Capacity Planner] has been removed from [!DNL Workfront]. </p> 
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
   <td>[!UICONTROL Budgeted Completion Date]</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that [!DNL Workfront] has removed. This field cannot be updated. </p>
   <p> This field is still visible in [!UICONTROL project] reports and lists.</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Cost]</td>

<td> <p>This is the cost associated with budgeting resources for a project. </p>
   <p>The field displays in the following areas of [!DNL Workfront] under the following names:</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Cost]</strong>: in the [!UICONTROL Business Case Summary] panel</li>
   <li><strong>[!UICONTROL Cost]</strong>: in the [!UICONTROL Utilization] areas when viewing information by [!UICONTROL Cost]</li>
   <li><strong>[!UICONTROL Project Budgeted Cost]</strong>: in lists and reports</li>
   </ul>   
    <p>The [!UICONTROL Budgeted Cost] for the project is calculated using the following formula:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>For more information about calculating [!UICONTROL Budgeted Cost] and to understand various names for this concept in [!DNL Workfront], see <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calculate Project Budgeted Cost</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Budgeted Hours]</td> 
   <td> <p>The hours budgeted for resources for the work they need to complete on projects. This field refers to the hours budgeted in the [!UICONTROL Resource Budgeting] area of the [!UICONTROL Business Case] (or in the [!UICONTROL Resource Planner]) for the project or for the project resources.</p> <p>For more information, see <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand [!UICONTROL Budgeted Labor Cost] and [!UICONTROL Budgeted Hours] for projects</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> For information about budgeting Users in the [!DNL Resource Planner], see the article <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the [!DNL Resource Planner] using the [!UICONTROL Project] and [!UICONTROL Role] views</a>. </p> 
    <p>The hours budgeted in the [!UICONTROL Resource Budgeting] area of the [!UICONTROL Business Case] or the [!UICONTROL Resource Planner] display in the following areas of [!DNL Workfront] and under the following names:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[!UICONTROL Budgeted Hours] display name</strong></td> 
        <td><strong>Areas of [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours]</td> 
        <td>[!UICONTROL Resource Budgeting] area of the [!UICONTROL Business Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Resource Planner] viewed by [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Budgeted Hours]</td> 
        <td> <p>Utilization report [!UICONTROL Hours] view</p> <p>For more information about the [!UICONTROL Utilization] report, see the article <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Overview of the [!UICONTROL Resource Utilization] report</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Hours]</td> 
        <td> <p>[!UICONTROL Budgeted Hour] report</p><p>The [!UICONTROL Budgeted Hour] object in the Budgeted Hour report refers to information related to a deprecated resource management tool. Only the "[!UICONTROL Bud. Hours]" field in this report refers to the hours budgeted in the [!UICONTROL Resource Planner] or the [!UICONTROL Resource Budgeting] area of the project's [!UICONTROL Business Case]. </p> <p>For more information about creating a report, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
        <td> <p>Found in the following reports:</p>
        <ul>
        <li>[!UICONTROL Project] report
        <li>[!UICONTROL Project (Financial Data)] report
        <li>[!UICONTROL Task] report
        <li>[!UICONTROL Issue] report
        <li>[!UICONTROL Budgeted Hour] report</li>
        </ul>
         <p>For more information about creating a report, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Any other mention of [!UICONTROL Budgeted Hours] in [!DNL Adobe Workfront] refers to hours budgeted using deprecated features that have been removed from Workfront . These are view-only fields and do not update with current information when you use current resource budgeting tools. </p>
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
   <td>[!UICONTROL Budgeted Labor Cost]</td> 
   <td> <p>This is the cost associated with the hours that you, as the Resource Manager, budget for your job roles for the work they need to complete on projects. </p> <p>The [!UICONTROL Budgeted Labor Cost] in a project report is calculated using the following formula:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>This field  may refer to the following:</p> 
    <ul> 
     <li> <p>Labor costs displayed in the [!UICONTROL Resource Budgeting] area of the [!UICONTROL Business Case] or in the [!UICONTROL Resource Planner] that are associated with the cost of job roles on a project. For information about calculating the [!UICONTROL Budgeted Labor Cost], see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Understand Budgeted Labor Cost] and [!UICONTROL Budgeted Hours] for projects</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Labor costs displayed in the [!UICONTROL Resource Budgeting] area of the [!UICONTROL Business Case] that reflect the [!UICONTROL People Costs] estimated in an initiative linked to the project from the [!DNL Scenario Planner] when you use the Scenario Planner to budget your project resources. For information about initiatives, see <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Initiatives overview in the Scenario Planner</a>. </p> <p>The [!DNL Scenario Planner] requires an additional license. For information about the [!DNL Workfront Scenario Planner], see <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The [!DNL Scenario Planner] overview</a>. </p> </li> 
     <p>It displays in the following areas of  under the following names:</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Labor Cost]</strong>: in the [!UICONTROL Resource Budgeting] area of the [!UICONTROL Business Case].
   <li><strong>[!UICONTROL Budgeted Cost]</strong>: in the [!UICONTROL Utilization] report [!UICONTROL Cost] view
   <p>For more information, see <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">View resource utilization information </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: in the [!DNL Resource Planner] Project or [!DNL Role] views, when viewing by Cost
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: in the following reports: 
   <ul>
    <li>[!UICONTROL Project] report</li>
    <li>[!UICONTROL Project (Financial Data)] report</li>
    <li>[!UICONTROL Task] report</li>
    <li>[!UICONTROL Issue] report</li>
    <li>[!UICONTROL Budgeted Hour] report</li> 
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
   <td>[!UICONTROL Budgeted Start Date]</td> 
  <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that [!DNL Workfront] has removed. This field cannot be updated.</p>
  <p>These areas have been removed from [!DNL Workfront]. </p> 
  <p>The field is still visible in [!UICONTROL project] reports and lists.</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Burndown Chart]</td> 
   <td>A line chart that provides a visual representation of completed and remaining work.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>A tool used to evaluate whether a project should be moved forward from the [!UICONTROL Idea] status to the [!UICONTROL Planning] status. In other words, a [!UICONTROL business case] helps the organization decide whether it is worthwhile to launch and complete the project or not, especially when comparing projects with others in a portfolio.</p> <p>For more information, see <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Create a [!UICONTROL Business Case] for a project </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case Budgeted Hours]</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that [!DNL Workfront] has removed. This field cannot be updated.</p> <p>This field is still visible in project and [!UICONTROL task] lists and reports. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Assignment]</td> 
   <td> <p>One of the task [!UICONTROL Duration Types] . This will calculate the percentage of an 8-hour work day that the user assigned to the task will be allocated to the task, based on the [!UICONTROL Duration] of the task and the [!UICONTROL Work Required].</p> <p>For more information, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task [!UICONTROL Duration] and [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Work]</td> 
   <td> <p>One of the task [!UICONTROL Duration Types]. This will calculate the [!UICONTROL Work Required] on a task, given the [!UICONTROL Duration] and the user [!UICONTROL Assignment] percentages (which are based on an 8-hour work day).</p> <p>For more information, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task [!UICONTROL Duration] and [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar]</td> 
   <td> <p>There are two types of calendars in [!DNL Workfront]: the [!UICONTROL Home Calendar] and calendar reports.</p> <p>The [!UICONTROL Home Calendar] is a personal calendar that allows a user to manage their workload against their available hours in [!DNL Workfront]. The users can also integrate their [!UICONTROL Home Calendar] with [!DNL Outlook] ([!DNL Google] and [!DNL Microsoft] integration to come). </p> <p>For more information about the [!UICONTROL Home Calendar], see <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[!UICONTROL Home Calendar] view</a>.</p> <p>A calendar report is a dynamic report in which users can view the date and other important details of an event, including the due date, status of work, and the user to whom the event is assigned.</p> <p> For more information about calendar reports, see <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Calendar reports overview</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Can Start]</td> 
   <td> <p>This field indicates whether a task is ready to start to be worked on. If the start is ready to be worked on the [!UICONTROL Can Start] field on the task is set to [!UICONTROL True]. </p> <p>For more information, see <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">"[!UICONTROL Can Start]" overview for tasks</a>.</p> 
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
   <td> <p>Capacity</p> </td> 
   <td> <p>A resource's available time when they can be allocated to work. See "Availability". </p></td> 
  </tr> 
    
  <tr> 
   <td> <p>[!UICONTROL Category]</p> </td> 
   <td> <p>A category is a custom form. You can build reports for this object and you can show it in other object reports, as well. Not all objects can have a custom form, or category. The following objects can have a custom form: <br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL Expense]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL User]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Category Name]</td> 
   <td> <p>When added as a column to the view of any of the following objects it displays a list of all custom forms associated with these objects:</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]<br></li> 
     <li>[!UICONTROL Issue]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL Expense]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL User]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Management]</td> 
   <td>A practice area focused on defining, understanding, and adapting planned work to changes in scope, schedule, cost, and resource factors.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Order]</td> 
   <td>A type of issue raised against a project that outlines a requested change to the agreed scope.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Only]</td> 
   <td>One of the project [!UICONTROL Update Types]. It only updates [!UICONTROL Project Projected] and [!UICONTROL Planned] timelines when Updates are made to tasks or edits are performed on the project or tasks.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Order]</td> 
   <td> <p>One of the [!UICONTROL Issue] types, usually indicating that an unplanned amount of work must be done before the project can be completed.</p> <p>For more information on [!UICONTROL Issue] types, see the section "Default issue types" in the article <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Customize default issue types</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Child Task]</td> 
   <td>A task that is a [!UICONTROL Subtask] of a [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>The collection of [!UICONTROL Subtasks] to a [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] and [!UICONTROL Training]</td> 
   <td>Learning modules, certifications, standards, or a community of practice.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>A communication tool for users to set expectations regarding task deliverables.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit Date]</td> 
   <td>A communication tool for user's to set expectations around task deliverables.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] and [!UICONTROL Reporting]</td> 
   <td>Standards to review the exceptions and health of a project, program, or portfolio</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>A [!UICONTROL Company] is an organizational unit in [!DNL Workfront]. </p> 
   <p> You can associate a user or a project with one company. For more information, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Create and edit companies</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion date]</td> 
   <td> <p>The date that a project, task, or issue is set to be completed. There are several types of [!UICONTROL Completion dates] in [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Actual Completion Date]. For more information, see <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Overview of the project [!UICONTROL Actual Completion Date] </a>.</li> 
     <li>[!UICONTROL Planned Completion Date]. For more information, see <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Set the project [!UICONTROL Planned Completion Date]</a> and <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overview of the task [!UICONTROL Planned Completion Date]</a>.</li> 
     <li>[!UICONTROL Projected Completion Date]. For more information, see <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Overview of the [!UICONTROL Projected Completion Date] for projects, tasks, and issues</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Day]</td> 
   <td>The day, relative to the start of the [!UICONTROL Template], that a [!UICONTROL Template Task] or a [!UICONTROL Template] is supposed to be complete.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Mode]</td> 
   <td> <p>This indicates how a project will be marked as [!UICONTROL Complete]. It can have two values:</p> 
    <ul> 
     <li>[!UICONTROL Manual]: A user must change the project status to [!UICONTROL Complete].</li> 
     <li>[!UICONTROL Automatic]: The project status will automatically change to [!UICONTROL Complete] when all of the tasks in the project are 100% Complete and all of the issues are closed.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>This is a visual representation of the progress of a task, issue or project.</p> <p>For projects, the condition can be manually set by the project owner or it can be automatically set by [!DNL Workfront], based on the progress status of the project. </p> <p>The possible values for the project condition are:</p> 
    <ul> 
     <li>[!UICONTROL On Target]</li> 
     <li>[!UICONTROL At Risk]</li> 
     <li>[!UICONTROL In Trouble]</li> 
    </ul> <p>For more information about project conditions, see the article <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Overview of [!UICONTROL Project Condition] and [!UICONTROL Condition Type]</a>.</p>
     <p>You can associate task and issue conditions with a number that can display in reports. The lists below display the default names and numbers for task and issue conditions. Your system administrator can update the names of conditions and they can add new conditions with different numbers. After a number is associated with a condition, it cannot be edited.  </p> 
     <p>For tasks, the condition is set manually by the task owner. The possible values for the task condition are:</p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li> [!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> <p>For more information about task conditions, see the article <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Update [!UICONTROL Condition] for tasks and issues</a>.</p> <p>For issues, the condition is set manually by the issue owner. The possible values for the issue condition are:<br></p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li>[!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> 
   <p><b>NOTE</b></p>
    <p>When the [!UICONTROL Condition] field is tracked in [!UICONTROL Journal Entry] reports, the [!UICONTROL New] and [!UICONTROL Old Number Values] display the number associated with the condition instead of its name. If a condition is originally not defined for a task or an issue and you later update it, the journal entry that captures the update will display the [!UICONTROL Old Number Value] of the [!UICONTROL Condition] field as -2,147,483,648. See also "[!UICONTROL New Number Value]", "[!UICONTROL Old Number Value]", and "[!UICONTROL Journal Entry]" in this article. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition Update]</td> 
   <td> <p>This field shows the current condition of tasks, projects or issues. This option shows the most recent updates that the owners of tasks, projects or issues have provided in the [!UICONTROL Update Status] field, along with the new condition.</p> <p>Comments made on condition updates are not displayed in the [!UICONTROL Condition Update] column; only the main update is displayed.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Date]</td> 
   <td> <p>If you are using a [!UICONTROL Task Constraint] that is tied to a specific date, such as [!UICONTROL Must Start On], then that specific date becomes the [!UICONTROL Constraint Date] of the task.</p> <p>The following task constraints update the [!UICONTROL Constraint Date] field:</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>TIP</b></p>   
     <ul> 
      <li> <p>A task with a [!UICONTROL Constraint] of [!UICONTROL Fixed Dates] has no [!UICONTROL Constraint Date]. </p> </li> 
      <li> <p> [!UICONTROL Constraint Date] is only viewable in a report or customized view.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Day]</td> 
   <td> <p>If you are using a Task Constraint in a template task that is tied to a specific day, such as Must Start On, then that specific day becomes the Constraint Day of the template task.</p> <p>The following task constraints update the [!UICONTROL Constraint Day] field:</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>TIP</b></p> <p>  [!UICONTROL Constraint Day] is only viewable in a report or customized view. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Type]</td> 
   <td> <p>The scheduling tendency of a task. For example, [!UICONTROL As Soon as Possible] will schedule a task to begin as soon as possible, and [!UICONTROL Finish No Later Than] will schedule a task to finish by the [!UICONTROL Constraint Date] and no later.</p> <p>For more information, see <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL Task Constraint] overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contextual Menu]</td> 
   <td>A menu, located on the left side of the screen, on which the items change to correlate with the active content. For example, when a user is viewing a project, the [!UICONTROL Contextual Menu] will display links to project-related information and tools.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converted Issue Originator]</td> 
   <td>A field in a project or task report that displays information about the user who is the [!UICONTROL Primary Contact] of an issue when the issue is converted into a project or task. The field also displays in the [!UICONTROL Project Details]  section  where it displays the name of the [!UICONTROL Primary Contact] of the converted issue. See also "[!UICONTROL Primary Contact]" in this article.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cost]</td> 
   <td> <p>The monetary amount that you must spend when completing a project, task, or issue. </p> <p>You can track various types of costs for labor, expenses, risks that relate to the project.For information about tracking costs in [!DNL Workfront] see <a href="../../../manage-work/projects/project-finances/track-costs.md">Track costs</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cost Type]</td> 
   <td>For a task, the [!UICONTROL Cost Type] determines how the task will accrue costs. Some examples include [!UICONTROL Fixed Hourly], [!UICONTROL User Hourly], and [!UICONTROL User Hourly plus Fixed]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cross-Project Dependencies]</td> 
   <td> <p>A task of one project is dependent on a task from a different project.</p> <p>For more information, see <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Create cross-project predecessors</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custom Data]</td> 
   <td> <p>Data that is unique to an organization. Organizations can customize the [!DNL Workfront] application by creating custom forms and custom fields. This custom information can drive reporting for KPIs, auditing, and demand mix. </p> <p>[!UICONTROL Custom Data] can be linked to:</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Iterations]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Data Type]</td> 
   <td>The option to specify if a [!UICONTROL Custom Data] Field is stored in the database as Text, a Date, a Number, or Currency.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Display Type]</td> 
   <td>The field display type of a custom field. Examples include [!UICONTROL Drop-Down], [!UICONTROL Text Field], [!UICONTROL Text Area], [!UICONTROL Radio Buttons], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Field]</td> 
   <td>For Custom data that allow the user to select from several options, these are the values from which a user can select. Custom Options are only valid on [!UICONTROL Drop-Down], [!UICONTROL Multi-Select Drop-Down], [!UICONTROL Radio Buttons], and [!UICONTROL Checkboxes].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Form Label]</td> 
   <td>When using a Custom Display Type with Custom Options, this is the user interface text that will display in the Drop-Down menu, the Checkboxes, or the Radio Buttons for that Custom Option.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Value]</td> 
   <td>When using a Custom field with Custom Options, this is the value that will be stored in the database for a particular Option.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom View]</td> 
   <td>A definition of the data fields, or columns that display for each object in a list.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
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
   <td>[!UICONTROL Dashboards]</td> 
   <td> <p> You can add this field in a report or a view of the Report object, to display the dashboards on which the report is listed in a list. </p> <p> You can use this field to filter for reports that are listed on a specific dashboard, as well. </p> <p> For more information about including dashboard information on report object reports, see the "Understanding What Reports Are Listed on Dashboards" section in the article <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Access and organize reports</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Type]</td> 
   <td>See "[!UICONTROL Custom Data Type]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Days Late]</td> 
   <td> <p>This field shows a date difference between [!UICONTROL Planned Start] and [!UICONTROL Today] if the [!UICONTROL Actual Completion Date] is missing.</p> <p>Also shows a date difference between [!UICONTROL Actual Completion] and [!UICONTROL Planned Completion], when an [!UICONTROL Actual Completion Date] is present.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Default Schedule]</td> 
   <td> <p>Customizable default working hours to be assigned to users and projects within an organization. </p> <p>Schedules are used to calculate the planned, start, and completion dates of tasks that are assigned to users.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Deliverable]</td> 
   <td>Quantifiable goods or services that must be provided upon the completion of a project.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>Scoring and prioritization of the intake processes.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Department Goals]</td> 
   <td>Goals unique to a specific department that focus on improving operational metrics within the department.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency]</td> 
   <td>The link between two tasks that require one task to change status before the other task can also change status.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency Type]</td> 
   <td> <p>The type of scheduling relationship between a task and its predecessor(s). One example is [!UICONTROL Finish-Start], which requires that the fist task must Finish before the second task can Start.</p> <p>For more information, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>Any file that is attached to an object within [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document Version]</td> 
   <td> <p>Each time the same document is uploaded to the same object, it is assigned a version number. Users can view and change several options for a previous version of a document.</p> <p>For more information, see <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Manage document versions</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration]</td> 
   <td> <p>The window of time allocated for completion of a task issue, or project (as determined by the number of days between the [!UICONTROL Planned Start] and the Planned Completion).</p> 
    <ul> 
     <li>For tasks, the Duration is an editable field if the Duration Type of the task is not Simple. If the Duration Type of the task is Simple, or if the Task Constraint is Fixed Dates, the Duration is a calculation performed by Workfront.</li> 
     <li>For issues, the Duration is always an editable field and it should represent an estimate of a number of days that would require the issue to be resolved.</li> 
     <li>For projects, the Duration is a calculation performed by [!DNL Workfront] and it represents the difference in days between the Planned Start of the earliest task and the [!UICONTROL Planned Completion] of the latest task on the project.</li> 
    </ul> <p>For more information about the difference between [!UICONTROL Duration] and [!UICONTROL Planned Duration] for tasks, see the article <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Difference between [!UICONTROL Planned Duration] and [!UICONTROL Duration] for tasks</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration in Minutes]</td> 
   <td>This field displays the same information as the [!UICONTROL Duration] field in minutes instead of days. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duration per Occurrence]</td> 
   <td> <p>This displays in the [!UICONTROL Task Details] and the [!UICONTROL Edit Task] boxes of a parent of recurring tasks. It displays the duration of each recurring task. For information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>. </p> <p> <span>Durations modified in individual recurring tasks do not display the value indicated in this field.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Duration Type]</td> 
   <td> <p>A task field that indicates how the work required to complete the task is allocated to the assignees across the task duration. It represents the relationship between the [!UICONTROL Duration] of the task, the [!UICONTROL Work Required], and the amount of time, or [!UICONTROL Allocation], the assigned resources should spend on the task to complete it. </p> <p>This field appears on the [!UICONTROL Details] tab of a task. </p> <p>The options for the Duration Type of a task are:</p> 
    <ul> 
     <li>[!UICONTROL Calculated assignment]</li> 
     <li>[!UICONTROL Calculated Work]</li> 
     <li>[!UICONTROL Effort Driven]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>For more information, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task [!UICONTROL Duration] and [!UICONTROL Duration Type]</a>.</p> 
    --> </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Duration Unit]</td> 
   <td>The unit that is used to measure time in a power search.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Effort Driven]</td> 
   <td>The relationship between the number of users and the amount of time the task will take to complete. As you add more users, the total time scheduled for the task to complete decreases, but the duration of the task stays the same. For example if a task is shelling a barrel of peanuts, adding more people will decrease the time scheduled, but the duration in person-days will remain the same.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elapsed Time]</td> 
   <td> <p>[!UICONTROL Elapsed time] is a unit of time for a task's [!UICONTROL Duration]. It is the time between the [!UICONTROL Planned Start Date] and the [!UICONTROL Planned Completion Date] of a task that includes holidays, weekends, and time off. In other words, elapsed time is the passage of calendar days. </p> <p>[!DNL Workfront] supports the following elapsed time units for task duration:</p> 
    <ul> 
     <li> <p>[!UICONTROL Elapsed Minutes]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Hours]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Days]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Weeks]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Months]</p> </li> 
    </ul> <p>For more information about task duration, including elapsed time, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task [!UICONTROL Duration] and [!UICONTROL Duration Type]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End Date]</td> 
   <td> <p> In a [!UICONTROL Rate] report, this is the date when a new billing rate for a job role at the project level ends. The hours associated with the project that are before this date are multiplied by this billing rate to calculate the revenue on the project. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>The [!UICONTROL Work Performance Indicator] (WPI) that indicates when commitment and belief in the task, project, team, or organization is waning. This indicates that you need to act to revive that belief and commitment. WPI would be measured by asking the simple questions, "Did you understand what was expected of you? Did the work you were assigned make a difference to the organization? Did you do great work?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>Cross-functional goals that contribute to the metrics of the company goals.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event]</td> 
   <td>Any change in a project or task.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event Handler]</td> 
   <td>Automated tasks that occur when Events take place. A common example is an automated email notification.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event notification]</td> 
   <td>Email that is generated from an event handler.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Expenses]</td> 
   <td>A non-labor cost on tasks or projects.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External]</td> 
   <td> <p>Typically, this is a license type, or a user with such a license. A user with such a license type only has the ability to review information in the system. They cannot actively participate in work.</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] licenses overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External System]</td> 
   <td>Any services or software that is stored and governed outside the designated system of record.</td> 
  </tr> 

 <tr> 
   <td>[!UICONTROL Field]</td> 
   <td><p>Any Workfront object or the information associated with it, as it appears in the database. </p>
   <p>For example, "project", "user", "hour" are both Workfront objects as well as fields. "Name", "status", "owner", "start date" are Workfront fields that are associated with the above objects. </p>

   <p>When referring to objects, the terms "objects" and "fields" can be used interchangeably.</p>
   <p>In the scope of reporting, the "fields" refer to the objects or the information about the object that you want to capture in the report.</p>
   
   <p><b>NOTE</b></p>

  <p>In text-more reporting, fields refer to the objects or their information as it appears in the database.</p>
   <p>Sometimes the name that you see in the user interface is different from the name of the field in the database. For example, "issue" is the name of the object in the Workfront interface, but "opTask" is the name of the object (or the field) in the Workfront database. </p> 
   <p> It's important to use the field as it appears in the database when writing a text-mode report, view, filter, or grouping, or when creating a calculated field.</p>

   <p>For more information, see <a href="../../../wf-api/general/api-explorer.md">API Explorer</a> and <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Text Mode overview</a>.</p>  

   <p>By default, Workfront comes with a set of fields that define both objects and their information. You can also create custom fields to define objects, but you cannot create custom objects.</p> 
   </td> 
  </tr>

  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>One of the main building blocks of a report or a list element that defines what information displays on the screen. For more information about reporting elements, see <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Reporting elements: filters, views, and groupings</a>.</p> <p>The Filter determines the results that display in a report or on an [!DNL Workfront] panel listing, like projects, tasks, or issues.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Process to manage labor costs, expenses, and revenue data in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Cost]</td> 
   <td>You can define a fixed amount of cost for a project. This is part of the [!UICONTROL Planned Cost] of the project which represents the amount of money that you need to complete the project. For information about costs, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Revenue]</td> 
   <td>You can define a fixed amount of revenue for a project. This is part of the [!UICONTROL Planned Revenue] of the project which represents the amount of money that you might obtain if you complete the project. For information about revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flags]</td> 
   <td> <p> This is the same field as [!UICONTROL Status Icons], but it is only available for the following views: </p> 
    <ul> 
     <li> [!UICONTROL Templates] </li> 
     <li> [!UICONTROL Expenses] </li> 
    </ul> <p> For more information, see the article <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Built-in Status Icons in Views</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Folders are used to organize documents or reports associated with an object.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (Full Time Equivalent)</td> 
   <td>This is the Full Time Equivalent which indicates the amount of time that a resource is available for work. 
   The [!UICONTROL FTE] field displays in the following areas: 
  <ul>
   <li> User's profile, when editing or creating the user </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL Scenario Planner] (requires additional license for the Workfront Scenario Planner) </li>
   <li> User lists and reports </li> </ul>
    
   <p>The [!UICONTROL FTE] must be a decimal number up to 1, and it cannot be 0. </p>
   <p> An [!UICONTROL FTE] of 1 (which is the default for a user's [!UICONTROL FTE] field, as defined in their profile) means that a resource (user or role) works the entire number of hours, based on the schedule that calculates their availability. </p>
   <p>Your Workfront administrator decides which schedule to use in determining user's availability.  </p>
   <ul>
   <li> When the [!UICONTROL Default Schedule] is used, Workfront uses the [!UICONTROL FTE] of the user found in their profile to calculate availability. </li>
   <li> When the User's Schedule is used, Workfront uses the user's time off, [!UICONTROL Work Time] value, and [!UICONTROL Default Schedule]'s hours to calculate the user's [!UICONTROL FTE]. </li> </ul>
    
   <p>For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>.  </p>
   <p>For more information about creating schedules in [!DNL Workfront], see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>. </p>

   <p><b>NOTE</b></p>
   <p>For all calculations in the [!UICONTROL Scenario Planner], Workfront uses the following value: 1 [!UICONTROL FTE] = 8 Hours.</p>
   <p>For more information, see <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Get started with the [!UICONTROL Scenario Planner]</a>. </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
--> 

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
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>A visual timeline of the project dates in a calendar view based on the planned or projected dates as the tasks of the project are currently scheduled.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal]</td> 
   <td><p>There are two concepts of goals in [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>Project goals</b>: A set of business objectives agreed to by the relevant stakeholders of a project. Project goals are part of the Business Case of a project. </p> <p>You cannot display project goals in lists or reports but you can access them through the API. </p> <p>For information about Business Case project goals, see <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Create Business Case goals </a>. </p> </li> 
     <li> <p><b>Strategic goals</b>: A strategic goal is an objective that you create to plan your work strategy for a specific time-period. You can create these types of goals using [!DNL Workfront Goals]. Your organization must purchase an additional license and you must have access to this feature to be able to create strategic goals. [!DNL Workfront Goals] are available only with an additional license.</p> 
     <p>For more information, see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] overview </a>. </p> 
     <p>You can display strategic goals in a goal or a project report and access them through the API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Hierarchy]</td> 
   <td> <p>In [!UICONTROL Goal] and [!UICONTROL Project] reports, this is a collection field that displays the goals in the hierarchy that a strategic goal belongs to when it aligns to other goals. The goals are separated by a ▸ delimiter. </p> <p>Only the parents of the goal and the goal display in this field. Children goals do not display. </p> <p>For information about aligning goals in [!DNL Workfront Goals], see <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Goal alignment overview in [!DNL Workfront Goals]</a>. </p> 
   <p>This field is visible only if your organization has purchased [!DNL Workfront Goals]. For information about managing strategic goals using [!DNL Workfront Goals], see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] overview </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Success Score]</td> 
   <td> In a [!UICONTROL Project report] this field used to refer to project-level goals associated with the [!UICONTROL Business] Case. Currently, this is a deprecated field and is not associated with any functionality.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Goals] </td> 
   <td> <p>In a [!UICONTROL Project] report, this is a collection field that displays all the strategic goals that are associated with a project. The goals are separated by commas.</p> <p>This field is visible only if your organization has purchased [!DNL Workfront Goals]. For information about managing strategic goals using [!DNL Workfront Goals], see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] overview</a>. For more information about strategic goals and project goals in [!DNL Workfront], see "[!UICONTROL Goal]" in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>Interface settings that affect all users. [!UICONTROL Global Interface Preferences] can be overwritten by the [!UICONTROL User Interface Preferences].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>A collection of users (possibly from the same department or business unit) that have access to the same objects. In addition to users, groups can be associated with portfolios, programs, projects,<span> project templates,</span> companies, teams, schedules, layout templates, and timesheet profiles.</p> <p>You can also grant permissions to objects by group. For more information, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> <p>In a list or report of objects of one of the following types, you can use the [!UICONTROL Group] field to list which objects of that type are associated with a particular group: user, portfolio, program, project, <span>project template</span>, company, team, schedule, layout template or timesheet profile.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Group Administrator]</td> 
   <td> <p>Users who manage the objects, access, and users of designated user groups.</p> <p> In a [!UICONTROL Group] report, this field displays the names of the users designated as [!UICONTROL Group Administrators] in the Group. For more information about Group Administrators, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group with Administration Access]</td> 
   <td> <p> In a [!UICONTROL Layout Template], [!UICONTROL Timesheet Profile], or [!UICONTROL Schedule report], this field displays the Groups whose Group Administrators have access to modify the template. You can also filter this report by this field. </p> <p> For more information, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Grouping]</td> 
   <td> <p>A reporting element used to categorize information in a list by a common criterion.</p> <p>For more information, see the "[!UICONTROL Groupings]" section in the article <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Reporting elements: filters, views, and groupings</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Handoff Date]</td> 
   <td> <p>The date when a task becomes available for work. The [!UICONTROL Handoff Date] is a calculation and cannot be set manually. <br>For more information about the [!UICONTROL Handoff Date], see the article <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL Task Handoff Date] overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>An alternative name to describe the [!UICONTROL Requests] area of [!DNL Workfront]. You can use the [!UICONTROL Requests] area to process customer support tickets, project requests, help desk tickets, etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Owner]</td> 
   <td>In an [!UICONTROL Hour] report, the [!UICONTROL Owner] is the user to whom the hours are attributed. This is different from the user who is actually logging the time. These two entities can sometimes be two different users. <br>For more information about logging time for another user, see the article <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Log time</a>.</td> 
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
   <td>[!UICONTROL Hour Type]</td> 
   <td> <p>An attribute that can be set for Actual Hours that users log for tasks, issues, or projects. This is also an attribute for the hours logged that are not directly linked to work, such as [!UICONTROL Vacation] and [!UICONTROL Time Off].</p> <p>For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Manage hour types</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>The ID is an alphanumeric indicator associated with every object in [!DNL Workfront]. It uniquely identifies each object in the [!DNL Workfront] database. You can view the ID of any object in a report or a list for each object. </p> <p><b>TIP</b></p>   <p>You can also view the ID in the URL of the object's page. For example, the ID of a project might look something like the number outlined in the following URL, when you access the [!UICONTROL Project Details] page:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Individual Goals]</td> 
   <td>Individual goals which contribute to the metrics of the team goals, but not related to personal or career development.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Inherited Access]</td> 
   <td>Sharing function that allows access to propagate from object to another. For example, project user's inherit access defined in program and portfolio records.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>In the [!DNL Workfront Scenario Planner], you can divide a plan into several initiatives to make it easier to manage the plan. <span>You can build an [!UICONTROL Initiative] report and you can access [!UICONTROL Initiative] information in a [!UICONTROL Project] report.</span></p> <p>The [!DNL Scenario Planner] requires an additional license. For information about the [!DNL Workfront Scenario Planner], see <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The [!DNL Scenario Planner] overview</a>. </p> <p>The [!DNL Initiative] report is not visible in your [!DNL Workfront] instance unless your company has purchased a [!DNL Workfront Scenario Planner] license. You cannot access [!UICONTROL Initiatives] through the API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>The [!UICONTROL Initiative Job Role] report type displays information about the job roles associated with a plan initiative in the [!DNL Workfront Scenario Planner].</span> </p> <p>The [!DNL Scenario Planner] requires an additional license. For information about the [!DNL Workfront Scenario Planner], see <a href="../../../scenario-planner/scenario-planner-overview.md">The [!DNL Scenario Planner] overview</a>. </p> <p><span>This report type is not visible in your [!DNL Workfront] instance unless your company has purchased a [!DNL Workfront Scenario Planner] license.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role Hours]</span> </td> 
   <td> <p><span> In an [!UICONTROL Initiative Job Role] report, this displays the number of hours associated with a job role in an initiative.</span> </p> <p>The [!DNL Scenario Planner] requires an additional license. For information about the [!DNL Workfront Scenario Planner], see <a href="../../../scenario-planner/scenario-planner-overview.md">The [!DNL Scenario Planner] overview</a>. </p> <p>This field and the [!UICONTROL Initiative Job Role] report type are not visible in your [!DNL Workfront] instance unless your company has purchased a [!DNL Workfront Scenario Planner] license.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role Count]</td> 
   <td> <p>In an [!UICONTROL Initiative Job Role] report, this displays the number of specific job roles associated with an initiative.</p> <p>The [!DNL Scenario Planner] requires an additional license. For information about the [!DNL Workfront Scenario Planner], see <a href="../../../scenario-planner/scenario-planner-overview.md">The [!DNL Scenario Planner] overview</a>. </p> <p>This field and the [!UICONTROL Initiative Job Role] report type are not visible in your [!DNL Workfront] instance unless your company has purchased a [!DNL Workfront Scenario Planner] license.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Last Published Date]</td> 
   <td> <p>A field in an [!UICONTROL Initiative], [!UICONTROL Initiative Job Role], and [!UICONTROL Project] report that displays the date that a plan initiative was last published to a project. You can publish initiatives to create projects or to update projects linked to the initiatives.</p> <p>The [!DNL Scenario Planner] requires an additional license. For information about the [!DNL Workfront Scenario Planner], see <a href="../../../scenario-planner/scenario-planner-overview.md">The [!DNL Scenario Planner] overview</a>. </p> <p><span>For information about publishing initiatives, see</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publish scenarios to create and update projects in the [!DNL Workfront Scenario Planner]</a>. This field is not visible in your [!DNL Workfront] instance unless your company has purchased a [!DNL Workfront Scenario Planner] license.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inline Search]</td> 
   <td>A search performed, in the process of completing a form, to find possible entries for one specific field.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface Setup]</td> 
   <td>The area of the application that allows defining Custom Views, Filters, Groupings, List Controls, etc.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Is Company Goal]</p></td> 
   <td> <p>In [!DNL goal reports], this displays a "[!UICONTROL True]/ [!UICONTROL False]" value for each strategic goal to indicate whether your organization is assigned to the goal as its owner. </p> 
   <p>This field is visible only if your organization has purchased [!DNL Workfront Goals]. For information about managing strategic goals using [!DNL Workfront Goals], see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] overview </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue]</td> 
   <td> <p>An unplanned work item that usually indicates that there is a problem preventing the completion of a task or project. It is triaged and evaluated for further work effort consideration</p> <p>An [!UICONTROL Issue] can also be a [!UICONTROL Help Desk] request. [!UICONTROL Change Orders], [!UICONTROL Requests], and [!UICONTROL Bugs] are also [!UICONTROL Issues].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Management]</td> 
   <td> <p>The process and rules governing the definition of issue types and the routing, triage, or traffic process associated with each type.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Owner]</td> 
   <td>The team or users responsible for triaging and completing an issue.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
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
   <td>[!UICONTROL Job Role]</td> 
   <td> <p>Used to identify a user's day-to-day job functions and responsibilities. Job roles can be assigned to work items to identify the required skill needed to complete a work process without assigning it to a specific user. </p> <p>A user can have more than one role. Examples include Graphic Designer or Consultant.</p> <p>For more information, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Journal Entry]</p> </td> 
   <td> <p>A reportable object that tells you information about system updates for tracked fields that appear in the [!UICONTROL Updates] area of projects, tasks, issues, and other objects.</p> <p>To learn more, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Report on the [!UICONTROL Updates] area</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban Flag]</td> 
   <td> <p>In a [!UICONTROL Task] Report or [!UICONTROL Issue] Report, the [!UICONTROL Kanban Flag] field displays the flag status that is set on the story on the [!UICONTROL Kanban board]. Possible values are [!UICONTROL On Track], [!UICONTROL Ready to Pull], and [!UICONTROL Is Blocked].</p> <p>For more information about setting flag status on stories on the [!UICONTROL Kanban story board], see  the article <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Use flags on stories on the [!UICONTROL Kanban board]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPIs</td> 
   <td>A measurable value that demonstrates how effectively a company is achieving key business objectives.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>Amount of time that must pass after the predecessor task's [!UICONTROL Planned Completion Date] has passed until the dependent task can begin.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag Types]</td> 
   <td> <p>The method of calculating the [!UICONTROL Lag]. It can be:</p> 
    <ul> 
     <li>[!UICONTROL Days] (work days)</li> 
     <li>[!UICONTROL Calendar Days] (ignore holidays)</li> 
     <li>[!UICONTROL Percent]</li> 
     <li>[!UICONTROL Day of Week]</li> 
    </ul> <p>For more information, see <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Lag Types overview</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Large Thumbnail]</td> 
   <td> <p> In a [!UICONTROL Document] list or report, it displays a preview of the document in a thumbnail. </p> <p>Select <strong>[!UICONTROL Large Thumbnail]</strong> to view a 400 pixel-wide thumbnail in the report.</p> <p>The size of the thumbnail adjusts when you modify the width of the column in a list or report.</p> <p>See also "[!UICONTROL Thumbnail]" in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last 10 Viewers]</td> 
   <td> <p>In a report list, this field displays the names of up to 10 users who have viewed the report most recently.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Condition Note]</td> 
   <td> <p>This field displays the update last entered on an object by the owner of the object, This is the owner's most recent activity or interaction on an object.</p> <p>The [!DNL Last Condition Note] column is empty if the note text of the last note of an object has been deleted. When a new note is entered on the object, it becomes the last note and it displays again in the column. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Finance Update Date]</td> 
   <td>In a [!UICONTROL project] report, this field captures the date and the time when the project finances were last calculated and updated. For information about project finances, see <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Project finances overview</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Note]</td> 
   <td> <p>This field displays the update last entered on an object by any user. This is the most recent activity or interaction on an object.</p> <p>The [!UICONTROL Last Note] column is empty if the text of the last note of an object has been deleted. When a new note is entered on the object, it becomes the last note and it displays again in the column.</p>
   <p>When this field is added to a [!UICONTROL Task] report, any updates left on child objects — such as issues, subtasks, documents, etc. — of the task do not display in this column.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed By]</td> 
   <td> <p>In a report list, this field displays information about the user who viewed the report last.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed Date]</td> 
   <td> <p>In a report list, this field displays the date on which the report was displayed last.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Layout Template]</td> 
   <td>Defined by the System Administrator or Group Administrator to identify the tabs and reports that display in a given user's workspace.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Layout Type]</td> 
   <td>In conjunction with [!UICONTROL Custom Views], the [!UICONTROL Layout Type] specifies the type of [!UICONTROL Custom View]. Currently, only List is available. In the future, [!UICONTROL Detail] (the [!UICONTROL Detail] view of an object) may become available.</td> 
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
   <td>[!UICONTROL Library Task]</td> 
   <td>A template for a single task that is used to provide consistent naming of [!UICONTROL Tasks] and [!UICONTROL Template Tasks] across the application.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Type]</td> 
   <td>The type of license allocated to an [!UICONTROL Access Level]. It is either [!UICONTROL Full User], [!UICONTROL Limited User], or [!UICONTROL Requester].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Plan]</td> 
   <td> <p>In a [!UICONTROL Group] view or report, this field shows the maximum number of [!UICONTROL Plan] licenses that can be assigned to users who have the respective group designated as their [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Work]</td> 
   <td> <p>In a [!UICONTROL Group] view or report, this field shows the maximum number of [!UICONTROL Work] licenses that can be assigned to users who have the respective group designated as their [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limited User]</td> 
   <td>A License Type that allows creation of an [!DNL Access Level] that contains view-only privileges, with the ability to submit issues, enter notes, and upload documents.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List Controls]</td> 
   <td> <p>A part of [!UICONTROL Interface Setup] that allows linking custom Filters, Views, and Groupings to individual Users or globally to all Users.</p> </td> 
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
   <td>[!UICONTROL Manual Only]</td> 
   <td> <p>One of a [!UICONTROL Project]'s [!UICONTROL Update Types]. This setting allows [!UICONTROL Project Projected] and [!UICONTROL Planned] timelines to be updated only when "[!UICONTROL Recalculated Timelines]" is clicked. Projects set up this way will be ignored during the nightly recalculation process and when the project or tasks in the project are updated.</p> <p>For more information, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project [!UICONTROL Update Type] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>This refers to the currently logged-in user. </p> <p>We recommend using this field in a filter to make reports more generic when sharing them with other users. This way, you can build only one report which will display different information depending on who logs in to view it, as the information is always customized for the logged-in user. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max Users]</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that [!DNL Workfront] has removed and the field cannot be updated. </p> <p>In previous releases of [!DNL Workfront], you could update this field when creating or editing a job role. It displayed the total number of users that can be associated with a role on each project. A value of zero allowed for an unlimited number of users that can be assigned on a project. </p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>A marker that you can associate with a task to indicate that a key point in the project has been achieved when the task is completed. You generally can use milestones to show a significant event such as the completion of a phase of the project or a set of critical activities. [!UICONTROL Milestones] are typically associated with parent tasks. You must create the milestones before you can attach them to tasks. For information about milestones, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Create a milestone path</a> and <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Associate milestones with tasks</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Milestone Path]</td> 
   <td>A collection of [!UICONTROL milestones]. [!UICONTROL Milestone Paths] are used on projects to distinguish projects with certain types of [!UICONTROL Milestones] from projects with a different set of [!UICONTROL Milestones].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone Task]</td> 
   <td>A task flagged to indicate a reportable event to measure.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>A single step within a scenario in [!DNL Workfront Fusion] that performs some function based upon the associated app.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Primary Role]</td> 
   <td> <p>When this is referenced in filters, this displays either users that have the same [!UICONTROL Primary Role] as the logged-in user, or work items assigned to the [!UICONTROL Primary Role] of the logged-in user.</p> <p>We recommend using this field in a filter to make reports more generic when sharing them with other users. This way, you can build only one report which will display different information depending on who logs in to view it, as the information is always customized for the logged-in user. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Home Team]</td> 
   <td> <p>When this is referenced in filters, this field displays either users that belong to the [!UICONTROL Home Team] of the logged-in user, or work items assigned to the [!UICONTROL Home Team] of the logged-in user. </p> <p>We recommend using this field in a filter to make reports more generic when sharing them with other users. This way, you can build only one report which will display different information depending on who logs in to view it, as the information is always customized for the logged-in user. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Naming convention]</td> 
   <td>An organization-wide set of rules that use data to create names of projects, tasks, and deliverables.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Native Integration]</td> 
   <td>An integration that requires no manual coding or API configuration. Also referred to as an "out-of-the-box" integration.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navigation Menu]</td> 
   <td>The top-center panel of the application that has links to main areas of [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL New Number Value]</td> 
   <td>In a [!UICONTROL Journal Entry] report, this displays the updated value of a field that replaces the [!UICONTROL Old Number Value].
   For more information, see "[!UICONTROL Old Number Value]" in this article.</td> 
  </tr>

  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Non-Billable Expense]</td> 
   <td> <p>An expense that is not marked as billable to the customer. This can be either a planned expense or an actual expense.</p> <p>The Planned Non-Billable Expense Cost and Actual Non-Billable Expense Cost fields are available for you to add to views and reports. They do not appear on the project or task details pages.</p>
   <p>You can find these fields in the following types of reports:</p>
   <ul>
   <li>Baseline</li>
   <li>Template</li>
   <li>Project (Financial Data)</li>
   </ul>
   <p>For more information about marking an expense as billable, see <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Manage project expenses</a>.</p>
   </td> 
  </tr>

  <tr> 
   <td>[!UICONTROL Non Work Day]</td> 
   <td>A day that is not allocated to the completion of any assignments. This is usually a vacation day, holiday, or weekend. The term display in the API explorer. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note]</td> 
   <td>A comment or update made on a [!DNL Workfront] object.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note Text]</td> 
   <td> <p>This displays the text of an update entered by a user on any object. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Number of Linked Goals]</td> 
   <td> <p>In a [!UICONTROL Project] report, this is the number of strategic goals that are associated with the project. For information about associating projects with strategic goals, see <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Add projects to goals in  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>For information about strategic goals, also see "[!UICONTROL Goal]" in this article.</p> 
   <p>This field is visible only if your organization has purchased [!DNL Workfront Goals]. For information about managing strategic goals using [!DNL Workfront Goals], see <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Add projects to goals in [!UICONTROL Adobe Workfront Goals]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object]</td> 
   <td> <p>The information you display in [!DNL Adobe Workfront] is represented by objects which are stored in the [!DNL Workfront] database. The objects are what drives the information in Workfront. Some examples of objects are:</p> 
    <ul> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Groups]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Custom forms]</li>
     <li>[!UICONTROL Custom fields]</li>  
     <li>[!UICONTROL Hours]</li> 
     <li>[!UICONTROL Billing Rates]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Template tasks]</li> 

  <p><b>NOTE</b></p>
  <p>This is not an extensive list. </p>

  </ul> <p>For more information, see <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object Types]</td> 
   <td>If you create a report or list containing all of your custom forms, you can use this field as a view or filter to see which object types are associated with each form. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Old Number Value]</td> 
   <td>In a [!UICONTROL Journal Entry] report, this displays the original value of a field before it was updated. Once a field's value is updated, it will display as the [!UICONTROL New Number Value] in a [!UICONTROL Journal Entry] report. For more information, also see "[!UICONTROL New Number Value]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL On Change Only]</td> 
   <td> <p>One of the [!UICONTROL Project Update] Types. When this is selected, the [!UICONTROL Project Projected] and [!UICONTROL Planned] timelines update only when an update or change is made to the project or to a task within the project. It does not update the project every night.</p> <p>For more information, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>The name for [!UICONTROL Issue] in the [!DNL Workfront] database, used in text mode reports or calculated custom data.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>An issue or task that is not complete, but being worked on.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Org Chart]</td> 
   <td>Short for Organizational Chart. This is a chart showing the hierarchy of an organization. It is also on the Tab on the [!UICONTROL User] detail screen that displays and allows setting the [!UICONTROL User]'s [!UICONTROL Company] and [!UICONTROL Reporting] relationships.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organizational Setup]</td> 
   <td>This defines [!UICONTROL Companies], [!UICONTROL Groups], and [!UICONTROL Security Profiles] for your organization.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Other Groups]</td> 
   <td> <p>In a report or view that lists users, this field displays all the groups where each user is a member. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency]</span> </td> 
   <td> 
    <div> 
     <p>In a [!UICONTROL Job Role] report, this is the currency associated with a job role. It is an override of the [!UICONTROL Base Currency] as established in the [!UICONTROL Setup] area by the [!DNL Workfront] administrator. </p> 
     <p>For more information, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Billing/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>In a [!UICONTROL Job Role] report, this is the billing per hour rate of the job role using the selected [!UICONTROL Override Currency] of the job role.</p> 
     <p> For more information, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Cost/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>In a [!UICONTROL Job Role] report, this is the cost per hour rate of the job role using the selected [!UICONTROL Override Currency] of the job role. </p> 
     <p>For more information, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Owner]</td> 
   <td>The user responsible for the completion of the designated object.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Owner Type]</span> </td> 
   <td> 
    <div> 
     <p>In a [!UICONTROL Goal] report, this displays the type of owner that is assigned to a strategic goal. The following are the goal owner types:</p> 
     <ul> 
      <li> <p>[!UICONTROL User]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>No value displays in this field when the goal owner is your organization. </p> 
     <p>This requires an additional license. For information about [!DNL Workfront Goals], see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] overview</a>. </p> 
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
   <td>[!UICONTROL Parameter]</td> 
   <td> <p>A [!UICONTROL parameter] is a custom field. You can build a report for all parameters, or custom fields in your system. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent]</td> 
   <td>In a report, this field shows information about the parent of the object. For example, in an [!UICONTROL issue] report, it might show information about the task or project that the issue is logged under; in a task report, it might show information about the direct parent task or about the project. For more information about what objects might have parents in [!DNL Workfront], see the "Interdependency and hierarchy of objects" section in the article <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Lag]</td> 
   <td>The amount of time that must pass between the [!UICONTROL Parent Task] start and the [!UICONTROL Subtask] Start.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Task]</td> 
   <td>Also known as a [!UICONTROL Summary Task]. This is a task that has Subtasks (also called [!UICONTROL Children Tasks]). The [!UICONTROL Duration], [!UICONTROL Work Required], and [!UICONTROL Percent Complete] of the Parent Task is calculated from the Subtasks.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Part-Time Resources]</td> 
   <td>A licensed user who has less capacity than the default schedule defined in the system.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percent Complete]</td> 
   <td> <p>A project, task, or issue field that shows what percentage of the work associated with the task, project, or issue is completed.</p> <p>You can update this field manually for issues and working tasks. </p> <p>For projects and parent tasks, this field is a roll-up from all the working tasks and you cannot update it manually. </p> <p>For more information, see <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Project [!UICONTROL Percent Complete] overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permission]</td> 
   <td> <p>Rights that are granted to a user on an object, typically given so they can complete work on the item or view the item. You can grant permissions to:</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL Views]</li> 
     <li>[!UICONTROL Filters]</li> 
     <li>[!UICONTROL Groupings]</li> 
    </ul> <p>For more information, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>This is a full license type in the [!DNL Workfront] system. Users must have this to access all of the features in [!DNL Workfront].</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] licenses overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (in the [!DNL Scenario Planner])</td> 
   <td> <p>A plan is the main object when working with the [!DNL Workfront] Scenario Planner. You can outline the strategy for your company's near and long-term future and identify each high-level outcome and add it as a plan to the [!DNL Workfront] Scenario Planner. </p> <p>You cannot display [!DNL Scenario Planner] plans in a report and you cannot access them through the [!DNL Workfront] API. </p> <p>The [!DNL Scenario Planner] requires an additional license. For information about the [!DNL Workfront Scenario Planner], see <a href="../../../scenario-planner/scenario-planner-overview.md">The [!DNL Scenario Planner] overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned]</td> 
   <td> <p>The time frame within which something is scheduled to occur. When you create projects, tasks, or issues in [!DNL Workfront], you establish the planned start and end dates, as well as the planned timeframe during which they occur. These values represent your original intention or estimate of how long an item should take to complete. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Benefit]</td> 
   <td>This is a manual entry for the Project Manager to estimate whether completing a project would bring any monetary benefit to the organization. Specifying this value can be part of putting together a [!UICONTROL Business Case] for the project. You must have [!UICONTROL Manage] permissions to the project to update this value.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Planned Budgeted Hours]</td> 
   <td> <p>In a [!UICONTROL Budgeted Hour] report, this displays the number of hours budgeted for projects or [!UICONTROL Job Roles] in the [!UICONTROL Resource Planner]. </p> <p>For information about budgeting projects or roles in the [!UICONTROL Resource Planner], see the article <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the [!UICONTROL Resource Planner] using the [!UICONTROL Project] and [!UICONTROL Role] views</a>. For information about the [!UICONTROL Budgeted Hours] report, see the article <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>You can manually set the [!UICONTROL Planned Completion Date] of a task, project, or issue to a date of your choosing. If you do not set the [!UICONTROL Planned Completion Date], [!DNL Workfront] sets it automatically. When set automatically, the [!UICONTROL Planned Completion Date] is: [!UICONTROL Planned Start Date] + [!UICONTROL Duration]</p> <p>For more information, see the following articles:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overview of the task [!UICONTROL Planned Completion Date]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Set the project [!UICONTROL Planned Completion Date]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Cost]</td> 
   <td> <p>A total of the [!UICONTROL Planned Labor Cost] and the [!UICONTROL Planned Expense Cost] of the project. This does not include the [!UICONTROL Planned Risk Cost] on the project.  </p> </td> 
  </tr> 



  <tr> 
   <td>[!UICONTROL Planned Date Alignment]</td> 
   <td> <p>This is an automatic indicator that Workfront assigns projects, tasks, and issues to show when an item will be completed in relation to its Planned Completion Date. </p>
   <p>The following are possible values for the Planned Date Alignment indicator: </p>
<ul>
<li>Will be done on the planned completion date</li>
<li>Will be done before the planned completion date</li>
<li>Will be done after the planned completion date</li></ul>
<p>The Planned Date Alignment is visible in project, task, and issue lists and reports. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration]</td> 
   <td> <p>A task's [!UICONTROL Planned Duration] is usually the same as the task's [!UICONTROL Duration]. It represents the difference in days between the [!UICONTROL Planned Start] and the [!UICONTROL Planned Completion Dates] of the task. </p> <p>When the task has a [!UICONTROL Duration] Type of [!UICONTROL Effort Driven], the [!UICONTROL Planned Duration] can differ from the [!UICONTROL Duration] of the task, based on how many resources you assign to the task. </p> <p>For example, if a task with a [!UICONTROL Duration] Type of [!UICONTROL Effort Driven] has a [!UICONTROL Duration] of 3 days and you assign one resource with a full-time schedule to the task, the [!UICONTROL Planned Duration] is 3 days, as well. If you assign three resources with a full-time schedule to the same task, the [!UICONTROL Duration] stays 3 days, but the [!UICONTROL Planned Duration] becomes 1 day. The [!UICONTROL Planned Duration] also changes the [!UICONTROL Planned Start] and [!UICONTROL Planned Completion] dates of the task, to reflect the new [!UICONTROL Planned Duration]. As a result, the timeline of the project is affected as well. </p> <p>For more information about the difference between [!UICONTROL Duration] and [!UICONTROL Planned Duration] for tasks, see the article <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Difference between [!UICONTROL Planned Duration] and [!UICONTROL Duration] for tasks</a>.</p> <p>Projects and issues don't have a [!UICONTROL Planned Duration]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration Minutes]</td> 
   <td> <p>The [!UICONTROL Planned Duration Minutes] of a project or an issue is the [!UICONTROL Duration] of the project or issue in minutes. </p> <p>Tasks don't have a [!UICONTROL Planned Duration Minutes] field. </p> <p>[!UICONTROL Template Tasks] have a [!UICONTROL Planned Duration Minutes] field which displays the [!UICONTROL Planned Duration] of the task in minutes. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Expense Cost]</td> 
   <td> <p>The sum of the [!UICONTROL Planned Amounts] for all expenses logged for a project or a task.</p> <p><b>EXAMPLE</b></p>
   <p>If you create an expense for Task 1 and enter $600.00 in the [!UICONTROL Planned Amount] field, the [!UICONTROL Planned Expense Cost] for this task is $600.00. </p> 
   <p>For a project, [!DNL Workfront] uses the following formula to calculate [!UICONTROL Planned Expense Cost]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Hours]</td> 
   <td> <p>This field appears in the [!UICONTROL projects], [!UICONTROL tasks], and issues areas, reports for projects, tasks, or issues, and resource management tools like the [!UICONTROL Resource Planner], [!UICONTROL Workload Balancer] and the [!UICONTROL Utilization] report. </p> <p>It shows the number of hours that the Project Owner estimates that each task or issue should take to complete. For projects, it is generally a roll-up of the [!UICONTROL Planned Hours] from the tasks on the project. </p> <p>The [!UICONTROL Planned Hours] field might display different information depending on where you view it from. For information about Planned Hours, see <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Planned Hours overview</a>.</p> <p>Planned Hours are stored in minutes in the [!DNL Workfront] database. When writing calculations using this field, ensure you account for the fact that the hours display as minutes.<br></p> <p>By default, Planned Hours are distributed equally to all the days within the duration of a work item and also equally for all resources assigned to the task. Users can update the daily number of Planned Hours for a work item or the individual Planned Hours for each assignee.</p> <p>Updating this field differs for projects, tasks, and issues: </p> 
    <ul> 
     <li> <p>For issues, you can manually update this field. Issue Planned Hours are not added to the Project Planned Hours. </p> <p><b>TIP</b></p> <p>In an issue report, one of the [!UICONTROL Planned Hours] fields is replaced by the [!UICONTROL Work] field. The field displays the number of Planned Hours on the issue. For more information, see the "work" or "[!UICONTROL Work]" fields in this table. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>For tasks, you can manually update this field when the [!UICONTROL Duration Type] of the task is [!UICONTROL Calculated Assignment] or [!UICONTROL Simple]. This field is calculated by [!DNL Workfront] when the [!UICONTROL Duration Type] of the task is [!UICONTROL Calculated Work] or [!UICONTROL Effort Driven].<br>For information about [!UICONTROL Task Duration], see the article <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task [!UICONTROL Duration] and [!UICONTROL Duration Type]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>For projects, [!DNL Workfront] calculates the Planned Hours by adding all Planned Hours from all the tasks on the project. </p> </li> 
    </ul> <p><b>TIP</b></p> <p>You can display [!UICONTROL Planned Hours] in [!UICONTROL project], [!UICONTROL task], or [!UICONTROL issues] reports also by using text mode and reference additional fields. For more information, see the "<code>work</code>", "[!UICONTROL Work]", and "<code>workRequiredExpression</code>" fields in this table. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Labor Cost]</td> 
   <td> 
    <p>For a task, the hourly rate of the user or role multiplied by the number of hours assigned to the user or role.</p> <p>For a project, it is a total of all [!UICONTROL Planned Labor Costs] of all the tasks.</p> <p>Whether the rate of the user or role is used depends on the Cost Type that is selected for the given task. </p> <p>For more information, see <a href="../../../manage-work/projects/project-finances/track-costs.md">Track costs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Revenue]</td> 
   <td> <p>Tasks and projects can display a value for [!UICONTROL Planned Revenue] in [!DNL Workfront]. [!UICONTROL Planned Revenue] represents the amount of money associated with the [!UICONTROL Planned Hours] of the tasks on the project. For projects, it can also include the [!UICONTROL Fixed Revenue] of the project. </p> <p>For tasks, this is the revenue associated with the [!UICONTROL Planned Hours] of tasks. The Planned Hours from all tasks roll up to the Planned Hours of the project to contribute to the calculation of the project [!UICONTROL Planned Hours]. </p> 
   <p>[!DNL Workfront] calculates [!UICONTROL Planned Revenue] for tasks and projects using the following formulas:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>The project [!UICONTROL Planned Revenue] that displays in the [!UICONTROL Project Details] area and in project reports differs from the Planned Revenue that displays in the [!UICONTROL Utilization] report. </p> <p>The [!UICONTROL Planned Revenue] in the [!UICONTROL Project Details] area reflects the task revenue as well as the Fixed Revenue of the project. The [!UICONTROL Planned Revenue] in the [!UICONTROL Utilization Report] displays [!UICONTROL Planned Revenue] associated only with the tasks in the project. </p> 
     <p><b>EXAMPLE</b></p>  
      <p>If the project has 1 task with 10 hours, assigned to a Consultant with $20 hourly rate, and the project has $100 [!UICONTROL Fixed Revenue], the [!UICONTROL Utilization] report displays $200 for [!UICONTROL Planned Revenue] (the [!UICONTROL Planned Revenue] associated with the hours on the task). The [!UICONTROL Project Details] section displays $300 (the [!UICONTROL Planned Revenue] from the task and the Fixed Revenue for the project.) </p> 
    <p>For information about tracking revenue in [!DNL Workfront] see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Overview of Billing and Revenue</a>. </p> 
    <p>For information about [!UICONTROL Planned Revenue] calculations in the [!UICONTROL Utilization report], see <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">View resource utilization information </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Risk Cost]</td> 
   <td> <p>The total of the [!UICONTROL Potential Cost] of all the risks on the project factoring in their Probability of occurring. This amount is not included in the [!UICONTROL Planned Cost] of the project.</p> <p>The [!UICONTROL Planned Risk Cost] of a project is calculated by the following formula:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>An administrator-defined collection of Tabs and Portal Sections that appears on the [!DNL Workfront] Application [!UICONTROL Home] and other Dashboards.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>One component of a Tab on a Dashboard or Portal Page. Usually a single Report, Chart, Calendar, or list of key information.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Tab]</td> 
   <td>A Tab on a Portal or Dashboard that contains up to three Portal Sections.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>A collection of projects that have unifying characteristics. Those projects usually compete for the same resources, budget, or time slot. You can divide Portfolios into Programs and associate the projects with the Programs before they are added to a Portfolio.</p> <p>For more information about portfolios, see <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Portfolio overview in [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>A practice area focused on managing a collection or related programs and project efforts.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>A [!DNL Workfront] tool to assist in assessing and prioritizing projects within a portfolio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Owner]</td> 
   <td>The stakeholder responsible for the prioritization and budget for a portfolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Potential Risk Cost]</td> 
   <td>This is a project field that you can locate in lists and reports. It shows the potential cost for the risks associated with the project, should they occur. For more information see <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calculate Potential Risk Cost </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessor]</td> 
   <td> <p>A task that must be completed prior to the completion of a dependent task. Also a task that is marked as a [!UICONTROL Dependency] for another task. Predecessors allow the planner to set sequence-dependency logic, such as to start a task after another task finishes.</p> <p>For more information, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Company]</td> 
   <td>The Company that the user belongs to as designated in their user settings. Companies can also be associated with projects.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Contact]</td> 
   <td><p>The [!UICONTROL Primary Contact] is the creator of an issue and it is automatically designated by [!DNL Workfront] when the someone creates the issue. You can manually update this field if you have [!DNL Manage] permissions to the issue. An issue can have only one Primary Contact.</p> 
   <p>If you change the Primary Contact, the user originally designated as the primary contact still has [!UICONTROL Manage] access to the issue.</p>
   <p>When converting an issue to a task or a project, the user designated as the [!UICONTROL Primary Contact] of the issue becomes the [!UICONTROL Converted Issue Originator] of the project or task. If the [!UICONTROL Primary Contact] of the issue is updated after the issue was converted, the [!UICONTROL Converted Issue Originator] will be preserved as the [!UICONTROL Primary Contact] of the issue at the moment when the conversion happened. See also "[!UICONTROL Converted Issue Originator]" in this article.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>A value that can be assigned to a task, issue or a project to designate how important it is. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>On a [!UICONTROL Note] or [!UICONTROL Document], this option makes that object hidden to most viewers. For a Private Help Request Queue, only users on the Project Team can submit issues to that queue (or project) through the [!UICONTROL Requests] area.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profile]</td> 
   <td>All information about a user account.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>A subset within a portfolio, where similar projects can be grouped together in order to achieve a well-defined benefit.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Management]</td> 
   <td>Management of cross-project dependencies, risks, issues, requirements, and solutions to keep the program healthy and achieve the defined program benefit.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Owner]</td> 
   <td>The stakeholder responsible for supervising and organizing activities to ensure that project goals align with the company objectives.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progress]</span> </td> 
   <td> <p>In a [!UICONTROL Goal] report, this displays the percent of how close a strategic goal is to completing. The percent of progress displays as a number. For information about strategic goals, also see "[!UICONTROL Goal]" in this table.</p> <p>This field is visible only if your organization has purchased [!DNL Workfront] Goals. For information about managing strategic goals using [!DNL Workfront Goals], see <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Add projects to goals in [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progress Status]</td> 
   <td> <p>In a Project, Task, and Goal report, this field displays the Progress Status of projects, tasks, or strategic goals. For more information, see the following articles:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Project Progress Status overview</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Task Progress Status overview</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Overview of goal progress and condition in [!DNL Adobe Workfront Goals]</a> </p>
     <p>The [!UICONTROL Goal] report and the [!UICONTROL Progress Status] for [!DNL goals] field are visible only if your organization has purchased [!DNL Workfront Goals]. For information about strategic goals in [!DNL Workfront Goals], see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] overview</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>A large amount of work that must be completed within a specific timeframe and must use a specific budget and number of resources. To make it manageable, you divide the project into a series of tasks. Completing all the tasks results in the completion of the project. For information about planning a project, see <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Plan a project overview</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Assignment Planned Hours]</td> 
   <td> <p>In an [!UICONTROL Initiative Job Role] report, this displays the number of [!UICONTROL Planned Hours] associated with a job role assigned to tasks or issues in the project. This field and the [!UICONTROL Initiative Job Role] report type do not display in your [!DNL Workfront] instance unless your company has purchased a [!DNL Workfront Scenario Planner] license. For information about the [!DNL Workfront Scenario Planner], see <a href="../../../scenario-planner/scenario-planner-overview.md">The [!DNL Workfront Scenario Planner] overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Details]</td> 
   <td>The details of the current status of a Project.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Budgeted Cost]</td> 
   <td> <p> This is the [!UICONTROL Budgeted Cost] of a project as it displays in lists and reports.</p><p>See also "[!UICONTROL Budgeted Cost]" in this article.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>A set of policies that governs the thresholds for project creation, categorization, and naming of the projects.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Project Overhead]</td> 
   <td>In an [!UICONTROL Hour] report, this field is reserved for financial information tied to the hours logged with the hour type of [!UICONTROL Project Time]. Projects can have their own Billing Rates and if an hour is logged directly on a project, then those rates will be used in calculations. Based on the project settings, projects can also have different currencies and there can be a currency conversion for those hours. The [!UICONTROL Project Overhead] object allows [!DNL Workfront] to get that information.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Owner]</td> 
   <td>The user responsible for managing the scope, timeline, and assignments of a project. The default approver for change orders, financial changes, and deliverables.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Planning]</td> 
   <td>Processes to develop and maintain the project schedule.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Sponsor]</td> 
   <td>A designated stakeholder profile that each of your user's should relate to. In [!DNL Workfront], these are designated as [!UICONTROL Access Levels]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Teams]</td> 
   <td> <p>The collection of users or roles assigned to a project</p> <p>For more information, see <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Project Team overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project tracking]</td> 
   <td>The data used to measure the health and scope of a project</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projected]</td> 
   <td> <p>An estimate of the timestamp of when the work will be completed based on the planned hours and percentage complete of a task, issue, or project.</p> <p>This refers to dates or the [!UICONTROL Duration] of tasks, issues, or projects. Usually, it designates dates and durations that are more true to the life of the work items, after some work has already been completed or some time has passed. </p> <p>For example, the [!UICONTROL Projected Completion Date] of a task is the date when [!DNL Workfront] estimates that the task will complete, based on how much work has been done on it so far, how many people are assigned to it, and how much time has passed since the start date.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Deadline]</td> 
   <td> <p>In reports that contain the [!UICONTROL Document Version] object (such as a [!UICONTROL Document Version] report and [!UICONTROL Proof Approval] report), This field displays the day of the week, date, time of day, and year of the proof deadline.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Decision]</td> 
   <td> <p>In reports that contain the [!UICONTROL Document Version] object (such as a [!UICONTROL Document Version] report  and [!UICONTROL Proof Approval] report), this field displays the decision status of the proof (pending, changes required, or approved)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td> <p>In reports that contain the [!UICONTROL Document Version] object (such as a [!UICONTROL Document Version] report and [!UICONTROL Proof Approval] report), this field displays the proof name.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Pages]</td> 
   <td> <p>In reports that contain the [!UICONTROL Document Version] object (such as a [!UICONTROL Document Version] report and [!UICONTROL Proof Approval] report), this field displays the number of pages included in the proof.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Progress]</td> 
   <td> <p>In reports that contain the [!UICONTROL Document Version] object (such as a [!UICONTROL Document Version] report and [!UICONTROL Proof Approval] report), displays the progress status of the proof ([!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Commented], [!UICONTROL Decision Made]).</p> <p>For more information, see <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Proof progress overview</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Proof progress and status overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>A review process where one or more users mark and comment on content that should be changed in an image, a text document, a video, or interactive web content.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>On a [!UICONTROL Note] or [!UICONTROL Document], this option makes that object accessible to other users, or even people from outside [!DNL Workfront]. For a [!UICONTROL Help Request Queue], [!UICONTROL Public] means that all users that can submit issues to a project can submit issues through the [!UICONTROL Requests] area.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>The perception of work quality within the organization.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue]</td> 
   <td>Also called Help Desk Queue or [!UICONTROL Help Request Queue]. This is a project that has been published to the [!UICONTROL Requests] area to allow users to submit issues to it. Usually queues are created for particular topics, such as [!UICONTROL Bugs], [!UICONTROL Project Requests], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Properties]</td> 
   <td>These settings define issue submission rules for a project that is being published to the [!UICONTROL Requests] area.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Topic]</td> 
   <td> <p>A property on a [!UICONTROL Help Request Queue] that allows users submitting an issue to select a Topic. Topics can:</p> 
    <ul> 
     <li>Be associated with a Custom Data Form.</li> 
     <li>Assign the issue automatically to a user, role, or team through the Routing Rule set on the selected Topic.</li> 
     <li>Move the issue to a different project or queue through the routing rule set on the selected topic.</li> 
    </ul> <p>For more information, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Create Queue Topics</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>In an [!UICONTROL Access Level] report, you can manually indicate a [!UICONTROL Rank] of the [!UICONTROL Access Level]. This helps you, as the [!DNL Workfront] administrator, to visually identify the level of complexity associated with each Access Level. For example, you can give lower numbers for more complex ([!UICONTROL Plan]-level) Access Levels, and higher numbers for less complex ([!UICONTROL Requester]-level) Access Levels. You cannot rank the standard Access Levels. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>This field on a task report indicates whether an [!UICONTROL Agile] task has been marked as [!UICONTROL Ready] on the backlog. This flag only applies to [!UICONTROL Agile] tasks, which are tasks assigned to an [!UICONTROL Agile] team. </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Recurrence Frequency]</td> 
   <td> <p>A field that displays in the [!UICONTROL Task Details] or the [!UICONTROL Edit Task] box of a parent of recurring tasks. It is the frequency with which the tasks in the recurrence occur. For information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference Number]</td> 
   <td> <p>Projects, tasks, and issues are automatically associated with a unique reference number as they are created. You can view the [!UICONTROL Reference Number] in the [!UICONTROL Details] page of projects, tasks, or issues, or in a list or report. </p> <p><b>TIP</b><p><br>You can defer to reference numbers when two items have the same name, as reference numbers are always unique. </p> <p>[!DNL Workfront] automatically generates sequential reference numberss at the system level. Each project, task, or issue gets the next available number in the sequence. <br></p> <p>For example, if User A creates a task, [!DNL Workfront] might automatically assign the task the Reference Number of 100. If User B creates an issue right after this, [!DNL Workfront] assigns the issue the Reference Number of 101. You cannot manually edit Reference Numbers. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rejection Issue]</td> 
   <td>In a project or a task report, this is the issue that is created when the approval for the project or the task is rejected. For information about rejection issues, see the article <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>. </td> 
  </tr> 
  
<tr>
  <td>Relationship types</td>
  <td><p>Workfront objects are always connected to each other using one of the following relationship types:</p> 
  
  <ul><li> <b>One to many</b>: In this relationship, one object can be connected to multiple other objects of different types. For example one project can have multiple tasks. The Project-Tasks relationship is a one to many relationship. You cannot display this relationship in a report using the Standard interface. You must use text mode reporting to view one to many relationships.</li>
  <li><b>One to one</b>: In this relationship, one object can only be connected to one other object of a different type. For example, a project can only have one Group. The Project-Group relationship is a one to one relationship. You can display one to one relationships between objects in a Standard report.</li>
  <li><b>Many to one</b>: In this relationship, multiple objects can be connected to only one other objects of a different type. For example multiple tasks can be connected to the same project. The Tasks-Project relationship is a many to one relationship. You can display many to one relationships between objects in a Standard report. </li>
  <li><b>Many to many</b>: In this relationship, multiple objects of the same type can be connected to multiple objects of a different type. For example, several users can belong to multiple Other Teams, and the teams can belong to several users. You cannot display this relationship in a report using the Standard interface. You must use text mode reporting to view many to many relationships. </li> </ul>
  </td></tr>
<tr> 
   <td>[!UICONTROL Remaining Risk Cost]</td> 
   <td> <p>A project field that shows the difference between the [!UICONTROL Planned Risk Cost] of a project and the total of all [!UICONTROL Actual Costs] of all risks on the project. </p> <p>The [!UICONTROL Remaining Risk Cost] for a project is calculated using on the following formula:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 

  <tr> 
   <td>[!UICONTROL Replanning]</td> 
   <td>Changing the dates of a project to repair or overcome problems. For example, a project that has been on hold for several months would need to be replanned to reflect accurate dates. This is a manual operation of adjusting either the dates of the project or those of the tasks. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>A chart or table containing information about one given [!DNL Workfront] object and its related attributes.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>A type of issue that is triaged in a single centralized queue and is unrelated to an ongoing work effort.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request Queue]</td> 
   <td>The backlog of issues that is managed by a traffic and triage process.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Request velocity]</td> 
   <td>Total work cycle time to intake and complete a request.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>Typically a license type. A user with a Requester license can submit requests for new work to occur in the system.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reserved Time]</td> 
   <td>Days specified on a user's Personal Time, indicating that the user will not be available for work. See "[!UICONTROL Non Work Days]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Issue]</td> 
   <td> <p>In an issue report, use this field in views or filters to refer to the issue that resolves the issue. </p> <p>For information about displaying resolving objects in reports, see <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">View Resolvable and Resolving Object information in a report</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Project]</td> 
   <td> <p>In an issue report, use this field in views or filters to refer to the project that resolves the issue. </p> <p>For information about displaying resolving objects in reports, see <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">View Resolvable and Resolving Object information in a report</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Task]</td> 
   <td> <p>In an issue report, use this field in views or filters to refer to the task that resolves the issue. </p> <p>For information about displaying resolving objects in reports, see <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">View Resolvable and Resolving Object information in a report</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>Users or roles that exist in [!DNL Workfront] and are assigned to Project Teams, tasks, and issues. They are responsible for completing the work associated with projects, tasks, or issues. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management] is an enterprise set of tools that allows you to accurately forecast the use of your resources based on their availability so that the work that must be done is completed on time and on budget. </p> <p>With Resource Management tools you can plan long-term capacity and short-term scheduling needs for your resources. </p> <p>For information about Resource Management in [!DNL Workfront], see <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Get started with Resource Management</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager IDs]</td> 
   <td><p>In a project report, you can use this option when creating a filter to find a specific resource manager. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Managers]</td> 
   <td> <p>In a project report or list view, this is an informational field that displays users designated to perform resource management activities on the project.  When you use "[!UICONTROL Resource Managers]" in a report, a list of resource managers is displayed, with each resource manager on the project separated by a comma. You can designate up to 30 resource managers on a given project.</p> <p>For more information, see the article <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Designate Resource Managers for a project or template </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
   <td>The hours budgeted for the project and the resources associated with it in the [!UICONTROL Resource Planner]. See also "[!UICONTROL Budgeted Hours]" in this article. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>An advanced [!DNL Workfront] tool that lets you view and manage resources across projects, job roles, or users. For information, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Labor Cost]</td> 
   <td> <p>These is the cost associated with the hours budgeted for project job roles using the Resource Planner. </p> <p>See also "Budgeted Labor Cost" in this article. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Resource Pools]</td> 
   <td> <p>Resource Pools are collections of users that can be associated with a project. The users in the same Resource Pool usually belong to the same department, have similar or complementary skills, or are funded by the same budget. You can associate multiple Resource Pools to a project or to a user. A resource pool can be assigned exclusively to a project or shared by several projects.</p> 
   <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> 
   <p>In project reports, Resource Pools show all the pools associated with a project. This object cannot be used in a grouping.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Utilization]</td> 
   <td>A Report displaying the number of hours available during a certain time period and the number of hours scheduled for each user in the report. This is also calculated into [!UICONTROL Average Hours Per Day] and an allocation percentage.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Result]</td> 
   <td>In [!DNL Workfront Goals], a result is a progress indicator for a goal. It can be a number, a percentage value, or a currency amount that you update manually. You cannot display results in a report and you cannot access them through the [!DNL Workfront] API. For information about activities, see <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Get started with results and activities in Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>A billable amount for the task or project. The amount can be hourly, fixed, or a combination of both.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revenue Type]</td> 
   <td>Revenue type determines how the task will accrue revenue. Some examples include [!UICONTROL Fixed Hourly], [!UICONTROL Role Hourly], and [!UICONTROL Role Hourly w/Cap]. For information about tracking revenue in [!DNL Workfront] see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>Typically a license type. A user with a [!UICONTROL Reviewer] license has the ability to review and approve work items in the system.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk]</td> 
   <td> <p>This may refer to the following concepts in [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>A field on a project that indicates how risky a project can be. You can prioritize the execution of your projects based on the level of risk. Projects can have the following levels of risk:</p> <p>- [!UICONTROL Very Low]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL High]</p> <p>- [!UICONTROL Very High]</p> <p>The levels of risks you indicate for a project cannot be customized. </p> <p> For information about updating the Risk of a project, see the " Project  Settings" section of the article <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>. You can display the risk field of a project in reports. </p> </li> 
     <li> <p>An event that might occur during the life of a project that identifies a potential impact to the cost, scope, or schedule of the project. You define potential risks to a project and associate a probability of them occurring or a cost as you build the project's Business Case. For information about adding risks to the Business Case of the project, see "Create and edit risks on projects". </p> <p>You cannot display risks defined in the [!UICONTROL Business Case] in reports. You can only display several types of Risk Costs in reports and lists. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Cost]</td> 
   <td> <p>The cost associated with the risks on a project. The following are risk costs associated with projects that you can display in reports:</p> 
    <ul> 
     <li> <p>[!UICONTROL Actual Cost]: a field on a risk that shows the actual cost for the risk that has occurred. In addition to reports and lists, you can locate it in the [!UICONTROL Edit Risk] box when editing or creating a risk. </p> <p>For project, task, or issue costs, see "[!UICONTROL Actual Cost]" in this article. </p> </li> 
     <li> <p>[!UICONTROL Planned Risk Cost]: a field on the project that shows a total of all [!UICONTROL Potential Risk Costs] for the project. See also "[!UICONTROL Planned Risk Cost]" in this article. </p> <p>For information about Potential Risk Cost, see <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calculate Potential Risk Cost </a>. </p> </li> 
     <li> <p>[!UICONTROL Remaining Risk Cost]: a field on the project that displays the difference between the total of the [!UICONTROL Actual Costs] of all risks and the [!UICONTROL Planned Risk Cost]. See also "Remaining Risk Cost" in this article. </p> </li>
    </ul> </td> 
  </tr> 
  
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Management]</td> 
   <td>Processes to identify, mitigate, and monitor risk.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td>See "[!UICONTROL Job Role]" in this article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>Automatically assigning or moving an issue, usually due to a Queue Topic or by way of being the Default Route (Routing Rule) for the queue.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing Rule]</td> 
   <td>A setting on projects and queue topics that automatically assigns an issue to a user, role, or team, or moves the issue to another project or queue topic. Routing Rules are generally used with Help Request Queues to automatically assign incoming issues.</td> 
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
   <td>[!UICONTROL Saved Search]</td> 
   <td>A search for which the search criteria have been saved. Saved Searches make it easy to run the same each again without having to enter the search criteria again.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Scenario] (in [!DNL Workfront Fusion]) </td> 
   <td> <p>A scenario is comprised of a series of steps (modules) that indicate how data should be transferred and transformed between apps/ services.</p> <p>For information about scenarios in [!DNL Workfront Fusion], see <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] scenario overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario] (in the [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>In the [!DNL Scenario Planner], a scenario is a copy of a plan. </p> <p>The [!DNL Scenario Planner] requires an additional license. For information about the [!DNL Workfront Scenario Planner], see <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The [!DNL Scenario Planner] overview</a>. </p> <p>For information about creating scenarios, see <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Create and compare plan scenarios in the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule]</td> 
   <td>The weekly work schedule, including working times, combined with Days off (such as Holidays) and exception days (such as a Saturday work day). Yiu can associate schedules with projects and users.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule Exemption]</td> 
   <td>Also known as a [!UICONTROL Modified Shift]. Days scheduled in contrast to the regular weekly working times as defined by the schedule. For example, a Saturday scheduled to work, when the Schedule is set up to only Work Monday Through Friday, would be a [!UICONTROL Schedule Exemption].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scheduled Report]</td> 
   <td> <p>When you build a report of reports, you can display information about the schedules of the report, if the report is scheduled for delivery using the [!UICONTROL Scheduled Report] field. This field shows multiple values, one for each schedule of each report, in a bulleted list. For more information about scheduling reports, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Report delivery overview</a>.</p> <p>Because this field shows multiple values, it cannot be used in a grouping. You can access it only in a filter or a view. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scope Change]</td> 
   <td>An [!UICONTROL Audit Trail] that, if active, generates a note anytime a change is made to the Scope of a project or task, such as if a [!UICONTROL Task Duration] or the [!UICONTROL Predecessors] are changed.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>An area on the screen, with its own header, created to organize the Custom Data for display purposes.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section Break]</td> 
   <td>A gap or border between sections.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>The settings that allow a user to interact with certain objects in the system and not others. See also "[!UICONTROL Access Levels]" in this article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>The area where administrators can set up system configurations and preferences.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severity]</td> 
   <td> <p>[!UICONTROL Severity] is an indication of how likely an item is to impact the completion of the work. For example, an issue with high [!UICONTROL Severity] may completely block a task's completion, but an issue with low [!UICONTROL Severity] may be merely cosmetic.</p> <p>For more information, see <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Update issue severity</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severities]</td> 
   <td>See "[!UICONTROL Severity]" in this article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>The action of allowing other Users to view or edit a specific item in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack Date]</td> 
   <td>In a task view or report, the [!UICONTROL Slack Date] displays the exact date when a task could definitely impact the [!UICONTROL Completion Date] of the project. For information about the [!UICONTROL Slack Date] of a task, see <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Task Slack Date overview</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assignments]</td> 
   <td> <p>When assigning tasks or issues to users, [!DNL Workfront] makes recommendations ([!UICONTROL Smart Assignments]) about who the best users are to complete the work, based on the time they have available to complete it and their relationship to the project.</p> <p>For more information , see <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Smart assignments overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Indicates the parent object of another object. For example, a document attached to a task has the name of the task in the [!UICONTROL Source] field of a [!UICONTROL Document] report or view; an issue logged under a project has the name of the project in the [!UICONTROL Source] field of an Issue report or view. </p> 
   <p>The following reports display a Source column where you can view information about the parent object:</p>
  <ul><li>Issue reports</li>
    <li>Hour reports</li>
    <li>Document reports </li>
    </ul>
   <p>If users don't have permissions to the parent object of an issue, hour, or document, the Source column of the report displays empty, even when the report is configured to display, or to be delivered with the access rights of another user. </p>
   <p> In order to show information about the parent object in the report, we recommend adding a column for the parent object where you can display the name of the parent. </p>
    <p>For example, you can add any of the following to a report with a Source column: </p>
    <ul><li>The Project Name, Task Name, or Issue Name columns to a document or hour report.</li>
    <li>The Project Name or Task Name columns to an issue report. </li> </ul>
    For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Run and deliver a report with the access rights of another user</a> 
   
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start Date]</td> 
   <td> <p>The Date when the work on an item is set to start. There are several Start Dates in [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL Planned]</li> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL Projected] </li> 
    </ul> <p>In a [!UICONTROL Rate report], this is the date when a new billing rate for a job role at the project level starts. The hours associated with the project that are after this date are multiplied by this billing rate to calculate the revenue on the project. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>An indicator used to signal a workflow position of a work item or of a strategic goal.</p> <p>For projects, the [!UICONTROL Status] is a setting on the project that indicates whether the project is:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL On Hold] </li> 
     <li>[!UICONTROL Complete] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>For more information on a project's Status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Access the list of system project statuses</a>.</p>
    <p>For tasks, the [!UICONTROL Status] is a setting on the task that indicates whether the task is:</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Complete]</li> 
    </ul> <p>For more information on task Status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Access the list of system task statuses</a></p> <p>For issues, the [!UICONTROL Status] is a setting on the issue that indicates whether this issue is:</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Awaiting Feedback]</li> 
     <li>[!UICONTROL On Hold]</li> 
     <li>[!UICONTROL Resolved]</li> 
     <li>[!UICONTROL Won't Resolve]</li> 
     <li>[!UICONTROL Cannot Duplicate]</li> 
     <li>[!UICONTROL Verified Complete]</li> 
     <li>[!UICONTROL Reopened]</li> 
    </ul> <p>For more information on issue Statuses, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Access the list of system issue statuses</a>.</p> 
    <p>For strategic goals, the [!UICONTROL Status] is a setting on the goal that indicates whether the goal is:</p> 
     <ul> 
      <li>[!UICONTROL Active]</li> 
      <li>[!UICONTROL Draft]</li> 
      <li>[!UICONTROL Inactive]</li> 
      <li>[!UICONTROL Closed]</li> 
     </ul> 
     <p>For more information about strategic goals, also see "[!UICONTROL Goal]" or "[!UICONTROL Goals]" in this article. </p> 
     <p>For strategic goals, this field is visible only if your organization has purchased [!DNL Workfront Goals]. For information about managing strategic goals using [!DNL Workfront Goals], see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] overview</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Change]</td> 
   <td>An [!UICONTROL Audit Trail]. A note is generated when a user changes the Status of the project, task, or issue.</td> 
  </tr> 
  <tr> 
   <td>Status Icons</td> 
   <td> <p>You can add the built-in [!UICONTROL Status Icons] field as a column in your views to enhance visibility into key points about your objects, like:</p> 
    <ul> 
     <li>An object has documents attached</li> 
     <li>An object is associated with an approval process</li> 
     <li>An object has additional notes associated with it</li> 
     <li>An expense is billable or reimbursable </li> 
     <li>A task is on a critical path</li> 
     <li>A user belongs to a company, a team, or is located in a different time zone </li> 
    </ul> <p>You can add the [!UICONTROL Status Icons] field in the views of the following objects: </p> 
    <ul> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Template Tasks]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Users]</li> 
    </ul> <p>For more information, see <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Built-in Status Icons in Views</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Update]</td> 
   <td> <p>In a project, task, or issue report, this field shows the most recent status update that object owners have provided in the '[!UICONTROL Updates]' area. For projects, this means that comments made by the Project Owner, and for tasks and issues, this means that comments made by the assignees.</p> 
   <p> Comments made when updating the status of an object do not display in the [!UICONTROL Status Update] column.</p> <p>To show the '[!UICONTROL New],' '[!UICONTROL In Process],' and '[!UICONTROL Complete]' statuses, use the [!UICONTROL Status] column.</p> <p>For more information on statuses, see the article <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Update task status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statuses]</td> 
   <td>See "[!UICONTROL Status]" in this article.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>A chart that represents the status of stories (tasks in the agile methodology) and how they are progressing toward completion.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Hours]</td> 
   <td>A metric used to measure the difficulty or complexity of a Story. Agile teams can choose whether to use Hours or Points.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>A metric used to measure the difficulty or complexity of a Story. Agile teams can choose whether to use Hours or Points.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>Long-term work that changes the organization or how the organization works.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategic Alignment]</td> 
   <td>Measuring and aligning company goals across portfolios and programs.</td> 
  </tr>

  <tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>This is used in report columns when using the Text Mode interface. </p>
   <p>The <code>[!UICONTROL stretch]</code> is used to identify which columns occupy extra space not needed by the view. The user interface width of the workspace for a typical user is about 850 pixels. This means that if you have a view with four
   columns (150 pixels each) that your view occupies 600 of 850 pixels. There are 250 extra pixels in the UI that will be added to the columns that have a stretch percentage provided. </p>
   <p>The stretch of a column is enforced when you use the additional line of code: <code>[!UICONTROL usewidths=true]</code> for at least one of the columns in the view. 
   </td> 
  </tr>

  <tr> 
   <td>[!UICONTROL Subscribers]</td> 
   <td> <p>Users that subscribe to projects, tasks, or issues.</p> <p>When you use this field in a report, a list of subscribers displays, with each subscriber separated by a comma.</p> <p>For more information, see the article <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Subscribe to items in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Summary Task]</td> 
   <td>See "[!UICONTROL Parent Task]" in this article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtask]</td> 
   <td>A child task, which is located under a parent task.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System Governance]</td> 
   <td>A set of policies that governs changes and maintenance of a system.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL System Integration]</td> 
   <td>The process of linking together different computing systems and software applications physically or functionally in order to act as a coordinated whole.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task]</td> 
   <td> <p>An activity that must be performed as a step toward achieving a final goal (completing the Project).</p> <p>For more information, see <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Tasks overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Attribute]</td> 
   <td>Other fields or objects that are associated with a task and indicate certain details about the task. Some examples are [!UICONTROL Planned Completion Date] and [!UICONTROL Status].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Constraint]</td> 
   <td>See "[!UICONTROL Constraint Type]" and "[!UICONTROL Constraint Date]".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Management]</td> 
   <td>A set of policies that governs the thresholds for task creation, assignment, closure, and visibility.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Owner]</td> 
   <td>The team or user responsible for the estimation of effort and completion of the task</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>A collection of users working toward similar goals or business objectives. These users can be collectively assigned to a work item by assigning the team to the work item.</p> <p>For more information on Teams, see <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Teams overview</a>.</p> <p>Projects can have a [!UICONTROL Project Team], which contains all the users or roles associated with the work on the project.</p> <p>For more information about Project Teams, see <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Project Team overview</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>Project templates are generic outlines of your most repeatable projects. You can define tasks, queue topics, custom forms, attach documents or approvals when you create a project template to save you time when you must create a new project. </p> <p>You can attach templates to existing projects, or you can use them to build new projects. All the information specified on the template transfers to the projects that are created using it. </p> <p>For more information about templates, see <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Project template overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Template Task]</td> 
   <td>A task that is part of a template. Template Tasks become Tasks in the project that is created by using the template.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>A [!UICONTROL Note] and its collection of replies that relate to a particular topic.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thumbnail]</td> 
   <td> <p> In a [!UICONTROL Document] list or report, it displays a preview of the document in a thumbnail. </p> <p> Select <strong>[!UICONTROL Thumbnail]</strong>  to view a 33-66 pixel-wide thumbnail in the report. </p> <p>The size of the thumbnail adjusts when you modify the width of the column in a list or report.</p> <p>See also "[!UICONTROL Large Thumbnail]" in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>You can build a [!UICONTROL Time Off] report to view when users have indicated time off in their profile. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet]</td> 
   <td> <p>A timecard that allows users to enter actual hours that they spent working on projects, tasks, or issues, or hours they spent for other activities not related to work, like meetings or training. In addition to entering the amount of time you spent working, you can also indicate whether the time is work-related or it amounts to overhead time by using Hour Types to define your time entries. For information about timesheets, see <a href="../../../timesheets/timesheets/timesheets-overview.md">Timesheets overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet Profile]</td> 
   <td> <p>A [!UICONTROL Timesheet Profile] is a template that [!DNL Workfront] uses to automatically create timesheets for the users associated with them. </p> <p>You can configure a number of settings that will apply to each timesheet as it is created. Some of these settings are: how often the timesheet should be created (weekly, every other week, twice a month, or monthly), the start day of the timesheet, the timesheet approvers, the available [!UICONTROL Hour Types] that users can associate with recorded hours.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL Top Parent ID] </td> 
   <td> <p>This field allows you to identify and filter data about a top-level group and its subgroups in a list or report.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Top Parent Name] </td> 
   <td> <p>This field allows you to identify data about a top-level group and its subgroups in a [!UICONTROL View] for a list or report.</p> <p>You can also do this using the [!UICONTROL Top Parent ID] field.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Hours]</td> 
   <td> <p>In a [!UICONTROL project report], this field displays the rounded sum of all hours on the project, the last time the project finances were calculated. [!UICONTROL Actual Hours] reflect the exact hours logged on the project. Typically, the [!UICONTROL Actual Hours] should match the [!UICONTROL Total Hours]. If the [!UICONTROL Total Hours] appears significantly different from the [!UICONTROL Actual Hours] field, you must Recalculate Finances on the project.</p> <p>For more information about recalculating project finances, see the article <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Recalculate project finances</a>.</p> <p>In a timesheet [!UICONTROL Standard] view, this field refers to the total hours logged for items for the dates displayed on a timesheet. The [!UICONTROL Total Hours] field for timesheets in this built-in view references the "[!UICONTROL hoursDuration]" field which dynamically calculates the difference in hours between the timesheet Start and End dates. This is used to display the [!UICONTROL Total Hours] column in red if the user logs more time than the available hours in the timesheet's time frame. For more information, see <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">View total hours on the timesheet</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracking Mode]</td> 
   <td> <p>An attribute of a task. This determines how and when the Projected timelines will be updated for a task. For example:</p> 
    <ul> 
     <li>[!UICONTROL User Must Update] requires that a task be updated manually. Otherwise, it will become [!UICONTROL Behind Schedule], then [!UICONTROL Late].</li> 
     <li>[!UICONTROL Auto Complete] will automatically complete a task when the Due Date, or [!UICONTROL Planned Completion Date], has passed.</li> 
    </ul> <p>For more information, see <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Task Tracking Mode overview</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>An event that starts a scenario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trouble Task]</td> 
   <td>An incomplete task with a condition of [!UICONTROL Late], [!UICONTROL Behind Schedule], or [!UICONTROL At Risk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unassigned Task]</td> 
   <td>A task that is not assigned to any User, Role, or Team.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Update Type]</td> 
   <td> <p>A setting on a project that determines when the project's Projected timeline will be recalculated. The [!UICONTROL Update Type] can have the following values:</p> 
    <ul> 
     <li>[!UICONTROL Automatic and On Change]</li> 
     <li>[!UICONTROL Automatic Only]</li> 
     <li>[!UICONTROL Manual Only] </li> 
    </ul> <p>For more information, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User]</td> 
   <td>An account created in [!DNL Workfront] to allow a person to log in and interact with the system.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL User Delegation]</p> </td> 
   <td> <p>A reportable object that tells you:</p> 
    <ul> 
     <li>Which users have delegated task, issue, and project approvals</li> 
     <li>Which users have had task, issue, and project approvals delegated to them</li> 
     <li>When these delegations start and end</li> 
    </ul> <p>To learn more, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Create a User Delegation report</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface]</td> 
   <td>All visual and interactive aspects of the [!DNL Workfront] application.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface Preferences]</td> 
   <td>[!UICONTROL User Interface Setup]. [!DNL Workfront] administrators can change these settings to customize aspects of the user interface.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilization]</td> 
   <td>The availability for a user or role based on the assigned schedule, PTO, and current workload.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Utilization]</td> 
   <td> <p>A search combined with a report that shows how Users (Resources) are allocated or over-allocated. See "[!UICONTROL Resource Utilization]" in this article.</p> </td> 
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
   <td>[!UICONTROL Velocity]</td> 
   <td>A measure of the total work cycle time (how long it takes to complete a piece of work) and how frequently work is done in the time originally committed (work-to-commit ratio).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL View]</td> 
   <td> <p>Views refer to a reporting element which allows you to modify the columns in a report or in a list of objects.</p> 
   <p> View also refers to a user's right to only view information on an object, according to their access level or at a permissions sharing level on that object.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL View Icons]</td> 
   <td> <p> This is the same field as Status Icons, but it is only available for the following views: </p> 
    <ul> 
     <li> [!UICONTROL Documents] </li> 
    </ul> <p> For more information, see the article <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Built-in Status Icons in Views</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Month]</td> 
   <td> <p>In a report list, it displays the number of times the report has been viewed during the last month.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Quarter]</td> 
   <td>In a report list, it displays the number of times the report has been viewed during the last quarter.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >View report usage</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Year]</td> 
   <td>In a report list, it displays the number of times the report has been viewed during the last year.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Month]</td> 
   <td> <p>In a report list, it displays the number of times the report has been viewed during this month.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Quarter]</td> 
   <td>In a report list, it displays the number of times the report has been viewed during this quarter.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">View report usage</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Year]</td> 
   <td>In a report list, it displays the number of times the report has been viewed during this year.<br>For more information about usage information in report lists, see the article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">View report usage</a>.</td> 
  </tr> 
  
  <tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> In a report, when using the [!UICONTROL Text Mode] interface, the line of code where you can specify the width of each column in pixels. Workfront provides a suggested width for each field,
though depending on the type of field and format, you may want to make adjustments.
You must use the additional <code>[!UICONTROL usewidths=true]</code> line of code to enforce the width specified for the column. 
  </td>

  </tr>
  
  <tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>In a project, task, or issue report, using the following statement in text mode displays the Planned Hours of the project, task, or issue:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>For information about using text mode, see <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Text mode syntax overview</a>. </p> 
   <p><b>TIP</b> 
   <p>In an issue report, adding one of the [!UICONTROL Planned Hours] fields adds the <code>work </code>field to the report. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>One of the two primary License Types. This has less access than [!UICONTROL Plan], but can create and make updates in the system. A user with a Work license has more abilities than an [!UICONTROL External], [!UICONTROL Reviewer], or [!UICONTROL Requester] license holder.</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] licenses overview</a>.</p> <p>Work might refer to the number of [!UICONTROL Planned Hours] for a project, task, or issue. For more information, see the "[!UICONTROL work]" field in this table. </p> <p><b>TIP</b></p> <p> In an issue report, adding one of the [!UICONTROL Planned Hours] fields adds the <code>work </code>field to the report. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Breakdown Structure]</td> 
   <td>A hierarchical structure of the tasks to be executed by the project team based on the parent/ child relationship.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Effort] </td> 
   <td> 
    <p>A project manager might decide to use this field instead of [!UICONTROL Planned Hours] to estimate the effort needed to complete a task. This field is visible only when the following conditions are met:</p> 
     <ul> 
      <li> <p>The task has a [!UICONTROL Simple Duration Type]. </p> <p><b>TIP</b></p> <p> If you update the task [!UICONTROL Duration Type] to any other type, this field becomes hidden. </p> </li> 
      <li>The project manager has enabled the [!UICONTROL Use Work Effort] to automatically calculate task [!UICONTROL Planned Hours] field on the project. </li> 
     </ul> 
     <p>For information about using [!UICONTROL Work Effort] instead of [!UICONTROL Planned Hours] to estimate task effort, see <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort overview</a>. </p> 
     <p>You can display this field in task reports and lists.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Item]</td> 
   <td> <p>This field refers to either tasks or issues in [!DNL Workfront]. </p> <p>The [!UICONTROL Work Item] report displays information for both tasks and issues. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management mix]</td> 
   <td>A [!UICONTROL Work Performance Indicator] (WPI) of the proportion of work allocated to run your business versus change your business. The Mix WPI helps you understand, at an organizational level, whether your strategy has any real work allocation applied to it.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Resource]</td> 
   <td>A designation of a persona in the system who is eligible to receive work or track time.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Role and Responsibilities]</td> 
   <td>Defining the owners and stakeholders for managing the scope, execution, and approvals of the designated issue, task, project, program, or portfolio.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management SLA]</td> 
   <td>A quantifiable metric agreed upon by all stakeholders.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Stakeholder]</td> 
   <td>A collection of users with a vested interest in the outcomes of a work request.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management touchpoints]</td> 
   <td>Digitized records of communication between stakeholders.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Performance Indicators] </td> 
   <td> <p>Mix ratio, capacity, velocity, quality, and engagement.</p> <p>WPI is a common acronym for [!UICONTROL Work Performance Indicator].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Process]</td> 
   <td> <p>The method in which work is received, prioritized, and executed. The way you execute the work is typically called "the workflow" or "project plan" (a list of tasks with dates, predecessor relationships, and so forth). </p> <p>Examples of a work process might be the production of a single asset or the delivery of a multi-asset campaign. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Workflow template]</td> 
   <td>In the [!UICONTROL Proof Approval] report, this field displays any workflow templates attached to a proof. If there are no templates attached, the column is blank.</td> 
  </tr>

  <tr> 
   <td>[!UICONTROL Work Time]</td> 
   <td>  
 
   <p>Represents the percentage of the Full Time Equivalent ([!UICONTROL FTE]) time that the user is available for actual work, not including overhead. [!UICONTROL Work Time] must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.</p>
   </p>The field's default is 1, indicating that a user spends their entire [!UICONTROL FTE] on actual, project-related work.  </p>
   <p>The system uses this number to calculate the availability of the user for actual, project-related work. </p>
   <p> Schedule exceptions and time off might also affect the user capacity. </p>
   <p>For more information about creating schedules in Workfront, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>. </p>
    <p>Workfront calculates a user's availability depending on the Resource Management preferences in the [!UICONTROL Setup] area. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Configure Resource Management preferences</a>. </p> 
   <p>You can update the [!UICONTROL Work Time] of a user when you edit or create the user. For information, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Edit a user's profile</a></p> 
   <b>TIP</b> 
   <p>Set the [!UICONTROL Work Time] value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Working time]</td> 
   <td>In Workfront documentation, this term is used to describe the time allocated to work, according to a schedule.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>In a project, task, or issue report, using the following statement in text mode displays the number of Planned Hours of the project, task, or issue followed by the word "Hours":</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>For information about using text mode, see <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Text mode syntax overview</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
