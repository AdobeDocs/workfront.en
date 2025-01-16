---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Receive a webhook from a web service
description: The Adobe Workfront Fusion documentation has moved to a new location. This article has been deprecated, but contains a link to the new article that covers this functionality.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
---
# Receive a webhook from a web service

>[!IMPORTANT]
>
>The Adobe Workfront Fusion documentation has moved to a new location. 
>
>The information in this article can now be found in the article:
>
>* [Configure a webhook for a web service without a connector](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/receive-a-webhook-from-a-web-service.html)
>
>Please update any bookmarks.
>
>This article is no longer being updated, and will be removed in the near future.

If a web service is not currently implemented as an app in [!DNL Adobe Workfront Fusion], but it supports sending webhooks, you can add the service to a scenario using the Custom webhook module as an instant trigger.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Receive a webhook

1. Add the **[!UICONTROL Webhooks] >[!UICONTROL Custom webhook]** module to your scenario.
1. Click **[!UICONTROL Add]**, type a **[!UICONTROL Webhook name]** in the box that displays, then click **[!UICONTROL Save]**.

1. Click **[!UICONTROL Copy address to clipboard]**, then click **[!UICONTROL OK]**.

1. Log in to the web service and do the following there:

   1. In the [!UICONTROL Settings] area for the web service, create a webhook.
   1. Paste the address you copied to your clipboard in step 3 .
   1. Select the event that will trigger the webhook.

1. In the [!DNL Workfront Fusion] scenario, specify the event or events that you want to trigger the [!UICONTROL Custom webhook] module.
1. Run the scenario.

   When the event or events occur, the [!UICONTROL Custom webhook] module triggers and the scenario runs.
