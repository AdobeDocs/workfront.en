---
filename: budget-resources-in-business-case
navigation-topic: business-case-and-scorecards
title: Budget resources in the Business Case
description: The information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Budget resources in the Business Case

The information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

As part of resource planning, you can budget the job roles necessary for completing the work in a project when you build the business case. For more information about creating a Business Case, see [Create a Business Case for a project in Adobe Workfront](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!NOTE]
>
>Budgeting resources is not the same as scheduling resources for a project. When you budget resources you estimate the roles that might be necessary to complete the work on a project. For actually scheduling or assigning users to the work on a project, see [Get started with Resource Scheduling](../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md). For information about resource planning in Adobe Workfront, see [Get started with Resource Planning](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

You must associate job roles with the project before you can budget the resources for it. The following are ways of allocating job roles to a project:

* Use the Resource Planner to apply Resource Pools to the project and budget job roles.

  For more information, see [Budget resources in the Business Case using the Adobe Workfront Resource Planner](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md). 

* Use the Scenario Planner to create initiatives with required job roles and link them to the project. For more information, see [Budget resources in the Business Case using the Adobe Workfront Scenario Planner](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

  >[!NOTE]
  >
  >This is available only in the new Adobe Workfront experience and requires an additional license. For information about the Workfront Scenario Planner, see [The Adobe Workfront Scenario Planner overview](../../../scenario-planner/scenario-planner-overview.md).

##

##

<!--
You can associate Resource Pools with a project as part of completing the Resource Budgeting section of the Business Case of the project. The information you update here is also reflected in the Resource Planner.
-->

<!--
For more information about creating a Business Case, see Create a Business Case for a project in Adobe Workfront. For more information about planning in the Resource Planner, see Resource Planner overview.
-->

<!--
Prerequisites for budgeting resources on a project
-->

<!--
To successfully budget your resources in the Business case, you must have the following information available in Adobe Workfront:
-->

  <!--
  You must have Edit access to projects in your access level.
  -->

  <!--
  You must have Manage permissions on the project to be able to edit the Business Case of the project.
  -->

* 

  <!--
  You must have Edit access to Resource Management and Financial Data, as well as Manage Finance permissions on the project.
  -->

  <!--
  For information about the access needed to budget resources, see Access needed to budget resources.
  -->

* 

  <!--
  You must have Resource Pools attached to the project.
  -->

  <!--
  Note: You cannot budget resources assigned to issues in the Business Case. You can budget them in the Resource Planner. For more information about the Resource Planner, see Resource Planner overview.
  -->

* 

  <!--
  You must understand user and job role availability according to the Resource Management Preferences in your system.
  -->

  <!--
  Obtaining information about user availability depends on how your Workfront administrator configures your Resource Management Preferences.
  -->

  <!--
  For more information about calculating user availability and setting Resource Management Preferences, see Configure Resource Management preferences.
  -->

* 

  <!--
  In order to calculate the Budgeted Labor Cost of the project, you must associate users and job roles with Cost per Hour rates.
  -->

  <!--
  Note: Cost displays in the Business Case in the currency of the project.
  -->

  <!--
  For more information about associating Cost per Hour rates with job roles, see Create and manage job roles.
  -->

  <!--
  For more information about associating Cost per Hour rates with users, see Edit a user's profile.
  -->

  <!--
  Although this is not a prerequisite, we also recommend that you might also have Planned Hours associated with your tasks, to understand the amount of work a task might need to complete.
  -->

<!--
Apply Resource Pools to a project and budget resources in the Business Case
-->

<!--
Important: You can budget your resources for a period of 15 years. If you budget resources for a project with a duration longer than 15 years the budgeting information might not be accurate.
-->

<!--
To apply Resource Pools and budget project resources in the Business Case for a project with no Resource Pool:
-->

   <!--
   Go to the project which you want to associate with the Resource Pools.
   -->

   <!--
   Select the Project Details tab.
   -->

1. 

   <!--
   Select the Business Case sub-tab.
   -->

   <!--
   Click Business Case in the left panel.
   -->

1. 

   <!--
   In the Resource Budgeting section, click Edit Resource Budgeting.
   -->

1. 

   <!--
   In the Select Resource Pool field, specify one or several Resource Pools.
   -->

   <!--
   You must specify only Resource Pools that are populated with active users.
   -->

   <!--
   Tip: If the project is already associated with Resource Pools, the Resource Planner displays by default. To add more Resource Pools to the project, edit the project. For information about editing a project, see Edit projects.
   -->

1. 

   <!--
   Click Apply.
   -->

   <!--
   The Resource Planner is displayed, for the selected project.
   -->

   <!--
   For more information about the Resource Planner, see Resource Planner overview.
   -->

   <!--

   -->

1. 

   <!--
   (Optional) Click Week, Month or Quarter to display information for the project in different time frames.
   -->

   <!--
   Click Today to return to today's time frame.
   -->

   <!--
   (Optional) Click the Hours drop-down menu, and select Hours, FTE, or Cost to change how information displays in the Resource Planner. Hours display by default.
   -->

   <!--
   (Optional) Click Export to export the Resource Planner to an Excel file. Note: You can export data for up to 12 time periods at a time.
   -->

   <!--
   (Optional) Click the Full Screen icon to display the Resource Planner in full screen mode.
   -->

   <!--
   Update the BDG (Budgeted Hours) field with Hour, FTE, or Cost values for the the users, roles, or the project by doing one of the following: Manually estimate the amount of Hours, FTE, or Cost values for roles, users, or the project. Or Click the Options icon for the project or the job roles and select an option to automatically budget the hours for roles, users, or the project. For more information about budgeting in the Project View of the Resource Planner, see the Using the Project and Role Views to Budget Resources. Note: You can budget hours, FTEs, or costs for your resources for any time frame displayed in the Resource Budgeting area, independent of the timeline of the project. For example, if you want to indicate that your resources might not be available during the timeline of the project (where they are associated with Planned Hours), but they might be available during another time, you can do so by budgeting them for time frames where the Planned Hours are zero, if that is when they become available to work.
   -->

1. 

   <!--
   (Optional) To understand whether you can move the budgeted Hours, FTEs, or Costs to another time frame, click the Options icon, then Adjust Budgeting Dates.
   -->

   <!--
   For more information about adjusting budgeted dates, see Adjust budgeting dates in the Resource Planner.
   -->

1. 

   <!--
   Click Save.
   -->

   <!--
   If you have Cost per Hour rates associated with your job roles, budgeting the resources in the Resource Budgeting area calculates the Budgeted Labor Cost of the project. The Budgeted Labor Cost is displayed in the Resource Budgeting area of the Business Case and in the Business Case Summary.
   -->

   <!--
   The budgeting information specified in the Business Case is also displayed in the Resource Planner.
   -->

