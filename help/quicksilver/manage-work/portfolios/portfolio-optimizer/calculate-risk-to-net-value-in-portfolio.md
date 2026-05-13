---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calculate the Risk to Net Value in a portfolio
description: In the Portfolio Optimizer, the [!UICONTROL Risk to Net Value] indicator measures the Potential Risk taking into account the Net Value provided by all projects displayed in the Portfolio Optimizer.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
TQID: https://experienceleague.adobe.com/mClkaUv0y-Y9wiqg4oJivWYtmJDuKG701nOr5TU5rCA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
    internal-label: Requests
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---
# Calculate the [!UICONTROL Risk to Net Value] in a portfolio

In the [!UICONTROL Portfolio Optimizer], the [!UICONTROL Risk to Net Value] indicator measures the Potential Risk taking into account the [!UICONTROL Net Value] provided by all projects displayed in the [!UICONTROL Portfolio Optimizer]. 

For achieving the most efficiency within the portfolio, you want to see that the [!UICONTROL Risk] indicator is low and the [!UICONTROL Net Value] indicator is high. 

The [!UICONTROL Risk] and [!UICONTROL Net Value] indicators are represented from the perspective of how they relate to each other.

[!DNL Adobe Workfront] calculates the [!UICONTROL Risk] and [!UICONTROL Net Value] indicators using the following formulas:

* The [!UICONTROL Risk] indicator is calculated by the following formula:

   ```
   Risk indicator = Risk / (Risk + Net Value)
   ```

* The [!DNL Net Value] indicator is calculated by the following formulas:

   ```
   Net Value indicator = 1 - Risk / (Risk + Net Value)
   ```

   Or

   ```
   Net Value indicator = Net Value / (Risk + Net Value)
   ```

>[!NOTE]
>
>The [!UICONTROL Risk to Net Value] indicator calculates based on the projects that you display in the [!UICONTROL Portfolio Optimizer], and not on all the projects which are associated with the portfolio. 
