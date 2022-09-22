---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Adobe Workfront for Salesforce overview
description: You can install [!DNL Adobe Workfront] for Salesforce to allow your Salesforce users to submit [!DNL Workfront] requests and automatically create projects without ever leaving Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
---
# Adobe Workfront for Salesforce overview

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>

A Pro Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)

You can install [!DNL Adobe Workfront] for Salesforce to allow your Salesforce users to submit [!DNL Workfront] requests and automatically create projects without ever leaving Salesforce.

As a [!DNL Workfront] administrator, you can download and configure [!DNL Workfront] for Salesforce. Then, you can share it will all other Salesforce users.

For more information about installing Workfront for Salesforce, see [Install Adobe Workfront for Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
For more information about configuring the Workfront section in Salesforce for all users, see [Configure the Adobe Workfront section for Salesforce users](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Access requirements

You must have the following access to use the functionality described in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Workfront for Salesforce

You can do the following when using [!DNL Workfront] for Salesforce:

* Manually create new [!DNL Workfront] requests from [!DNL Salesforce] within an Opportunity or an Account.

   For more information about creating [!DNL Workfront] requests from [!DNL Salesforce], see [Submit Adobe Workfront requests from Salesforce objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Automatically trigger the creation of projects in [!DNL Workfront] when certain criteria are met in Salesforce. Your Salesforce system administrator must configure triggers for creating projects from Salesforce.

   For more information about creating [!DNL Workfront] projects from [!DNL Salesforce], see [Create Adobe Workfront projects from Salesforce objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Consider the following when working with [!DNL Workfront] for Salesforce:

* We support both the [!DNL Salesforce] Classic and Lightning Experience frameworks.
* Items can be created only from Salesforce in to Workfront.
* You can view some information about the [!DNL Workfront] items in Salesforce.

   This information cannot be customized.

   For a list of [!DNL Workfront] fields that you can view from Salesforce, see  [Submit [!DNL Adobe Workfront] requests from Salesforce objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)&nbsp; and [Create Adobe Workfront projects from Salesforce objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* You can directly access items linked to Salesforce by clicking the **[!UICONTROL Go to the Salesforce]** link from Workfront.

   You cannot view any information about the [!DNL Salesforce] items in [!DNL Workfront], but you have a link to the [!UICONTROL Salesforce] item from [!DNL Workfront] to review it in Salesforce.

   [!UICONTROL The **Go to Salesforce**] link displays in the following areas:

   * The Details section of a project or and issue
   * The header of a project <span class="preview"> or an issue.</span>

      Your system or group administrator must add the [!UICONTROL Integrations] field to your Layout Template to view the [!UICONTROL Go to Salesforce] link in the project <span class="preview"> or issue</span> header.
   * The Summary panel  of an issue when selecting the issue in a list, after clicking [!UICONTROL Open Summary] ![](assets/summary-panel-icon.png) in the list's toolbar.

      >[!NOTE]
      >
      >The [!UICONTROL Go to Salesforce] link is visible to all [!DNL Workfront] users who can view the project or the issue. You must have a [!DNL Salesforce] account to be able to go to the [!DNL Salesforce] Opportunity or Account where the issue was logged.

* Updating fields on one item in one application does not update any information on linked items in the other application.
