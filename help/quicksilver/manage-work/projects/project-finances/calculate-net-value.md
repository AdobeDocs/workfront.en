---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculate Net Value
description: The Net Value of a project is the total expected value of the project after calculating its benefit and removing the costs.
author: Lisa
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
---
# Calculate Net Value

The Net Value of a project is the total expected value of the project after calculating its benefit and removing the costs.

## Overview of the project Net Value

Adobe Workfront calculates the Net Value of a project using the following formula:

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

The following fields can affect the Net Value of a project:

* **Planned Benefit**: This is a manual entry specified by the Project Owner when completing the **Project Info** area of the Business Case.  
  For more information about the Planned Benefit of a project, see the [Project Info](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) section in article [Overview of the Areas of the Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md). 

* **Budgeted Cost**:&nbsp;This is the total cost associated with the project as estimated when you first launch the project.

  The **Budgeted Cost**&nbsp;uses the&nbsp;**Budgeted Labor Cost**&nbsp;value which is calculated in the Resource Budgeting area of the Business Case and it takes into account the hours budgeted for your job roles in the Resource Planner and the Cost per Hour rate of each job role.   
  The Budgeted Cost affects the **Net Value** of the project.&nbsp;For more information about how the Budgeted Cost is calculated, see [Calculate Budgeted Cost](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Potential Risk Cost**: This is the cost associated with any risks on the project, as they are defined in the Business Case, or the Risks tab of the project.  
  For more information about calculating the Potential Risk Cost of a project, see the article [Calculate Potential Risk Cost](../../../manage-work/projects/project-finances/potential-risk-cost.md).

  &nbsp;

## Locate the project Net Value

You can find the Net Value for a project in the following areas in Workfront:

* In Business Case Summary area of the Business Case&nbsp;  
  For more information about the Business Case Summary area, see the "Understanding the Business Case Summary" section in&nbsp;the article [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

  ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* In the Portfolio Optimizer&nbsp;if the project is associated with a portfolio

  >[!TIP]
  >
  >The total of all project Net Values is the Net Value of the portfolio.

  For more information about the Portfolio Optimizer, see [Portfolio Optimizer overview](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* In the Project Net&nbsp;Value field of the following lists and reports:

   * Project
   * Task
   * Issue
   * Project (Financial Data)

  For more information about creating a report, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
