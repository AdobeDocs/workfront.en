---
product-area: resource-management
navigation-topic: resource-utilization
title: View resource utilization information
description: You can view the utilization of your resources in the Utilization report.
author: Alina, Lisa
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
---
# View resource utilization information

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

You can view the utilization of your resources in the Utilization report.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Vazgen's response about these hours ie below and he asked us to NOT document them:</p>
<p>It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours.</p>
<p>In some cases, like for Planned Hours, it takes them from Assignments</p>
<p>But Budgeted Hours come from projects.</p>
<p>And Actual Hours are their own object - Hour)</p>
</div>
-->

<!--
<p style="color: #dc143c;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This report displays information about the assignments on work items for projects in your environment, like Planned, Actual, and Budgeted Hours, FTE, or Cost.&nbsp;These are hours,&nbsp;FTE, or costs associated with the assignments and not with the tasks and issues themselves.(PRIVATE NOTE:&nbsp;Vazgen's response about these hours: It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours. In some cases, like for Planned Hours, it takes them from Assignments; But Budgeted Hours come from projects. And Actual Hours are their own object - Hour.)</p>
-->

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to access the Utilization report: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>New: Any</p>
       <p>Or</p>
       <p>Current: Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p>
       <p>Or</p>
       <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li> <p>Resource Management </p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Portfolios</p> </li> 
     <li> <p>Programs</p> </li> 
     <li> <p>Financial Data, if you want to view information by Cost</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to projects, portfolios, and programs to access the Utilization  section in the  Resourcing area</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>Manage access to a project to access the Utilization section of the project</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Prerequisites for accessing utilization information</h2>
<p>(NOTE: drafted, replaced with above table)</p>
<p>To access utilization information as described in this section, ensure that the following conditions are met:</p>
<ul>
<li>You have at least&nbsp;View access to the project, program, or portfolio for which you want to view the utilization information.</li>
<li>Your Workfront administrator must grant you at least View access to&nbsp;Financial&nbsp;Data in your Access Level to be able to view cost and revenue information in the Utilization report. The Workfront administrator must enable both View Role Billing & Cost Rates as well as View User Billing &&nbsp;Cost Rates when they grant you the View access to Financial Data. For information about granting access to&nbsp;Financial&nbsp;Data, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. </li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;drafted. No longer the case.) </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Reporting area. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Resourcing area. </p>
</li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is available by default in the Reporting area if the system administrator has not assigned a custom layout template to you. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is available by default in the Resourcing area if the system administrator has not assigned a custom layout template to you. </p>
</li>
</ul>
</div>
-->

## Overview of the Utilization report {#overview-of-the-utilization-report}

The Utilization report allows you to view the progress, cost, or revenue of a project, program, or portfolio in a single report. You can also compare revenue against cost.

You can view the Utilization report in the Resourcing area to display utilization across multiple projects, or you can view it at the level of one project, to display utilization for the individual resources (job roles and users) associated with that project.

