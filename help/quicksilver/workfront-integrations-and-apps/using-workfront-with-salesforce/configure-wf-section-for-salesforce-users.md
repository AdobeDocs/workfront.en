---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Configure the [!DNL Adobe Workfront] section for [!DNL Salesforce] users
description: After you install [!DNL Adobe Workfront] for Salesforce as a [!DNL Workfront] administrator, you can make it available to your users by adding it in a new section to their Opportunity and Account page layouts in Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
---
# Configure the [!DNL Adobe Workfront] section for [!DNL Salesforce] users

A [!UICONTROL Pro] [!DNL Workfront] Plan is required to use this feature. For more information about the various plans available, see [[!DNL Workfront] Plans.](https://www.workfront.com/plans)

After you install [!DNL Adobe Workfront] for [!DNL Salesforce] as a [!DNL Workfront] administrator, you can make it available to your users by adding it in a new section to their [!UICONTROL Opportunity] and [!UICONTROL Account]
 page layouts in [!UICONTROL Salesforce]. 

For information about installing [!DNL Workfront for Salesforce], see [Install [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

For users to have [!DNL Workfront] available in both the [!DNL Classic] and [!DNL Lightning Experience] frameworks, you must add the [!DNL WorkfrontOpportunities] and the [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] pages to the [!UICONTROL Opportunity] and [!UICONTROL Accounts] page layouts, respectively.

## Access requirements

You must have the following access to use the functionality described in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Prerequisites

* You must have a [!DNL Salesforce] instance with access to a system administrator account.
* You must have a [!DNL Workfront] instance with access to a system administrator account.

## Configure the [!DNL Workfront] section in the [!DNL Salesforce Classic] framework

1. Log in to [!DNL Salesforce] as a Workfront administrator.
1. Click **[!UICONTROL Setup].**
1. In the **[!UICONTROL Build]** section, expand **[!UICONTROL Customize].**

1. Expand **[!UICONTROL Opportunities]**, then click **[!UICONTROL Page Layouts]** to add the [!DNL Workfront] section to an Opportunity.

   Or

   Expand **[!UICONTROL Accounts]**, then click **[!UICONTROL Page Layouts]** to add the [!DNL Workfront] section to an Account
.

1. Click **[!UICONTROL Edit]** on an existing layout.

   Or

   Click **[!UICONTROL New]** to add a new layout. 

1. (Optional) Drag the **[!UICONTROL Section]** component to the layout and drop it in the desired position.\
   ![salesforce_new_section_properties.png](assets/salesforce-new-section-properties-350x210.png)

1. (Optional) Specify a name for the new section.

   We recommend that you name this section **[!DNL Workfront]**.

1. (Optional) Specify the desired **[!UICONTROL Layout]** and **[!UICONTROL Tab-key Order]** for the new section.

   We recommend that you select **[!UICONTROL 1-Column]** layout for the [!DNL Workfront] section. 

1. Click **[!UICONTROL OK]**.
1. In the **[!UICONTROL Layout]** area, click **[!UICONTROL Visualforce Pages].**

1. Drag and drop the **[!UICONTROL WorfrontOpportunities]** component to the new section in the **[!UICONTROL Opportunities]** Layout.

   Or

   Drag and drop the **[!UICONTROL WorkfrontAccounts]** component to the new section in the  **[!UICONTROL Account]** Layout.\
   ![[!DNL WorkfrontAccounts_component].png](assets/workfrontaccounts-component-350x139.png)

1. Click the **[!UICONTROL Properties]** icon in the upper right of the newly added component.\
   ![](assets/salesforce-visualforce-page-properties-350x174.png)

1. To achieve an optimal display, specify the following properties for the [!DNL Workfront Visualforce] page:

   * **[!UICONTROL Width (in pixels or %)]**: 100%
   * **[!UICONTROL Height (in pixels)]**: 600
   * Select **[!UICONTROL Show scrollbars]**.

1. Click **[!UICONTROL OK]**. 
1. Click **[!UICONTROL Save]** to save your layout.

   All users who have this layout assigned to them are now able to see the [!DNL Workfront] section on their [!UICONTROL Opportunities] or [!UICONTROL Accounts] objects.

   Users see a [!DNL Workfront] login screen on the [!DNL Workfront] section. If they do not have a [!DNL Workfront] account, they can collapse the section, but not remove it from their layout. 

   ![[!DNL salesforce_classic_opportunity_with_workfront_panel].png](assets/salesforce-classic-opportunity-with-workfront-panel-350x161.png)

## Configure the [!DNL Workfront] section in the [!DNL Salesforce Lightning Experience] framework

You can add the [!DNL Workfront] section to the layout of a [!DNL Salesforce] [!UICONTROL Opportunity] or Account
 in the [!DNL Salesforce Lightning Experience] framework either by accessing the [!UICONTROL Setup] area, or from an Account
 or [!UICONTROL Opportunity] object. 

* [Configure the [!DNL Workfront] section at the [!UICONTROL Setup] level](#configure-the-dnl-workfront-section-at-the-uicontrol-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configure the [!DNL Workfront] Section at the Opportunity or Account level](#configure-the-dnl-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configure the [!DNL Workfront] section at the [!UICONTROL Setup] level {#configure-the-workfront-section-at-the-setup-level}

1. Log into [!DNL Salesforce] as a system administrator. 
1. Click the **[!UICONTROL Setup]** icon, then click **[!UICONTROL Setup]**.

1. Expand **[!UICONTROL Object and Fields]**, then click **[!UICONTROL Object Manager]**.

1. Click **[!UICONTROL Opportunity]** to customize the layout of an Opportunity.

   Or

   Click **[!UICONTROL Account]** to customize the layout of an Account.

1. Click **[!UICONTROL Page Layouts]**.
1. Click the name of an existing page layout to edit it.

   Or

   Click **[!UICONTROL New]** to create a new page layout.

1. Continue with [Configure the [!DNL Workfront] Section at the Opportunity or Account level](#configure-the-dnl-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) below.

### Configure the [!DNL Workfront] Section at the Opportunity or Account level {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Log in to [!DNL Salesforce] as a system administrator. 
1. Go to an **[!UICONTROL Opportunity]** or **[!UICONTROL Account]**.

1. Click the **[!UICONTROL Setup]** icon, then click **[!UICONTROL Edit Page]**.\
   ![salesforce_lightning_opportunity_edit_area.png](assets/salesforce-lightning-opportunity-edit-area-350x116.png)

1. Expand the **[!UICONTROL Custom-Managed]** section.
1. Drag and drop the **[!DNL Workfront]** component on your [!UICONTROL Opportunity] or Account
 page.

   We recommend using the full width of the page for the [!DNL Workfront] section instead of one of the columns of the layout.

   ![[!DNL salesforce_lightning_builder].png](assets/salesforce-lightning-builder-350x229.png)

1. Click **[!UICONTROL Save]**.

   All users who have this layout assigned to them are now able to see the [!DNL Workfront] section on their [!UICONTROL Opportunities] or [!UICONTROL Accounts] objects.

   >[!NOTE]
   >
   >Users see a [!DNL Workfront] login screen on the [!DNL Workfront] section. If they do not have a [!DNL Workfront] account, they can collapse the section, but not remove it from their layout. Users can log in using the authentication method you have enabled: Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.

   ![[!DNL salesforce_lightning__workfront_panel].png](assets/salesforce-lightning--workfront-panel-350x127.png)
