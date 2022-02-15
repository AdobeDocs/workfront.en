---
filename: view-utilization-information
product-area: resource-management
navigation-topic: resource-utilization
---



# View resource utilization information  {#view-resource-utilization-information}

You can view the utilization of your resources using the Utilization report. 


## Access requirements {#access-requirements}

You must have the following to access the Utilization report: 

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>View or higher access to the following:</p> 
    <ul> 
     <li> <p>Resource Management </p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Portfolios</p> </li> 
     <li> <p>Programs</p> </li> 
     <li> <p>Financial Data if you want to view information by Cost</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View access to projects, portfolios, and programs to access the Utilization <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      section 
     </MadCap:conditionalText>in the <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Resourcing 
     </MadCap:conditionalText>area</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>Manage access to the project to access the Utilization <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      section 
     </MadCap:conditionalText>of a project</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


The following sections describe how to view and use utilization information. 


## Overview of the Utilization report {#overview-of-the-utilization-report}

The Utilization report enables you to view the progress, cost, or revenue of a project, program, or portfolio in a single report. You can also compare revenue against cost.


For information about accessing and using the Utilization report, see the [Track progress, cost, and revenue with the Utilization report](#tracking-progress-and-cost-with-a-utilization-report) section in this article.



* [Track hours (progress)](#tracking-hours) 
* [Track cost](#tracking-cost) 
* [Track revenue](#tracking-revenue) 
* [Compare Revenue against Planned and Actual Costs](#comparing-revenue-against-cost) 




### Track hours (progress) {#track-hours-progress}

You can track progress by viewing how the budgeted and planned hours compare to the actual hours.


When tracking the progress of a project, program, or portfolio, progress against both tasks and issues are included in the Utilization report.


The following information is available in the Utilization report when tracking Hours: 

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Column Title When Viewing Hours</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"><span class="bold">Function</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Budgeted Hours</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The total budgeted hours on the included projects. You can view the total budgeted hours for the overall life of the included projects, or you can view total budgeted hours only for the specified date range (you can specify an individual week or month). </p> <p>Note: Budgeted Hours are populated from information available in the new Resource Budgeting area of the Business Case<em>.</em></p> <p>Budgeted Hours appear on the Utilization report in any of the following rows:</p> 
    <ul> 
     <li> Budgeted hours are summarized by job role and by individual user in the Utilization report, as follows:<br><span class="bold">Individual User:</span> Budgeted Hours are summarized for each user in the utilization report. These Budgeted Hours are associated with the tasks and issues that the user is assigned to on the included projects. (You can expand the row of the corresponding job role to view a list of users with that job role.)<br><span class="bold">Job Role:</span> Budgeted Hours are summarized by job role in the utilization report.<br>Budgeted Hours appear in a particular job role as a result of any of the following scenarios: 
      <ul>
       <li>The job role is defined as the primary job role of the user who is assigned to the task or issue where the Budgeted Hours are associated. </li>
       <li>When you view utilization information for a single project, the job role of the user assigned the hours is used whether there is no assignment on the task or issue, another user is assigned with no job role assignment, another user is assigned with a different job role, or another team is assigned.</li>
       <li>When you view utilization information for several projects, programs, or portfolios, the job role of the user assigned the hours is used only when the role is assigned on a task or issue in a project. </li>
       <li>The job role is assigned to the task or issue that has Budgeted Hours associated, and the user assigned to the task or issue does not have a job role defined in the system.</li>
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><span class="bold">Unallocated Hours</span>: Budgeted Hours are displayed in the utilization report in the Unallocated Hours section when Budgeted Hours are associated with a task or issue and there is no user or role assigned to the task or issue.<br>This section appears only when there are hours on the project that match this description and when viewing the Utilization report by or from a project. </p> <p>This section appears only when there are hours on the project that match this description and when viewing the Utilization report by or from a project. </p> </li> 
    </ul> <p>For more information about budgeted hours, see the "Locate the Budgeted Hours of a project" section in the <a href="budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a> article.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Planned Hours</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The total planned hours on the included projects. You can view the total planned hours for the overall life of the included projects, or you can view total planned hours only for the specified date range (you can specify an individual week or month). The planned hours of projects are a total of the Planned Hours allocated to tasks and issues on the project. </p> <p>Tip: The planned hours from items that have a Duration of 0 are not taken into account. </p> <p>Planned Hours in the Utilization report take into consideration whether the Planned Hours have been re-allocated across the duration of a task or issue. When the user allocation for hours has been modified using the <span class="mc-variable WFVariables.Workload_Balancer variable varname">Workload Balancer</span>, the data in the Utilization report can be affected if the dates selected in the Utilization report contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p> <p>Planned Hours appear on the Utilization report in any of the following rows:</p> 
    <ul> 
     <li> Planned Hours are summarized by job role and by individual user in the utilization report, as follows:<br><span class="bold">Individual User:</span> Planned Hours are summarized for each user in the utilization report. These Planned Hours are associated with the tasks and issues that the user is assigned to on the included projects. (You can expand the row of the corresponding job role to view a list of users with that job role.)<br><span class="bold">Job Role:</span> Planned Hours are summarized by job role in the utilization report.<br>Planned Hours appear in a particular job role as a result of any of the following scenarios: </li> 
    </ul> 
    <ul> 
     <ul> 
      <li>The job role is defined as the primary job role of the user who is assigned to the task or issue where the Planned Hours are associated. </li> 
      <li> <p>When you view utilization information for a single project, the job role of the user assigned the hours is used whether there is no assignment on the task or issue, another user is assigned with no job role assignment, another user is assigned with a different job role, or another team is assigned.</p> </li> 
      <li> <p>When you view utilization information for several projects, programs, or portfolios, the job role of the user assigned the hours is used only when the role is assigned on a task or issue in a project.</p> </li> 
      <li>The job role is assigned to the task or issue that has Planned Hours associated, and the user assigned to the task or issue does not have a job role defined in the system.</li> 
     </ul> 
     <li><span class="bold">Unallocated Hours</span>: Planned Hours are displayed in the utilization report in the Unallocated Hours section when Planned Hours are associated with a task or issue and there is no user or role assigned to the task or issue.<br>This section appears only when there are hours on the project that match this description and when viewing the Utilization report by or from a project. <br></li> 
    </ul> <p>For more information about planned hours, see <a href="planned-hours.md" class="MCXref xref">Planned Hours overview</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Actual Hours</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> The total hours logged on the tasks, issues, <span>and on the project</span> for the included projects. You can view the total actual hours for the overall life of the included projects, or you can view the total actual hours only for the specified date range (you can specify an individual week or month). </p> <p class="warning" data-mc-autonum="<b>Warning: </b>"><span class="autonumber"><span><b>Warning: </b></span></span>The utilization report includes hours logged to the project, children tasks, issues, and parent tasks that have at least one assignment. It does not include hours logged to parent tasks without assignments. We recommend that you do not use parent tasks as working tasks and assign only children tasks to your resources. </p> <p>Actual Hours appear on the utilization report in any of the following rows:</p> 
    <ul> 
     <li> Actual Hours are summarized by job role and by individual user in the utilization report, as follows:<br><span class="bold">Individual User:</span> Actual Hours are displayed in the utilization report in the row of the user who logged the hours. (You can expand the row of the corresponding job role to view a list of users with that job role who have logged hours.)<br><span class="bold">Job Role:</span> Actual Hours logged by users are summarized in the utilization report in the row of the corresponding job role.<br>Actual Hours appear in a particular job role as a result of any of the following scenarios: </li> 
     <ul> 
      <li>The job role is defined as the primary job role of the user who logged the hours.</li> 
      <li>The job role of the user logging the hours is used whether there is no assignment on the task or issue, another user is assigned with no job role assignment, another user is assigned with a different job role, or another team is assigned.</li> 
      <li>The job role is assigned to the task or issue where hours are logged, and the user logging hours does not have a job role defined in the system.</li> 
     </ul> 
     <li><span class="bold">Other Hours:</span> Actual Hours are displayed in the utilization report in the Other Hours section, in the row of the user who logged in the hours.<br>Hours appear in this section when the user who logged the hours does not have a job role defined in the system.<br>This section appears only when there are hours on the project that match this description. </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Budgeted Variance (for Hours)</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The total budgeted hours minus the total actual hours on the included projects. You can view the total budgeted variance for the overall life of the included projects, or you can view the total budgeted variance only for the specified date range (you can specify an individual week or month). </p> <p>If the value is positive, it is displayed in green. This indicates that the total budgeted hours are greater than the actual hours.</p> <p>If the value is negative, it is displayed in red. This indicates that the total budgeted hours are less than the actual hours.</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><span class="bold">Planned Variance (for Hours)</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>The total planned hours minus the total actual hours on the included projects. You can view the total planned variance for the overall life of the included projects, or you can view the total planned variance only for the specified date range (you can specify an individual week or month).</p> <p>If the value is positive, it is displayed in green. This indicates that the total planned hours are greater than the actual hours.</p> <p>If the value is negative, it is displayed in red. This indicates that the total planned hours are less than the actual hours.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Track cost {#track-cost}

You can track cost by viewing how the Budgeted Cost and Planned Cost compares to the Actual Costs. 


When tracking the cost of a project, program, or portfolio, information in the Utilization report comes from tasks. Cost information from tasks is always available on the Utilization report. Cost for tasks is calculated based on the cost type of the task. For information about the cost type of tasks, see "Modify Cost Types for individual tasks" in [Track costs](track-costs.md).


You can display cost information on the Utilization report in the following ways:



* For a given week or month, or for the overall project, program, or portfolio. 
* By role or individual, for projects.


The currency used on the utilization report is determined by the currency set on the project. For information about how to adjust the currency for a project, see [Change the project currency](change-project-currency.md).


The following information is available in the Utilization report when tracking Cost: 

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Column Title When Viewing Cost</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p><span class="bold">Function</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Budgeted Cost</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The total Budgeted Cost on the included projects. You can view the total Budgeted Cost for the overall life of the included projects, or you can view the total Budgeted Cost only for the specified date range (you can specify an individual week or month).</p> <p>Because the Budgeted Cost in the Utilization Report is focused on cost by role, the calculation is the same as the Budgeted Labor Cost within other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. For information about how Budgeted Labor Cost is calculated, see <a href="budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Planned Cost</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The total Planned Cost on the included projects. You can view the total Planned Cost for the overall life of the included projects, or you can view the total Planned Cost only for the specified date range (you can specify an individual week or month).</p> <p>For information about how the Planned Cost for the project is calculated, see the "How <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates Planned, Budgeted, and Actual Costs" section in the article <a href="track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Actual Cost</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The total Actual Cost on the included projects. You can view the total Actual Cost for the overall life of the included projects, or you can view the total Actual Cost only for the specified date range (you can specify an individual week or month).</p> <p>For information about how the Actual Cost for the project is calculated, see the "How <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates Planned, Budgeted, and Actual Costs" section in the article <a href="track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Budgeted Variance (for Cost)</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The total Budgeted Cost minus the total Actual Cost on the included projects. You can view the total budgeted variance for the overall life of the included projects, or you can view the total budgeted variance only for the specified date range (you can specify an individual week or month).</p> <p>If the value is positive, it is displayed in green. This indicates that the total Budgeted Cost is greater than the Actual Cost.</p> <p>If the value is negative, it is displayed in red. This indicates that the total Budgeted Cost is less than the Actual Cost.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><span class="bold">Planned Variance (for Cost)</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>The total Planned Cost minus the total Actual Cost on the included projects. You can view the total planned variance for the overall life of the included projects, or you can view the total planned variance only for the specified date range (you can specify an individual week or month). </p> <p>If the value is positive, it is displayed in green. This indicates that the total Planned Cost is greater than the Actual Cost.</p> <p>If the value is negative, it is displayed in red. This indicates that the total Planned Cost is less than the Actual Cost.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Track revenue {#track-revenue}

You can track revenue by viewing how the budgeted and planned revenue compare to the actual revenue.


When tracking the revenue of a project, program, or portfolio, revenue only from tasks is included in the Utilization report.


The information in the following table is available in the Utilization report when tracking Revenue.


For information on the specific fields and how *`Workfront`* calculates them, also see the following articles:



* [Track costs](track-costs.md) 
* [Overview of Billing and Revenue](billing-and-revenue-overview.md) 



<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Column Title When Viewing Revenue</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <span class="bold">Function</span></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Budgeted Revenue</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The total Budgeted Hours multiplied by the Role Billing Rate on the included projects. You can view the total budgeted revenue for the overall life of the included projects, or you can view the total budgeted revenue only for the specified date range (you can specify an individual week or month).</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Planned Revenue</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Planned Revenue is the revenue associated with the Planned Hours of the tasks.</p> <p>The way the Utilization report calculates and displays Planned Revenue for the included projects differs depending on the Revenue Type set on the task, as follows:</p> <p><span class="bold">Fixed Revenue:</span> Regardless of the task assignments, the revenue on the task is always calculated using the Fixed Amount specified on the task, as described in the section "Overview of Revenue Types" in the article <a href="billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> <p>Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, the Utilization report calculates Planned Revenue by dividing Fixed Revenue evenly by the number of Planned Hours on the task. <br>For example, a task has a revenue of $200. If there are 4 Planned Hours on the task, each hour would be $50. This is distributed on a user and role level. This distribution is unique to the Utilization report.</p> <p>Note:  If you have a Fixed Revenue task and there are no hours (Planned or Actual), it does not display correctly in the Utilization Report because there is no way to distribute hours. </p> <p><span class="bold">Role Hourly:</span> The revenue on the task is calculated using t he billing rate set for a specific role, multiplied by the number of Planned Hours, as described in the section "Overview of Revenue Types" in the article <a href="billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>. </p> <p><span class="bold">User Hourly:</span> The revenue on the task is calculated using the billing rate set for a specific user, multiplied by the number of hours logged against the task from that user, as described in the section "Overview of Revenue Types" in the article <a href="billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>. </p> <p><span class="bold">Role Hourly Plus Fixed: </span>The revenue on the task is calculated using the billing rate set for a specific role, multiplied by the number of Planned Hours. In addition, a fixed amount that is specified on the task is added to the role rate.</p> <p>Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, the Utilization report calculates Planned Revenue by dividing Fixed Revenue evenly by the number of Planned Hours on the task. </p> <p><span class="bold">User Hourly Plus Fixed:</span> The billing rate set for a specific user, multiplied by the number of Planned Hours on the task from that user. In addition, a fixed amount that is specified on the task is added to the user rate. </p> <p>Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, the Utilization report calculates Planned Revenue by dividing Fixed Revenue evenly by the number of Planned Hours on the task.</p> <p><span class="bold">Role Hourly w/Cap: </span> Tasks are billed hourly as in Role Hourly, but they have a maximum Cap Amount that you can specify, as described in the section "Overview of Revenue Types" in the article <a href="billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> <p> Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, if the Planned Revenue exceeds the cap, the remainder is calculated as if it were Fixed Revenue, and Planned Revenue is calculated by dividing Fixed Revenue evenly by the number of hours logged on the task.<br></p> <p><span class="bold">User Hourly w/Cap:</span> Tasks are billed hourly as in User Hourly, but they have a maximum Cap Amount that you can specify, a s described in the section "Overview of Revenue Types" in the article <a href="billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> <p> Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, if the Planned Revenue exceeds the cap, the remainder is calculated as if it were Fixed Revenue, and Planned Revenue is calculated by dividing Fixed Revenue evenly by the number of hours logged on the task. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Actual Revenue</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Actual Revenue is the revenue associated with the Actual Hours of the tasks <span>and of the project</span>. For more information about Planned Revenue, see the section "Track Revenue amounts" in the article <a href="billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> <p>The way that the Utilization report calculates Actual Revenue for the included projects differs depending on the Revenue Type set on the task, as follows:</p> <p><span class="bold">Fixed Revenue:</span> Regardless of the task assignments, the revenue on the task is always calculated using the Fixed Amount specified on the task, as described in the section "Overview of Revenue Types" in the article <a href="billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> <p>Note:  If you have a Fixed Revenue task and there are no hours (Planned or Actual), it does not display correctly in the Utilization Report because there is no way to distribute hours. </p> <p><span class="bold">Role Hourly:</span> The revenue on the task is calculated using t he billing rate set for a specific role, multiplied by the number of Planned Hours, as described in the section "Overview of Revenue Types" in the article <a href="billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>. </p> <p><span class="bold">User Hourly:</span> The revenue on the task is calculated using the billing rate set for a specific user, multiplied by the number of hours logged against the task from that user, as described in the section "Overview of Revenue Types" in the article <a href="billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>. </p> <p><span class="bold">Role Hourly Plus Fixed:</span> The billing rate set for a specific role, multiplied by the number of hours logged against the task from a user with that role. In addition, a fixed amount that is specified on the task is added to the role rate. </p> <p>Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, the Utilization report calculates Actual Revenue by dividing Fixed Revenue evenly by the number of hours logged on the task.</p> <p> <p>Note:  If you have a Fixed Revenue task and there are no hours (Planned or Actual), it does not display correctly in the Utilization Report because there is no way to distribute hours. </p> </p> <p><span class="bold">User Hourly Plus Fixed:</span> The billing rate set for a specific user, multiplied by the number of hours logged against the task from that user. In addition, a fixed amount that is specified on the task is added to the user rate. </p> <p>Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, the Utilization report calculates Actual Revenue by dividing Fixed Revenue evenly by the number of hours logged on the task.</p> <p> <p>Note:  If you have a Fixed Revenue task and there are no hours (Planned or Actual), it does not display correctly in the Utilization Report because there is no way to distribute hours. </p> </p> <p><span class="bold">Role Hourly w/Cap:</span> Tasks are billed hourly as in Role Hourly, but they have a maximum Cap Amount that you can specify.</p> <p> Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, if the Actual Revenue exceeds the cap, the remainder is calculated as if it were Fixed Revenue, and Actual Revenue is calculated by dividing Fixed Revenue evenly by the number of hours logged on the task. </p> <p> <p>Note:  If you have a Fixed Revenue task and there are no hours (Planned or Actual), it does not display correctly in the Utilization Report because there is no way to distribute hours.</p> </p> <p><span class="bold">User Hourly w/Cap: </span> Tasks are billed hourly as in User Hourly, but they have a maximum Cap Amount that you can specify.</p> <p> Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, if the Actual Revenue exceeds the cap, the remainder is calculated as if it were Fixed Revenue, and Actual Revenue is calculated by dividing Fixed Revenue evenly by the number of hours logged on the task. </p> <p>Note:  If you have a Fixed Revenue task and there are no hours (Planned or Actual), it does not display correctly in the Utilization Report because there is no way to distribute hours.</p> 
    <div> 
     <p><span class="bold">Project Revenue</span>: The revenue associated with the hours logged on the project is calculated taking into account the Billing per Hour amount of the primary job role of the user who logs the time. </p> 
     <p>Note: If the user is not associated with a job role or if the Billing per Hour of the Primary Role is zero, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates Actual Revenue using the Billing per Hour amount for the user. If the user does not have a Billing per Hour amount in their profile, the Actual Revenue is zero. </p> 
    </div> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Budgeted Variance (for Revenue)</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The total Actual Revenue minus Budgeted Revenue on the included projects.<br>You can view the total budgeted variance for the overall life of the included projects, or you can view the total budgeted variance only for the specified date range (you can specify an individual week or month).</p> <p>If the value is positive, it is displayed in green. This indicates that the total Budgeted Revenue is greater than the Actual Revenue.</p> <p>If the value is negative, it is displayed in red. This indicates that the total Budgeted Revenue is less than the Actual Revenue.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><span class="bold">Planned Variance (for Revenue)</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>The total Actual Revenue minus the total Planned Revenue on the included projects.<br>You can view the total planned variance for the overall life of the included projects, or you can view the total planned variance only for the specified date range (you can specify an individual week or month). </p> <p>If the value is positive, it is displayed in green. This indicates that the total Planned Revenue is greater than the Actual Revenue.</p> <p>If the value is negative, it is displayed in red. This indicates that the total Planned Revenue is less than the Actual Revenue.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Compare Revenue against Planned and Actual Costs {#compare-revenue-against-planned-and-actual-costs}

You can view the Planned or Actual Cost alongside the Planned Revenue. The Margin (%) is also displayed (margin is calculated as Revenue - Cost / Revenue).


The following information is available in the Utilization report when comparing Revenue against Planned and Actual Costs: 

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 159px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Column Title When Viewing Revenue vs Cost (Planned)</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <span class="bold">Function</span></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Planned Cost</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> The total Planned Cost on the included projects. You can view the total Planned Cost for the overall life of the included projects, or you can view the total Planned Cost only for the specified date range (you can specify an individual week or month). </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Planned Revenue</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Planned Revenue is the revenue associated with the Planned Hours of the tasks. </p> <p>The way the Utilization report calculates and displays Planned Revenue for the included projects differs depending on the Revenue Type set on the task, as follows:</p> <p><span class="bold">Fixed Revenue:</span> Regardless of the task assignments, the revenue on the task is always calculated using the Fixed Amount specified on the task.</p> <p>Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, the Utilization report calculates Planned Revenue by dividing Fixed Revenue evenly by the number of hours logged on the task. <br>For example, a task has a revenue of $200. If 4 hours are logged on the task, each hour would be $50. This is distributed on a user and role level. This distribution is unique to the Utilization report.</p> <p>Note:  If you have a Fixed Revenue task and there are no hours (Planned or Actual), it does not display correctly in the Utilization Report because there is no way to distribute hours. </p> <p><span class="bold">Role Hourly:</span> The revenue on the task is calculated using t he billing rate set for a specific role, multiplied by the number of Planned Hours. </p> <p><span class="bold">User Hourly:</span> The revenue on the task is calculated using the billing rate set for a specific user, multiplied by the number of hours logged against the task from that user. </p> <p><span class="bold">Role Hourly Plus Fixed: </span>The revenue on the task is calculated using the billing rate set for a specific role, multiplied by the number of Planned Hours. In addition, a fixed amount that is specified on the task is added to the role rate.</p> <p>Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, the Utilization report calculates Planned Revenue by dividing Fixed Revenue evenly by the number of hours logged on the task. </p> <p><span class="bold">User Hourly Plus Fixed:</span> The billing rate set for a specific user, multiplied by the number of hours logged against the task from that user. In addition, a fixed amount that is specified on the task is added to the user rate. </p> <p>Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, the Utilization report calculates Planned Revenue by dividing Fixed Revenue evenly by the number of hours logged on the task.</p> <p><span class="bold">Role Hourly w/Cap: </span> Tasks are billed hourly as in Role Hourly, but they have a maximum Cap Amount that you can specify.</p> <p> Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, if the Planned Revenue exceeds the cap, the remainder is calculated as if it were Fixed Revenue, and Planned Revenue is calculated by dividing Fixed Revenue evenly by the number of hours logged on the task.<br></p> <p><span class="bold">User Hourly w/Cap:</span> Tasks are billed hourly as in User Hourly, but they have a maximum Cap Amount that you can specify.</p> <p> Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, if the Planned Revenue exceeds the cap, the remainder is calculated as if it were Fixed Revenue, and Planned Revenue is calculated by dividing Fixed Revenue evenly by the number of hours logged on the task. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Margin</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The Margin percentage is calculated as follows:</p> <p>Planned Revenue - Planned Cost / Planned Revenue * 100. </p> <p>Note:  If Planned Revenue equals 0, Margin is displayed as 0.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Column Title When Viewing Revenue vs Cost (Actual)</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"><span class="bold">Function</span> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Actual Cost</span> </td> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The total Actual Cost on the included projects. You can view the total Actual Cost for the overall life of the included projects, or you can view the total Actual Cost only for the specified date range (you can specify an individual week or month).</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Actual Revenue</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Actual Revenue is the revenue associated with the Actual Hours of the tasks.</p> <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p> <p>The way that the Utilization report calculates Actual Revenue for the included projects differs depending on the Revenue Type set on the task, as follows:</p> <p><span class="bold">Fixed Revenue:</span> Regardless of the task assignments, the revenue on the task is always calculated using the Fixed Amount specified on the task.</p> <p>Note:  If you have a Fixed Revenue task and there are no hours (Planned or Actual), it does not display correctly in the Utilization Report because there is no way to distribute hours. </p> <p><span class="bold">Role Hourly:</span> The revenue on the task is calculated using t he billing rate set for a specific role, multiplied by the number of Planned Hours. </p> <p><span class="bold">User Hourly:</span> The revenue on the task is calculated using the billing rate set for a specific user, multiplied by the number of hours logged against the task from that user. </p> <p><span class="bold">Role Hourly Plus Fixed:</span> The billing rate set for a specific role, multiplied by the number of hours logged against the task from a user with that role. In addition, a fixed amount that is specified on the task is added to the role rate. </p> <p>Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, the Utilization report calculates Actual Revenue by dividing Fixed Revenue evenly by the number of hours logged on the task.</p> <p> <p>Note:  If you have a Fixed Revenue task and there are no hours (Planned or Actual), it does not display correctly in the Utilization Report because there is no way to distribute hours. </p> </p> <p><span class="bold">User Hourly Plus Fixed:</span> The billing rate set for a specific user, multiplied by the number of hours logged against the task from that user. In addition, a fixed amount that is specified on the task is added to the user rate. </p> <p>Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, the Utilization report calculates Actual Revenue by dividing Fixed Revenue evenly by the number of hours logged on the task.</p> <p> <p>Note:  If you have a Fixed Revenue task and there are no hours (Planned or Actual), it does not display correctly in the Utilization Report because there is no way to distribute hours. </p> </p> <p><span class="bold">Role Hourly w/Cap:</span> Tasks are billed hourly as in Role Hourly, but they have a maximum Cap Amount that you can specify.</p> <p> Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, if the Actual Revenue exceeds the cap, the remainder is calculated as if it were Fixed Revenue, and Actual Revenue is calculated by dividing Fixed Revenue evenly by the number of hours logged on the task. </p> <p> <p>Note:  If you have a Fixed Revenue task and there are no hours (Planned or Actual), it does not display correctly in the Utilization Report because there is no way to distribute hours.</p> </p> <p><span class="bold">User Hourly w/Cap: </span> Tasks are billed hourly as in User Hourly, but they have a maximum Cap Amount that you can specify.</p> <p> Unlike in other areas of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, if the Actual Revenue exceeds the cap, the remainder is calculated as if it were Fixed Revenue, and Actual Revenue is calculated by dividing Fixed Revenue evenly by the number of hours logged on the task. </p> <p> <p>Note:  If you have a Fixed Revenue task and there are no hours (Planned or Actual), it does not display correctly in the Utilization Report because there is no way to distribute hours.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><span class="bold">Margin</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>The Margin percentage is calculated as follows:</p> <p>Actual Revenue - Actual Cost / Actual Revenue * 100. </p> <p>Note:  If Actual Revenue equals 0, Margin is displayed as 0.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Track progress, cost, and revenue with the Utilization report {#track-progress-cost-and-revenue-with-the-utilization-report}

You can track the progress or cost of a project, program, or portfolio.


You can display information on the Utilization report for a given week or month, or for the overall life of the projects. 


To track the progress or cost of one or more projects with a Utilization report:



1. Do any of the following, depending on whether you are viewing utilization information for an individual project, multiple projects, a program, or a portfolio: 
    
    
    * To view utilization information for a single project:     
        
        
        1. Go to a project for which you want to view utilization information, then click `Show More> Utilization`. 
        1. Utilization information is displayed automatically when viewing an individual project, and applying a filter is not required.   
           If you want to filter the Utilization report, you can apply a filter, then click `Run`.  
           For information about how to filter the Utilization report, see the section [Filter utilization information](#filtering-utilization-information) in this article.   
           Utilization information is displayed for individual users and roles (users are grouped within their associated role).
        
        
    * To view utilization information for multiple projects:     
        
        
        1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Resourcing`, then `Utilization` in the left panel. 
        1. Apply a filter to the Utilization report, then click `Run`.   
           You must specify one or more projects in the filter prior to running the Utilization report. For information about how to filter the Utilization report, see the section [Filter utilization information](#filtering-utilization-information) in this article.  
           Utilization information is displayed for individual roles and projects (roles are grouped within their associated project).  

        
        
    * To view utilization information for a program:     
        
        
        1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Resourcing`, then `Utilization` in the left panel and click the `Show`> `Programs`.
        1. Apply a filter to the Utilization report, then click `Run`.   
           You must specify one or more programs in the filter prior to running the Utilization report. For information about how to filter the Utilization report, see the section [Filter utilization information](#filtering-utilization-information) in this article.   
           Utilization information is displayed for individual projects and programs (projects are grouped within their associated program).  

        
        
    * To view utilization information for a portfolio:     
        
        
        1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Resourcing`, then `Utilization` in the left panel and click `Show`> `Portfolios`.
        1. Apply a filter to the Utilization report, then click `Run`.   
           You must specify one or more portfolios in the filter prior to running the Utilization report. For information about how to filter the Utilization report, see the section [Filter utilization information](#filtering-utilization-information) in this article.   
           Utilization information is displayed for individual projects, programs, and portfolios (projects are grouped within their associated program, and programs are grouped within their associated portfolio).  

        
        
    
    
1. In the upper-right corner of the Utilization report, click the `View` drop-down menu, then select from the following: 
    
    
    * `Cost`
    * `Hours`
    * `Revenue`
    * `Revenue vs. Cost (Planned)`
    * `Revenue vs Cost (Actual)`.
    
    
   The option you select determines which columns and information are available in the report. For more details about the information available in each column, see the table in Step 5.  
   ![](assets/utilization-view-dropdown.png)



1. (Optional) Select the date range for which utilization information is displayed. You can display information for a given week or month to the left of the `Overall` column. Information for the overall project, program, or portfolio is always displayed in the `Overall` column.  
   For more information, see the section [Adjust the date range for which information is displayed](#adjusting-the-date-range-for-which-information-is-displayed) in this article. 

1. (Optional) Click any column title to sort the utilization report by the information in that column. Sorting works only when you include multiple items in your report. For example, you can sort the results of your report when you are looking at more than one project (or portfolio or program). You cannot sort the results when you are looking at only one project (or one portfolio or one program) at a time.  
1. Use the information in the section [Overview of the Utilization report](#understanding-the-utilization-report) in this article to learn about each column in the Utilization report.




## Filter utilization information {#filter-utilization-information}

You can filter the content displayed in a Utilization report on a project. You can filter on tasks, issues, roles, and custom data. When you apply a filter to the Utilization report, the Utilization report contains information based on the criteria that you select.


You can create a filter, or apply a filter that you previously created.



* [Create or modify a filter](#creating-a-filter) 
* [Apply a saved filter](#applying-a-saved-filter) 
* [Duplicate a filter](#duplicating-a-filter) 
* [Rename a filter](#renaming-a-filter) 
* [Delete a filter](#deleting-a-filter) 




### Create or modify a filter {#create-or-modify-a-filter}

When you create a filter, all *`Workfront`* users who have access to the Utilization report also have access to the filter you create. Similarly, when you modify an existing filter, the filter is modified for all users who have access to the Utilization report.


To create or modify a filter:



1.  To filter utilization information for a single project, go to the project for which you want to filter utilization information, then click `Show More>Utilization` in the left panel. 


   Or


   To filter utilization information for multiple projects, for a program, or for a portfolio, click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Resourcing`, then `Utilization` in the left panel and click `Show`> `Programs` `or` `Portfolios` `or` `Projects`.

1.  Click the `Filter` icon to display the filter options.  

1. (Conditional) To modify an existing filter, click the `Filter` drop-down menu, then select the filter you want to modify.
1.  Specify the following information to create or modify the filter:

    
    
    * `Portfolios:` Begin typing the name of the portfolio that contains the information you want to include in the Utilization report, then click the name when it appears in the drop-down menu.  
      Repeat this process to include information from multiple portfolios in the Utilization report.  
      To include all portfolios from your system in your filter, click `Add all`. (This option is available only if you have fewer than 10 portfolios in your system.)
    
    * `Programs:` Begin typing the name of the program that contains the information you want to include in the Utilization report, then click the name when it appears in the drop-down menu.  
      Repeat this process to include information from multiple tasks in the Utilization report.  
      If you already designated any portfolios in the filter, the program you specify must be from the portfolios already included in the filter. If it is not, data from the program is not included in the Utilization report.  
      To include all programs from your system in your filter, click `Add all`. (This option is available only if you have fewer than 20 programs in your system.)
    
    * `Projects:` Begin typing the name of the project that contains the information you want to include in the Utilization report, then click the name when it appears in the drop-down menu.  
      Repeat this process to include information from multiple projects in the Utilization report.  
      If you already designated any portfolios or programs in the filter, the project you specify must be from one of the portfolios or programs already included in the filter. If it is not, data from the project is not included in the Utilization report.  
      To include all projects from your system in your filter, click `Add all`. (This option is available only if you have fewer than 250 projects in your system.)
    
    * `Tasks:` Begin typing the name of the task that contains the information you want to include in the Utilization report, then click the name when it appears in the drop-down menu.  
      Repeat this process to include information from multiple tasks in the Utilization report.  
      If you already designated any portfolios, programs, or projects in the filter, the task you specify must be from one of the portfolios, programs, or projects already included in the filter. If it is not, data from the task is not included in the Utilization report.
    
    * `Issues:` Begin typing the name of the issue that contains the information you want to include in the Utilization report, then click the name when it appears in the drop-down menu.  
      Repeat this process to include information from multiple issues in the Utilization report.  
      If you already designated any portfolios, programs, or projects in the filter, the issue you specify must be from one of the portfolios, programs, or projects already included in the filter. If it is not, data from the issue is not included in the Utilization report.  
      Cost information for issues is not always included in the Utilization report. For more information about when cost information for issues is included in the Utilization report, see the section [Track progress, cost, and revenue with the Utilization report](#tracking-progress-and-cost-with-a-utilization-report) in this article. 
    
    * `Roles:` Begin typing the name of the role you want to be represented in the Utilization Report, then click the name when it appears in the drop-down menu. Repeat this process to include additional roles.  
      The Utilization Report contains information only for the roles you specify. For example, a task contains 10 Actual Hours. 6 of those hours are from a Designer role and 4 are from a Developer role. If you filter the Utilization Report by role for Designer, the 4 hours that come from the Developer role are excluded from the report.
    
    *  `Add Filter Rule:` Click `Add Filter Rule`, click in the first field, then begin typing the field name that you want to filter on. If the field is available, it populates for each object where it can be associated. Click the name of the field to add it to the filter. 
    
    
      >[!IMPORTANT] {type="important"}
      >
      >`You must type the field name and not the field label. The field label displays on a custom form attached to an object. For information about the difference between the label and the name of a custom field, see` ` [Create or edit a custom form](create-or-edit-a-custom-form.md)`. 
    
    
      For more information about the fields you see in the columns, see [Glossary of Adobe Workfront terminology](workfront-terminology-glossary.md).   
      Choose the filter and condition modifiers for the filter. The available modifiers are described in [Filter and condition modifiers](filter-condition-modifiers.md).
    
    
    

1. To create a new filter, click `Save Filter`.  
   Or  
   To modify an existing filter, click the drop-down arrow next to the `Save Filter` button, then click `Save New Filter`.  
   In the `Filter Name` field, specify a name for the filter, then click `Save`.  
   The Utilization area is filtered with the information you included in the filter.





### Apply a saved filter {#apply-a-saved-filter}




1.  To apply a filter on the Utilization Report for a single project, go to the project for which you want to filter, then click `Show More>Utilization` in the left panel. 


   Or


   To apply a filter on the Utilization Report for multiple projects, for a program, or for a portfolio, click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Resourcing`, then `Utilization` in the left panel and click `Show`> `Programs` `or` `Portfolios` `or` `Projects`.

1. Click `Saved Filters`, then select the filter you want to apply from the drop-down menu.




### Duplicate a filter {#duplicate-a-filter}




1.  To duplicate a filter on the Utilization Report for a single project, go to the project for which you want to duplicate the filter, then click `Show More>Utilization` in the left panel. 


   Or


   To duplicate a filter on the Utilization Report for multiple projects, for a program, or for a portfolio, click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Resourcing`, then `Utilization` in the left panel.

1.  Click `Saved Filters`, mouse over the filter you want to duplicate in the drop-down menu, then click the `Duplicate` icon.  



   ![](assets/utilization-filter-duplicate.png)   
   The Duplicate Filter dialog box is displayed.

1. In the `Filter Name` field, specify a name for the new filter, then click `Save`.





### Rename a filter {#rename-a-filter}

When you rename a filter, all *`Workfront`* users who have access to the Utilization report see the new name that you choose.


To rename a filter:



1.  To rename a filter on the Utilization Report for a single project, go to the project for which you want to rename the filter, then click `Show More>Utilization` in the left panel. 


   Or


   To rename a filter on the Utilization Report for multiple projects, for a program, or for a portfolio, click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Resourcing`, then `Utilization` in the left panel.

1. Click `Saved Filters`, mouse over the filter you want to duplicate in the drop-down menu, then click the `Rename` icon.  
   ![](assets/utilization-filter-rename.png)  
   The Rename Filter dialog box is displayed.

1. In the `Filter Name` field, specify a name for the new filter, then click `Save`.





### Delete a filter {#delete-a-filter}

When you delete a filter, the filter is deleted for all *`Workfront`* users who have access to the Utilization report.


To delete a filter: 



1.  To delete a filter on the Utilization Report for a single project, go to the project for which you want to delete the filter, then click `Show More>Utilization` in the left panel. 


   Or


   To delete a filter on the Utilization Report for multiple projects, for a program, or for a portfolio, click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Resourcing`, then `Utilization` in the left panel.

1.  Click `Saved Filters`, mouse over the filter you want to duplicate in the drop-down menu, then click the `Delete` icon.  



   ![](assets/utilization-filter-delete.png)



1. Click `Delete` when prompted whether you want to delete the filter. 




## Adjust the date range for which information is displayed {#adjust-the-date-range-for-which-information-is-displayed}

You can adjust the date range for which utilization information is displayed. You can select a past or future date. Changes you make are visible only to you.



1.  To adjust the date range of the Utilization Report for a single project, go to the project for which you want to adjust the date range, then click `Show More>Utilization` in the left panel. 


   Or


   To adjust the date range of the Utilization report for multiple projects, for a program, or for a portfolio, click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Resourcing`, then `Utilization` in the left panel.

1.  Click the date range next to the `Export` button. 


   The current week is selected by default. 

1.  Select from the following options:

    
    
    * `Week:` Select this option to select a given week (from Sunday through Saturday).
    * `Month:` Select this option to select a given month.
    
    
   The date range you select is displayed in the utilization report, to the left of the `Overall` column.  
   *`Workfront`* remembers whether you want to view a week or month view. The next time you access the utilization report, the current week or current month is shown, depending on the option you select.





## Export utilization information {#export-utilization-information}

You can export utilization information for a project, program, or portfolio from *`Workfront`*. Information can be exported only in XLSX, TSV, and PDF formats.


When viewed in Microsoft Excel, negative numbers are displayed in parenthesis.


To export utilization information:



1.  To export utilization information for a single project, go to the project for which you want to export utilization information, then click the `Utilization` tab (depending on your layout settings, this might be located under the `More` tab).


   Or


   To export utilization information for multiple projects, for a program, or for a portfolio, click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Resourcing`, then `Utilization` in the left panel.

1. Click `Export`, located in the upper-left corner of the `Utilization` tab.

1. Select from the following options: 
    
    
    * `PDF:` Exports the report in PDF format. This is the recommended format if you are planning to print the report.  
      Select either `Letter - Portrait`, `Letter - Landscape`, or `Other Sizes` (provides options for exporting in Legal (8.5" x 14"), Ledger (11" x 17"), and A4).  
      Depending on the operating system you use, you might have the option of opening or saving the file. Either open the file with the associated application or save it to your hard drive.
    
    * `Excel:` Exports the report in XLSX format. This is the recommended format if you are planning to further analyze the data in Excel.  
      Depending on the operating system you use, you might have the option of opening or saving the file. Either open the file with the associated application or save it to your hard drive.
    
    * `Tab Delimited:` Exports the report in TSV format. This is the recommended format if you are planning to import the data into third-party software for further analysis.  
      Depending on the operating system you use, you might have the option of opening or saving the file. Either open the file with the associated application or save it to your hard drive.
    
    
    
1. Read the information in the article [Export data](export-data.md) to understand how to use the exported file. 




## View utilization information in a chart {#view-utilization-information-in-a-chart}

You can visualize the data from the Utilization report in a chart view. 



1.  To view a Utilization report for a single project in a chart format, go to the project you want to view, then click `Show More> Utilization` in the left panel. 


   Or


   To view a Utilization report in a chart format for multiple projects, for a program, or for a portfolio, click `Reporting` in the Global Navigation Bar to go to the Reporting area, then click the `Utilization` tab.

1. In the upper-right corner of the Utilization report, click the `Chart` icon.  
   ![](assets/utilization-chart.png)  
   The Utilization report is displayed in a chart view. 

1. (Optional) Configure this to show Projects, Programs, or Portfolios by selecting the appropriate option from the `Show` drop-down menu.
1.  (Optional) Mouse over a specific point in time on the report to view data for that point in time. 
1. (Optional) Adjust the filters to decide what information is displayed in the chart. For information about adjusting the filters, see the section [Filter utilization information](#filtering-utilization-information) in this article. 
1. (Optional) Configure the timeframe of the chart report, as described in the section [Adjust the date range for which information is displayed](#adjusting-the-date-range-for-which-information-is-displayed) in this article. 


