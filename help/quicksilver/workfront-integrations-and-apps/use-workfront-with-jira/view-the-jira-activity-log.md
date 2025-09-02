---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: View the Jira Activity Log
description: As a [!DNL Jira] administrator, you can view the exceptions and errors that occur during the synchronization or creation of the tickets between [!DNL Adobe Workfront] and [!DNL Jira] in an Activity Log.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
---
# View the [!UICONTROL [!DNL Jira] Activity Log]

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

As a [!DNL Jira] administrator, you can view the exceptions and errors that occur during the synchronization or creation of the tickets between [!DNL Adobe Workfront] and [!DNL Jira] in an [!UICONTROL Activity Log]. 

You can see up to 500 items in the Activity Log, and they are listed starting with the most recent ones.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira access</td> 
   <td> <p>System administrator access</p> <p>Important:  We recommend that you create separate system administrator accounts in Jira and Workfront to dedicate to this integration, rather than using existing ones that might be attached to users.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you can link items between [!DNL Workfront] and [!DNL Jira], you must

* Install [!DNL Workfront for Jira]

   For instructions on installing [!DNL Workfront for Jira], see [Install [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Access the [!UICONTROL [!DNL Jira] Activity Log]: 

1. Log into Jira as a system administrator.
1. Click **[!UICONTROL Settings]** in the main [!DNL Jira] menu.
1. Click **[!UICONTROL Add-ons]**, then **[!UICONTROL Manage add-ons]**.

1. Expand the **[!DNL Workfront]** add-on.
1. Click **[!UICONTROL Configure]**.
1. Log in to [!DNL Workfront] as a system administrator.
1. Select the **[!UICONTROL Activity Log]** tab.

   View information about exceptions and errors that occurred during the creation of items or synchronization of fields between the two applications.

   The log includes the following fields:

   * Date of the occurrence
   * The name of the user in Jira
   * Jira issue number
   * A brief description of the error that occurred.
