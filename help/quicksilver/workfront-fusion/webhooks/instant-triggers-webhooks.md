---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Instant triggers (webhooks) in [!DNL Adobe Workfront Fusion]
description: Many services provide webhooks to deliver instant notifications whenever a certain change occurs in the service. To process these notifications, we recommend that you use instant triggers. This article describes the use and functionality of instant triggers in Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
---
# Instant triggers (webhooks) in [!DNL Adobe Workfront Fusion]

Many services provide webhooks to deliver instant notifications whenever a certain change occurs in the service. To process these notifications, we recommend that you use instant triggers. You can recognize these easily in [!DNL Adobe Workfront Fusion] because of their tag:

![](assets/instant-350x256.png)

If the service does not provide webhooks, you need to use polling triggers to periodically poll the service.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## View a webhook's queue

All messages from incoming webhooks are stored in the webhook's queue.

1. Click **[!UICONTROL Webhooks]** in the menu on left.
1. Find the Webhook for which you want to view the queue.
1. Click the button with a truck icon and the number of received webhooks.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >Incoming webhook data is always stored in the queue regardless of how you have set the option [!UICONTROL Data] is confidential (described in [The scenario settings panel in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). As soon as the data is processed in a scenario, it is permanently deleted from the system.

## Schedule instant triggers

If your scenario contains an instant trigger, you can schedule the scenario to run immediately:

![](assets/schedule-setting-350x185.png)

In this case your scenario will run immediately when [!DNL Workfront Fusion] receives new data from the service. After the scenario executes, the total amount of pending webhooks waiting in the queue is counted and the scenario performs as many cycles as there are pending webhooks, processing one webhook per cycle. For more information, see [Scenario execution, cycles, and phases in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* A cycle is not the same as a scenario run. There can be multiple cycles within 1 scenario run. 
>* When you execute a scenario with an instant trigger scheduled to be immediate, the following exceptions apply:
>
>     * The interval between two executions is not subject to the Minimum interval according to the pricing plan.
>
>       For example, once the scenario finishes its execution, the webhook's queue is checked again. If there are any pending webhooks, the scenario executes immediately again, processing all the pending webhooks once again.
>   
>     * The Maximum number of cycles scenario setting is ignored and set to 100, which means that no more than 100 pending webhooks will be processed during a single scenario execution (at the rate of 1 event per one cycle).
>


If you use any other schedule setting than [!UICONTROL Immediately], the scenario executes at the intervals you specify. As several webhooks can be gathered in the queue during the interval, it is recommended to set the [[!UICONTROL Maximum number of cycles]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) to a higher value than the default 1 to process more webhooks in one scenario run:

1. Click the [!UICONTROL Scenario settings] icon ![](assets/gear-icon-settings.png) at the bottom of your scenario.
1. In the **[!UICONTROL Scenario settings]** box that appears, type a number in the **[!UICONTROL Max number of cycles]** box to indicate the number of webhooks from the queue that you want to run each time you execute the scenario.

## Rate limits

The current rate limit is 5 webhooks per second. If the limit is exceeded, a 429 status code is returned.

## Expiration of inactive webhooks

A webhook that has not been assigned to any scenario for more than 120 hours is removed.

## Webhook payloads

[!DNL Workfront Fusion] stores webhook payloads for 30 days. Accessing a webhook payload more than 30 days after it was created results in the error "[!UICONTROL Failed to read file from storage.]"

## Error handling

When there is an error in your scenario with an instant trigger, the scenario:

* Stops immediately - when the scenario is set to run [!UICONTROL Immediately].
* Stops after 3 unsuccessful attempts (3 errors) - when the scenario is set to run as scheduled.

If an error occurs during the scenario execution, the webhook is placed back into the queue during the instant trigger's rollback phase. In such a situation, you have the possibility to fix the scenario and rerun it again. For more information, see [Rollback](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) in the article [Scenario execution, cycles, and phases in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

If there is a Webhook response module in your scenario, the error is sent to the Webhook response. The Webhook response module is always executed last (in the case where the [!UICONTROL Auto commit] option in the Scenario settings is not enabled). For more information, see [Responding to webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) in the article [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Custom webhooks

You can create your own webhooks. For more information, see [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhook deactivation

Webhooks are deactivated automatically if either of the following applies:

* The webhook has not been connected to any scenario for more than 5 days
* The webhook is used only in inactive scenarios, which have been inactive for more than 30 days.

Deactivated webhooks are deleted and unregistered automatically if they are not connected to any scenarios and have been in deactivated status for over 30 days.


