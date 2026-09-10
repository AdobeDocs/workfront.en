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
TQID: https://experienceleague.adobe.com/EbnybXqWehstH2ziLqNZfMHtarMvUiugvWioYv9wLds
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Override job role billing rates at the company level

{{preview-fast-release-general}}

When a job role is created, you have the option to select an hourly billing rate for that role. You can create multiple hourly billing rates that are specific to a company. Each billing rate is effective for a specific date range.

At the project level, you can enable an option to allow company-level billing rates to override project-level rates. For more information, see [Override Project-Level Billing Rates with Company-Level Billing Rates](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>To add rate attributes to company-level billing rates: Workflow Ultimate</p>
       <p>To create company-level billing rates and edit all other rate settings: Any Workfront or Workflow package</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td> <p>Administrative access to Companies if you are not a System Administrator</p>
   <p>Edit access to Financial Data</p> </td>
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Override or change an established billing rate used for a specific job role

{{step-1-to-setup}}

1. Click **[!UICONTROL Companies]**.
1. Locate the company where the job role is assigned.
1. Click the company name in the list.
1. Click **[!UICONTROL Billing Rates]** in the left panel.
1. Click **[!UICONTROL Add Billing Rate] > [!UICONTROL New Billing Rate]**, or <span class="preview">**Add Billing Rate**</span>.
1. In the [!UICONTROL New Billing Rate] dialog, select a [!UICONTROL **Job Role**] to define the billing rate for.

### In the Production environment:

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
   >Job role rates changed on the project will only impact only that project. Rates changed at the company level will impact all projects. For more information, see [Overview of overriding billing rates and calculating revenue on a project](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

<div class="preview">   

### In the Preview environment:

1. Select attributes for the rate such as Agency, Location, or Cost Center.

   These attributes are defined separately and may affect revenue and cost calculations. For more information, see [Define rate attributes](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

   ![New Billing Rate dialog](assets/company-billing-rates-090326.png)

1. Select the **Currency** for the rate. The Workfront administrator adds the Base Currency in the Setup area. You can change the selection to another available currency, and you can change the currency on effective dated time ranges.

   >[!TIP]
   >
   >Only currencies available in the Exchange Rates area in your system are available in this field. If you only have one currency set up, only that currency is available.
   
   For information about setting up the Base Currency in Workfront, see [Set up exchange rates](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
   
   For information about changing the currency of a project, see [Change the project currency](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

1. In the [!DNL **Billing Rate**] field, enter the billing rate for the job role.

   This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the selected currency.

   If you use attributes, the attributes and the job role combine to define a unique rate. For example, a Designer role in New York for Agency A can have a separate rate from a Designer role in Paris for Agency B.

   For date effective billing rates, click **Add date effective rate**. Enter the hourly billing rate for the time period, and assign a Start Date and End Date as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.

   Workfront allows you to leave gaps between date ranges, but you will receive a warning to confirm this is intentional.

   For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

   >[!TIP]
   >
   >When editing an existing rate, you can sort the list to see the most recent start date at the top of the rate list.

1. Click [!UICONTROL **Save**].

   >[!NOTE]
   >
   >Job role rates changed on the project will only impact only that project. Rates changed at the company level will impact all projects that have the company assigned. For more information, see [Overview of overriding billing rates and calculating revenue on a project](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

</div>

