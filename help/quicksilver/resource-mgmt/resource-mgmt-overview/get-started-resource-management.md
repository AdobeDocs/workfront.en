---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: Get started with Resource Management
description: Resource Management allows you to configure your system to accurately forecast the use of your resources based on their availability so that the work that must be done is completed on time and on budget.
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
---
# Get started with Resource Management

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

Resource Management allows you to configure your system to accurately forecast the use of your resources based on their availability so that the work that must be done is completed on time and on budget.

## Overview of Resource Management in Adobe Workfront

Resource Management refers to all the activities performed by the Adobe Workfront administrator, the resource manager, and the Project Owner to plan (Resource or Scenario Planning) and schedule (Workload Balancer) an organization's resources and assign them to the work that needs to be done, taking into account their availability. Additionally, resource management also refers to viewing information about the planned and actual resource allocations in a report view (Utilization report). 

Workfront has several sets of tools used to manage resources. Each tool has an individual scope. Currently, you can use the following Resource Management tools in Workfront, depending on which stage of resource management you are in:

* To plan how resources are allocated at a higher level, before the actual work on projects begins, use the following tools:

   * **The Resource Planner**: You can use the Resource Planner in the first stage of resource management to budget project time for your resources according to their scheduled availability. During the planning of resources phase, you can organize users in resource pools and assign multiple resource pools to a project.
   
      For more information about Resource Planning, see [Resource Planning in Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **The Scenario Planner**: This is a higher-level planning of resources that allows you to manage them across multiple initiatives that can span over a one, three, or five year plan and include multiple projects. You can use the best scenario for making the most out of their availability and your budget.

     The Scenario Planner requires a separate license, in addition to the Workfront license. For information about the Workfront Scenario Planner, see [The Scenario Planner overview](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* To schedule or assign resources to actual work (tasks and issues), use the following tool:

  * **The Workload Balancer**: This belongs to a lower-level stage of resource management, where you can assign your resources to the actual work (tasks and issues) that they must complete, based on the amount of hours needed to complete them and their availability. Using the Workload Balancer you can assign users to actual work that is currently unassigned or assigned to job roles.

     For information about the Workfront Balancer, see [The Workload Balancer: article index](../../resource-mgmt/workload-balancer/workload-balancer.md). 
  
<!--

  * **Scheduling** (deprecated <span class="preview">and removed from the Preview environment</span>): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This happens at a lower-level in the process of managing resources, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  

     For more information about resource scheduling, see the section [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

    >[!CAUTION]
    >
    >
    >We are no longer supporting the Resource Scheduling tools and they will be removed from Workfront in **January 2023**. We recommend that you use the Workload Balancer for scheduling your resources. 
    >
    >
    >* For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
    >
    >
    >* For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

--> 
* To analyze budgeted, planned, and actual allocations across multiple projects, use the following tool:

   * **Utilization Report**: Use this report to view the utilization of resources for projects. You can compare budgeted, planned, and actual allocations for your projects and their impact on the cost and revenue of the projects. 
   
      For information about the Utilization Report, see [View resource utilization information](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## The components of the Resource Management process

>[!NOTE]
>
>Resource Management is never a stagnant process in Workfront. As the schedules of your projects, the availability of your users, or their roles change, you must continually adjust the information about your resources, their assignments, and their allocations to projects, tasks, and issues.

The process of managing resources in Workfront includes the following stages:

* **Configuration**: As a system administrator, resource manager, or Project Owner you must configure certain fields and objects in your Workfront instance before managing your resources. For more information about the prerequisites necessary to start managing resources in Workfront, see the [Prerequisites for accurate resource management](#prerequisites-for-accurate-resource-management) section in this article.   
  In addition to having projects with work items, you must configure the following items in Workfront:

   * Users  
     For more information about creating users, see the article [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
   
   * Job Roles  
     For more information about creating job roles, see the article [Create and manage job roles](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
   
   * Schedules  
     For more information about creating schedules, see the article [Create a schedule](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
   
   * Project Preferences

     >[!TIP]
     >
     >Only a system or group administrator can modify Project Preferences for your system or for your group.

     For more information about defining Project Preferences, see the article [Configure system-wide project preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
   
   * Resource Pools  
     
     For more information about creating resource pools, see [Create resource pools](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).
   
   * Resource Management preferences

     As a system, you must decide how Workfront calculates user availability at the system level, whether using the user's schedule or the Default Schedule of your system.

     For more information, see [Configure Resource Management preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Resource allocation**: As a resource manager, or a Project Owner, you can define allocation of resources for your projects as well as assign work. For this step, you can manage the estimate the allocation of your resources using the Resource Planner or the Scenario Planner, and assign actual work to users in the Workload Balancer. 

  For more information about resource planning and assigning work, see the following sections:

   * [Resource Planning in Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Adobe Workfront Scenario Planner](../../scenario-planner/scenario-planning.md)
   * [The Workload Balancer: article index](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Overview of the Workload Balancer](../workload-balancer/overview-workload-balancer.md). 
-->

* **Analysis**: As a resource manager, Project Owner, or people manager, review the Utilization Report to understand how the budgeted and planned allocations of your resources compare to the actual ones. Review information by hours, cost, or revenue. For information about the Utilization report, see [View resource utilization information](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Access needed to view and manage resources using the Resource Management tools in Workfront

The following users have access to the Resource Management tools in Workfront:

You must be one of the following users and have the following access and permissions to access resource management tools:

* The system administrator.
* A user with a Plan license.  
  
  A user with a Work license can use the Workload Balancer of a project and manage assignments and allocations.

  In addition to having a Work or higher license, you must have the following to use specific resource management tools:

   * Edit access to Resource Management (not needed for making assignments in the Workload Balancer)
   * Edit access to Financial Data to display Cost information in the Resource Planner
   * View access to Financial Data to view Cost and Revenue information in the Utilization Report (only users with a Plan license)

* Contribute or higher permissions that includes Make Assignments on the projects you want to manage resources for.  

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

For information about the access needed to budget resources, see the article [Access needed to budget resources](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

For information about the access needed to manage resources in the Workload Balancer, see [Access needed to manage resources in the Workload Balancer](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## Prerequisites for accurate resource management  {#prerequisites-for-accurate-resource-management}

You must meet a set of requirements before you can efficiently use the resource management tools in Workfront.

For information about what the requirements are for each resource management tool in Workfront see the following:

* The section [Prerequisites for working in the Resource Planner](../../resource-mgmt/resource-planning/get-started-resource-planner.md#prerequisites-for-working-in-the-resource-planner) in the article [Resource Planner overview](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
<!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* The section [Best practices for using the Workload Balancer](../../resource-mgmt/workload-balancer/overview-workload-balancer.md#best-practices-for-using-the-workload-balancer) in the article [Overview of the Workload Balancer](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [Access needed to budget resources in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [Access needed to manage resources in the Workload Balancer](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and replaced with the links to each prerequisites instead) </p>
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in Workfront, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to Workfront, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->
