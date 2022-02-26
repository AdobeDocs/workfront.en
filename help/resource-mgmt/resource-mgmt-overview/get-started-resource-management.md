---
filename: get-started-resource-management
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: Get started with Resource Management
description: Resource Management allows you to configure your system to accurately forecast the use of your resources based on their availability so that the work that must be done is completed on time and on budget.
---

# Get started with Resource Management

Resource Management allows you to configure your system to accurately forecast the use of your resources based on their availability so that the work that must be done is completed on time and on budget.

## Overview of Resource Management in *Adobe Workfront*

Resource Management refers to all the activities performed by the *Adobe Workfront administrator*, the resource manager, and the Project Owner for the forecasting and scheduling of resources to the work that these resources are assigned to taking into account their availability.

*Workfront* has several sets of tools used to manage resources. Although some of these tools overlap, each one has an individual scope. Currently, you can use the following Resource Management tools in *Workfront*, depending on which stage of resource management you are in:

* To plan how resources are allocated at a higher level, before the actual work on projects begins, use the following tool

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  s
  </MadCap:conditionalText>
  -->

  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> s</MadCap:conditionalText>`:

  * `The *Resource Planner*`: You can use the *Resource Planner* in the first stage of resource management to budget project time for your resources according to their scheduled availability. During the planning of resources phase, you can organize users in&nbsp;resource pools and assign multiple resource pools to a project. * 
    *For more information about Resource Planning, see the section [Resource Planning in Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md).

    <!--  
    <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p><span><b>The <em>Scenario Planner</em></b>: This is a higher-level planning of resources that allows you to manage them across multiple initiatives and to use the best scenario for making the most out of their availability and your budget.</span> </p> <p><span>T</span><span>his is available only in <em>the new Adobe Workfront experience</em> and requires an additional license. For information about the <em>Workfront Scenario Planner</em>, see</span><a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref" xrefformat="{para}">The Adobe Workfront Scenario Planner overview</a>. </p> </li>  
    -->  
  
  * `**The *Scenario Planner***: This is a higher-level planning of resources that allows you to manage them across multiple initiatives and to use the best scenario for making the most out of their availability and your budget.`

    `T` `his is available only in *the new Adobe Workfront experience* and requires an additional license. For information about the *Workfront Scenario Planner*, see` [The Adobe Workfront Scenario Planner overview](../../scenario-planner/scenario-planner-overview.md).

<ul> 
 <li> <p>To schedule or assign resources to actual work (tasks and issues), use the following tools: </p> 
  <ul> 
   <li><span class="bold">The Workload Balancer</span> (recommended): This is a lower-level stage of resource management, where you can assign your resources to the actual work (tasks and issues) that they must complete, based on the amount of hours needed to complete them and their availability. Using the <em>Workload Balancer</em> you can assign to users actual work that is currently unassigned or assigned to job roles.<p>For information about the Workfront Balancer, see the section <a href="../../resource-mgmt/workload-balancer/workload-balancer.md" class="MCXref xref" xrefformat="{para}">The Workload Balancer </a>. </p></li> 
   <li> <p><span class="bold">Scheduling</span> (deprecated): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This is a lower-level view of resource management, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.<br>For more information about resource scheduling, see the section <a href="../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md" class="MCXref xref" xrefformat="{para}">Resource Scheduling</a>. </p> <note type="note"> 
     <p>We are no longer developing the Resource Scheduling tools and they will soon be removed from <em>Adobe Workfront</em>. We recommend that you use the <em>Workload Balancer</em> for scheduling your resources. </p> 
     <p>For information about scheduling resources using the new <em>Workload Balancer</em>, see the section <a href="../../resource-mgmt/workload-balancer/workload-balancer.md" class="MCXref xref" xrefformat="{para}">The Workload Balancer </a>.</p> 
     <p>For more information about the timeline for removing the Resource Scheduling tools and replacing them with the <em>Workload Balancer</em>, see <a href="../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md" class="MCXref xref" xrefformat="{para}">Deprecation of Resource Scheduling tools in Adobe Workfront</a>.</p> 
    </note> </li> 
  </ul> </li> 
</ul>

* To analyze budgeted, planned, and actual allocations across multiple projects, use the following tool:

  * `Utilization Report`: Use this report to view the utilization of resources for projects. You can compare budgeted, planned, and actual allocations for your projects and their impact on the cost and revenue of the projects. For information about the Utilization&nbsp;Report, see [View resource utilization information](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## The components of the Resource Management process

>[!NOTE]
>
>Resource Management is never a stagnant process in *Workfront*. As the schedules of your projects, the availability of your users, or their roles change, you must continually adjust the information about your resources, their assignments, and their allocations to projects, tasks, and issues.

The process of managing resources in&nbsp;*Workfront* includes the following stages:

<ul> 
 <li><span class="bold">Configuration</span>: As a resource manager or Project Owner, you or your <em>Workfront administrator</em> must configure certain fields and objects in your <em>Workfront</em> instance before managing your resources. For more information about the prerequisites necessary to start managing resources in <em>Workfront</em>, see the <a href="#prerequisites" class="MCXref xref" xrefformat="{para}"> Prerequisites for accurate resource management </a> section in this article. <br>In addition to having projects with work items, you must configure the following items in <em>Workfront</em>:<br>
  <ul>
   <li>Users<br>For more information about creating users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref" xrefformat="{para}">Add users</a>.</li>
   <li>Job Roles<br>For more information about creating job roles, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
   <li>Schedules<br>For more information about creating schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
   <li><p>Project Preferences</p><note type="tip">
      Only a system administrator can modify Project Preferences.
    </note><p>For more information about defining Project Preferences, see the article <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref" xrefformat="{para}">Configure system-wide project preferences</a>.</p></li>
   <li>Resource Pools<br>For more information about creating resource pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref" xrefformat="{para}">Create resource pools in Adobe Workfront</a>.</li>
  </ul></li> 
 <li> <p><span class="bold">Resource allocation</span>: As a resource manager, or a Project Owner, you can define allocation of resources for your projects as well as assign work. For this step, you can manage the allocation of your resources at the project level using the <em>Resource Planner</em>. Then, you can assign work items (tasks and issues) to users based on their job roles using the resource scheduling tools. </p> <p>For more information about resource planning, see the following sections:</p> </li> 
 <ul style="list-style-type: circle;"> 
  <li> <a href="../../resource-mgmt/resource-planning/resource-planning-overview.md" class="MCXref xref" xrefformat="{para}">Resource Planning in Adobe Workfront</a></li> <draft-comment>
   <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p><a href="../../scenario-planner/scenario-planning.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner</a> </p> </li>
  </draft-comment>
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p><a href="../../scenario-planner/scenario-planning.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner</a> </p> </li> 
 </ul> 
 <p>For more information about resource scheduling, see the section <a href="../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md" class="MCXref xref" xrefformat="{para}">Resource Scheduling</a>.</p> 
 <li><span class="bold">Analysis</span>: As a resource manager, Project Owner, or people manager, review the Utilization&nbsp;Report to understand how the budgeted and planned allocations of your resources compare to the actual ones. Review information by hours, cost, or revenue. For information about the Utilization report, see <a href="../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref" xrefformat="{para}">View resource utilization information </a>. </li> 
</ul>

## Access needed to view and manage resources using the Resource Management tools in *Workfront*

The following users have access to the Resource Management tools in *Workfront*:

You must be one of the following users and have the following access and permissions to access Resource Planning and Scheduling tools:

<ul> 
 <li> <p>The system administrator.</p> </li> 
 <li> <p>A user with a Plan license </p> <p>In&nbsp;addition to having a <em>Plan</em> license, you must have the following to use specific resource management tools:</p> 
  <ul> 
   <li> <p>Edit access to Resource Management to use the Scheduling tool</p> </li> 
   <li>Edit access to Financial Data to display Cost information in the Planner</li> 
   <li>View access to&nbsp;Financial&nbsp;Data to view Cost and&nbsp;Revenue information in the Utilization Report</li> 
  </ul> </li> 
 <li>Manage permissions on the projects you want to manage resources for.</li> 
 <li> <p>Designated as a Resource Manager for projects to use the Scheduling tool. </p> <note type="tip">
   This is not required for using the 
   <em>Resource Planner</em> and&nbsp;the 
   <em>Workload Balancer</em>. 
  </note> </li> 
</ul>

For information about the access needed to budget resources, see the article [Access needed to budget resources](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

For information about the access needed to manage resources in the *Workload Balancer*, see [Access needed to manage resources in the Workload Balancer](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

##  Prerequisites for accurate resource management

You must meet a set of requirements before you can efficiently use the resource management tools in *Workfront*.

For information about what the requirements are for each resource management tool in&nbsp;*Workfront* see the following:

* The section "Prerequisites for working in the *Resource Planner*" in the article [Resource Planner overview](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).
* The section "Best practices for using the *Workload Balancer*" in the article [Overview of the Workload Balancer](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

* [Access needed to budget resources](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [Access needed to manage resources in the Workload Balancer](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in
<em>Workfront</em>, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to <em>Workfront</em>, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates in Adobe Workfront</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->

We recommend that the following settings exist before starting to manage resources for your organization:

<ul> 
 <li> You must have users in the system who have active accounts. </li> 
 <li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
    Although you can assign work to a Reviewer or a Requestor, they cannot complete it. 
   <br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in 
   <em>Workfront</em>, see 
   <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>. 
  </note></li> 
 <li> You must have job roles configured in the system.<br>For information about adding job roles to <em>Workfront</em>, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li> 
 <li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li> 
 <li> You must associate at least one job role with your users. </li> 
 <li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li> 
 <li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li> 
 <li>The Time Off calendar of the users must be up to date. </li> 
 <li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p> 
  <ul> 
   <li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates in Adobe Workfront</a>.</p> </li> 
  </ul> </li> 
 <li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources</a>.</p> </li> 
 <li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li> 
 <li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li> 
</ul>

