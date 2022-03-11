---
filename: budgeted-cost
content-type: reference
product-area: projects
navigation-topic: financials
title: Calculate Budgeted Cost
description: The Budgeted Cost of a project is the total cost associated with the project as estimated when you plan the project.
---

# Calculate Budgeted Cost

The Budgeted Cost of a project is the total cost associated with the project as estimated when you plan the project.

## Overview of Budgeted Cost in a project

You cannot manually change the Budgeted Cost of a project. Adobe Workfront calculates the Budgeted Cost using the following formula:

```
Budgeted Cost = Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project
```

* The `Budgeted Labor Cost` in the calculation above is the cost associated with the job roles in the project.

  You can track the Budgeted Labor Cost of a project in the following area of Workfront:

  * Resource Budgeting area of the Business Case or the Resource Planner

  For information about Budgeted Labor Costs, see the article [Understand Budgeted Labor Cost and Budgeted Hours for projects](../../../manage-work/projects/project-finances/budgeted-labor-cost.md). 

* The `Budgeted Expenses Cost` in the calculation above is the Planned Cost associated with the expenses on the project, as they are calculated in the Expenses area of the Business Case or the Expenses tab of the project.  
  For more information about Expenses on a project, see the article [Manage project expenses](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* The `Fixed Cost` in the calculation above is the fixed amount associated with the Cost of the project, as defined in the Finances area of the Details sectionof the project.  
  For more information about the Finance sub-tab of a project, see the article [Manage information in the project Finance area](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront calculates all cost information using the currency of the project. If you specify Budgeted Hours for your resources in the Resource Planner, the option to change project currency is disabled. 
>
>For more information about changing the currency of a project, see the article [Change the project currency](../../../manage-work/projects/project-finances/change-project-currency.md).

## Locate the Budgeted Cost of a project

You can view the following Budgeted Cost information in Workfront:

<ul> 
 <li> <p>The Budgeted Cost as reflected in the Resource Budgeting area of the Business Case or the Resource Planner displays in the following areas of Workfront under the following names:</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Budgeted Cost display name</td> 
     <td>Area of Workfront</td> 
    </tr> 
    <tr> 
     <td>Budgeted Cost</td> 
     <td> <p>Business Case Summary</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Cost</td> 
     <td> <p>Portfolio Optimizer</p> <note type="tip">
       The total of all project Budgeted Cost values is the Budgeted Cost of the portfolio.
      </note> </td> 
    </tr> 
    <tr> 
     <td>Project Budgeted Cost</td> 
     <td> <!--
       Resource Estimates report
      --> <p>Project report</p> <p>Project (Financial Data) report</p> <p>Task report</p> <p>Issue report</p> <p>Budgeted Hour report</p> <p>For more information about creating a report, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ul>

