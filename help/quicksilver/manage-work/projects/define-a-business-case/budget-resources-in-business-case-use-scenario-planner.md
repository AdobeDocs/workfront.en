---
navigation-topic: business-case-and-scorecards
title: Budget resources in the Business Case using the Scenario Planner
description: As part of resource planning, you can use the Adobe Workfront Scenario Planner to budget the job roles necessary for completing the work in a project when you build the business case.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
---
# Budget resources in the Business Case using the Scenario Planner

As part of resource planning, you can use the Adobe Workfront Scenario Planner to budget the job roles necessary for completing the work in a project when you build the business case.

For more information about creating a business case, see [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>The job role information for the initiative linked to the project that you enter in the system-level Scenario Planner is visible in the Resource Budgeting area of the project's business case when you publish the initiative. The Scenario Planner is available only in the new Adobe Workfront experience and requires an additional license. For information about the Workfront Scenario Planner, see [The Scenario Planner overview](../../../scenario-planner/scenario-planner-overview.md).

You can also budget resources in the business case using the Resource Planner. For more information, see the following:

* [Budget resources in the Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md) 
<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>We recommend that you make the decision whether to use the&nbsp;Resource Planner or the&nbsp;Scenario Planner when you begin working on a project. Frequently switching between the two during the life of the project may create inconsistencies in the way you budget your resources for the project.

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Business or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>You must purchase an additional license for the Adobe Workfront Scenario Planner to access functionality described in this article.</p> <p>For information about obtaining the Workfront Scenario Planner, see <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the following: </p> 
    <ul> 
     <li> <p>Projects</p> </li> 
     <li> <p>Financial Data</p> </li> 
     <li> <p>Scenario Planner </p> </li> 
    </ul> <p>For information about the access needed to budget resources, also see <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> <p>Note: If you still don't have access, ask your Adobe Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you begin, you must do the following:

* Create a plan using the Scenario Planner.

  For information, see [Create and edit plans in the Scenario Planner](../../../scenario-planner/create-and-edit-plans.md).

* Create an initiative on the plan and link it to a project.

  Ensure that you indicate the required job roles information for the initiative and update the linked project with this information.

  For more information, see the following articles:

   * [Create and edit initiatives in the Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md) 
   * [Import projects to plans in the Scenario Planner](../../../scenario-planner/import-projects-to-plans.md) 
   * [Update or create projects by publishing initiatives in the Scenario Planner](../../../scenario-planner/publish-scenarios-update-projects.md).

* Although these are not prerequisites, we also recommend the following:

   * Assign tasks on the project to the job roles budgeted in the Scenario Planner.
   * Indicate the number of Planned Hours for the tasks on the project.

     This helps you understand the amount of work a task might need to complete, which helps with the decision of how much time the resources should be budgeted for to complete the task.

     For information about associating tasks with Planned Hours, see [Edit tasks](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Budget resources in the Business Case using the Scenario Planner for projects linked to initiatives

>[!IMPORTANT]
>
>You can budget your resources for a period of 15 years. If you budget resources for a project with a duration longer than 15 years the budgeting information might not be accurate.
><!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->

1. Go to the project for which you want to budget resources.

   >[!TIP]
   >
   >This is a project linked to an initiative in the Scenario Planner whose linked initiative has been published at least once.

1. Click **Business Case** in the left panel.
1. (Conditional) In the **Resource Budgeting** section, do one of the following:

   * If you just published information from the Scenario Planner, select Scenario Planner in the **Choose which hours to use to calculate the Budgeted Labor Cost of the project** field in the Resource Budgeting area, then click **Choose**.

     ![Business case in Resource Planner with Choose button](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * If the Resource Planner was previously selected for budgeting resources for the project, click **Change** > **Scenario Planner** > **Choose**.

     ![Business case in Scenario Planner with Choose button](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

     Workfront uses the required job role hours from the linked initiative to calculate the project's Budgeted Labor Cost and Budgeted Hours. This is the recommended option. Cost displays in the Business Case in the currency of the project.

     When you copy a project, and you select to copy the Budgeted Hours to the new project, the hours budgeted using the Scenario Planner are not copied to the new project. Only hours budgeted in the Resource Planner are copied. For more information, see [Copy a project](../manage-projects/copy-project.md). 

      >[!IMPORTANT]
      >
      >When you use the Scenario Planner to budget resources for the project, the Budgeted Labor Cost displays in the following areas of Workfront:
      >
      >   
      >   
      >   * Resource Budgeting area of the Business Case 
      >   * The system-level Scenario Planner as the People Cost of the initiative linked to the project. For more information, see [Create and edit initiatives in the Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md). 
      >   
      >

1. (Optional) Click **View in Scenario Planner** to open the plan that contains the initiative linked to the project. This opens the Scenario Planner in a new browser tab. 
1. (Optional) Update information on the initiative. For more information, see [Create and edit initiatives in the Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   >
   >You must publish the initiative after every change for the Resource Budgeting area on the project to update.
