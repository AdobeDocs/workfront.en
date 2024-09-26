---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Override Job Role Billing Rates at the Company Level
description: When a job role is created, you have the option to select an hourly billing rate for that role. You can create an hourly billing rate that is specific to a company.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
---
# Override job role billing rates at the company level

When a job role is created, you have the option to select an hourly billing rate for that role. You can create multiple hourly billing rates that are specific to a company. Each billing rate is effective for a specific date range.

At the project level, you can enable an option to allow company-level billing rates to override project-level rates. For more information, see [Override Project-Level Billing Rates with Company-Level Billing Rates](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>New: [!UICONTROL Standard]</p>
   <p>Or</p>
   <p>Current: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Administrative access to Companies if you are not a System Administrator</p>
   <p>Edit access to Financial Data</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Override or change an established billing rate used for a specific job role

{{step-1-to-setup}}

1. Click **[!UICONTROL Companies]**.
1. Locate the company where the job role is assigned.
1. Click the company name in the list.
1. Click **[!UICONTROL Billing Rates]** in the left panel.
1. Click **[!UICONTROL Add Billing Rate] > [!UICONTROL New Billing Rate]**, or choose an existing rate to edit.
1. In the [!UICONTROL New Billing Rate] dialog, select a [!UICONTROL **Job Role**] to define the billing rate for.

   The [!UICONTROL **Default Billing Rate**] displays the system-level rate for this job role.

   ![New Billing Rate dialog](assets/date-effective-billing-rates-for-company.png)

1. In the [!DNL **Billing Rates 1**] field, enter the billing rate. Then, click [!UICONTROL **Save**] to override the billing rate one time.

   Or

   Click [!UICONTROL **Add Rate**] to add more billing rates with effective dates.

1. (Conditional) If you are adding more than one billing rate, enter the following information:

   * **[!UICONTROL Billing Rates 1], 2, etc.**: The value of the billing rate for the time period.
   * **[!UICONTROL Start Date]**: The date when the rate becomes effective.
   * **[!UICONTROL End Date]**: The date when the rate ends.

     Billing Rate 1 will not have a start date and the last billing rate will not have an end date. Some dates are added automatically. For example, if Billing Rate 1 does not have an end date, and you add Billing Rate 2 with a start date of May 1, 2023, an end date of April 30, 2023 is added to Billing Rate 1 so that no gaps exist.

1. Click [!UICONTROL **Save**].

   >[!NOTE]
   >
   >Job role rates changed on the project will only impact only that project. Rates changed at the company level will impact all projects. For more information, see [Overview of overriding Job Role Billing Rates and calculating Revenue on a project](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
