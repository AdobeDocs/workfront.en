---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculate Potential Risk Cost
description: The Potential Risk Cost of a project takes into account the Potential Costs of the project risks and their probability of occurring.
author: Lisa
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
TQID: https://experienceleague.adobe.com/32kwPUhdtWhFeqQ34oReoU8xl2JlaWQeZlq7MI1jqtc
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
# Calculate Potential Risk Cost

The Potential Risk Cost of a project takes into account the Potential Costs of the project risks and their probability of occurring.

## Overview of Potential Risk Cost of a project

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
