---
filename: calculate-roi
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculate Return On Investment (ROI)
description: Return On Investment (ROI) is Adobe Workfront metric that allows portfolio managers to quickly see how the project is performing against the original Planned Benefit and Budgeted Cost of the project.
---

# Calculate Return On Investment (ROI)

Return On Investment (ROI) is Adobe Workfront metric that allows portfolio managers to quickly see how the project is performing against the original Planned Benefit and Budgeted Cost of the project.

## Overview of the project Return on Investment (ROI)

Workfront calculates ROI using the following formula:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

The following fields affect the ROI of a project:

* **Project Planned Benefit**: This is a manual entry specified by the Project Owner when completing the Project Info area of the Business Case. This is an estimation of what you, as the Project Owner, think that the benefit of the project might be if you complete the project. This is a specific amount of currency and it must be a positive value.  
  For more information about the Planned Benefit of a project, see the section "Project Info" in the article [Create a Business Case for a project in Adobe Workfront](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Project Budgeted Cost**:&nbsp;This is the total cost associated with the project as estimated when you first launch the project.

  The **Budgeted Cost**&nbsp;uses the&nbsp;**Budgeted Labor Cost**&nbsp;value which is calculated in the Resource Budgeting area of the Business Case and it takes into account the hours budgeted for your job roles in the Resource Planner and the Cost per Hour rate of each job role.   
  For more information, see [Calculate Budgeted Cost](../../../manage-work/projects/project-finances/budgeted-cost.md).

  <!--
  There are two different Budgeted Cost values depending on which Budgeted Labor Cost is used for their calculation:
  <ul> <!--
  <p>The <strong>Legacy Budgeted Cost</strong> uses the&nbsp;<strong>Legacy Budgeted Labor Cost</strong> value which&nbsp;is calculated in the Legacy Resource Estimates area of the Business Case and it takes into account the hours estimated for your job roles in the Capacity Planner and the Cost per Hour rate of each job role. <br>The Legacy Budgeted Cost affects the <strong>Legacy Net Value</strong> of the project.<br>For more information about how the Budgeted Cost is calculated, see the article <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calculate Budgeted Cost</a></p>
  <p>You might not have access to this functionality because it is supported by Flash, which has been deprecated in most environments.<br></p>
  -->
  </ul>
  -->

## Locate the project Return on Investment (ROI)

You can view the ROI value for a project in the following areas in Workfront:

* In the Portfolio Optimizer&nbsp;if the project is associated with a portfolio

  >[!NOTE]
  >
  >The total of all project ROI values is the ROI of the portfolio.

  For information about the Portfolio Optimizer, see the article [Portfolio Optimizer overview](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).   

* In the Project&nbsp;ROI field in the following lists and reports:&nbsp;

   * Project
   * Task
   * Issue
   * Project (Financial&nbsp;Data)

  For more information about building reports in Workfront, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

