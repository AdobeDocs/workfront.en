---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Install [!DNL Adobe Workfront] for [!DNL Salesforce]
description: To install the app before it becomes available in the [!DNL Salesforce] AppExchange, see Installing [!DNL Workfront] for Salesforce before It Becomes Available in the AppExchange Marketplace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
---
# Install [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>To install the app before it becomes available in the [!DNL Salesforce AppExchange], see [Installing [!DNL Workfront for Salesforce] before It Becomes Available in the [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

As a [!DNL Salesforce] and [!DNL Adobe Workfront] administrator, you can install [!DNL Workfront for Salesforce] to allow your [!DNL Salesforce] users to submit [!DNL Workfront] requests and automatically create projects without ever leaving Salesforce.

For a general understanding about what you can expect by installing [!DNL Workfront for Salesforce], see [[!DNL Adobe Workfront for Salesforce] overview](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Prerequisites for Installing and Using [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Installing [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to use the functionality described in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: [!UICONTROL Standard]</p><p>Or</p><p>Current: [!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites for Installing and Using [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* You must have a [!DNL Salesforce] instance with access to a system administrator account in order to install the app.
* You must have a [!DNL Workfront] instance with access to a system administrator account in order to configure the integration.
* [!UICONTROL Salesforce] users must have a [!DNL Workfront] account in order to be able to:

    * Create [!DNL Workfront] requests from [!DNL Salesforce]
    * View [!DNL Workfront] requests or projects in Salesforce

## Installing [!DNL Workfront for Salesforce]  {#installing-workfront-for-salesforce}

You must be a [!DNL Salesforce] and a [!DNL Workfront] system administrator to install and configure [!DNL Workfront for Salesforce]. 

The following subsections describe how to install [!DNL Workfront] for your [!DNL Salesforce] Production environment. You can follow the same steps to install [!DNL Workfront] for your [!DNL Salesforce] Sandbox environment.

* [Installing [!DNL Workfront for Salesforce] before It Becomes Available in the [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Installing [!DNL Workfront for Salesforce] in the [!DNL Salesforce Classic] Framework](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Installing [!DNL Workfront for Salesforce] in the [!DNL Salesforce Lightning Experience] Framework](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Installing [!DNL Workfront for Salesforce] before It Becomes Available in the [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] will be available in the [!DNL Salesforce AppExchange] soon.

To install the app before it's available:

1. In your Production environment, go to

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   In your Sandbox environment, go to

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   >[!NOTE]
   >
   >You must be logged into Salesforce to access these pages.

1. Check the **[!UICONTROL Yes, grant access to these third-party web sites]** box.

   A loading screen displays. The installation may take some time.

1. Click **[!UICONTROL Done]** when the installation completes.

1. Navigate to **[!UICONTROL Setup]** > **[!UICONTROL Security] Controls** > **[!UICONTROL Remote Site Settings]**.
1. (Conditional) Select Workfront from the list.
    
    Or
    
    If you do not see your [!DNL Workfront] URL listed in the **[!UICONTROL All Remote Sites]** list, click **[!UICONTROL New Remote Site]**.

1. (Conditional) If adding the site, specify the **[!UICONTROL Remote Site Name]**.

   For example, *[!DNL Workfront]*.

1. (Conditional) If adding the site, specify the **[!UICONTROL Remote Site URL]**.

   For example, *yourDomain.my.workfront.com*.

1. Click **[!UICONTROL Save]**.

   The [!DNL Workfront] app is now installed on your [!DNL Salesforce] instance and the **[!UICONTROL WorkfrontOpportunities]** and **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] Pages have been created in your environment.

   [!DNL Salesforce] users can use the app once you add the [!DNL Workfront] section to their [!UICONTROL Opportunity] or [!UICONTROL Account] page layouts.\
   For information about configuring the Workfront section for users, see [Configure the Adobe Workfront section for Salesforce users](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installing [!DNL Workfront] for [!DNL Salesforce] in the [!DNL Salesforce Classic] Framework 

1. Log in to [!DNL Salesforce] as a system administrator.
1. Go to **Setup.**
1. In the **Build** section, click **AppExchange Marketplace**.

1. In the **Search AppExchange Apps** box, type **Workfront**.

1. Click the Workfront app when you find it, then click **Get It Now**.
1. Click **[!UICONTROL Install in Production]** to install the [!DNL Workfront] app in your [!DNL Salesforce] Production environment. (recommended)
1. After you have read and agreed with the terms and conditions, enable the **[!UICONTROL I have read and agree to the terms and conditions]** field.
1. Click **[!UICONTROL Confirm and Install]**.
1. Select **[!UICONTROL Install for All Users]** (recommended), then click **[!UICONTROL Install]**. 

1. (Conditional) If asked if you want to approve a third party access, you must select **[!UICONTROL Yes, grant access to these third-party web sites]**, then click **[!UICONTROL Continue]**. 

1. Click **[!UICONTROL Done]** when the installation completes. 

   The [!DNL Workfront] app is listed under **[!UICONTROL Installed Packages]**.


1. Navigate to **[!UICONTROL Setup>Security Controls>Remote Site Settings]**.
1. (Conditional) If you do not see your [!DNL Workfront] URL listed in the **[!UICONTROL All Remote Sites]** list, click **[!UICONTROL New Remote Site]**.

1. (Conditional) If adding the site, specify the **[!UICONTROL Remote Site Name]**.
   For example, *[!DNL Workfront]*.

1. (Conditional) If adding the site, specify the **[!UICONTROL Remote Site URL]**.
   For example, *yourDomain.my.workfront.com*.

1. Click **[!UICONTROL Save]**.\
   The [!DNL Workfront] app is now installed on your [!DNL Salesforce] instance. The **[!UICONTROL WorkfrontOpportunities]** and **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] pages have been created in your environment.\
   [!DNL Salesforce] users cannot yet use the app until you add the [!DNL Workfront] section to their [!UICONTROL Opportunity] or [!UICONTROL Account] page layouts.\
   For information about configuring the [!DNL Workfront] section for users, see [Configure the [!DNL Adobe Workfront] section for [!DNL Salesforce] users](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installing [!DNL Workfront for Salesforce] in the [!DNL Salesforce Lightning Experience] Framework  

1. Log in to [!DNL Salesforce] as a system administrator.
1. Click the **[!UICONTROL Setup] icon**, then click **[!UICONTROL Setup]**.

1. In the **[!UICONTROL PLATFORM TOOLS]** section, expand **[!UICONTROL Apps].**

1. Click **[!DNL AppExchange Marketplace]**.
1. In the **[!UICONTROL Search [!DNL AppExchange] Apps]** box, type **[!DNL Workfront]**.

1. Click the Workfront app when you find it, then click **Get It Now**.
1. Click **[!UICONTROL Open Login Screen]**.\
   You must sign in with your [!DNL Workfront] administrator account for [!DNL Salesforce].

1. Click **[!UICONTROL Allow]**.
1. In the **[!UICONTROL Install in This Org]** box, click **[!UICONTROL Install Here]** to install [!DNL Workfront] in your [!DNL Salesforce] Production environment. (recommended)

1. After you have read and agreed with the terms and conditions, enable the **[!UICONTROL I have read and agree to the terms and conditions]** field.
1. Click **[!UICONTROL Confirm and Install]**.
1. Select **[!UICONTROL Install for All Users]** (recommended), then click **[!UICONTROL Install]**. 

1. (Conditional) If asked if you want to approve a third party access, you must select **[!UICONTROL Yes, grant access to these third-party web sites]**, then click **[!UICONTROL Continue]**.

1. Click **[!UICONTROL Done]** when the installation completes. 

   The [!DNL Workfront] app is listed under **[!UICONTROL Installed Packages]**.

1. Navigate to **[!UICONTROL Setup].**
1. In the **[!UICONTROL SETTINGS]** section, expand **[!UICONTROL Security].**

1. Click **[!UICONTROL Remote Site Settings]**.
1. (Conditional) If you do not see your [!DNL Workfront] URL listed in the **[!UICONTROL All Remote Sites]** list, click **[!UICONTROL New Remote Site]**.

1. (Conditional) If adding the site, specify the **[!UICONTROL Remote Site Name]**.
   For example, *[!DNL Workfront]*.

1. (Conditional) If adding the site, specify the **[!UICONTROL Remote Site URL]**.
   For example, *yourDomain.my.workfront.com*.

1. Click **[!UICONTROL Save]**.

   The [!DNL Workfront] app is now installed on your [!DNL Salesforce] instance, and the **[!DNL Workfront]** component is now added to your environment.

   [!UICONTROL Salesforce] users can use the [!DNL Workfront] app once you add the [!DNL Workfront] section to their [!UICONTROL Opportunity] or [!UICONTROL Account] page layouts.\
   For information about configuring the [!DNL Workfront] section for users, see [Configure the [!DNL Adobe Workfront] section for [!DNL Salesforce] users](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md). 
