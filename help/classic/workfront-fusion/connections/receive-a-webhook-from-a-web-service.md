---
filename: receive-a-webhook-from-a-web-service
product: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Receive a webhook from a web service
description: If a web service is not currently implemented as an app in Adobe Workfront Fusion, but it supports sending webhooks, you can add the service to a scenario using the Custom webhook module as an instant trigger.
---

# Receive a webhook from a web service

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

If a web service is not currently implemented as an app in Adobe Workfront Fusion, but it supports sending webhooks, you can add the service to a scenario using the Custom webhook module as an instant trigger.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Receive a webhook

1. Add the **Webhooks > Custom webhook** module to your scenario.
1. Click **Add**, type a **Webhook name** in the box that displays, then click **Save**. 

1. Click **Copy address to clipboard**, then click **OK**.

1. Log in to the web service and do the following there:

   1. In the Settings area for the web service, create a webhook.
   1. Paste the address you copied to your clipboard in step 3 .
   1. Select the event that will trigger the webhook.

1. In the Workfront Fusion scenario, specify the event or events that you want to trigger the Custom webhook module.
1. Run the scenario.

   When the event or events occur, the Custom webhook module triggers and the scenario runs.

