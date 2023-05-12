---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Override job role billing rates at the company level
description: When a job role is created, you have the option to select an hourly billing rate for that role. You can create an hourly billing rate that is specific to a company.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
---
# Override job role billing rates at the company level

When a job role is created, you have the option to select an hourly billing rate for that role. You can create an hourly billing rate that is specific to a company.

At the project level, you can enable an option to allow company-level billing rates to override project-level rates. For more information, see [Override Project-Level Billing Rates with Company-Level Billing Rates](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to Companies if you are not a System Administrator</p> <p>[!UICONTROL Edit] access to Financial Data</p> <p><b>NOTE</b>: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Override or change an established billing rate used for a specific job role

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe] Workfront, then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Click **[!UICONTROL Companies]**.
1. Locate the company where the job role is assigned.
1. Click **[!UICONTROL Edit Company]** in the upper-right corner.
1. In the **[!UICONTROL Billing Rates]** section, select the job role you want to edit, and enter the new billing rate for that job role in the **[!UICONTROL Company Billing Rate]** box.

   >[!NOTE]
   >
   >Job role rates changed on the project will only impact only that project. Rates changed at the company level will impact all projects. For more information, see [Overview of overriding Job Role Billing Rates and calculating Revenue on a project](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
