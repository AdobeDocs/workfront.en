---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Enable Custom Quarters
description: For reporting purposes, you might want to create custom quarters if your organization's quarters are based on specific criteria other than calendar dates (such as business days or shopping days).
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
---
# Enable custom quarters 

<!--Audited: 11/2024-->

For reporting purposes, you might want to create custom quarters if your organization's quarters are based on specific criteria other than calendar dates (such as business days or shopping days).

Depending on what products your company has purchased, you can configure the following number of quarters in your Workfront Setup area: 

* Customers who purchased [!DNL Workfront] only, can configure up to eight custom quarters for their [!DNL Adobe Workfront] system.
* Customers who purchased [!DNL Workfront] and [!DNL Workfront Planning], can configure up to 100 quarters for their [!DNL Workfront] system which are also available in [!DNL Planning]. 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Set up custom quarters for your [!DNL Workfront] system

{{step-1-to-setup}}

1. Click **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects].**

1. In the **[!UICONTROL Timelines]** section, select **[!UICONTROL Enable Custom Quarters]**.

1. Type a name for the custom quarter, such as "Fiscal Q1 2021."
1. Select start and end dates for the custom quarter.

   ![Custom quarters](assets/custom-quarters-nwe.png)

1. (Optional) Click **[!UICONTROL Add Custom Quarter]** to add additional custom quarters to the system.

      >[!IMPORTANT]
      >
      > If your company purchased [!DNL Workfront Planning], you cannot save your custom quarters if there are gaps or overlaps between the quarters. 
      >![Custom quarters with overlap warning](assets/custom-quarters-with-overlap-warning.png)
      >Gaps and overlaps between the quarters are allowed for [!DNL Workfront] only customers. 

1. (Optional and conditional) If your company purchased only [!DNL Workfront], without [!DNL Workfront Planning], create a reporting element that refers to the fiscal quarters.


   **Example:** Create a filter for a [!UICONTROL project] list and include the Planned Completion Date of a project referencing the custom quarters.

   ![Project filter with custom quarters](assets/example-of-project-filter-with-custom-quarters.png)

   The references to "This Quarter", "Next Quarter", and "Last Quarter" are replaced with new references to the custom quarters.

   For information about reporting elements, see [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   For information about creating filters, see [Create or edit filters in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Optional and conditional) If you have access to [!DNL Workfront Planning], go to a record type page and open a timeline view. The view displays the new custom quarters. 
For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md). 
