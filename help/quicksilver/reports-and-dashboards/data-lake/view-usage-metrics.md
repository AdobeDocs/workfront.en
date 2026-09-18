---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: View Workfront Data Connect usage metrics
description: Using the Workfront Data Connect Metrics tab, you can view your organization's usage metrics according to both monthly compute hours used and number of queries performed.
author: Courtney
feature: Reports and Dashboards
exl-id: 29185bd1-e058-4b42-a508-53406fb9ddd2
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UKWAj3Tfm1GQXd-WGpluBgDIaVlxe0wls0G2UrfbgdI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# View [!DNL Workfront Data Connect] usage metrics

Using the [!DNL Workfront Data Connect] [!UICONTROL Metrics] tab, you can view your organization's usage metrics according to both compute hours used and number of queries performed. Organizations have a limited number of monthly compute hours available based on their license type and Data Connect add-on purchases. The [!UICONTROL Metrics] tab displays information on available monthly compute hours in relation to what has been used.

## Access requirements

+++ Expand to view access requirements. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## View usage metrics and available compute hours

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click [!UICONTROL **Setup**].

1. In the left panel, click [!UICONTROL **System**] > [!UICONTROL **Data Access**].

1. Click on the [!UICONTROL **Metrics**] tab. Your usage metrics are displayed in the **Compute Usage** graph, while the number of queries performed is displayed in the **Query Count** graph.

    ![Data Connect usage metrics](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. (Optional) You can use the [!UICONTROL **Select a view**] dropdown menu to change the time range for the information included in both graphs.

1. (Optional) You can use the checkboxes above the **Compute Usage** graph to show or hide:
    * [!UICONTROL **Daily Compute Hours**] - The number of compute hours used by your organization on a daily basis.
    * [!UICONTROL **Monthly Cumulative Compute Hours**] - The total number of compute hours used by your organization in a month. Resets to zero every month.
    * [!UICONTROL **Monthly Compute Hour Allowance**] - The number of compute hours available to your organization based on license and/or add-on purchases.