For information about accessing and using the Utilization report, see the [Track progress, cost, and revenue with the Utilization report](#track-progress-cost-and-revenue-with-the-utilization-report) section in this article.

### Track hours (progress) {#track-hours-progress}

You can track progress by viewing how the budgeted and planned hours compare to the actual hours.

When tracking the progress of a project, program, or portfolio, progress against both tasks and issues is included in the Utilization report.

The following information is available in the Utilization report when tracking Hours: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Column Title When Viewing Hours</strong> </th> 
   <th><strong>Function</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Budgeted Hours</strong> </td> 
   <td scope="col"> <p>The total budgeted hours on the included projects. You can view the total budgeted hours for the overall life of the included projects, or you can view total budgeted hours only for the specified date range (you can specify an individual week or month). </p> <p>Budgeted Hours are populated from information available in the Resource Budgeting area of the Business Case or the Resource Planner<em>.</em></p> <p>Budgeted Hours appear on the Utilization report in any of the following rows:</p> 
    <ul> 
     <li> Budgeted hours are summarized by job role and by individual user in the Utilization report, as follows:<br><strong>Individual User:</strong> Budgeted Hours are summarized for each user in the utilization report. These Budgeted Hours are associated with the tasks and issues that the user is assigned to on the included projects. (You can expand the row of the corresponding job role to view a list of users with that job role.)<br><strong>Job Role:</strong> Budgeted Hours are summarized by job role in the utilization report.<br>Budgeted Hours appear in a particular job role as a result of any of the following scenarios:
     <ul>
     <li>The job role is defined as the primary job role of the user who is assigned to the task or issue where the Budgeted Hours are associated. </li> 
       <li>When you view utilization information for a single project, the job role of the user assigned the hours is used whether there is no assignment on the task or issue, another user is assigned with no job role assignment, another user is assigned with a different job role, or another team is assigned.</li> 
       <li>When you view utilization information for several projects, programs, or portfolios, the job role of the user assigned the hours is used only when the role is assigned on a task or issue in a project. </li> 
       <li>The job role is assigned to the task or issue that has Budgeted Hours associated, and the user assigned to the task or issue does not have a job role defined in the system.</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>Unallocated Hours</strong>: Budgeted Hours are displayed in the utilization report in the Unallocated Hours section when Budgeted Hours are associated with a task or issue and there is no user or role assigned to the task or issue.<br>This section appears only when there are hours on the project that match this description and when viewing the Utilization report by or from a project. </p> <p>This section appears only when there are hours on the project that match this description and when viewing the Utilization report by or from a project. </p> </li> 
    </ul> <p>For more information about budgeted hours, see <a href="/help/quicksilver/manage-work/projects/project-finances/budgeted-labor-cost.md#locate-the-budgeted-hours-of-a-project">Locate the Budgeted Hours of a project</a> in <a href="/help/quicksilver/manage-work/projects/project-finances/budgeted-labor-cost.md">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Planned Hours</strong> </td> 
   <td scope="col">
<p>
The Planned Hours on the included projects that are associated with the assignments on each task and issue. You can view the total planned hours of all assignments on the project for the overall life of the included projects, or you can view total planned hours only for the specified date range (you can specify an individual week or month).
</p>
<p>
<strong>TIP </strong>
</p>
<p>
The planned hours from items that have a Duration of 0 are not taken into account. 
</p>
<p>
Planned Hours in the Utilization report take into consideration whether the Planned Hours have been re-allocated across the duration of a task or issue. 
</p>
<p>
When the user daily allocation for hours has been modified using the Workload Balancer, the data in the Utilization report can be affected if the dates selected in the Utilization report contain only a portion of a task's or issue's Duration. 
</p>
<p>
For information about modifying allocations for users, see <a href="../workload-balancer/manage-user-allocations-workload-balancer.md">Manage user allocations in the Workload Balancer</a>.


</p>
<p>
Planned Hours appear on the Utilization report in any of the following rows:
</p>
<ul>

<li>Planned Hours are summarized by job role and by individual user in the utilization report, as follows: 
<ul>
 
<li><strong>Individual User</strong>: Planned Hours are summarized for each user in the utilization report. These Planned Hours are associated with the tasks and issues that the user is assigned to on the included projects. (You can expand the row of the corresponding job role to view a list of users with that job role.)
 
<li><strong>Job Role</strong>: Planned Hours are summarized by job role in the utilization report of a single project.<br>Planned Hours appear in a particular job role as a result of any of the following scenarios:  
<ul>
  
<li>The job role is defined as the primary job role of the user who is assigned to the task or issue where the Planned Hours are associated. 
  
<li>When you view utilization information for a single project, the hours associated with a job role do not display for the job role in the following scenarios:   
<ul>
   
<li>There is no assignment on the task or issue
   
<li>A user is assigned with no job role assignment
   
<li>A user is assigned with a different job role 
   
<li>A team is assigned to the task or issue
</li>   
</ul>
  
<li>When you view utilization information for several projects, programs, or portfolios, the job role of the user assigned the hours is used only when the role is assigned on a task or issue in a project. Job role hours do not display separately when viewing the Utilization report for multiple projects. 
  
<li>The job role is assigned to the task or issue that has Planned Hours associated, and the user assigned to the task or issue does not have a job role defined in the system.
</li>  
</ul>
 
<li><strong>Unallocated Hours</strong>: Planned Hours are displayed in the utilization report in the Unallocated Hours section when Planned Hours are associated with a task or issue and there is no user or role assigned to the task or issue. This section appears only when there are hours on the project that match this description and when viewing the Utilization report for a single project. <br>For more information about planned hours, see <a href="../../manage-work/tasks/task-information/planned-hours.md">Planned Hours overview</a>.
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Actual Hours</strong> </td> 
   <td> <p> The total hours logged on the tasks, issues, <span>and on the project</span> for the included projects. You can view the total actual hours for the overall life of the included projects, or you can view the total actual hours only for the specified date range (you can specify an individual week or month). </p> <p><strong>Warning:</strong> The utilization report includes hours logged to the project, children tasks, issues, and parent tasks that have at least one assignment. It does not include hours logged to parent tasks without assignments. We recommend that you do not use parent tasks as working tasks and assign only children tasks to your resources. </p> <p>Actual Hours appear on the utilization report in any of the following rows:</p> 
    <ul> 
     <li> Actual Hours are summarized by job role and by individual user in the utilization report of a project, as follows:<br><strong>Individual User:</strong> Actual Hours are displayed in the utilization report in the row of the user who logged the hours. (You can expand the row of the corresponding job role to view a list of users with that job role who have logged hours.)<br><strong>Job Role:</strong> Actual Hours logged by users associated with those roles are summarized in the utilization report in the row of the corresponding job role.<br>Actual Hours appear in a particular job role as a result of any of the following scenarios: 
      <ul> 
       <li>The job role is defined as the primary job role of the user who logged the hours</li> 
       <li>There is no assignment on the task or issue</li> 
       <li>Another user is assigned with no job role assignment</li> 
       <li>Another user is assigned with a different job role</li> 
       <li> <p>A team is assigned</p> </li> 
      </ul></li>  
     <p>If the user logging the hours does not have a job role assocaited with their profile, the job role used for the Utilization report is the job role assigned to the task or issue where hours are logged or the job role associated with the Primary Owner of the task or issue. </p> 
     <li><strong>Other Hours:</strong> Actual Hours are displayed in the utilization report in the Other Hours section, in the row of the user who logged in the hours.<br>Hours appear in this section when the user who logged the hours does not have a job role defined in the system.<br>This section appears only when there are hours on the project that match this description. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Budgeted Variance (for Hours)</strong> </td> 
   <td> <p>The total budgeted hours minus the total actual hours on the included projects. You can view the total budgeted variance for the overall life of the included projects, or you can view the total budgeted variance only for the specified date range (you can specify an individual week or month). </p> <p>If the value is positive, it is displayed in green. This indicates that the total budgeted hours are greater than the actual hours.</p> <p>If the value is negative, it is displayed in red. This indicates that the total budgeted hours are less than the actual hours.</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Planned Variance (for Hours)</strong> </td> 
   <td> <p>The total planned hours minus the total actual hours on the included projects. You can view the total planned variance for the overall life of the included projects, or you can view the total planned variance only for the specified date range (you can specify an individual week or month).</p> <p>If the value is positive, it is displayed in green. This indicates that the total planned hours are greater than the actual hours.</p> <p>If the value is negative, it is displayed in red. This indicates that the total planned hours are less than the actual hours.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Track cost {#track-cost}

You can track cost by viewing how the Budgeted Cost and Planned Cost compares to the Actual Costs.

When tracking the cost of a project, program, or portfolio, information in the Utilization report comes from tasks. Cost information from tasks is always available on the Utilization report. Cost for tasks is calculated based on the cost type of the task. For information about the cost type of tasks, see [How Workfront calculates Cost Types for tasks](/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-cost-types-for-tasks) in [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

You can display cost information on the Utilization report in the following ways:

* For a given week or month, or for the overall project, program, or portfolio
* By role or individual, for projects

The currency on the utilization report is determined by the currency set on the project. For information about how to adjust the currency for a project, see [Change the project currency](../../manage-work/projects/project-finances/change-project-currency.md).

The following information is available in the Utilization report when tracking cost: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Column Title When Viewing Cost</strong> </th> 
   <th> <p><strong>Function</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Budgeted Cost</strong> </td> 
   <td scope="col"> <p>The Budgeted Cost on the included projects. You can view the total Budgeted Cost for the overall life of the included projects, or you can view the total Budgeted Cost only for the specified date range (you can specify an individual week or month).</p> <p>Because the Budgeted Cost in the Utilization Report is focused on cost by role, the calculation is the same as the Budgeted Labor Cost within other areas of Workfront. For information about how Budgeted Labor Cost is calculated, see <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Planned Cost</strong> </td> 
   <td scope="col"> <p>The total Planned Cost on the included projects. You can view the total Planned Cost for the overall life of the included projects, or you can view the total Planned Cost only for the specified date range (you can specify an individual week or month).</p> <p>Note that for the week, month, and quarterly views, the planned costs are calculated as an average of the chosen period when the cost rates for job roles or users are date effective.</p><p>For information about how the Planned Cost for the project is calculated, see <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-planned-budgeted-and-actual-costs">How Workfront calculates Planned, Budgeted, and Actual Costs</a> in <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md">Track costs</a>.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"><strong>Actual Cost</strong> </td> 
   <td scope="col"> <p>The total Actual Cost on the included projects. You can view the total Actual Cost for the overall life of the included projects, or you can view the total Actual Cost only for the specified date range (you can specify an individual week or month).</p> <p>For information about how the Actual Cost for the project is calculated, see <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-planned-budgeted-and-actual-costs">How Workfront calculates Planned, Budgeted, and Actual Costs</a> in <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md">Track costs</a>.</p> </td>
  </tr> 
  <tr> 
   <td><strong>Budgeted Variance (for Cost)</strong> </td> 
   <td scope="col"> <p>The total Budgeted Cost minus the total Actual Cost on the included projects. You can view the total budgeted variance for the overall life of the included projects, or you can view the total budgeted variance only for the specified date range (you can specify an individual week or month).</p> <p>If the value is positive, it is displayed in green. This indicates that the total Budgeted Cost is greater than the Actual Cost.</p> <p>If the value is negative, it is displayed in red. This indicates that the total Budgeted Cost is less than the Actual Cost.</p> </td>
  </tr> 
  <tr> 
   <td><strong>Planned Variance (for Cost)</strong> </td> 
   <td> <p>The total Planned Cost minus the total Actual Cost on the included projects. You can view the total planned variance for the overall life of the included projects, or you can view the total planned variance only for the specified date range (you can specify an individual week or month). </p> <p>If the value is positive, it is displayed in green. This indicates that the total Planned Cost is greater than the Actual Cost.</p> <p>If the value is negative, it is displayed in red. This indicates that the total Planned Cost is less than the Actual Cost.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Track revenue {#track-revenue}

You can track revenue by viewing how the budgeted and planned revenue compare to the actual revenue.

When tracking the revenue of a project, program, or portfolio, revenue only from tasks is included in the Utilization report.

The information in the following table is available in the Utilization report when tracking Revenue.

For information on the specific fields and how Workfront calculates them, also see [Track costs](../../manage-work/projects/project-finances/track-costs.md) and [Overview of Billing and Revenue](../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Column Title When Viewing Revenue</strong> </th> 
   <th> <strong>Function</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Budgeted Revenue</strong> </td> 
   <td scope="col"> <p>The total Budgeted Hours multiplied by the Role Billing Rate on the included projects. You can view the total budgeted revenue for the overall life of the included projects, or you can view the total budgeted revenue only for the specified date range (you can specify an individual week or month).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Planned Revenue</strong> </td> 
   <td scope="col"> <p>Planned Revenue in the Utilization report is the revenue associated with the Planned Hours allocated to the resources assigned to the tasks on the project.</p> <p>Workfront calculates the project Planned Revenue for the Utilization report using the following formula:</p> <p><code>Project Planned Revenue = SUM (All Tasks Planned Revenue)</code> </p> 
   <p><b>NOTE</b>
   <p>The project Planned Revenue that displays in the Utilization report differs from the Planned Revenue that displays in the Project Details area and project reports. </p> <p>The Planned Revenue in the Project Details area reflects the task revenue as well as the Fixed Revenue of the project. The Planned Revenue in the Utilization Report displays Planned Revenue associated only with the tasks in the project. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>If the project has 1 task with 10 hours, assigned to a Consultant with $20 hourly rate, and the project has $100 Fixed Revenue, the Utilization report displays $200 for Planned Revenue (the Planned Revenue associated with the hours on the task). The Project Details section displays $300 (the Planned Revenue from the task and the Fixed Revenue for the project.) </p> 
     </div> <p>For more information about the task and project Planned Revenue outside of the Utilization report, see <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> </p> <p>The way the Utilization report calculates and displays Planned Revenue for the included projects takes into account the Revenue Type set on the task. </p> <p>Depending on the Revenue Type of each task in the project, the following scenarios exist: </p> <p><strong>Fixed Revenue:</strong> Regardless of the task assignments, the revenue on the task is always calculated using the Fixed Amount specified on the task.</p> <p><b>IMPORTANT</b>
     
   Unlike in other areas of Workfront, the Utilization report calculates Planned Revenue for Fixed Revenue tasks by dividing Fixed Revenue evenly by the number of Planned Hours on the task. </p> <p>For example, a task has a revenue of $200. If there are 4 Planned Hours on the task, each hour would be $50. This is distributed on a user and role level. This distribution is unique to the Utilization report.</p> <p><b>NOTE</b>
     
   If you have a Fixed Revenue task and there are no Planned Hours for the task, the Revenue does not display in the Utilization Report because there is no way to distribute it to the hours. If you have Planned Hours on tasks with Fixed Revenue and no assignments, the Revenue displays as Unallocated Revenue. </p> <p><strong>Role Hourly:</strong> The revenue on the task is calculated using the billing rate set for a specific role, multiplied by the number of Planned Hours associated with that role. Workfront uses the following formula:</p> <p><code>Role Hourly Planned Revenue = SUM(Planned Hours from role on all tasks) * Role Billing Rate</code></p><p><b>NOTE:</b> The billing hourly rate in the formula considers any date effective changes of the rate.</p>   <p><strong>User Hourly:</strong> The revenue on the task is calculated using the billing rate set for a specific user, multiplied by the number of Planned Hours associated with that user. Workfront uses the following formula:</p> <p><code>User Hourly Planned Revenue = SUM(Planned Hours from users on all tasks) * User Billing Rate</code> </p> <p><b>NOTE:</b> The billing hourly rate in the formula considers any date effective changes of the rate.</p> <p><b>Role Hourly or User Hourly Plus Fixed</b> </p> <p><b>IMPORTANT</b>
   
   Unlike in other areas of Workfront, the Utilization report calculates Planned Revenue by dividing Fixed Revenue evenly by the number of Planned Hours on the task. </p> <p>The following cases exist: </p> 
    <ul> 
     <li> <p><strong>Role Hourly Plus Fixed:</strong> The revenue on the task is calculated using the billing rate set for a specific role, multiplied by the number of Planned Hours associated with the role. In addition, a fixed amount that is specified on the task is added to the role rate. Workfront uses the following formula:</p> <p><code>Role Hourly Plus Fixed Planned Revenue = [SUM(Planned Hours from role on all tasks) * Role Billing Rate] + SUM(Cap or Fixed Amount of the task / Planned Hours of the task)</code> </p> </li>
     <li> <p><strong>User Hourly Plus Fixed:</strong> The billing rate set for a specific user, multiplied by the number of Planned Hours on the task from that user. In addition, a fixed amount that is specified on the task is added to the user rate. Workfront uses the following formula:</p> <p><code>User Hourly Plus Fixed Planned Revenue = [SUM(Planned Hours from user on all tasks) * User Billing Rate] + SUM(Cap or Fixed Amount of the task / Planned Hours of the task)</code> </p> </li> 
    </ul> <p><b>Role or User Hourly w/ Cap</b> </p> <p><b>IMPORTANT</b>
    
   Unlike in other areas of Workfront, if the Planned Revenue exceeds the cap, the amount over the Cap Amount is considered Fixed Revenue. The Planned Revenue is calculated by dividing Fixed Revenue evenly by the number of Planned Hours on the task, then adding to that the Cap Amount and the role or user hourly revenue. <br></p> <p>The following cases exist: </p> 
    <ul> 
     <li> <p><strong>Role Hourly w/Cap:</strong> Tasks are billed hourly as in Role Hourly, but they have a maximum Cap Amount that you can specify. Workfront uses the following formula:</p> <p><code>Role Hourly w/ Cap Planned Revenue = [SUM(Planned Hours from role on all tasks and issues) * Role Billing Rate] + Cap Amount of the task + SUM(Amount over the Cap Amount / Planned Hours of the task)</code> </p> </li>
     <li> <p><strong>User Hourly w/Cap:</strong> Tasks are billed hourly as in User Hourly, but they have a maximum Cap Amount that you can specify. Workfront uses the following formula: </p> <p><code>User Hourly w/ Cap Planned Revenue = [SUM(Planned Hours from user on all tasks) * User Billing Rate] + Cap Amount of the task + SUM(Amount over the Cap Amount / Planned Hours of the task)</code> </p> </li> 
    </ul> <p>For more information about which role or user is taken into account when calculating Planned Revenue, see <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Actual Revenue</strong> </td>
   <td> <p>Actual Revenue is the revenue associated with the Actual Hours of the tasks and of the project. For more information about Actual Revenue, see <a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#track-revenue-amounts">Track Revenue amounts</a> in <a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md">Overview of Billing and Revenue</a>.</p>
   
   <p>The way that the Utilization report calculates Actual Revenue for the included projects differs depending on the Revenue Type set on the task, as follows:</p> <p><strong>Fixed Revenue:</strong> Regardless of the task assignments, the revenue on the task is always calculated using the Fixed Amount specified on the task.</p> <p><b>IMPORTANT</b>

Unlike in other areas of Workfront, the Utilization report calculates Actual Revenue by dividing Fixed Revenue evenly by the number of hours logged on the task. </p> <p> </p> <p>For example, a task has an Actual Revenue of $200. If there are 4 Actual Hours on the task, each hour would be $50. This is distributed on a user and role level. This distribution is unique to the Utilization report.</p> <p><b>NOTE</b>
   
   If you have a Fixed Revenue task and there are no Actual Hours on the task, the Actual Revenue does not display in the Utilization Report because there is no way to distribute hours. </p> <p><strong>Role Hourly:</strong> The revenue on the task is calculated using the billing rate set for a specific role, multiplied by the number of Actual Hours.</p> <p>Workfront uses the following formula:</p> <p><code>Role Hourly Actual Revenue = SUM(Actual Hours from role on all tasks) * Role Billing Rate</code> </p> <p><b>NOTE:</b> The billing hourly rate in the formula considers any date effective changes of the rate.</p> <p><strong>User Hourly:</strong> The revenue on the task is calculated using the billing rate set for a specific user, multiplied by the number of hours logged against the task from that user. Workfront uses the following formula:</p> <p><code>User Hourly Actual Revenue = SUM(Actual Hours from user on all tasks) * User Billing Rate</code></p> <p><b>NOTE:</b> The billing hourly rate in the formula considers any date effective changes of the rate.</p> <p><b>Role or User Hourly Plus Fixed</b> </p> <p><b>IMPORTANT</b>
   
Unlike in other areas of Workfront, the Utilization report calculates Actual Revenue by dividing Fixed Revenue evenly by the number of hours logged on the task. </p> <p>The following cases exist: </p> 
    <ul> 
     <li> <p><strong>Role Hourly Plus Fixed:</strong> The billing rate set for a specific role, multiplied by the number of hours logged against the task from a user with that role. In addition, a fixed amount that is specified on the task is added to the role rate. </p> <p>Workfront uses the following formula:</p> <p><code>Role Hourly Plus Fixed Actual Revenue = [SUM(Actual Hours from role on all tasks) * Role Billing Rate] + SUM(Cap or Fixed Amount of the task / Actual Hours of the task)</code> </p> </li>
     <li> <p><strong>User Hourly Plus Fixed:</strong> The billing rate set for a specific user, multiplied by the number of hours logged against the task from that user. In addition, a fixed amount that is specified on the task is added to the user rate. </p> <p>Workfront uses the following formula:</p> <p><code>User Hourly Plus Fixed Actual Revenue = [SUM(Actual Hours from role on all tasks) * User Billing Rate] + SUM(Cap or Fixed Amount of the task / User Hours of the task)</code> </p> </li> 
    </ul> <p><b>Role or User Hourly w/ Cap</b> </p> <p><b>IMPORTANT</b>
    
   Unlike in other areas of Workfront, if the Planned Revenue exceeds the cap, the amount over the Cap Amount is considered Fixed Revenue. The Planned Revenue is calculated by dividing Fixed Revenue evenly by the number of Planned Hours on the task, then adding to that the Cap Amount and the role or user hourly revenue. <br></p> <p>The following cases exist:</p> 
    <ul> 
     <li> <p><strong>Role Hourly w/Cap:</strong> Tasks are billed hourly as in Role Hourly, but they have a maximum Cap Amount that you can specify. Workfront uses the following formula:</p> <p><code>Role Hourly w/ Cap Actual Revenue = [SUM(Actual Hours from role on all tasks and issues) * Role Billing Rate] + Cap Amount of the task + SUM(Amount over the Cap Amount / Actual Hours of the task)</code></p> </li>
     <li> <p><strong>User Hourly w/Cap:</strong> Tasks are billed hourly as in User Hourly, but they have a maximum Cap Amount that you can specify.</p> <p> Workfront uses the following formula:</p> <p><code>User Hourly w/ Cap Actual Revenue = [SUM(Actual Hours from role on all tasks and issues) * User Billing Rate] + Cap Amount of the task + SUM(Amount over the Cap Amount / Actual Hours of the task)</code> </p> </li> 
    </ul>
     <p><strong>Project Revenue</strong>: The revenue associated with the hours logged on the project is calculated taking into account the Billing per Hour amount of the primary job role of the user who logs the time. We do not recommend logging time on the project. </p> 
     <p><b>NOTE</b>
   
   If the user is not associated with a job role or if the Billing per Hour of the Primary Role is zero, Workfront calculates Actual Revenue using the Billing per Hour amount for the user. If the user does not have a Billing per Hour amount in their profile, the Actual Revenue is zero. </p> 
   </td> 
  </tr> 
  <tr> 
   <td><strong>Budgeted Variance (for Revenue)</strong> </td> 
   <td> <p>The total Actual Revenue minus Budgeted Revenue on the included projects.<br>You can view the total budgeted variance for the overall life of the included projects, or you can view the total budgeted variance only for the specified date range (you can specify an individual week or month).</p> <p>If the value is positive, it is displayed in green. This indicates that the total Budgeted Revenue is greater than the Actual Revenue.</p> <p>If the value is negative, it is displayed in red. This indicates that the total Budgeted Revenue is less than the Actual Revenue.</p> </td>
  </tr> 
  <tr> 
   <td><strong>Planned Variance (for Revenue)</strong> </td> 
   <td> <p>The total Actual Revenue minus the total Planned Revenue on the included projects.<br>You can view the total planned variance for the overall life of the included projects, or you can view the total planned variance only for the specified date range (you can specify an individual week or month). </p> <p>If the value is positive, it is displayed in green. This indicates that the total Planned Revenue is greater than the Actual Revenue.</p> <p>If the value is negative, it is displayed in red. This indicates that the total Planned Revenue is less than the Actual Revenue.</p> </td>
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### Compare Revenue against Planned and Actual Costs {#compare-revenue-against-planned-and-actual-costs}

You can view the Planned or Actual Cost alongside the Planned Revenue. The Margin (%) is also displayed (margin is calculated as Revenue - Cost / Revenue).

The following information is available in the Utilization report when comparing Revenue against Planned and Actual Costs:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Column Title When Viewing Revenue vs Cost (Planned)</strong> </th> 
   <th> <strong>Function</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Planned Cost</strong> </td> 
   <td scope="col"> The total Planned Cost on the included projects. You can view the total Planned Cost for the overall life of the included projects, or you can view the total Planned Cost only for the specified date range (you can specify an individual week or month). </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Planned Revenue</strong> </td> 
   <td scope="col"> <p>Planned Revenue is the revenue associated with the Planned Hours of the tasks. </p> <p>The way the Utilization report calculates and displays Planned Revenue for the included projects differs depending on the Revenue Type set on the task, as described in the <a href="#track-revenue" class="MCXref xref">Track revenue</a> section in this article.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Margin</strong> </td> 
   <td scope="col"> <p>The Margin percentage is calculated as follows:</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>NOTE</b>
   
   If Planned Revenue equals 0, Margin is displayed as 0. </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>Column Title When Viewing Revenue vs Cost (Actual)</strong> </p>  </td> 
   <td scope="col"><p><strong>Function</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Actual Cost</strong> </td> 
   <td scope="col"> <p>The total Actual Cost on the included projects. You can view the total Actual Cost for the overall life of the included projects, or you can view the total Actual Cost only for the specified date range (you can specify an individual week or month).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Actual Revenue</strong> </td> 
   <td> <p>Actual Revenue is the revenue associated with the Actual Hours of the tasks.</p> <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p> <p>The way that the Utilization report calculates Actual Revenue for the included projects differs depending on the Revenue Type set on the task, as described in the <a href="#track-revenue" class="MCXref xref">Track revenue</a> section in this article. </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Margin</strong> </td> 
   <td> <p>The Margin percentage is calculated as follows:</p> <p>Actual Revenue - Actual Cost / Actual Revenue * 100. </p> <p><b>NOTE</b> 
   
   If Actual Revenue equals 0, Margin is displayed as 0. </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->
    
## Track progress, cost, and revenue with the Utilization report {#track-progress-cost-and-revenue-with-the-utilization-report}

You can track the progress or cost of a project, program, or portfolio.

You can display information on the Utilization report for a given week or month, or for the overall life of the projects.

To track the progress or cost of one or more projects with a Utilization report:

1. Do any of the following, depending on whether you are viewing utilization information for an individual project, multiple projects, a program, or a portfolio:

   * To view utilization information for a single project:

      1. Go to a project for which you want to view utilization information, then click **Show More> Utilization**. 
      1. Utilization information is displayed automatically when viewing an individual project, and applying a filter is not required.   
         If you want to filter the Utilization report, you can apply a filter, then click **Run**.  
         For information about how to filter the Utilization report, see [Filter utilization information](#filter-utilization-information) in this article.   
         Utilization information is displayed for individual users and roles (users are grouped within their associated role).

   * To view utilization information for multiple projects:

      {{step1-to-utilization-report}}

      1. Apply a filter to the Utilization report, then click **Run**.
         You must specify one or more projects in the filter prior to running the Utilization report. For information about how to filter the Utilization report, see [Filter utilization information](#filter-utilization-information) in this article.  
         Utilization information is displayed for individual roles and projects (roles are grouped within their associated project).

   * To view utilization information for a program:

      {{step1-to-utilization-report}}

      1. Click **Show**>**Programs**.
      1. Apply a filter to the Utilization report, then click **Run**.   
         You must specify one or more programs in the filter prior to running the Utilization report. For information about how to filter the Utilization report, see [Filter utilization information](#filter-utilization-information) in this article.   
         Utilization information is displayed for individual projects and programs (projects are grouped within their associated program).

   * To view utilization information for a portfolio:

      {{step1-to-utilization-report}} 
      
      1. Click **Show**>**Portfolios**.
      1. Apply a filter to the Utilization report, then click **Run**.   
         You must specify one or more portfolios in the filter prior to running the Utilization report. For information about how to filter the Utilization report, see [Filter utilization information](#filter-utilization-information) in this article.   
         Utilization information is displayed for individual projects, programs, and portfolios (projects are grouped within their associated program, and programs are grouped within their associated portfolio).

1. In the upper-right corner of the Utilization report, click **View**, then select from the following in the menu:

   * **Cost**
   * **Hours**
   * **Revenue**
   * **Revenue vs. Cost (Planned)**
   * **Revenue vs Cost (Actual)**

   The option you select determines which columns and information are available in the report.
   ![View options](assets/utilization-view-dropdown.png)

1. (Optional) Select the date range for which utilization information is displayed. You can display information for a given week or month to the left of the **Overall** column. Information for the overall project, program, or portfolio is always displayed in the **Overall** column.  
   For more information, see [Adjust the date range for which information is displayed](#adjust-the-date-range-for-which-information-is-displayed) in this article. 

1. (Optional) Click any column title to sort the utilization report by the information in that column. Sorting works only when you include multiple items in your report. For example, you can sort the results of your report when you are looking at more than one project (or portfolio or program). You cannot sort the results when you are looking at only one project (or one portfolio or one program) at a time.  
1. Use the information in the section [Overview of the Utilization report](#overview-of-the-utilization-report) in this article to learn about each column in the Utilization report.

## Filter utilization information {#filter-utilization-information}

You can filter the content displayed in a Utilization report on a project. You can filter on tasks, issues, roles, and custom data. When you apply a filter, the Utilization report contains information based on the criteria that you select.

You can create a new filter, or apply a filter that you previously created.

### Create or modify a filter {#create-or-modify-a-filter}

When you create a filter, all Workfront users who have access to the Utilization report also have access to the filter you create. Similarly, when you modify an existing filter, the filter is modified for all users who have access to the Utilization report.

To create or modify a filter:

1. Open the Utilization report.
   See [Track progress, cost, and revenue with the Utilization report](#track-progress-cost-and-revenue-with-the-utilization-report) to do this.

1. Click the **Filter** icon to display the filter options.
1. (Conditional) To modify an existing filter, click the **Filter** drop-down menu, then select the filter you want to modify.
1. Specify the following information to create or modify the filter:

   * **Portfolios:** Begin typing the name of the portfolio that contains the information you want to include in the Utilization report, then click the name when it appears in the drop-down list  
     Repeat this process to include information from multiple portfolios in the Utilization report.  
     To include all portfolios from your system in your filter, click **Add all**. (This option is available only if you have fewer than 10 portfolios in your system.)
   
   * **Programs:** Begin typing the name of the program that contains the information you want to include in the Utilization report, then click the name when it appears in the drop-down list.  
     Repeat this process to include information from multiple tasks in the Utilization report.  
     If you already designated any portfolios in the filter, the program you specify must be from the portfolios already included in the filter. If it is not, data from the program is not included in the Utilization report.  
     To include all programs from your system in your filter, click **Add all**. (This option is available only if you have fewer than 20 programs in your system.)
   
   * **Projects:** Begin typing the name of the project that contains the information you want to include in the Utilization report, then click the name when it appears in the drop-down list.  
     Repeat this process to include information from multiple projects in the Utilization report.  
     If you already designated any portfolios or programs in the filter, the project you specify must be from one of the portfolios or programs already included in the filter. If it is not, data from the project is not included in the Utilization report.  
     To include all projects from your system in your filter, click **Add all**. (This option is available only if you have fewer than 250 projects in your system.)
   
   * **Tasks:** Begin typing the name of the task that contains the information you want to include in the Utilization report, then click the name when it appears in the drop-down list.  
     Repeat this process to include information from multiple tasks in the Utilization report.  
     If you already designated any portfolios, programs, or projects in the filter, the task you specify must be from one of the portfolios, programs, or projects already included in the filter. If it is not, data from the task is not included in the Utilization report.
   
   * **Issues:** Begin typing the name of the issue that contains the information you want to include in the Utilization report, then click the name when it appears in the drop-down list.  
     Repeat this process to include information from multiple issues in the Utilization report.  
     If you already designated any portfolios, programs, or projects in the filter, the issue you specify must be from one of the portfolios, programs, or projects already included in the filter. If it is not, data from the issue is not included in the Utilization report.  
     Cost information for issues is not always included in the Utilization report. For more information about when cost information for issues is included in the Utilization report, see [Track progress, cost, and revenue with the Utilization report](#track-progress-cost-and-revenue-with-the-utilization-report) in this article.
   
   * **Roles:** Begin typing the name of the role you want to be represented in the Utilization Report, then click the name when it appears in the drop-down list. Repeat this process to include additional roles.
     The Utilization Report contains information only for the roles you specify. For example, a task contains 10 Actual Hours. Six of those hours are from a Designer role and four are from a Developer role. If you filter the Utilization Report by role for Designer, the four hours that come from the Developer role are excluded from the report.
   
   * **Add Filter Rule:** Click **Add Filter Rule**, click in the text field, and begin typing the field name that you want to filter on. If the field is available, it populates for each object where it can be associated. Click the name of the field to add it to the filter.

     >[!IMPORTANT]
     >
     >You must type the field name and not the field label. The field label displays on a custom form attached to an object. For information about the difference between the label and the name of a custom field, see  [Create or edit a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

     For more information about the fields you see in the columns, see [Glossary of Adobe Workfront terminology](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).   
     Choose the filter and condition modifiers for the filter. The available modifiers are described in [Filter and condition modifiers](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. To create a new filter, click **Save Filter**.  
   Or  
   To modify an existing filter, click the arrow next to the **Save Filter** button, then click **Save New Filter**.
   In the **Filter Name** field, type a name for the filter and click **Save**.
   The Utilization area is filtered with the information you included in the filter.

### Apply a saved filter {#apply-a-saved-filter}

1. Open the Utilization report.
   See [Track progress, cost, and revenue with the Utilization report](#track-progress-cost-and-revenue-with-the-utilization-report) to do this.

1. Click **Saved Filters**, then select the filter you want to apply from the drop-down list.

### Duplicate a filter {#duplicate-a-filter}

1. Open the Utilization report.
   See [Track progress, cost, and revenue with the Utilization report](#track-progress-cost-and-revenue-with-the-utilization-report) to do this.

1. Click **Saved Filters**, hover over the filter you want to duplicate, and click the **Duplicate** icon.

   ![Duplicate icon](assets/utilization-filter-duplicate.png)

   The Duplicate Filter dialog box is displayed.

1. In the **Filter Name** field, type a name for the new filter and click **Save**.

### Rename a filter {#rename-a-filter}

When you rename a filter, all Workfront users who have access to the Utilization report see the new name that you entered.

To rename a filter:

1. Open the Utilization report.
   See [Track progress, cost, and revenue with the Utilization report](#track-progress-cost-and-revenue-with-the-utilization-report) to do this.

1. Click **Saved Filters**, hover over the filter you want to rename, and click the **Rename** icon.

   ![Rename filter icon](assets/utilization-filter-rename.png)

   The Rename Filter dialog box is displayed.

1. In the **Filter Name** field, type a name for the new filter and click **Save**.

### Delete a filter {#delete-a-filter}

When you delete a filter, the filter is deleted for all Workfront users who have access to the Utilization report.

To delete a filter:

1. Open the Utilization report.
   See [Track progress, cost, and revenue with the Utilization report](#track-progress-cost-and-revenue-with-the-utilization-report) to do this.

1. Click **Saved Filters**, hover over the filter you want to delete, and click the **Delete** icon.

   ![Delete icon](assets/utilization-filter-delete.png)

1. Click **Delete** when prompted whether you want to delete the filter.

## Adjust the date range for which information is displayed {#adjust-the-date-range-for-which-information-is-displayed}

You can adjust the date range for which utilization information is displayed. You can select a past or future date. Changes you make are visible only to you.

1. Open the Utilization report.
   See [Track progress, cost, and revenue with the Utilization report](#track-progress-cost-and-revenue-with-the-utilization-report) to do this.

1. Click the date range next to the **Export** button.

   The current week is selected by default. 

1. Choose from the following options:

   * **Week:** Select this option to select a given week (from Sunday through Saturday).
   * **Month:** Select this option to select a given month.

   The date range you select is displayed in the Utilization report, to the left of the **Overall** column.  
   Workfront remembers whether you want to view a week or month view. The next time you access the Utilization report, the current week or current month is shown, depending on the option you select.

## Export utilization information

You can export utilization information for a project, program, or portfolio from Workfront. Information can be exported only in XLSX, TSV, and PDF formats.

When viewed in Microsoft Excel, negative numbers are displayed in parenthesis.

To export utilization information:

1. Open the Utilization report.
   See [Track progress, cost, and revenue with the Utilization report](#track-progress-cost-and-revenue-with-the-utilization-report) to do this.

1. Click **Export** on the upper left of the report.

1. Select from the following options:

   * **PDF:** Exports the report in PDF format. This is the recommended format if you are planning to print the report.  
     Select either **Letter - Portrait**, **Letter - Landscape**, or **Other Sizes** (provides options for exporting in Legal (8.5" x 14"), Ledger (11" x 17"), and A4).
     Depending on the operating system you use, you might have the option of opening or saving the file. Either open the file with the associated application or save it to your computer.
   
   * **Excel:** Exports the report in XLSX format. This is the recommended format if you are planning to further analyze the data in Excel.
     Depending on the operating system you use, you might have the option of opening or saving the file. Either open the file with the associated application or save it to your computer.
   
   * **Tab Delimited:** Exports the report in TSV format. This is the recommended format if you are planning to import the data into third-party software for further analysis.
     Depending on the operating system you use, you might have the option of opening or saving the file. Either open the file with the associated application or save it to your computer.

1. Read the information in the article [Export data](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) to understand how to use the exported file.

## View utilization information in a chart

You can visualize the data from the Utilization report in a chart view.

1. Open the Utilization report.
   See [Track progress, cost, and revenue with the Utilization report](#track-progress-cost-and-revenue-with-the-utilization-report) to do this.

1. In the upper-right corner of the Utilization report, click the **Chart** icon.

   ![Chart icon](assets/utilization-chart.png)

   The Utilization report is displayed in a chart view.

1. (Optional) Configure the chart to show Projects, Programs, or Portfolios by selecting the appropriate option from the **Show** drop-down menu.
1. (Optional) Hover over a specific point in time on the report to view data for that point in time.

   ![Hover over a data point](assets/utilization-chart-hover.png)

1. (Optional) Adjust the filters to change what information is displayed in the chart. For information about adjusting the filters, see [Filter utilization information](#filter-utilization-information) in this article. 
1. (Optional) Configure the time frame of the chart report, as described in [Adjust the date range for which information is displayed](#adjust-the-date-range-for-which-information-is-displayed) in this article.
