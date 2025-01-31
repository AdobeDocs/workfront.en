---
navigation-topic: business-case-and-scorecards
title: Budget resources in the Business Case using the Resource Planner
description: As part of resource planning, you can use the project-level Resource Planner to budget the job roles necessary for completing the work in a project when you build the business case.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
---
# Budget resources in the Business Case using the Resource Planner

<!--Audited: 01/2025-->

As part of resource planning, you can use the project-level Resource Planner to budget the job roles necessary for completing the work in a project when you build the business case.

For more information about creating a business case, see [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>The information you enter in the project-level&nbsp;Resource Planner is also visible in the system-level Resource Planner. The reverse is also true. For information about the Resource Planner, see [Resource Planner overview](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

You can also budget resources in the business case using the Adobe Workfront Scenario Planner. For more information, see [Budget resources in the Business Case using the Scenario Planner](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Access requirements

You must have the following to perform the steps in this article:

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Prime or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Light or higher</p>
   <p>Current: Review or higher</p> 
   
   <p><b>IMPORTANT:</b></p> 
   <p>New: You must have a Standard license to modify resource budgeting information. </p> 
   <p>Current: You must have a Plan license to modify resource budgeting information. </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to the following: </p> 
    <ul> 
     <li> <p>Projects</p> </li> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Financial Data</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you begin, you must do the following:

* Meet all the prerequisites for resource planning in Adobe Workfront. For information, see [Resource Planner overview](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Associate Resource Pools with the project.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

  >[!NOTE]
  >
  >You cannot budget resources assigned to issues in the Business Case. You can budget them in the system-level Resource Planner. For more information about the Resource Planner, see [Resource Planner overview](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Although this is not a prerequisite, we also recommend that you indicate Planned Hours for the tasks on the project. This helps you understand the amount of work a task might need to complete which helps with the decision of much time the resources should be budgeted for to complete the task. For information about associating tasks with Planned Hours, see [Edit tasks](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Apply Resource Pools to a project and budget resources in the Business Case

>[!IMPORTANT]
>
>You can budget your resources for a period of 15 years. If you budget resources for a project with a duration longer than 15 years the budgeting information might not be accurate.

To apply Resource Pools and budget project resources in the Business Case for a project with no Resource Pool:

1. Go to the project for which you want to budget resources. 
1. Click **Business Case** in the left panel. 
1. (Conditional) If your company does not have a license for the&nbsp;Workfront Scenario Planner, click **Edit Resource Budgeting** in the **Resource Budgeting** section, then continue with step 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Optional and conditional) If the project information has been published from an initiative on the Scenario Planner, do one of the following:

   * Select Resource Planner in the **Choose which hours to use to calculate the Budgeted Labor Cost of the project** field, then click&nbsp;**Choose > Edit Resource Budgeting**.

     ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * If the Scenario Planner was selected for budgeting resources for the project, click **Change** > **Edit Resource Budgeting**.

     ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)

   This uses the Budgeted Hours of the project to calculate the Budgeted Labor Cost for the project.

   The Scenario Planner is available only in the new Adobe Workfront experience and requires an additional license. For information about the Workfront Scenario Planner, see [The Scenario Planner overview](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   >
   >We recommend that you make the decision whether to use the&nbsp;Resource Planner or the&nbsp;Scenario Planner when you begin working on a project. Frequently switching between the two during the life of the project may create inconsistencies in the way you budget your resources for the project.

1. In the **Select Resource Pool** field, specify one or several **Resource Pools**.

   You must specify only Resource Pools that are populated with active users.

   >[!TIP]
   >
   >If the project is already associated with Resource Pools, the Resource Planner displays by default. To add more Resource Pools to the project, edit the project. For information about editing a project, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Click **Apply**.

   The Resource Planner is displayed, for the selected project.

   By default, the first 20 job roles associated with this project are listed in the Resource Budgeting section in alphabetical order.&nbsp;

   For more information about the Resource Planner, see [Resource Planner overview](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Optional and conditional) Expand the job roles to see the users associated with them.

   >[!NOTE]
   >
   >Active users are displayed under the job roles associated with them only if they meet the following criteria:
   >
   >   
   >   
   >   * They belong to one of the Resource Pools of the project. 
   >   * They have Budgeted Hours assigned to them. 
   >   * They are associated with one of the job roles of the project. 
   >   
   >

   &nbsp;

1. Click **Today** to return to today's time frame.
1. (Optional) Click **Week**, **Month** or **Quarter** to display information for the project in different time frames.
1. (Optional) Click the **Hours** drop-down menu, and select **Hours**,**FTE**, or **Cost** to change how information displays in the Resource Planner. Hours display by default.

1. (Optional) Click **Export** to export the Resource Planner to an Excel file.

   >[!NOTE]
   >
   >You can export data for up to 12 time periods at a time.

1. (Optional) Click the **Full Screen** icon ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) to display the Resource Planner in full screen mode.  

1. Update the **BDG** (Budgeted Hours) field with Hour, FTE, or Cost values for the users, roles, or the project by doing one of the following:

   * Manually estimate the amount of Hours, FTE, or Cost values for roles, users, or the project.

     Or 
   
   * Click the **Options** icon for the project or the job roles and select an option to automatically budget the hours for roles, users, or the project.

   For more information about budgeting in the Project View of the Resource Planner, see [Budget resources in the Resource Planner using the Project and Role views](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   >
   >You can budget hours, FTEs, or costs for your resources for any time frame displayed in the Resource Budgeting area, independent of the timeline of the project. For example, if you want to indicate that your resources might not be available during the timeline of the project (where they are associated with Planned Hours), but they might be available during another time, you can do so by budgeting them for time frames where the Planned Hours are zero, if that is when they become available to work.

1. (Optional) To understand whether you can move the budgeted Hours, FTEs, or Costs to another time frame, click the **Options** icon, then **Adjust Budgeting Dates**.

   For more information about adjusting budgeted dates, see [Adjust budgeting dates in the Resource Planner](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Click **Save**.

   If you have Cost per Hour rates associated with your job roles, budgeting the resources in the Resource Budgeting area calculates the **Budgeted Labor Cost** of the project. The Budgeted Labor Cost is displayed in the Resource Budgeting area of the Business Case and in the Business Case Summary.

   >[!TIP]
   >
   >Cost displays in the Business Case in the currency of the project.

   The budgeting information specified in the Business Case is also displayed in the Resource Planner.

   When you copy a project, you have the option to also copy the Budgeted Hours to the new project. Only hours budgeted in the Resource Planner are copied. For more information, see [Copy a project](../manage-projects/copy-project.md).
