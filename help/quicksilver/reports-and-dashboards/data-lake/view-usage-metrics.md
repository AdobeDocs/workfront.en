---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: View Workfront Data Connect usage metrics
description: Using the Workfront Data Connect Metrics tab, you can view your organization's usage metrics according to both monthly compute hours used and number of queries performed.
author: Nolan
feature: Reports and Dashboards
exl-id: 29185bd1-e058-4b42-a508-53406fb9ddd2
---
# View [!DNL Workfront Data Connect] usage metrics

Using the [!DNL Workfront Data Connect] [!UICONTROL Metrics] tab, you can view your organization's usage metrics according to both compute hours used and number of queries performed. Organizations have a limited number of monthly compute hours available based on their license type and Data Connect add-on purchases. The [!UICONTROL Metrics] tab displays information on available monthly compute hours in relation to what has been used.

## Access requirements

+++ Expand to view access requirements. 

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>Included in the following plans:</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>Workfront Data Connect is not available for legacy Workfront plans.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p></td> 
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
