---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculate Potential Risk Cost
description: The Potential Risk Cost of a project takes into account the Potential Costs of the project risks and their probability of occurring.
author: Lisa
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
---
# Calculate Potential Risk Cost

The Potential Risk Cost of a project takes into account the Potential Costs of the project risks and their probability of occurring.

## Overview of Potential Risk&nbsp;Cost of a project

Adobe Workfront calculates the Potential Risk Cost of a project using the following formula:

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

Consider the following when reviewing the Potential Risk Cost of a project:

* The Planned Risk Cost of a project is identical to the Potential Risk Cost.
* The Potential Risk Cost is not incorporated into the Planned Cost of a project. It is instead used to determine its Net Value.

## Locate the Potential Risk Cost of a project

You can find the Risks for a project and their Potential Cost in the following areas in Workfront:

* In the Risks tab of the project.
* In the Business Case Summary.  
  For more information about the Business Case of a project, see the article [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* In a project report when you add the Planned Risk Cost field to the columns of the report.  
  For more information about building reports in Workfront, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* In the Portfolio Optimizer, when the project is associated with a Portfolio, in the Risk column.  
  The sum of all Potential Risk Costs of all projects in the portfolio adds up to the Risk of the Portfolio.  
  For more information about the Portfolio Optimizer, see the article [Portfolio Optimizer overview](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

For more information about creating Risks on a project, see the article [Create and edit risks on projects](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

For more information about the Business Case of a project, see the article [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md).
