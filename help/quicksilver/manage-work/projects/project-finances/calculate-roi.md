---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculate Return On Investment (ROI)
description: Return On Investment (ROI) is Adobe Workfront metric that allows portfolio managers to quickly see how the project is performing against the original Planned Benefit and Budgeted Cost of the project.
author: Lisa
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
TQID: https://experienceleague.adobe.com/x7MGrAZbtlDd0oTePPgRdLQfUg8-M4GkkQdeWXUTyh4
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
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
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
  For more information about the Planned Benefit of a project, see the section "Project Info" in the article [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Project Budgeted Cost**: This is the total cost associated with the project as estimated when you first launch the project.

  The **Budgeted Cost** uses the **Budgeted Labor Cost** value which is calculated in the Resource Budgeting area of the Business Case and it takes into account the hours budgeted for your job roles in the Resource Planner and the Cost per Hour rate of each job role.   
  For more information, see [Calculate Budgeted Cost](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Locate the project Return on Investment (ROI)

You can view the ROI value for a project in the following areas in Workfront:

* In the Portfolio Optimizer if the project is associated with a portfolio

  >[!NOTE]
  >
  >The total of all project ROI values is the ROI of the portfolio.

  For information about the Portfolio Optimizer, see the article [Portfolio Optimizer overview](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).   

* In the Project ROI field in the following lists and reports: 

   * Project
   * Task
   * Issue
   * Project (Financial Data)

  For more information about building reports in Workfront, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
