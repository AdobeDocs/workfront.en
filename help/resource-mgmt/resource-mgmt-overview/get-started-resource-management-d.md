---
filename: get-started-resource-management-d
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: Get started with Resource Management
description: This replaces this: Get started with Resource Management
---

# Get started with Resource Management

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> This replaces this:&nbsp;<a href="../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md" class="MCXref xref" xrefformat="{para}">Get started with Resource Management </a>&nbsp; </p>
-->

This replaces this:&nbsp; [Get started with Resource Management](../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)&nbsp;

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> - this has no reference to Legacy Res Management tools - replace when flash is removed.&nbsp; </p>
-->

- this has no reference to Legacy Res Management tools - replace when flash is removed.&nbsp;

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><span class="wysiwyg-color-pink">***</span> </p>
-->

`***`

Resource Management allows you to configure your system to accurately forecast the use of your resources based on their availability so that the work that must be done is completed on time and on budget.&nbsp;

## Overview of Resource Management in *Adobe Workfront*

Resource Management refers to all the activities performed by the system administrator, the Resource Manager, and the Project Owner&nbsp;for the forecasting and scheduling of resources in relation to the work that these resources are assigned to and their availability. &nbsp;

*Workfront* has several sets of tools used to manage resources. Although some of these tools overlap, each one has an individual scope.&nbsp;

To plan how resources are allocated on projects, use the following area:&nbsp;

* `Resource Planning`: Refers to organizing your users in Resource Pools which can be assigned to your projects. You can assign multiple Resource Pools to a project. The availability of users based on their schedules and allocations to tasks in projects is managed in the `Resource Planner`. This is a high-level view on resource management, allowing you to budget hours for your resources at the project level, according to their scheduled availability. &nbsp;* 
  *For more information about Resource Planning, see the [Resource Planning in Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md) section.&nbsp;

To schedule resources to actual work (tasks and issues), use the following area:&nbsp;

* `Resource Scheduling`: Refers to assigning actual work to users&nbsp;by matching the job roles assigned to the tasks and issues with the&nbsp;job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned.&nbsp;This is a lower-level view on resource management, allowing you to assign&nbsp;your resources to the actual work (tasks and issues) that they must complete, according to the hours needed in the project plan to fulfill them.  
  For more information about Resource Scheduling, see the [Scheduling Resources](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md)section.

## `Overview of the two components of Resource Management`

`Resource Management is done in two steps:`

<ul> 
 <li><span class="wysiwyg-color-pink"><span class="bold">Configuration</span>: As a Resource Manager or Project Owner, you or your <em>Workfront administrator</em> must configure certain fields and objects in your <em>Workfront</em> instance before managing your resources.&nbsp;</span> <br><span class="wysiwyg-color-pink">You must configure&nbsp;the following items in <em>Workfront</em>:</span> <br> 
  <ul> 
   <li><span class="wysiwyg-color-pink">Users</span> <br><span class="wysiwyg-color-pink">For more information about creating users, see <a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref" xrefformat="{para}">Add users</a>.</span> </li> 
   <li><span class="wysiwyg-color-pink">Job Roles</span> <br><span class="wysiwyg-color-pink">For more information about creating job roles, see <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</span> </li> 
   <li><span class="wysiwyg-color-pink">Schedules</span> <br><span class="wysiwyg-color-pink">For more information about creating schedules, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</span> </li> 
   <li><span class="wysiwyg-color-pink">Project Preferences</span> <br><span class="wysiwyg-color-pink">
     <note type="tip">
       Only a system administrator can modify Project Preferences.
      <br>
     </note>For more information about defining Project Preferences, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref" xrefformat="{para}">Configure system-wide project preferences</a>.</span> </li> 
   <li><span class="wysiwyg-color-pink">Resource Pools</span> <br><span class="wysiwyg-color-pink">For more information about creating Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref" xrefformat="{para}"> Resource pools overview in Adobe Workfront</a>.</span> </li> 
  </ul> </li> 
 <li><span class="wysiwyg-color-pink"><span class="bold">Resource Allocation</span>: As a Resource Manager, or a Project Owner, you can assign work and define allocation of resources to work tasks and issues. For this step, a Resource Manager manages the allocation of their resources at the project level using the Resource Planner. Then, they assign work items (tasks and issues) to users based on their job roles using the Resource Scheduling tools.&nbsp;</span> <br><span class="wysiwyg-color-pink">For more information about Resource Planning, see the <a href="../../resource-mgmt/resource-planning/resource-planning-overview.md">Resource Planning</a> section.</span> <br><span class="wysiwyg-color-pink">For more information about Resource Scheduling, see the <a href="../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md">Scheduling Resources</a> section.&nbsp;</span> </li> 
