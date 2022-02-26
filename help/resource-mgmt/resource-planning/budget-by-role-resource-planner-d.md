---
filename: budget-by-role-resource-planner-d
product-area: resource-management
navigation-topic: resource-planning
title: Budget resources by role in the Resource Planner
description: As a Resource Manager, you can budget your resources by Job Roles, to determine how much time should be allocated to each role. You can do this in the Role View of the Resource Planner.
---

# Budget resources by role in the Resource Planner

As a Resource Manager, you can budget your resources by Job Roles, to determine how much time should be allocated to each role. You can do this in the Role View of the Resource Planner.&nbsp;

* Prerequisites for Using the Role View in the Resource Planner
* Understanding Budgeting in the Role View of the Resource Planner
* Budgeting Resources in the Role View of the Resource Planner

## Prerequisites for Using the Role View in the Resource Planner

`**^`

You must be a Resource Manager to populate the Role View of the Resource Planner.&nbsp;

To successfully use the Resource Planner, you must first ensure that your users, projects, tasks, and issues meet&nbsp;a set of prerequisites. These prerequisites are mandatory to display the correct information in the Resource Planner.

For&nbsp;more information about the prerequisites that must be met before you can start using the Resource Planner, see the [Get started with Resource Planning](../../resource-mgmt/resource-planning/get-started-resource-planning.md) [Get started with Resource Planning](../../resource-mgmt/resource-planning/get-started-resource-planning.md) section in [Get started with Resource Planning](../../resource-mgmt/resource-planning/get-started-resource-planning.md).&nbsp;

## Understanding Budgeting in the Role View of the Resource Planner

We recommend that you budget your resources in the Role View, when you are mostly concerned with how a bulk number of hours, FTE, or amount of Cost is distributed amongst all your Job Roles in the system.&nbsp;

Consider the following when selecting the Role view in the Resource Planner:&nbsp;

<ul> 
 <li>You can see roles that are associated with projects for which you are designated as the Resource Manager in the Role view of the Resource Planner.</li> 
 <li>You can expand each role to display a list of projects, and every project to display a list of users that can fulfill those roles on the projects.&nbsp;</li> 
 <li> The number of items you display or can export from the Role view is limited, to improve performance.<br>For more information about limitations when viewing the Resource Planner in the Role view, see the "Role View" section in <a href="../../resource-mgmt/resource-planning/resource-planner-display-limitations.md" class="MCXref xref">Resource Planner display limitations</a>. </li> 
 <li> The projects are listed under the job role in the same order of priority as they are listed in the Project view.&nbsp; </li> 
 <li> When this view is applied, the Project&nbsp;Hours, FTE or Cost add up to the Role&nbsp;Hours, FTE or Cost.<br><img src="assets/resource-planner-view-by-role-350x222.png" alt="resource_planner_view_by_role.png" style="width: 350;height: 222;"></li> 
</ul>

## Budgeting Resources in the Role View of the Resource Planner

<ol> 
 <li value="1"> Go to the&nbsp;<span class="bold">People</span>&nbsp;area in the Global Navigation Bar. </li> 
 <li value="2"> Select the&nbsp;<span class="bold">Planning</span>&nbsp;tab. </li> 
 <li value="3"> Select the&nbsp;<span class="bold">Resource Planner</span>&nbsp;sub-tab. </li> 
 <li value="4"> (Conditional) Select the <span class="bold">View by Role</span>&nbsp;view.&nbsp; </li> 
 <li value="5"> Expand the job roles and the projects to manage the allocation for the project, job roles, or users. </li> 
 <li value="6"> To budget allocation for users, do one of the following: &nbsp; 
  <ul>
   <li> In the <span class="bold">BDG</span> column, manually specify a number of budgeted hours, FTE, or cost for the users. </li>
   <li>Click the&nbsp;<span class="bold">Options</span> icon for the project, then click <span class="bold">Set Users' Planned Hours as Budgeted</span>.<br>The Budgeted Hours of each user are calculated using the following formula:<br><em>User Budgeted Hours = User Planned Hours</em></li>
  </ul></li> 
 <li value="7">To budget allocation for job roles, do one of the following:<br>
  <ul>
   <li>In the <span class="bold">BDG</span> column, manually specify a number of budgeted hours, FTE, or cost for the job roles.<br><note type="tip">
      This adds the Role Budgeted Hours to the Project Budgeted Hours.
    </note></li>
   <li>Click the <span class="bold">Options</span> icon for the job role, then click <span class="bold">Set Projects' Planned Hours as Budgeted.<br></span>The Role Budgeted Hours are calculated using the following formula:<br><em>Role Budgeted Hours = SUM(Project Budgeted Hours)<br></em>The Project Budgeted Hours are calculated using the following formula:<br><em>Project Budgeted Hours = Project Planned Hours</em></li>
   <li>In the <span class="bold">BDG</span> column, manually specify a number of budgeted hours, FTE, or cost for the projects listed under the job role.<br>This adds the number of Project Budgeted Hours to the role.&nbsp;<em><br></em><note type="tip">
      Users can be budgeted for both Primary and Other (or secondary) Roles. The 
     <span class="bold">Percentage of FTE Availability</span> for the&nbsp;roles of the user must be a number different than 0% for&nbsp;the Available Hours to display a value in the Resource Planner for a job role. If a user is associated with a role with a 0% 
     <span class="bold">Percentage of FTE Availability</span>, the Available Hours value is zero for that job role. In this case, the role might show a negative 
     <span class="bold">Net Value</span>.
    </note><em><br>For more information about&nbsp;the <span class="bold">Percentage of FTE Availability</span> for job roles, see <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</em><em><br></em></li>
  </ul></li> 
 <li value="8">To budget allocation for the project, do one of the following: 
  <ul>
   <li>In the <span class="bold">BDG</span> column, manually specify a number of budgeted hours, FTE, or cost for the projects.<br>This also updates the Budgeted Hours for the roles under which the project is listed.&nbsp;</li>
   <li>Click the <span class="bold">Options</span> icon for the job role, then click <span class="bold">Set Projects' Planned Hours as Budgeted</span>.<br>The Project Budgeted Hours are calculated by the following formula:<br><em>Project Budgeted Hours = Project Planned Hours</em><br>The Project Budgeted Hours are added to the Role Budgeted Hours.&nbsp;</li>
   <li>(Conditional) If you have budgeted the hours for the users, click the <span class="bold">Options</span> icon for the project, then click <span class="bold">Total Users' Budgeted Hours for Project</span>.<br>The Project Budgeted Hours is calculated using the following formula:<br><em>Project Budgeted Hours = SUM(User Budgeted Hours)</em><br><img src="assets/budget-by-role-350x181.png" alt="budget_by_role.png" style="width: 350;height: 181;"></li>
  </ul></li> 
 <li value="9">Click <span class="bold">Save</span>.<br>After you budget your resources in the Resource Planner, the Budgeted Hours for your resources and any cost associated with them are listed in the Business Case of every project.<br>For more information about understanding the Resource Budgeting area of the Business Case, see the "Resource Budgeting" section in&nbsp;<a href="../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Create a Business Case for a project in Adobe Workfront</a>.</li> 
 <li value="10"> (Optional) Select the <span class="bold">View by User</span> view to notice any user overallocations or underutilization between the Available and the Planned Hours for each user. Budgeted Hours are not visible in the View by User view.&nbsp; </li> 
</ol>

`**^ This section repeats between the Role, Project view articles and the main Planning in the Res Planner article.`
