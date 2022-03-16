---
filename: portfolio-optimizer-overview
content-type: overview
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
title: Portfolio Optimizer overview
description: The Portfolio Optimizer is the tool used for project evaluation and comparison. The process of reviewing and comparing Business Case values for projects assigned to a portfolio is how a portfolio manager can prioritize projects and generate the most value for an organization.
---

# Portfolio Optimizer overview

##  

The Portfolio Optimizer is the tool used for project evaluation and comparison. The process of reviewing and comparing Business Case values for projects assigned to a portfolio is how a portfolio manager can prioritize projects and generate the most value for an organization.

The purpose of the portfolio optimizer is to provide an interface through which a portfolio manager, steering committee, or product management office can view summary information about the business case of each project. Projects can then be prioritized according to strategic values and goals, or according to their overall score.

The Portfolio Optimizer can only assist you if you have completed the following prerequisites:

* The Business Cases have been completed on the projects
* A portfolio is defined for the projects you want to review
* You provide a budget to represent the total financial cap of the selected projects.

For information about locating the Portfolio Optimizer, see [Locate the Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

<!--
Locate the Portfolio Optimizer Go to the Projects area in the Global Navigation Bar. Click the Portfolios tab and click the portfolio you want to view. Click the Portfolio Optimization tab. The Portfolio Optimizer displays.
-->

## Finances in the Portfolio Optimizer

* [The financial areas in the Portfolio Optimizer](#financial-areas) 
* [The financial fields in the Portfolio Optimizer](#financial-fieds-subsection)

You can see the financial state of your portfolio at any time during the life of your projects when using the Portfolio Optimizer.

Consider the following when working with finances in the Portfolio Optimizer:

* Projects are each given a score when their Business Cases are completed according to what criteria they match in the Portfolio Optimizer. For example, low cost or high alignment projects receive a higher score.

  For more information about calculating the portfolio optimizer score of a project, see the article [Overview of the Portfolio Optimizer Score](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* The financial calculations for the Portfolio Optimizer use the Budgeted Cost in the Business Case of the project.
* You can manually prioritize your projects in the Portfolio Optimizer, taking into account all the information about them. This includes financial data, alignment to their scorecards, ROI, for example.

### The financial areas in the Portfolio Optimizer

You can view financial information in the following areas of the Portfolio Optimizer:

* `Portfolio Header`: This area displays financial information gathered from all the projects in the portfolio. It displays on every tab of the Portfolio object. 
* `Portfolio Finances for Selected Projects`: This area displays financial information gathered from the projects which are selected in the Portfolio Optimizer. You can add or remove projects and understand how this will affect the finances of the portfolio by viewing the information in this area. 
* `Projects Finances`: This area displays the financial information of each project listed in the Portfolio Optimizer.

### The financial fields in the Portfolio Optimizer

The following financial fields display in the Portfolio Optimizer:

* [Portfolio header](#portfoli) 
* [Portfolio finances for selected projects](#portfoli2)<![CDATA[   ]]>
*

#### `Portfolio header`

Adobe Workfront calculates the financial fields in the portfolio header using information from projects with statuses that equate only with Approved or Current.

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Name of Field</span> </th> 
   <th><span class="bold">Description</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>On Time</td> 
   <td> <p>The percentage of projects in the portfolio which are considered to be On Time. This is visible from any tab inside a Portfolio.</p> <p>A project is considered to be On Time when the Project <span class="bold">Condition</span> is <span class="bold">On Target</span>. <br>For more information about Project Conditions, see the article <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Overview of Project Condition and Condition Type</a>.</p> <p>The <span class="bold">On Time</span> percentage is calculated by using the following formula:</p> <p><em>On Time Portfolio Percentage = Number of On Time Projects/ Total Number of Projects in a Current or Approved status</em> </p> </td> 
  </tr> 
  <tr> 
   <td>On Budget</td> 
   <td> <p>The percentage of projects in the portfolio which are considered to be On Budget. This is visible from any tab inside a Portfolio.</p> <p>Projects are <span class="bold">On Budget</span> when they have not exceeded their pre-defined budget. <br>For more information about the budget of a project, see the article <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Manage information in the project Finance area</a>.</p> <p>The On Budget percentage is calculated by using the following formula:</p> <p><em>On Budget Portfolio Percentage = Number of On Budget Projects/ Total Number of Projects </em><em>in a Current or Approved status</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (for portfolio)</td> 
   <td> <p>The Return on Investment (ROI) for the portfolio is calculated by taking into account the total Benefit of the Portfolio and the total of the Budgeted Costs of the projects. This is visible from any tab inside a Portfolio.</p> <p>The Portfolio ROI value is calculated by using the following formula:</p> <p><em>Portfolio ROI = (Total Benefit - Total Budgeted Cost)/ Total Cost * 100</em> </p> <p>For more information about how the ROI is calculated for a project, see the article <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Calculate Return On Investment (ROI)</a> .</p> </td> 
  </tr> Legacy ROI (for portfolio) The Legacy Return on Investment (ROI) for the portfolio is calculated by taking into account the Total Benefit of the portfolio and the Total of the Legacy budgeted costs of the projects. This is visible from any tab inside a portfolio. You might not have access to this functionality because it is supported by Flash, which has been deprecated in most environments. The portfolio Legacy ROI value is calculated by using the following formula: Portfolio Legacy ROI = [(Total Benefit - Total Legacy Budgeted Cost)/ Total Cost] * 100 For more information about how the ROI is calculated for a project, see the articleCalculate Return On Investment (ROI). 
  <tr> 
   <td>Aligned or Alignment Score </td> 
   <td> <p>An average of all the Project Alignment Score values which are calculated after completing the Scorecard in the Business Case of the project. The alignment score of each project is listed in the Alignment column of the Portfolio Optimizer. This is visible from any tab inside a portfolio.</p> <p>For more information about generating an alignment score for a project, see the article <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Apply a scorecard to a project and generate an Alignment Score</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Net Value</td> 
   <td> <p>The sum of all the Net Values of all the projects in the portfolio. This is visible from any tab inside a portfolio.</p> <p>For more information about how Net Value is calculated for a project, see the article <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calculate Net Value</a>.</p> </td> 
  </tr> Legacy Net Value The sum of all the Legacy Net Values of all the projects in the portfolio. This is visible from any tab inside a portfolio. You might not have access to this functionality because it is supported by Flash, which has been deprecated in most environments. For more information about how Net Value is calculated for a project, see the article Calculate Net Value. 
 </tbody> 
</table>

#### Portfolio finances for selected projects

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Name of Field</span> </th> 
   <th> <p><span class="bold">Description</span> </p> <p>&nbsp;</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Number of projects</td> 
   <td> <p>The total number of active projects in the portfolio. Projects that are considered active in a portfolio can be in any of the following statuses:</p> 
    <ul> 
     <li>Current</li> 
     <li>Planning</li> 
     <li>Approved</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Budget</td> 
   <td>You can manually update this field to indicate what is the total budget for the entire portfolio. This budget is used for all the projects inside the portfolio. </td> 
  </tr> 
  <tr> 
   <td>Remaining</td> 
   <td> <p>The remaining budget after all the Budgeted Costs on all the projects inside the portfolio have been subtracted from the Budget of the portfolio.</p> <p>The Remaining Portfolio Budget is calculated using the following formula:</p> <p><em>Remaining Portfolio Budget = Total Portfolio Budget - Total Budgeted Cost of All Portfolio Projects</em> </p> If you are using the Legacy Portfolio Optimizer, the Remaining Portfolio Budget is calculated by using the following formula: Remaining Portfolio Budget = Total Portfolio Budget - Total Legacy Budgeted Cost of All Portfolio Projects <p>The overall Budgeted Cost of all the projects in the portfolio is represented in the indicator bar under the Budget field. If you are using the Legacy Portfolio Optimizer, the Legacy Budgeted Cost of each project is listed in the Cost column.</p> <p>For more information about tracking costs on a project, see the article<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Total Cost</td> 
   <td> <p>The sum of the costs of all the projects displayed in the Portfolio Optimizer. The cost of each project is the same as the Budgeted Cost of the Project as it is displayed in the Business Case Summary. </p> <p>For more information about the financial fields of projects in the Business Case, see the section "Understanding Financial Fields in the Business Case" in the article <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Create a Business Case for a project in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Risk </td> 
   <td> <p>The sum of all the Potential Risk Costs of all the projects in the portfolio. The Potential Risk Cost of each project is listed in the Risk column of the Portfolio Optimizer. </p> <p>For more information about calculating risks for projects, see the article <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calculate Potential Risk Cost </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Benefit</td> 
   <td> <p>The sum of all the Planned Benefit values of all the projects in the portfolio. The Planned Benefit value of each project is listed in the Benefit column of the Portfolio Optimizer. </p> <p>For more information about the Planned Benefit of a project, see the article <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Overview of project Planned Benefit</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Risk to Net Value indicator</td> 
   <td> <p>Measures the Potential Risk value taking into account the Net Value provided by all projects in the portfolio. For achieving the most efficiency within the portfolio, you want to see that the Risk indicator is low and the Net Value indicator is high. </p> <p>For more information about calculating Risk to Net Value, see the article <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Calculate the Risk to Net Value in a portfolio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Customize the Portfolio Optimizer

You can customize only the project list area of the Portfolio Optimizer by using settings to change the information in the list.

The following icons and options are available for the Portfolio Optimizer:

<table cellspacing="15">   
 <col> 
 <col> 
 <thead> 
  <tr> Icon in the Legacy Portfolio Optimizer Icon in the Portfolio Optimizer Name Function 
  </tr> 
 </thead> 
 <tbody> 
  <tr>   Set project priority Use this icon when you want to save the project order, based on their priority. 
  </tr> 
  <tr>   Optimize portfolio 
   <td>Use this icon to optimize the portfolio based on the following financial values of the projects:
    <ul>
     <li>Cost</li>
     <li>Alignment</li>
     <li>Value</li>
     <li>Risk to Benefit</li>
     <li>ROI</li>
    </ul><p>For more information about optimizing your portfolio, see the article <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Optimize projects in the Portfolio Optimizer </a> .</p></td> 
  </tr> 
  <tr>   Undo/ Redo icons Use these icons to cancel or redo the changes you made to the Portfolio Optimizer before saving. 
  </tr> 
  <tr>   Show/ Hide unchecked projects Use these icons to display or hide the projects in the portfolio that you have unchecked. 
  </tr> 
  <tr>   Export 
   <td> <p>Use this icon to export the data in the Project Prioritization area of the Portfolio Optimizer. You can export it to the following formats:</p> 
    <ul> 
     <li>PDF</li> 
     <li>Excel</li> 
     <li>Tab Delimited</li> 
    </ul> </td> 
  </tr> 
  <tr>   Preferences Use this icon to modify the project fields displayed in the columns of the Portfolio Optimizer, or to modify what projects you display in the Optimizer, based on their statuses. Tips: Not all Workfront standard fields are available to add in the columns. You can add only the custom fields that have a value other than zero in any of the projects in the portfolio. 
  </tr> <!--
   Full screen Use this icon to display the Portfolio Optimizer in full-screen mode, or to end the full-screen mode and return to the default view. Note: This view is not supported in the new Portfolio Optimizer.
  --> 
 </tbody> 
</table>

