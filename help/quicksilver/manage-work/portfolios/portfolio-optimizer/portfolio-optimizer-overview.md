---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Portfolio Optimizer overview
description: The [!UICONTROL Portfolio Optimizer] is the tool used for project evaluation and comparison. The process of reviewing and comparing Business Case values for projects assigned to a portfolio is how a portfolio manager can prioritize projects and generate the most value for an organization.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
---
# [!UICONTROL Portfolio Optimizer] overview

The [!UICONTROL Portfolio Optimizer] is the tool used for project evaluation and comparison. The process of reviewing and comparing [!UICONTROL Business Case] values for projects assigned to a portfolio is how a portfolio manager can prioritize projects and generate the most value for an organization.

![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

The purpose of the [!UICONTROL portfolio optimizer] is to provide an interface through which a portfolio manager, steering committee, or product management office can view summary information about the business case of each project. Projects can then be prioritized according to strategic values and goals, or according to their overall score.

The [!UICONTROL Portfolio Optimizer] can only assist you if you have completed the following prerequisites:

* The [!UICONTROL Business Cases] have been completed on the projects. For information, see the articles in [Define a Business Case: article index](../../projects/define-a-business-case/define-business-case.md).
* A portfolio is defined in the Project Overview area of Project Details section for the projects you want to review.
* You have indicated the Project Budget and Planned Benefit for the projects you want to review. Fixed Cost and Fixed Revenue are optional but add additional value. For information, see [Project finances fields](../../projects/project-finances/project-finances-overview-1.md).

For information about locating the [!UICONTROL Portfolio Optimizer], see [Locate the [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finances in the [!UICONTROL Portfolio Optimizer]

* [The financial areas in the [!UICONTROL Portfolio Optimizer]](#the-financial-areas-in-the-portfolio-optimizer)
* [The financial fields in the [!UICONTROL Portfolio Optimizer]](#the-financial-fields-in-the-portfolio-optimizer)

You can see the financial state of your portfolio at any time during the life of your projects when using the [!UICONTROL Portfolio Optimizer].

Consider the following when working with finances in the [!UICONTROL Portfolio Optimizer]:

* Projects are each given a score when their [!UICONTROL Business Cases] are completed according to what criteria they match in the [!UICONTROL Portfolio Optimizer]. For example, low cost or high alignment projects receive a higher score.

   For more information about calculating the portfolio optimizer score of a project, see the article [Overview of the [!UICONTROL Portfolio Optimizer] Score](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* The financial calculations for the [!UICONTROL Portfolio Optimizer] use the [!UICONTROL Budgeted Cost] in the [!UICONTROL Business Case] of the project.
* You can manually prioritize your projects in the [!UICONTROL Portfolio Optimizer], taking into account all the information about them. This includes financial data, alignment to their scorecards, ROI, for example.

### The financial areas in the [!UICONTROL Portfolio Optimizer] {#the-financial-areas-in-the-portfolio-optimizer}

You can view financial information in the following areas of the [!UICONTROL Portfolio Optimizer]:

* **[!UICONTROL Portfolio Header]**: This area displays financial information gathered from all the projects in the portfolio. It displays on every tab of the Portfolio object.
* **[!UICONTROL Portfolio Finances for Selected Projects]**: This area displays financial information gathered from the projects which are selected in the [!UICONTROL Portfolio Optimizer]. You can add or remove projects and understand how this will affect the finances of the portfolio by viewing the information in this area.
* **[!UICONTROL Projects Finances]**: This area displays the financial information of each project listed in the [!UICONTROL Portfolio Optimizer].

### The financial fields in the [!UICONTROL Portfolio Optimizer]  {#the-financial-fields-in-the-portfolio-optimizer}

The following financial fields display in the [!UICONTROL Portfolio Optimizer]:

* [Portfolio header](#portfolio-header)
* [Portfolio finances for selected projects](#portfolio-finances-for-selected-projects)

#### Portfolio header {#portfolio-header}

![](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] calculates the financial fields in the portfolio header using information from projects with statuses that equate only with [!UICONTROL Approved] or [!UICONTROL Current].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Name of Field</strong> </th> 
   <th><strong>Description</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL On Time]</td> 
   <td> <p>The percentage of projects in the portfolio which are considered to be [!UICONTROL On Time]. This is visible from any tab inside a Portfolio.</p> <p>A project is considered to be [!UICONTROL On Time] when the Project <strong>[!UICONTROL Condition]</strong> is <strong>[!UICONTROL On Target]</strong>. <br>For more information about [!UICONTROL Project Conditions], see the article <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Overview of Project Condition and Condition Type</a>.</p> <p>The <strong>[!UICONTROL On Time]</strong> percentage is calculated by using the following formula:</p> <p><em>[!UICONTROL On Time Portfolio Percentage] = Number of [!UICONTROL On Time] Projects/ Total Number of Projects in a [!UICONTROL Current] or [!UICONTROL Approved] status</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL On Budget]</td> 
   <td> <p>The percentage of projects in the portfolio which are considered to be [!UICONTROL On Budget]. This is visible from any tab inside a [!UICONTROL Portfolio].</p> <p>Projects are <strong>[!UICONTROL On Budget]</strong> when they have not exceeded their pre-defined budget. <br>For more information about the budget of a project, see the article <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">[!UICONTROL Manage] information in the project Finance area</a>.</p> <p>The [!UICONTROL On Budget] percentage is calculated by using the following formula:</p> <p><em>[!UICONTROL On Budget Portfolio Percentage] = Number of [!UICONTROL On Budget] Projects/ Total Number of Projects </em><em>in a [!UICONTROL Current] or [!UICONTROL Approved] status</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (for portfolio)</td> 
   <td> <p>The [!UICONTROL Return on Investment] (ROI) for the portfolio is calculated by taking into account the total [!UICONTROL Benefit] of the [!UICONTROL Portfolio] and the total of the [!UICONTROL Budgeted Costs] of the projects. This is visible from any tab inside a Portfolio.</p> <p>The Portfolio ROI value is calculated by using the following formula:</p> <p><em>Portfolio ROI = ([!UICONTROL Total Benefit] - [!UICONTROL Total Budgeted Cost])/ [!UICONTROL Total Cost] * 100</em> </p> <p>For more information about how the ROI is calculated for a project, see the article <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Calculate Return On Investment (ROI)</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aligned] or [!UICONTROL Alignment Score] </td> 
   <td> <p>An average of all the [!UICONTROL Project Alignment Score] values which are calculated after completing the [!UICONTROL Scorecard] in the [!UICONTROL Business Case] of the project. The alignment score of each project is listed in the [!UICONTROL Alignment] column of the [!UICONTROL Portfolio Optimizer]. This is visible from any tab inside a portfolio.</p> <p>For more information about generating an alignment score for a project, see the article <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Apply a scorecard to a project and generate an Alignment Score</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Net Value]</td> 
   <td> <p>The sum of all the [!UICONTROL Net Values] of all the projects in the portfolio. This is visible from any tab inside a portfolio.</p> <p>For more information about how [!UICONTROL Net Value] is calculated for a project, see the article <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calculate Net Value</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Portfolio finances for selected projects {#portfolio-finances-for-selected-projects}

![](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Name of Field</strong> </th> 
   <th> <p><strong>Description</strong> </p> <p> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Number of projects]</td> 
   <td> <p>The total number of active projects in the portfolio. Projects that are considered active in a portfolio can be in any of the following statuses:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL Planning]</li> 
     <li>[!UICONTROL Approved]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget]</td> 
   <td>You can manually update this field to indicate what is the total budget for the entire portfolio. This budget is used for all the projects inside the portfolio. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Remaining]</td> 
   <td> <p>The remaining budget after all the [!UICONTROL Budgeted Costs] on all the projects inside the portfolio have been subtracted from the Budget of the portfolio.</p> <p>The [!UICONTROL Remaining Portfolio Budget] is calculated using the following formula:</p> <p><em>[!UICONTROL Remaining Portfolio Budget] = [!UICONTROL Total Portfolio Budget] - Total [!UICONTROL Budgeted Cost] of All Portfolio Projects</em> </p> <p>The overall [!UICONTROL Budgeted Cost] of all the projects in the portfolio is represented in the indicator bar under the Budget field. </p> <p>For more information about tracking costs on a project, see the article<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Cost]</td> 
   <td> <p>The sum of the costs of all the projects displayed in the [!UICONTROL Portfolio Optimizer]. The cost of each project is the same as the [!UICONTROL Budgeted Cost] of the Project as it is displayed in the [!UICONTROL Business Case Summary]. </p> <p>For more information about the financial fields of projects in the [!UICONTROL Business Case], see the section "Understanding Financial Fields in the Business Case" in the article <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Create a Business Case for a project </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risk] </td> 
   <td> <p>The sum of all the [!UICONTROL Potential Risk Costs] of all the projects in the portfolio. The [!UICONTROL Potential Risk Cost] of each project is listed in the [!UICONTROL Risk] column of the [!UICONTROL Portfolio Optimizer]. </p> <p>For more information about calculating risks for projects, see the article <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calculate Potential Risk Cost </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benefit]</td> 
   <td> <p>The sum of all the [!UICONTROL Planned Benefit] values of all the projects in the portfolio. The Planned Benefit value of each project is listed in the [!UICONTROL Benefit] column of the [!UICONTROL Portfolio Optimizer]. </p> <p>For more information about the [!UICONTROL Planned Benefit] of a project, see the article <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Overview of project Planned Benefit</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risk to Net Value] indicator</td> 
   <td> <p>Measures the [!UICONTROL Potential Risk] value taking into account the [!UICONTROL Net Value] provided by all projects in the portfolio. For achieving the most efficiency within the portfolio, you want to see that the [!UICONTROL Risk] indicator is low and the [!UICONTROL Net Value] indicator is high. </p> <p>For more information about calculating Risk to [!UICONTROL Net Value], see the article <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Calculate the Risk to Net Value in a portfolio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Customize the [!UICONTROL Portfolio Optimizer]

