---
title: Replacement of Flash-based tools in Adobe Workfront
description: Replacement of Flash-based tools in Adobe Workfront
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
---
# Replacement of Flash-based tools in Adobe Workfront

We have removed all Flash-based tools from Adobe Workfront Classic.

Replacement tools that are based on current standards are available now in Workfront. These changes align with the end of support for Flash products as announced by Adobe.

## Important dates

The following dates are important for the removal process of all Flash-based tools in Workfront:

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **November 19, 2020**: All Flash-based tools have been removed from all Workfront products. 

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## Legacy Flash-based tools

The tools listed in the following sections have been removed from the Workfront system and replaced with new solutions.

For information about replacement tools, see [Legacy Flash-based tools and their replacements](#legacy-flash-based-tools-and-their-replacements) in this article.

### Resource Management

* The Legacy Resource Planning tab in the People area and all the tools contained in the tab, which includes the following:

   * Resource Budget Manager
   * Capacity Planner
   * Resource Estimates
   * Resource Grid  
     For more information, see [Resource Planning: article index](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* The Legacy Resource Estimates area in the Business Case of a project

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  is displayed in view-only mode
  </MadCap:conditionalText>
  -->

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  For more information, see
  <a href="../../../resource-mgmt/resource-mgmt-overview/migrate-resource-estimates-to-budgeting.md" class="MCXref xref">Migrate from Legacy Resource Estimates to Resource Budgeting </a>
  </MadCap:conditionalText>
  -->

  .   

* The Resource Grid subtab in the Staffing tab of a project
* The Use New Scheduling Area option in the Scheduling subtab of the Staffing tab of a project which removes the legacy Scheduling area or the Team Builder. In this case, the Scheduling timeline now displays by default.
* The Allocation tab under the user profile

### Reports

The following reporting features and reports have been removed:

* Removed reporting features:

   * The Resource Grid option in a user report
   * The Legacy Gantt option in a project or task report  
     For more information, see [View information in the Gantt Chart](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* Removed reports:

   * The Legacy Resource Pool report
   * The Resource Estimates report

  >[!NOTE]
  >
  >All legacy fields accessed through reports or through the API (Legacy Resource Pool, Legacy Budgeted Cost, Legacy Cost, Legacy Budgeted Hours, Legacy Budgeted Labor Cost, etc) display in various reports, but do not populate with new information.

### Legacy Gantt

* All Legacy Gantt views from project and task lists, as well as reports and reporting options
* The Legacy Gantt subtabs in Portfolios and Programs
* The Legacy Gantt subtab in a list of Template Tasks on a Template, the Legacy Gantt view in the Subtasks tab of a Template Task, and in a Template Task report

### Proofing

The Legacy proofing viewer has been replaced with the new Web Proofing Viewer and Desktop Proofing Viewer for most customers and has been removed for all customers in November 2020.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

For more information, see the following resources:

* [Review proofs in the Web Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md) 
* [Review proofs in the Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-proof/wp-work-proofsfiles/review-proofs-lpv/lpv-removed-2018.md" class="MCXref xref">Legacy proofing viewer removed in 2018.3</a> </li>
  -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Additional features to be removed</h3>
<ul>
<li>The Legacy Portfolio Optimizer<br>For more information, see <a href="../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md" class="MCXref xref">Portfolio Optimizer overview</a>.<br></li>
<li>The Legacy financial fields in the Business Case of the project and the Portfolio Optimizer</li>
<li>The dialog boxes used when sharing reports, calendars, and documents no longer rely on Flash-based technology</li>
</ul>
</div>
-->

## Legacy Flash-based tools and their replacements {#legacy-flash-based-tools-and-their-replacements}

Except where specified otherwise, all Legacy features have been replaced by new ones, as shown in the following table.

>[!CAUTION]
>
>The legacy Flash-based tools have been removed from all environments.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Legacy Tools</strong> </p> </th> 
   <th> <p><strong>New Tools</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Legacy Resource Pools</strong> </p> <p>Legacy Resource Pools were groups or collections of job roles needed at the same time for the completion of a project. Legacy Resource Pools had a number of shortcomings:</p> 
    <ul> 
     <li> You could associate a user with one Legacy Resource Pool but it was only used for reporting purposes. Since Legacy Resource Pools were operating with abstract job role entities, none of the users' schedule exceptions and time off were taken into account, resulting in inaccurate data about resource availability. </li> 
    </ul> 
    <ul> 
     <li>You could specify only one Legacy Resource Pool per project, which resulted in multiple Legacy Resource Pools supporting only the flow of separate groups working independently of each other and never sharing resources. In all other cases, it was recommended to keep one Legacy Resource Pool that included all resources in the system, which led to performance problems with large amounts of projects and data.</li> 
    </ul> </td> 
   <td> <p><strong>Resource Pool</strong> </p> <p>New Resource Pools are a collection of users that are needed at the same time for the completion of the project. Workfront also realizes that there are cases when specialized users need to have work allocated to them separately. For this reason, you can now budget users instead of job roles. </p> Advantages of the Resource Pool over the Legacy Resource Pools include the following: 
    <ul>
     <li>Because Resource Pools are based on the users, their time off and schedule exceptions are already taken into account for the user and role availability calculations. This results in precise and up-to-date data, allowing for correct budgeting decisions and minimizing the likelihood of changes when the project is in flight.</li>
     <li>Because there is now more control over the availability of resources and accuracy of data, Workfront allows you to associate multiple Resource Pools with a project. One user can also belong to more than one Resource Pool, in case they have multiple skills that could be used in multiple projects at the same time. </li>
    </ul><p>With such control over the data, it is no longer necessary to have one Resource Pool that includes all resources for distributing the available budget. In fact, we do not recommend this. Instead, we recommend diversifying your Resource Pools and only associating relevant Resource Pools with projects.</p><p> For more information about Resource Pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Resource Budget Manager</strong> </p> <p>You could use the Resource Budget Manager to specify the availability of job role resources across multiple Resource Pools. However, due to the shortcomings of the Legacy Resource Pool, this functionality was rarely used. When it was used, it forced users to manually input availability of job roles to make budgeting more accurate. The schedule exceptions and the users' time off were not taken into account.</p> </td> 
   <td> <p>With the automatic calculation of availability based on the users in the Resource Pools, the Resource Budget Manager is no longer needed. The tool has been eliminated, along with all the manual work for calculating availability.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Resource Estimates</strong> </p> <p>The Resource Estimates tab under each Legacy Resource Pool served the same purpose as the Resource Budget Manager, only in the context of one Legacy Resource Pool. This tool presented the same limitations as the Resource Budget Manager and the Legacy Resource Pools: inaccurate data and manual input of availability. </p> </td> 
   <td> <p>With the automatic calculation of user availability, Resource Estimates have become obsolete and have been removed.</p> <p>The tool is eliminated on the Legacy Resource Pools and the Legacy Resource Estimates in the Business Case of a project. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Capacity Planner</strong> </p> <p>The Capacity Planner was a Workfront tool for budgeting resources and prioritizing projects inside a Legacy Resource Pool, according to the availability of the resources. Given the incompleteness of data from Resource Estimates and the Resource Budget Manager which provided the information for the Capacity Planner, project prioritization had to be double-checked against the availability of the users.</p> <p>Using a single Legacy Resource Pool that included all the job roles in the system was the most common scenario, which led to performance problems with the Capacity Planner trying to load a large number of projects.</p> </td> 
   <td> <p><strong>The Project View of the Resource Planner</strong> </p> <p>In the Project-based view of the Resource Planner, you can budget resources and prioritize projects similarly to how you used to do it in the Legacy Capacity Planner. Unlike the legacy tool, more data is now supported, with the available information being more precise by taking into account both the users' time off and schedule exceptions.</p> <p>Available, Planned, and Budgeted information is visible at a glance so that Resource Managers can see both whether there are enough people to do the work and whether the project plans exceed initial budget estimations.</p> <p> For information about using the Project View in the Resource Planner, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a></p> <p><strong>The Scenario Planner</strong> </p> <p>For long-term capacity planning, what-if scenario modeling and prioritization, we have also introduced the Workfront Scenario Planner . </p> <p>The Scenario Planner is available only in the new Adobe Workfront experience and requires an additional license. For information about the Workfront Scenario Planner, see <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The Scenario Planner overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Legacy Resource Estimates (Business Case)</strong> </p> <p>You could use the Legacy Resource Estimates area of the Business Case to budget a certain amount of labor hours and costs as part of the project planning and request for resources. This view didn't provide any visibility into the availability of resources, which resulted in approximate requests for resources and an increased chance for rejected project work.</p> </td> 
   <td> <p><strong>Resource Budgeting (Business Case)</strong> </p> <p>The Resource Budgeting section under the Business Case brings Resource Planner capabilities to the Business Case, providing visibility into user and role availability, as well as the ability to budget at the user level. </p> <p> For information about the Resource Budgeting area of the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">Overview of the Areas of the Business Case</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Resource Estimate Reports</strong> </p> <p>When using the legacy tools for Resource Management, you could report on Budgeted and Planned hours from the Business Case. This allowed you to build matrix reports showing the total Budgeted and Planned work for each job role in a specific time frame. This report was not editable, and you could not make any changes in the budgeting of your resources based on the report findings. </p> </td> 
   <td> <p><strong>Utilization Report</strong> </p> <p>The built-in Utilization report displays Planned, Budgeted, and Actual Hours, Cost, and Revenue side-by-side. </p> <p>For information about using the Utilization report, see <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">View resource utilization information </a>. </p> 
    <div> 
     <p><strong>Reportable Budgeted Hours</strong> </p> 
     <p>Create a report for Budgeted Hours to review hours budgeted in the Resource Planner in a report form. </p> 
     <p>For information about Budgeted Hours, see <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossary of Adobe Workfront terminology</a>.</p> 
     <p>For information about creating a report, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> 
    </div> <p><strong>The Role View of the Resource Planner</strong> </p> <p>The budgeted and planned hours from the Business case in the Legacy Resource Management tools are now available in a new native view - the Role-based view of the Resource Planner. This view provides Available, Planned, and Budgeted Hours information at a glance and allows you to control and change budgeting all in the same place. This ensures better decision making during high-level job role planning. </p> <p> For information about budgeting resources in the Role View of the Resource Planner, see the <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">Use the Project and Role Views to budget resources </a> section in <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Resource Grid</strong> </p> <p>The Resource Grid gave you visibility into the allocation of specific users as a project progressed towards completion. </p> <p>For example, you could easily see when someone on your project team got their work done early, and when someone fell behind, as well as whether they were overallocated or underallocated for a specific time frame. </p> <p>Unfortunately, you were not able to act upon the information in the same view. To rectify overallocation problems you had to go to the projects and manually adjust the information there without any visibility into the result of your actions.</p> </td> 
   <td> <p>The Resource Grid has been replaced by two new tools. You can use the following tools, depending on which phase of resource planning you find yourself in:</p> 
    <ul> 
     <li> <p><strong>For the Analytical Phase:</strong> </p> 
      <ul> 
       <li> <p><strong>The Workload Balancer</strong>: Use the Workload Balancer to view the users' workload at a more granular level. When you use the Workload Balancer, you can view which users have availability in their workload to complete the task on time. This includes their time off and schedule exceptions details. </p> <p>For information about the Workload Balancer, see <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Workload Balancer overview</a>.</p> </li> 
       <li> <p><strong>The User View of the Resource Planner</strong><strong>:</strong> When trying to understand on a higher level what projects your users are allocated to, use the User View of the Resource Planner. This allows you to see what users are working on as well as their over- and underallocation for a specific time frame. The Resource Planner also provides visualization of the overall allocation of users as a whole, as well as visibility into the Actual Hours logged, which is helpful in analyzing progress of the work done. </p> <p>For information about using the User View in the Resource Planner, see the <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">Use the User View to view Available, Planned, and Actual Hours or FTE </a> section in <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a></p> </li> 
      </ul> </li> 
     <li><strong>For the Tactical Phase:</strong> 
      <ul> 
       <li><strong>The Workload Balancer</strong> You can do the following using the Workload Balancer: 
        <ul>
         <li>Assign work to users.</li>
         <li>Manage users' allocations to work items. </li>
         <li>Share the Workload Balancer with other users who may not have visibility into the People area. Use the Shareable link functionality to share a link to the Workload Balancer and embed it in custom dashboards. Any users with access to View users are able to view these dashboards when you share them.</li>
        </ul><p>The Workload Balancer is available in the People area. </p><p>For information about the Workload Balancer, see <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Workload Balancer overview</a>.</p></li> 
      </ul> <!--
       <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <li><strong>The Resource Scheduling Areas</strong><strong>:</strong> When assigning your resources to the actual work that must be completed, use the Resource Scheduling areas in the People or Team areas, or at the project level. These areas allow you to visualize and manage the users' workload by day and rectify any problems from one view using the following actions: 
         <ul>
          <li> manual dragging and dropping of tasks to the correct assignee </li>
          <li> automatic assigning of tasks </li>
          <li> bulk swapping assignments </li>
          <li><p>adjusting Planned Hours according to the true availability of users. </p></li>
         </ul><p>These actions provide even more control over managing workload. </p><p> For information about managing user assignments and allocations in the Resource Scheduling areas, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p><p>With this new functionality, the Resource Grid is replaced by the User View of the Resource Planner and the Resource Scheduling areas in the following areas of the application: </p>
         <ul>
          <li>People - the Resource Grid is eliminated along with the Legacy Resource Planning tab.</li>
          <li>Project - the Scheduling area under the Staffing tab of the project is available to Work and Plan license users. They do not have to have Manage access to the project to view this area. </li>
          <li>Reporting - the ability to view User reports in the Resource Grid view is removed. Instead, there is an option to share a URL for the User View of the Resource Planner and embed it in custom dashboards, providing visibility into user utilization to virtually anyone in the system. Any users with access to View users are able to view these dashboards when you share them. </li>
          <li>User - the Allocation tab is eliminated as the same information can be accessed in the User View of the Resource Planner.</li>
         </ul></li> 
       </ul>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Legacy Gantt Chart, Task List</strong> </p> <p> The Legacy Gantt chart on the task list provided users with the ability to visually see the timeline of the project and perform what-if scenario planning without committing changes to the database. The Legacy Gantt chart was based on Flash technology, which presented security risks. </p> </td> 
   <td> <p><strong>Gantt Chart,</strong> <strong>Task List</strong></p> <p> The new HTML-based Gantt Chart is serving the same purpose as the Legacy Gantt. Users can visualize the timeline of the project and perform what-if scenario planning without committing changes to the database by changing to the Manual Save option from the task list toolbar. </p> <p>The new Gantt Chart is interactive when using the Autosave option which you can use when you want to automatically save your changes as they happen. </p> <p>The new Task List Gantt Chart is built on the newest technology and is reliable. This new Gantt chart is located directly on the task list and is easily accessed while working on the task list without switching tabs or changing the view. </p> <p>Although the new Gantt chart offers the same functionality as the previous chart, there are some differences in features by comparison with the Legacy Gantt. </p> <p> The Legacy Gantt subtab in a list of Template Tasks on a Template, the Legacy Gantt view in the Subtasks tab of a Template Task, and the Legacy Gantt chart in a Template Task report have been replaced with the HTML-based Gantt chart as well. </p> <p>If you use the Legacy Gantt Chart mostly for the simple view and quick edits and don't use the actual chart, the new Timeline Planning option allows you to make quick changes to key planning fields. You can select Timeline Planning instead of Autosave from the task list toolbar.</p> <p>For more information about saving a task list using the Timeline Planning option, see the section "Save changes in a task list manually when you select the Timeline Planning option" in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Edit tasks in a list</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Legacy Gantt Chart for a Project List</strong> </p> <p>The Legacy Gantt chart on the project list provided users with the ability to see projects and their tasks in one view. Without leaving the context of the project list, users could see details about the tasks in a project as well as the dependencies between the projects. The Legacy Gantt chart on the project list was based on Flash technology, which presented security risks. </p> </td> 
   <td> <p><strong>Gantt Chart, Project List</strong> </p> <p>The HTML-based Gantt chart serves the same purpose as the Legacy Gantt chart. Users can view projects and their tasks in one view to visually identify dependencies between projects as well as tasks. The Project List Gantt chart is located directly on the project list. The new Gantt chart has a modern interface and is built on the newest technology.</p> <p>For information about the project list Gantt chart, see <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">View information in the Gantt Chart </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Sharing Dialog Boxes for Reports, Calendars, and Documents</strong> </p> <p>When sharing reports, calendars, and documents, the dialog boxes that were used were based on Flash technology.</p> </td> 
   <td> <p>The experience when sharing reports, calendars, and documents in Workfront has not changed. However, the experience no longer relies on Flash.</p> <p>For more information about sharing these items, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Legacy proofing viewer</strong> </p> <p>The Legacy proofing viewer was a web-based proofing viewer that provided proofing capabilities for static, video, and interactive proofs.</p> </td> 
   <td> <p><strong>Web Proofing Viewer and Desktop Proofing Viewer</strong> </p> <p>The Web Proofing Viewer provides proofing capabilities for static and video proofs.</p> <p>The Desktop Proofing Viewer provides proofing capabilities for interactive proofs, in addition to providing full support for static and video proofs.</p> <p>The SWF file format is no longer supported by any of the major providers and has been replaced with HTML5 banners for proofing. </p> <p>For more detailed information about the differences between the available proofing viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
