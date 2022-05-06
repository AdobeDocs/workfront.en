---
filename: budget-by-role-resource-planner-d
product-area: resource-management
navigation-topic: resource-planning
title: Budget resources by role in the Resource Planner
description: (new article. drafted. publish when ready -- will this be broken of this article: /Content/Resource Mgmt/Resource Planning/budget-resources-project-role-views-resource-planner.htm ??)
hidefromtoc: true
---

# Budget resources by role in the Resource Planner

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(new article. drafted. publish when ready -- will this be broken of this article: /Content/Resource Mgmt/Resource Planning/budget-resources-project-role-views-resource-planner.htm ??)</p>
-->

As a Resource Manager, you can budget your resources by Job Roles, to determine how much time should be allocated to each role. You can do this in the Role View of the Resource Planner.&nbsp;

* Prerequisites for Using the Role View in the Resource Planner
* Understanding Budgeting in the Role View of the Resource Planner
* Budgeting Resources in the Role View of the Resource Planner

## Prerequisites for Using the Role View in the Resource Planner

```**^```

You must be a Resource Manager to populate the Role View of the Resource Planner.&nbsp;

To successfully use the Resource Planner, you must first ensure that your users, projects, tasks, and issues meet&nbsp;a set of prerequisites. These prerequisites are mandatory to display the correct information in the Resource Planner.

For&nbsp;more information about the prerequisites that must be met before you can start using the Resource Planner, see the [Get started with Resource Planning](../../resource-mgmt/resource-planning/get-started-resource-planning.md) [Get started with Resource Planning](../../resource-mgmt/resource-planning/get-started-resource-planning.md) section in [Get started with Resource Planning](../../resource-mgmt/resource-planning/get-started-resource-planning.md).&nbsp;

## Understanding Budgeting in the Role View of the Resource Planner

We recommend that you budget your resources in the Role View, when you are mostly concerned with how a bulk number of hours, FTE, or amount of Cost is distributed amongst all your Job Roles in the system.&nbsp;

Consider the following when selecting the Role view in the Resource Planner:&nbsp;

* You can see roles that are associated with projects for which you are designated as the Resource Manager in the Role view of the Resource Planner.
* You can expand each role to display a list of projects, and every project to display a list of users that can fulfill those roles on the projects.&nbsp;
* The number of items you display or can export from the Role view is limited, to improve performance.  
  For more information about limitations when viewing the Resource Planner in the Role view, see the "Role View" section in [Resource Planner display limitations](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md). 

* The projects are listed under the job role in the same order of priority as they are listed in the Project view.&nbsp; 
* When this view is applied, the Project&nbsp;Hours, FTE or Cost add up to the Role&nbsp;Hours, FTE or Cost.  
  ![resource_planner_view_by_role.png](assets/resource-planner-view-by-role-350x222.png)

## Budgeting Resources in the Role View of the Resource Planner

1. Go to the&nbsp;**People**&nbsp;area in the Global Navigation Bar. 
1. Select the&nbsp;**Planning**&nbsp;tab. 
1. Select the&nbsp;**Resource Planner**&nbsp;sub-tab. 
1. (Conditional) Select the **View by Role**&nbsp;view.&nbsp; 
1. Expand the job roles and the projects to manage the allocation for the project, job roles, or users. 
1. To budget allocation for users, do one of the following: &nbsp;

   * In the **BDG** column, manually specify a number of budgeted hours, FTE, or cost for the users. 
   * Click the&nbsp;**Options** icon for the project, then click **Set Users' Planned Hours as Budgeted**.  
     The Budgeted Hours of each user are calculated using the following formula:

     ```   
     User Budgeted Hours = User Planned Hours
     ```

1. To budget allocation for job roles, do one of the following:

   * In the **BDG** column, manually specify a number of budgeted hours, FTE, or cost for the job roles.

     >[!TIP]
     >
     >This adds the Role Budgeted Hours to the Project Budgeted Hours.

   * Click the **Options** icon for the job role, then click **Set Projects' Planned Hours as Budgeted.**The Role Budgeted Hours are calculated using the following formula:  
   * * 
   
     ```   
     Role Budgeted Hours = SUM(Project Budgeted Hours)
     ```   
   
     * 
     *The Project Budgeted Hours are calculated using the following formula:

     ```   
     Project Budgeted Hours = Project Planned Hours
     ```

   * In the **BDG** column, manually specify a number of budgeted hours, FTE, or cost for the projects listed under the job role.  
     This adds the number of Project Budgeted Hours to the role.&nbsp;* 
     *
   
   * 
   
     >[!TIP]
     >
     >Users can be budgeted for both Primary and Other (or secondary) Roles. The **Percentage of FTE Availability** for the&nbsp;roles of the user must be a number different than 0% for&nbsp;the Available Hours to display a value in the Resource Planner for a job role. If a user is associated with a role with a 0% **Percentage of FTE Availability**, the Available Hours value is zero for that job role. In this case, the role might show a negative **Net Value**.

     For more information about the Percentage of FTE&nbsp;Availability for job roles, see [Edit a user's profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). * 
     *

1. To budget allocation for the project, do one of the following:

   * In the **BDG** column, manually specify a number of budgeted hours, FTE, or cost for the projects.  
     This also updates the Budgeted Hours for the roles under which the project is listed.&nbsp;
   
   * Click the **Options** icon for the job role, then click **Set Projects' Planned Hours as Budgeted**.  
     The Project Budgeted Hours are calculated by the following formula:

     ```   
     Project Budgeted Hours = Project Planned Hours
     ```

     The Project Budgeted Hours are added to the Role Budgeted Hours.&nbsp;
   
   * (Conditional) If you have budgeted the hours for the users, click the **Options** icon for the project, then click **Total Users' Budgeted Hours for Project**.  
     The Project Budgeted Hours is calculated using the following formula:

     ```   
     Project Budgeted Hours = SUM(User Budgeted Hours)
     ```

     ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. Click **Save**.  
   After you budget your resources in the Resource Planner, the Budgeted Hours for your resources and any cost associated with them are listed in the Business Case of every project.  
   For more information about understanding the Resource Budgeting area of the Business Case, see the "Resource Budgeting" section in&nbsp; [Create a Business Case for a project](../../manage-work/projects/define-a-business-case/create-business-case.md).

1. (Optional) Select the **View by User** view to notice any user overallocations or underutilization between the Available and the Planned Hours for each user. Budgeted Hours are not visible in the View by User view.&nbsp;

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;<span class="wysiwyg-color-pink">**^ This section repeats between the Role, Project view articles and the main Planning in the Res Planner article.</span></p>
-->