You can customize only the project list area of the [!UICONTROL Portfolio Optimizer] by using settings to change the information in the list.

The following icons and options are available for the [!UICONTROL Portfolio Optimizer]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Icon in the Portfolio Optimizer</td> 
   <td>Name</td> 
   <td>Function</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Set project priority]</td> 
   <td>Use this icon when you want to save the project order, based on their priority. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL Optimize portfolio]</td> 
   <td>Use this icon to optimize the portfolio based on the following financial values of the projects:
    <ul>
     <li>[!UICONTROL Cost]</li>
     <li>[!UICONTROL Alignment]</li>
     <li>[!UICONTROL Value]</li>
     <li>[!UICONTROL Risk to Benefit]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>For more information about optimizing your portfolio, see the article <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Optimize projects in the [!UICONTROL Portfolio Optimizer] </a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>[!UICONTROL Undo]/ [!UICONTROL Redo] icons</td> 
   <td>Use these icons to cancel or redo the changes you made to the [!UICONTROL Portfolio Optimizer] before saving.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL Show]/ [!UICONTROL Hide unchecked] projects</td> 
   <td>Use these icons to display or hide the projects in the portfolio that you have unchecked.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Export] </td> 
   <td> <p>Use this icon to export the data in the [!UICONTROL Project Prioritization] area of the [!UICONTROL Portfolio Optimizer]. You can export it to the following formats:</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL Tab] Delimited</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL Preferences]</td> 
   <td> <p>Use this icon to modify the project fields displayed in the columns of the [!UICONTROL Portfolio Optimizer], or to modify what projects you display in the [!UICONTROL Optimizer], based on their statuses. </p> <p>Tip:  
     <ul> 
      <li> <p>Not all [!DNL Workfront] standard fields are available to add in the columns. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>You can add only the custom fields that have a value other than zero in any of the projects in the portfolio.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
