---
filename: budget-resources-project-role-views-resource-planner
product-area: resource-management
navigation-topic: resource-planning
title: Budget resources in the Resource Planner using the Project and Role views
description: The main function of the Resource Planner is to budget your resources for the work that must be completed on projects.
---

# Budget resources in the `Resource Planner` using the Project and Role views

The main function of the `Resource Planner` is to budget your resources for the work that must be completed on projects.

>[!IMPORTANT]
>
>You can budget your resources only if you apply the `View by Project` or `View by Role` views to the `Resource Planner`.

##  

Before starting to budget information in the `Resource Planner`, see the following articles:

* [Resource Planner overview](../../resource-mgmt/resource-planning/get-started-resource-planner.md) 
* [Access needed to budget resources](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md) 
* [Overview of hours, FTE, and cost information in the Project and Role views of the Resource Planner](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> and higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Resource Management that includes access to&nbsp;Edit priorities and budget hours in the <span>Resource Planner</span></p> <p>Edit access to Financial Data to budget resources by&nbsp;Cost</p> <p>Edit access to&nbsp;Projects and Users</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the projects you want to budget information for</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Budget resources in the `Resource Planner`

* [Budget resources in the Project View](#budgeting-in-the-project-view) 
* [Budget resources in the Role View](#budgeting-in-the-role-view) 
* [Budget resources in bulk](#budget)

### `Budget resources in the Project View`<![CDATA[   ]]>

<ol> 
 <li value="1"><![CDATA[
				]]>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>.<![CDATA[      ]]></li> 
 <li value="2"><![CDATA[
				]]><![CDATA[
			]]>Click Resourcing.<![CDATA[    ]]></li> 
 <li value="3"><![CDATA[
			]]>The Planner displays by default. </li> 
 <li value="4"> (Conditional) Select the <span class="bold">View by Project</span> view. </li> 
 <li value="5"> Expand the projects and the job roles to manage the allocation for the project, job roles, or users. </li> 
 <li value="6"> To budget allocation for users do one of the following: 
  <ul>
   <li> In the <span class="bold">BDG</span> column, manually specify a number of budgeted hours, FTE, or cost for the users.<br></li>
   <li>Click the <span class="bold">More</span> menu for the job role of the user, then click <span class="bold">Set Users' Planned Hours as Budgeted</span>.<br>The Budgeted Hours of each user are calculated using the following formula:<br><code>User Budgeted Hours = User Planned Hours</code></li>
  </ul></li> 
 <li value="7">To budget allocation for job roles, do one of the following:<br>
  <ul>
   <li>In the <span class="bold">BDG</span> column, manually specify a number of budgeted hours, FTE, or cost for the job role.<br><note type="note">
      The Role Budgeted Hours are added to the Project Budgeted Hours. 
    </note></li>
   <li>(Conditional) If you have budgeted hours for users, click the <span class="bold">More</span> menu for the job role, then click <span class="bold">Total Users' Budgeted Hours for Role</span>.<br>The Budgeted Hours for each role are calculated using the following formula:<br><code>Role Budgeted Hours = SUM(User Budgeted Hours)</code></li>
   <li>Click the <span class="bold">More</span> menu for the project, then click <span class="bold">Set Roles' Planned Hours as Budgeted</span>.<br>The Budgeted Hours for each role are calculated using the following formula:<br><em><code>Role Budgeted Hours = Role Planned Hours</code></em><note type="note">
     <ul>
      <li> The Role Budgeted Hours are added to the Project Budgeted Hours.</li>
      <li>Users can be budgeted for both Primary and Other (or secondary) Roles. </li>
      <li>The <span class="bold">Percentage of FTE Availability</span> for the roles of the user must be a number different than 0% for the Available Hours to display a value in the <span>Resource Planner</span> for a job role. If a user is associated with a role with a 0% <span class="bold">Percentage of FTE Availability</span>, the Available Hours value is zero for that job role. In this case, the role might show a negative <span class="bold">Net Value</span>.<br>For more information about the <span class="bold">Percentage of FTE Availability</span> for job roles, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>. </li>
     </ul>
    </note></li>
   <li>In the <span class="bold">BDG</span> column, manually specify a number of budgeted hours, FTE, or cost for the project. This distributes the number of Project Budgeted Hours to each role under the project. The following scenarios exist: 
    <ul>
     <li>If the number of Project Budgeted Hours your specify equals the Project Planned Hours, the Role Budgeted Hours match the Role Planned Hours.</li>
     <li>If the number of Project Budgeted Hours you specify does not equal the Project Planned Hours, the Role Budgeted Hours are distributed according to the percentage of Planned Hours needed for each role.<br>For example, if a project has 20 Planned Hours, and they are distributed between two job roles (Consultant requires 12 Planned Hours and Engineer requires 8 Planned Hours), and you budget 30 hours for the Project, the hours are distributed as follows: the Consultant role receives 18 Budgeted Hours, and the Engineer role receives 12 Budgeted Hours. </li>
    </ul></li>
  </ul></li> 
 <li value="8">To budget allocation for the project, do one of the following: 
  <ul>
   <li>Budget the roles under the project, as described in Step 7.<br>The Project Budgeted Hours is calculated by the following formula: <br><code>Project Budgeted Hours = SUM(Role Budgeted Hours)</code></li>
   <li>In the <span class="bold">BDG</span> column, manually specify a number of budgeted hours, FTE, or cost for the project.<br>This updates the Role Budgeted Hours, as described in Step 7.<br><img src="assets/budget-for-project-350x182.png" alt="budget_for_project.png" style="width: 350;height: 182;"></li>
  </ul></li> 
 <li value="9">Click <span class="bold">Save</span>.<br>After you budget your resources in the <span>Resource Planner</span>, the Budgeted Hours for your resources and any cost associated with them are listed in the Business Case of every project.<br>For more information about understanding the Resource Budgeting area of the Business Case, see the section "Resource Budgeting" in the article <a href="../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">Overview of the Areas of the Business Case</a>.</li> 
 <li value="10"> (Optional) Select the User view to notice any user overallocations or underutilization between the Available and the Planned Hours for each user. Budgeted Hours are not visible in the User view. </li> 
</ol>

### `Budget resources in the Role View`

You must have Edit access to Resource Management and Financial Data and Manage Finance permissions on the projects in order to budget resources in the `Resource Planner`. If you only have View access to at least one project listed under a job role, you cannot budget allocations for the role in the Role view. You can still budget allocation for the projects where you have Manage permissions.

For information about the access needed for budgeting resources, see the article [Access needed to budget resources](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

To budget allocations in the `Resource Planner` in the `` Role view:

<ol> 
 <li value="1"><![CDATA[
				]]><![CDATA[
			]]>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>.<![CDATA[      ]]></li> 
 <li value="2"><![CDATA[
				]]><![CDATA[
			]]>Click Resourcing.<![CDATA[     ]]></li> 
 <li value="3"><![CDATA[
			]]>The Planner displays by default.</li> 
 <li value="4"> (Conditional) Select the <span class="bold">View by Role</span> view. </li> 
 <li value="5"> Expand the job roles and the projects to manage the allocation for the project, job roles, or users. </li> 
 <li value="6"> To budget allocation for users, do one of the following: 
  <ul>
   <li> In the <span class="bold">BDG</span> column, manually specify a number of budgeted hours, FTE, or cost for the users. </li>
   <li>Click the <span class="bold">More</span> menu for the project, then click <span class="bold">Set Users' Planned Hours as Budgeted</span>.<br>The Budgeted Hours of each user are calculated using the following formula:<br><code>User Budgeted Hours = User Planned Hours</code></li>
  </ul></li> 
 <li value="7">To budget allocation for job roles, do one of the following:<br>
  <ul>
   <li>In the <span class="bold">BDG</span> column, manually specify a number of budgeted hours, FTE, or cost for the job roles.<br>This distributes the Role Budgeted Hours to the Project Budgeted Hours for the projects that you have access to manage.</li>
   <li>Click the <span class="bold">More</span> menu for the job role, then click <span class="bold">Set Projects' Planned Hours as Budgeted.<br></span>The Role Budgeted Hours are calculated using the following formula:<br><em><code>Role Budgeted Hours = SUM(Project Budgeted Hours)</code><br></em>The Project Budgeted Hours are calculated using the following formula:<br><code>Project Budgeted Hours = Project Planned Hours</code></li>
   <li><p>In the <span class="bold">BDG</span> column, manually specify a number of budgeted hours, FTE, or cost for the projects listed under the job role.<br>This adds the number of Project Budgeted Hours to the role. </p></li>
  </ul><note type="note">
    Users can be budgeted for both Primary and Other (or secondary) Roles. The 
   <span class="bold">Percentage of FTE Availability</span> for the roles of the user must be a number different than 0% for the Available Hours to display a value in the 
   <span>Resource Planner</span> for a job role. If a user is associated with a role with a 0% 
   <span class="bold">Percentage of FTE Availability</span>, the Available Hours value is zero for that job role. In this case, the role might show a negative 
   <span class="bold">Net Value</span>.
   <br>For more information about the 
   <span class="bold">Percentage of FTE Availability</span> for job roles, see the article 
   <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.
  </note></li> 
 <li value="8">To budget allocation for the project, do one of the following: 
  <ul>
   <li>In the <span class="bold">BDG</span> column, manually specify a number of budgeted hours, FTE, or cost for the projects.<br>This also updates the Budgeted Hours for the roles under which the project is listed. </li>
   <li>Click the <span class="bold">More</span> menu for the job role, then click <span class="bold">Set Projects' Planned Hours as Budgeted</span>.<br>The Project Budgeted Hours are calculated by the following formula:<br><code>Project Budgeted Hours = Project Planned Hours</code><br>The Project Budgeted Hours are added to the Role Budgeted Hours. </li>
   <li>(Conditional) If you have budgeted the hours for the users, click the <span class="bold">More</span> menu for the project, then click <span class="bold">Total Users' Budgeted Hours for Project</span>.<br>The Project Budgeted Hours is calculated using the following formula:<br><code style="font-style: normal;">Project Budgeted Hours = SUM(User Budgeted Hours)</code><br><img src="assets/budget-by-role-350x181.png" alt="budget_by_role.png" style="width: 350;height: 181;"></li>
  </ul></li> 
 <li value="9">Click <span class="bold">Save</span>.<br>After you budget your resources in the <span>Resource Planner</span>, the Budgeted Hours for your resources and any cost associated with them are listed in the Business Case of every project.<br>For more information about understanding the Resource Budgeting area of the Business Case, see the article <a href="../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md" class="MCXref xref">Budget resources in the Business Case</a>.</li> 
 <li value="10"> (Optional) Select the <span class="bold">View by User</span> view to notice any user overallocations or underutilization between the Available and the Planned Hours for each user. Budgeted Hours are not visible in the View by User view. </li> 
</ol>

### Budget resources in bulk

You can budget allocations for your resources in bulk when using quick links. The quick links are available only for the Project and Role Views.

![](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>When using the quick links to budget allocations for resources, the budgeting is automatically applied only to the time periods displayed on the screen. If the timeline of a project spans over a period of time longer than the one displayed on your screen, you must scroll from left to right, and then use the quick links to automatically budget your resources.

To budget your resources in bulk:

<ol> 
 <li value="1">Go to the .<br>For more information about accessing the <span>Resource Planner</span>, see the "Access the <span>Resource Planner</span>" section in the article <a href="../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. <br>A list of projects you can manage displays in the list.<br></li> 
 <li value="2">(Optional) Expand each project to see a list of job roles associated with it.<br>Or</li> 
 <li value="3">(Optional) Select <span class="bold">View by Role</span>, then expand each role to see a list of projects associated with it. </li> 
 <li value="4">Hover over the name of a project or of a job role.</li> 
 <li value="5">Click the <span class="bold">More</span> icon <img src="assets/options-icon-resource-planner.png" alt="options_icon_resource_planner.png">which displays to the far right of the project or role name.<br></li> 
 <li value="6"> <p>Click one of the available options to automatically specify the amount of Budgeted Hours (BDG) for other objects.</p> <p>Depending on whether you clicked the More icon on a project or a role, the options for budgeting in bulk differ. The table below illustrates the options available for projects and roles:</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td> </td> 
     <td><span class="bold">Project View</span> </td> 
     <td><span class="bold">Role View</span> </td> 
    </tr> 
    <tr> 
     <td>Project Options</td> 
     <td> 
      <ul> 
       <li><span class="bold">Set Roles' Planned Hours as Budgeted</span>: Select this option to make the Budgeted Hours of the role become identical to their Planned Hours. The total of the Budgeted Hours for the roles will display for the Project Budgeted Hours. </li> 
       <li><span class="bold">Adjust Budgeting Dates</span> : Select this option to move the Budgeted Hours to a different timeframe.<br>For more information about adjusting budgeting dates, see <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">Adjust budgeting dates in the Resource Planner</a>.</li> 
      </ul> </td> 
     <td> 
      <ul> 
       <li><span class="bold">Set Users' Planned Hours as Budgeted</span>: Select this option to make the Budgeted Hours of the user become identical to the their Planned Hours. </li> 
       <li><span class="bold">Total Users' Budgeted Hours for Project</span>: Select this option to add all the user Budgeted Hours together and display the total as the Budgeted Hours for the project and for the role. We recommend that you use this option after you have either manually budgeted your users, or you have used the previous option first. </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td>Role Options</td> 
     <td> 
      <ul> 
       <li><span class="bold">Set Users' Planned Hours as Budgeted</span>: Select this option to make the Budgeted Hours of the user become identical to their Planned Hours. </li> 
       <li><span class="bold">Total Users' Budgeted Hours for Role</span>: Select this option to add all the Budgeted Hours of the user together and display the total as the Budgeted Hours for the role and the project. We recommend that you use this option after you have either manually budgeted your users, or you have used the previous option first. </li> 
      </ul> </td> 
     <td> 
      <ul> 
       <li><span class="bold">Set Projects' Planned Hours as Budgeted</span>: Select this option to make the project Budgeted Hours become identical with the project Planned Hours. </li> 
      </ul> </td> 
    </tr> 
   </tbody> 
  </table> <note type="note"> 
   <p> Some of the options might not display if some of the prerequisites of working in the <span>Resource Planner</span> are missing. </p> 
   <p>For more information about the prerequisites that must be met for accurate budgeting in the <span>Resource Planner</span>, see the "Prerequisites for working in the <span>Resource Planner</span>" section in the <a href="../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a> article.<br>For example, some of the options might not display in the following scenarios:</p> 
   <ul> 
    <li>When projects are not associated with Resource Pool</li> 
    <li>When Resource Pools that are associated with projects do not contain users</li> 
    <li>When Resource Pools that are associated with projects contain users with no job role associated with them.</li> 
   </ul> 
  </note> </li> 
</ol>

##  

