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
# [!DNL Adobe Workfront for Salesforce] overview

<!-- Audited: 5/2025 -->

You can install [!DNL Adobe Workfront for Salesforce] to allow your [!DNL Salesforce] users to submit [!DNL Workfront] requests and automatically create projects without ever leaving [!DNL Salesforce].

As a [!DNL Workfront] administrator, you can download and configure [!DNL Workfront for Salesforce]. Then, you can share it with all other [!DNL Salesforce] users.

For more information about installing [!DNL Workfront for Salesforce], see [Install [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

For more information about configuring the [!DNL Workfront] section in [!DNL Salesforce] for all users, see [Configure the [!DNL Adobe Workfront] section for [!DNL Salesforce] users](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

>[!NOTE]
>
>A [!UICONTROL Pro] [!DNL Workfront] Plan is required to use this feature. For more information about the various plans available, see [[!DNL Workfront] Plans.](https://business.adobe.com/products/workfront/pricing.html)

## Access requirements

You must have the following access to use the functionality described in this article:

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Plan</p>
   
   
   </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## [!DNL Workfront for Salesforce]

You can do the following when using [!DNL Workfront for Salesforce]:

* Manually create new [!DNL Workfront] requests from [!DNL Salesforce] within an Opportunity or an Account.

   For more information, see [Submit [!DNL Adobe Workfront] requests from [!DNL Salesforce] objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Automatically trigger the creation of projects in [!DNL Workfront] when certain criteria are met in [!DNL Salesforce]. Your [!DNL Salesforce] system administrator must configure triggers for creating projects from [!DNL Salesforce].

   For more information about creating [!DNL Workfront] projects from [!DNL Salesforce], see [Create [!DNL Adobe Workfront] projects from [!DNL Salesforce] objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Consider the following when working with [!DNL Workfront] for [!DNL Salesforce]:

* We support both the [!DNL Salesforce Classic] and [!DNL Lightning Experience] frameworks.
* Items can be created only from [!DNL Salesforce] to [!DNL Workfront].
* You can view some information about the [!DNL Workfront] items in [!DNL Salesforce]. This information cannot be customized.

   For a list of [!DNL Workfront] fields that you can view from [!DNL Salesforce], see  [Submit [!DNL Adobe Workfront] requests from [!DNL Salesforce] objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)  and [Create [!DNL Adobe Workfront] projects from [!DNL Salesforce] objects](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* You can directly access items linked to [!DNL Salesforce] by clicking the [!UICONTROL Go to Salesforce] link from Workfront.

   You cannot view any information about the [!DNL Salesforce] items in [!DNL Workfront], but there's a link in Workfront that takes you to the item in Salesforce so you can review it there.

   [!UICONTROL The Go to Salesforce] link displays in the following areas:

    * The [!UICONTROL Details] section of a project or an issue.
    * The header of a project or an issue.

      Your system or group administrator must add the [!UICONTROL Integrations] field to your Layout Template to view the [!UICONTROL Go to Salesforce] link in the project or issue header.
    * The [!DNL Summary] panel  of an issue when selecting the issue in a list, after clicking [!UICONTROL Open Summary] ![Summary panel icon](assets/summary-panel-icon.png) in the list's toolbar.

      >[!NOTE]
      >
      >The [!UICONTROL Go to Salesforce] link is visible to all [!DNL Workfront] users who can view the project or the issue. You must have a [!DNL Salesforce] account to be able to go to the [!DNL Salesforce] Opportunity or Account where the issue was logged.

* Updating fields on one item in one application does not update any information on linked items in the other application.
