---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Resource Planner overview
description: You can estimate and budget the allocation of your resources to the projects they are assigned to and forecast their availability for future work using the Resource Planner.
author: Alina
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
---
# Resource Planner overview

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

You can estimate and budget the allocation of your resources to the projects they are assigned to and forecast their availability for future work using the Resource Planner.

For a general overview of resource planning in Adobe Workfront, see the article [Get started with Resource Planning](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Resource Planner overview

You can use the Resource Planner to easily understand the availability of users and job roles, as well as the planned time necessary to complete work on projects. You can then decide how to allocate your users and their job roles on the projects they are assigned to based on their available time.

>[!IMPORTANT]
>
>You cannot use the Resource Planner to assign actual work (tasks and issues) to users. You can only estimate the amount of time needed for the users or job roles to complete a project, regardless of the tasks and issues they are assigned to.  
>To assign actual work to users you must use the Workload Balancer. For more information about the Workload Balancer, see [Workload Balancer overview](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

You can view information in the Resource Planner using three separate views. You can use each view to fulfill one of the following purposes:

* To budget the time or cost of your resources for the work that needs to be accomplished using the Project and Role views. This is the main purpose of the Resource Planner.   
  For more information about budgeting in the Resource Planner, see the article [Budget resources in the Resource Planner using the Project and Role views](../resource-planning/budget-resources-project-role-views-resource-planner.md).

* To view the following information using the User view:

   * The availability of your users according to their schedule
   * The planned amount of time needed to complete the work according to the project plan 
   * The amount of time that users have already logged on actual work items

  For more information about viewing Available, Planned, and Actual Hours or FTE for users in the Resource Planner, see the article [View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using).

## Resource Planner considerations

* You can prioritize the projects you are working on, and budget your resource allocation according to their priority, to ensure that you have resources allocated to the most important projects first.

  For information about prioritizing projects in the Resource Planner, see [Prioritize projects in the Resource Planner](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md). 

* You can display hours, FTE, and cost information from the tasks and issues of projects.

  >[!NOTE]
  >
  >Tasks and issues do not display in the Resource Planner. However, the hours, FTE, and cost information from the resource allocations on the tasks displays in the Resource Planner as a total number for the project.

* The hour, FTE, and cost information from parent tasks is excluded from the projects that display in the Resource Planner. We recommend assigning resources only to children tasks if you want to manage those resources' time or cost in the Resource Planner.

  For information about parent tasks, see the following articles:

   * [Tasks overview](../../manage-work/tasks/task-information/tasks-overview.md) 
   * [Create subtasks](../../manage-work/tasks/create-tasks/create-subtasks.md)

  >[!TIP]
  >
  >Parent tasks display a total of the hours and costs of the children tasks. Because of this, counting hours, FTE, and cost from the children tasks and the parent tasks would count these amounts twice. This is why the parent task information is excluded from the Resource Planner.

* You cannot manage the allocation of teams on the projects on which they have tasks or issues in the Resource Planner. 
* You can budget resources for multiple projects at a time using the Resource Planner, or for a single project using the Resource Budgeting area of the Business Case. The information you budget for one project also displays in the Resource Planner.

  For information about how you can budget resources for a single project, see the article [Budget resources in the Business Case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

  For information about how you can budget resources in the Resource Planner for multiple projects at a time, see the section "Budget resources in the Resource Planner" in the article [Budget resources in the Resource Planner using the Project and Role views](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

## Prerequisites for working in the Resource Planner {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

To successfully use the Resource Planner for budgeting your resources, you must first ensure that you, your projects, and your tasks meet a set of prerequisites. These prerequisites are mandatory to display the correct information in the Resource Planner and to accurately manage your resources.

>[!IMPORTANT]
>
>If any of the following prerequisites are missing, you might find that some of the information about the allocation or the availability of the resources is missing or has a zero value.   
>For more information understanding why fields are missing data or have zero values, hover over the fields.

![](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>The following prerequisites are required only when viewing the Resource Planner by project or by job role or when budgeting resources in the Business Case of a project.

The following types of prerequisites are required for the correct functionality of the Resource Planner when viewing it by project or by role:

* [User prerequisites](#user-prerequisites) 
* [Project prerequisites](#project-prerequisites) 
* [Tasks and issues prerequisites](#tasks-and-issues-prerequisites) 
* [System-level prerequisites](#system-level-prerequisites)

### User prerequisites {#user-prerequisites}

Ensure the following user setup exists before starting using the Resource Planner:

* You have the correct access to budget resources.

  For information about the access needed to budget resources, see the article [Access needed to budget resources in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Users who are assigned to tasks are added to the resource pools associated with the project.

  For information about adding users to resource pools, see [Associate resource pools with users](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

  >[!NOTE]
  >
  >When users are not added to resource pools, the following scenarios may exist: 
  >
  >   
  >   
  >   * The users do not appear in the Resource Planner although they might be assigned to tasks on the projects. 
  >   * If the tasks they are associated with have Planned Hours, those hours do not appear for the project in the Resource Planner, unless the user is also associated with a job role on those tasks. 
  >   * If the users are associated with a job role on a task on the project, the Planned Hours display in the Resource Planner for the job role, but the job role cannot be budgeted. 
  >   
  >

* Users who are assigned to work and resource pools must have Schedules and Job Roles associated with their profile.

  For information about associating Schedules and Job Roles with users, see [Edit a user's profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Users who are not associated with a Schedule but are in the resource pool of the project cannot be budgeted in the Resource Planner.

* For accurate Available Hours information, ensure that the schedules associated with your users have the schedule exceptions and time off updated.

  >[!NOTE]
  >
  >If a user is not associated with a Schedule, the Default Schedule of your Workfront system is associated with the user by default, for the purposes of the Resource Planner.

  For information about creating schedules, see the article [Create a schedule](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* If you want to budget your resources by Cost, you must associate Job Roles with Cost/Hr. rates. The cost associated with Job Roles assigned to users in your resource pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.  
  For information about associating job roles with rates, see the article [Create and manage job roles](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).  
  For information about calculating Budgeted Labor Cost, see the article [Understand Budgeted Labor Cost and Budgeted Hours for projects](../../manage-work/projects/project-finances/budgeted-labor-cost.md).  
  For information about calculating Budgeted Cost, see the article [Calculate Budgeted Cost](../../manage-work/projects/project-finances/budgeted-cost.md).

### Project prerequisites {#project-prerequisites}

Ensure the following project setup exists before starting using the Resource Planner:

* Your projects are associated with resource pools.  
  For more information about adding resource pools to projects, see [Associate resource pools with projects and templates](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md).

  >[!IMPORTANT]
  >
  >Projects without resource pools do not display Planned Hour or assignments information in the Resource Planner.

### Tasks and issues prerequisites {#tasks-and-issues-prerequisites}

Although you cannot display tasks and issues in the Resource Planner, their information transfers to the projects that display in the Resource Planner .

Ensure the following task and issue setup exists before starting budgeting resources in the Resource Planner:

* The tasks or issues on the projects for which you are budgeting resources are assigned to one of these entities:

   * Users in the resource pools of the project who are also associated with Job Roles
   * Job Roles

  >[!NOTE]
  >
  >The Planned Hours of tasks and issues assigned to job roles display in the Resource Planner, but these hours cannot be budgeted unless a user who is associated with the job role is listed in a resource pool associated with the project.

* You should not assign parent tasks to users or roles.

  To display hour information in the Resource Planner for users or roles associated with parent tasks you must also assign them to the children tasks. The Resource Planner does not display information from parent tasks. 

* Tasks and issues have a value for Planned Hours which is greater than zero. 
* Tasks and issues have a value for their Duration which is greater than zero. 
* The Planned Dates of the issues are within the timeline of the project.

### System-level prerequisites {#system-level-prerequisites}

You must understand how your instance of Workfront calculates user availability according to the Resource Management Preferences in your system. Workfront can calculate user availability using the user's schedule as defined in their User Profile page, or the Default Schedule of your system.

![](assets/resource-management-preferences-section-in-setup-350x89.png)

Your Workfront administrator configures your Resource Management Preferences.

For more information, see [Configure Resource Management preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Locate the Resource Planner

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

You can locate the Resource Planner in two areas of Workfront, depending on whether you want to budget your resources for multiple projects, or for just one project.

For information about locating the Resource Planner, see [Locate the Resource Planner](../../resource-mgmt/resource-planning/locate-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(this is drafted and moved to its own article: locate-resource-planner) </p>
<p>Ensure that all prerequisites are met before starting to use the Resource Planner. This way, you ensure that the Resource Planner displays the correct information before you start budgeting your resources.<br>For information about the prerequisites that must be met before you can start using the Resource Planner, see the <a href="#prerequisites-for-working-in-the-resource-planner" class="MCXref xref">Prerequisites for working in the Resource Planner</a> section in this article. </p>
<p>You can locate the Resource Planner in two areas of Workfront, depending on whether you want to budget your resources for multiple projects, or for just one project.</p>
<ul>
<li><a href="#use-the-resource-planner-for-multiple-projects" class="MCXref xref">Use the Resource Planner for multiple projects</a> </li>
<li> <p><a href="#use-the-resource-planner-for-one-project" class="MCXref xref">Use the Resource Planner for one project</a> </p> </li>
</ul>
<p><strong>Use the Resource Planner for multiple projects</strong></p>
<p>When using the Resource Planner for multiple projects, the allocation numbers for your resources represent numbers across multiple projects. </p>
<p>To access the  Planner section  in the  Resourcing area: </p>
<ol>
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.  </li>
<li value="2"> <p>  Click <strong>Resourcing</strong>. The Resource Planner displays by default.  For information about budgeting resources in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> <p> <img src="assets/qs-resource-management-area-with-planner-as-default-350x152.png" style="width: 350;height: 152;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">  Hover over the left panel, and click <strong>Resource Pools</strong>. <br>For information about creating new resource pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a>.</li>
</ol>
<p><strong>Use the Resource Planner for one project</strong></p>
<p>When using the Resource Planner for one project, the allocation numbers for your resources represent numbers for the selected project. </p>
<ol>
<li value="1"> <p>Go to a project you want to budget resources for.</p> </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Business Case</strong> in the left panel.</p> </li>
<li value="3"> <p>Scroll to the <strong>Resource Budgeting</strong> section of the Business Case.</p> </li>
<li value="4"> <p>Click <strong>Edit Resource Budgeting</strong> to add resource pools to your project and start budgeting your resources. </p> <note type="tip">
You can only add a resource pool in the Resource Budgeting area of the Business Case when the project has no resource pools associated with it. When the project already has a resource pool, the users in the pool and their job roles display in the Resource Budgeting area by default.
</note> <p> <img src="assets/resource-budgeting-area-on-project-350x70.png" style="width: 350;height: 70;"> </p> <p>For information about budgeting resources for one project, see the article <a href="../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md" class="MCXref xref">Budget resources in the Business Case</a>.</p> </li>
</ol>
</div>
-->

## The areas of the Resource Planner

You can view the following information or perform the following actions in the Resource Planner:

* Information about the resources assigned to your projects in the Resource Planner in a general timeline. 
* Overallocation or underutilization of your resources in the Resource Planner. 
* Budget your resources for work manually, or automatically.

For more information about what areas display in the Resource Planner and how to configure what information displays in these areas, see the article [Resource Planner navigation overview](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Limitations in displaying information in the Resource Planner

To improve performance, Workfront limits the amount of items you can display in the Resource Planner.

For more information about these limitations, see the article [Resource Planner display limitations](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) .

## Calculate FTE in the Resource Planner

You can display availability, allocation, and planned values in the Resource Planner in Hours, FTE, or Cost.

For more information about changing the information you display in the Resource Planner, see the section [View information by Hour, FTE, or Cost](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) in the article [Review resource availability and allocation using the Adobe Workfront Resource Planner](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

For more information about how the Hours and FTE for users and roles are calculated in Workfront, see the article [Overview of calculating hours and FTE for users and roles in the Resource Planner](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Calculate Costs in the Resource Planner

You must have View access to Financial Data and View Finance permissions on the projects to see the information by Cost in the Resource Planner.

Along with displaying availability, allocation, and planned values in the Resource Planner in Hours and FTE, you can also display them by Cost.

>[!TIP]
>
>You must associate your users and your job roles with Cost per Hour rates in order to display information by Costs in the Resource Planner.

For more information about associating Cost per Hour rates with job roles, see the article [Create and manage job roles](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).  
For more information about associating Cost per Hour rates with users, see the article [Edit a user's profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Consider the following when viewing information by Cost in the Resource Planner:

* The Cost of each type of hours (Planned, Available, Budgeted, Actual for Users, Roles, or the Projects) is calculated using a different Cost Rate.
* The Planned Cost is affected by the Cost Type of the tasks on the projects.
* When applying the User View to the Resource Planner, you cannot display the allocation and availability information by Cost.

For more information about how Costs are calculated in the Resource Planner for users and roles, see the article [Calculate costs in the Resource Planner](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the User View to view Available, Planned, and Actual Hours or FTE </h2>
<p>(this information is repeated from above where it exists in shorter form. Drafted to simplify the amount of info of this article.) </p>
<p>You can use the User View of the Resource Planner to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources. </p>
<p>For information about using the Resource Planner to review the Available, Planned, and Actual Hours and FTE for resources, see the article <a href="../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md" class="MCXref xref">View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view</a>.</p>
<p><strong>Use the Project and Role Views to budget resources </strong></p>
<p> The main function of the Resource Planner is to budget your resources for the work that needs to be completed on the projects that you can manage. </p>
<p> You can budget your resources only if you apply the <strong>View by Project</strong> or <strong>View by Role</strong> views to the Resource Planner.</p>
<p>For information about budgeting resources using the Project and Role views in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md"><a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a></a>.</p>
</div>
-->

## Filter information in the Resource Planner

You can reduce the number of projects, roles, or users that display in the Resource Planner by creating a filter.   
For more information, see the article [Filter information in the Resource Planner](../../resource-mgmt/resource-planning/filter-resource-planner.md).
