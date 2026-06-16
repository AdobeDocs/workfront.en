---
content-type: reference
product-area: projects
navigation-topic: financials
title: Calculate Budgeted Cost
description: Calculate Budgeted CostTracking Project Progress with a Utilization Report
author: Lisa
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/20gQnapiR9T6hm3WCv6-8ymhphOOEcZWqUi-05a4CUU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---
# Calculate Budgeted Cost

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

The Budgeted Cost of a project is the total cost associated with the project as estimated when you plan the project.

## Overview of Budgeted Cost in a project

You cannot manually change the Budgeted Cost of a project. Adobe Workfront calculates the Budgeted Cost using the following formula:

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* The **Resource Planner Budgeted Labor Cost** in the calculation above is the cost associated with the job roles in the project.

  You can track the Budgeted Labor Cost of a project in Resource Budgeting area of the Business Case or the Resource Planner. 

  >[!TIP]
  >
  >  The Budgeted Labor Cost of a project in the Business Case displays as Resource Planner Budgeted Labor Cost in reports and lists.

  For information about Budgeted Labor Costs, see the article [Understand Budgeted Labor Cost and Budgeted Hours for projects](../../../manage-work/projects/project-finances/budgeted-labor-cost.md). 

* The **Budgeted Expenses Cost** in the calculation above is the Planned Cost associated with the expenses on the project, as they are calculated in the Expenses area of the Business Case or the Expenses tab of the project.  
  For more information about Expenses on a project, see the article [Manage project expenses](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* The **Fixed Cost** in the calculation above is the fixed amount associated with the Cost of the project, as defined in the Finances area of the Details section of the project.  
  For more information about the Finance sub-tab of a project, see the article [Manage information in the project Finance area](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront calculates all cost information using the currency of the project. If you specify Budgeted Hours for your resources in the Resource Planner, the option to change project currency is disabled. 
>
>For more information about changing the currency of a project, see the article [Change the project currency](../../../manage-work/projects/project-finances/change-project-currency.md).

## Locate the Budgeted Cost of a project

The Budgeted Cost as reflected in the Resource Budgeting area of the Business Case or the Resource Planner displays in the following areas of Workfront under the following names:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Budgeted Cost display name</strong></td> 
     <td><strong>Area of Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Budgeted Cost</td> 
     <td> <p>Business Case Summary</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Cost</td> 
     <td> <p>Portfolio Optimizer</p> <p>Tip: The total of all project Budgeted Cost values is the Budgeted Cost of the portfolio.</p> </td> 
    </tr> 
    <tr> 
     <td>Project Budgeted Cost</td> 
     <td>
     <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      -->
      <p>Project report</p> <p>Project (Financial Data) report</p> <p>Task report</p> <p>Issue report</p> <p>Budgeted Hour report</p> <p>For more information about creating a report, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </td>
    </tr> 
   </tbody> 
  </table>
