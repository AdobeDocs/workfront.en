---
content-type: overview
product-area: portfolios
navigation-topic: portfolios-overview
title: Understand Portfolio Methodology
description: A Portfolio is a collection of projects that have unifying characteristics. Those projects usually compete for the same resources, budget, or time slot. You can divide Portfolios into Programs and associate the projects with the Programs before they are added to a Portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: b340501e-1190-415e-aa96-5aad177c4b7b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/mLs5mZiSsS-ApmxUkD08wiBUmMV5VKtoUB0u23gCeRA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Understand portfolio methodology

<!-- Audited: 1/2024 -->

Portfolio or Project Portfolio Management (PPM) is the process of prioritizing and managing a list of projects in order to achieve specific business objectives. 

For general information about PPM, see [Portfolio Management overview](/help/quicksilver/manage-work/portfolios/portfolios-overview/portfolio-managament-overview.md). 

In Adobe Workfront, a portfolio is a collection of projects that have unifying characteristics. Those projects usually compete for the same resources, budget, or time slot. You can divide Portfolios into Programs and associate the projects with the Programs before they are added to a Portfolio.

You can use Portfolios and Programs to organize projects. Through organizing projects, you can compare similar projects and determine where resources will be best spent.

For information about using Programs, see [Create a program](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

This article contains general information about portfolios in Workfront.

## Access needed to create portfolios

<!--leave the table uncollapsed as this article is about access-->

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] packages</td> 
   <td> <p>Workfront Prime or higher</p>
   <p>Workflow Prime or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>After you create a portfolio, you have Manage permissions to it, by default</p> 
   <p>Manage permissions to edit a portfolio or add projects to it</p>
   <p>View permissions to a portfolio to view it in Workfront</p>
    </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>New: Any</p>
   <p>Current:[!UICONTROL Business] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard]</p>
   <p>Current:[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>After you create a portfolio, you have Manage permissions to it, by default</p> 
   <p>Manage permissions to edit a portfolio or add projects to it</p>
   <p>View permissions to a portfolio to view it in Workfront</p>
    </td> 
  </tr> 
 </tbody> 
</table>
-->

## Understand the [!DNL Adobe Workfront] portfolio methodology

In [!DNL Workfront], you can add projects to portfolios to create and organize your portfolios.

We recommend that you follow these steps for an efficient organization of your portfolios:

1. Create a Business Case for a project and associate the project with a Portfolio.

    To create efficient portfolios that bring value to your organization, you must start with a Project Request where you define the Business Case for each project which is later added to the portfolio.

    The [!UICONTROL Business Case] contains the following information:

     * General information about the project (description, Portfolio and Program assignments, Project Owner and Sponsor)
     * The goals or objectives of the project
     * Estimated expense costs
     * Resource budgets for labor costs
     * An alignment score
     * A risk assessment

    For more information about the [!UICONTROL Business Case], see [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

    You can associate the project with a portfolio while  building its business case. You must create a portfolio before you can associate it with a project. For information, see [Create a portfolio](/help/quicksilver/manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)

    The details you collect during building a business case are used in the [!UICONTROL portfolio optimizer] and the [!UICONTROL resource planner] to assist management in project selection.
1. Associate Resource Pools with projects as you build their Business Case.

    Portfolios are usually configured to correspond with Resource Pools. The Programs in a Portfolio also align with a Resource Pool. This correlation helps to ensure all resource planning fits within the purpose of the Portfolio, as the projects within the same Portfolio usually compete for the same resources.

    For more information, see [Create resource pools](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/create-resource-pools.md). 

1. Get the [!UICONTROL Business Case] approved by your Portfolio Manager.

    For information, see [Approve a Business Case](/help/quicksilver/manage-work/projects/define-a-business-case/approve-business-case.md). 
1. Manage the performance of your projects within the portfolio in the [!UICONTROL Portfolio Optimizer].

    Portfolio Managers can track financial performance inside the portfolio using the Portfolio dashboard. This dashboard is displayed in the header of the Portfolio.

    For information about the financial fields of a Portfolio, see the [Understanding the Financial Fields in the Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md#financial-fieds-subsection) section in [Portfolio Optimizer overview](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).