</ul>

`

>[!TIP]
>
>Resource Management is never a stagnant&nbsp;process&nbsp;in *Workfront*. As the schedules of your projects, the availability&nbsp;of your users, or their roles change, you must continually adjust the information about your resources, their assignments, and their allocations to projects, tasks, and issues. We recommend that you designate Resource Mangers for your projects. The role of the Resource Manager is to manage this process, to&nbsp;accurately allocate&nbsp;your resources and prioritize your projects.&nbsp;

`

## Access needed to use resource management tools

The following users have access to the Resource Management Tools in *Workfront*:

* The system administrator.
* A user with a Plan license who also has administrative access to Resource Pools.   
  For more information about granting administrative access to a Plan user, see [Grant users administrative access to certain areas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>You must be designated as a Resource Manager on at least one project to be able to plan and schedule your resources.&nbsp;

## Prerequisites for accurate resource management&nbsp;

All of the following conditions must be met before you can start managing your resources in *Workfront*:

<ul> 
 <li> You must have users in the system who have active accounts.<br>For more information about creating users, see <a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref" xrefformat="{para}">Add users</a>.</li> 
 <li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage.<br><note type="tip">
    Although you can assign work to a Reviewer or a Requestor, they cannot complete it. 
   <br>We recommend against assigning work to Reviewers or Requestors.
  </note></li> 
 <li> You must have job roles configured in the system.<br>For more information about adding job roles to <em>Workfront</em>, see <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li> 
 <li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li> 
 <li> You must associate at least one job role with your users.<br></li> 
 <li> You must specify a valid value for the FTE field of all users.<br>For more information about editing users to ensure they have a job role, FTE, or cost associated with them,&nbsp;see<a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>.</li> 
 <li>You must associate accurate Schedules with your users.<br>For more information about creating and editing schedules, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creating Schedules.</a></li> 
 <li>You must associate projects with Resource Managers and Resource Pools.<br>For more information about associating projects with Resource Managers, see <a href="../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Designate Resource Managers for a project or template </a>.For more information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref" xrefformat="{para}"> Resource pools overview in Adobe Workfront</a>.</li> 
 <li>You must assign the tasks and issues in your system to job roles (recommended) or users.</li> 
 <li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For more information about Planned Hours, see <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.<br>For more information about Duration, see <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li> 
 <li>You must be designated as a Resource Manager on projects to use the Resource Planner, and all Resource Scheduling tools.&nbsp;</li> 
 <li>When using the Legacy Resource Planning tools, your projects must include Resource Estimates in the Business Case.<br>For more information about using Resource Estimates in the Business Case, see <a href="apply-legacy-pools-to-business-case.md">Applying Resource Pools to the Business Case</a>.</li> 
</ul>

## Manage resources in *Workfront*

In addition to project planning, managing resources in *Workfront* is a key component of work planning.&nbsp;

After you have ensured that all the prerequisites for Resource Management are in place, you can continue with managing your resources. You can manage your resources by estimating how many hours, FTE, or how much Cost you need to fulfill the work that must be completed. Then, you can assign the work to individual users. Budgeting hours is identical to budgeting FTEs or Costs.&nbsp;

To manage your resources in *Workfront*:

1. Decide how your organization budgets resources.  
   You can budget by:

  * Spreading a bulk number of hours across all the job roles in the system.  
  * Spreading a bulk number of hours across all the projects in the system

1. (Conditional) If you want to budget a total number of hours or cost for all roles in the system, Go to the `People` area, then `Planning` and `Resource Planner` and select the `View by Role`.  
   For information about budgeting resources by role, see [Budget resources by role in the Resource Planner](../../resource-mgmt/resource-planning/budget-by-role-resource-planner-d.md).  
   Or  
   If you want to budget a total number of hours or cost for several projects in the system, Go to the `People` area, then `Planning` and `Resource Planner` and select the `View by Project`.  
   For information about budgeting resources by project, see [Budget resources by project in the Resource Planner](../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md).

1. (Optional) Go to the `Scheduling` tab and assign work to users.  
   For more information about assigning work to users in the Scheduling tab, see [Manually assign unassigned tasks and issues in the Scheduling areas](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><span class="wysiwyg-color-pink">***</span> </p>
-->

`***`

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><span class="wysiwyg-color-pink">As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.</span> </p>
-->

`As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.`

&nbsp;
