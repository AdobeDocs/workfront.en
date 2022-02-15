---
filename: instant-triggers-webhooks
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
---



# Instant triggers (webhooks) {#instant-triggers-webhooks}

Many services provide webhooks to deliver instant notifications whenever a certain change occurs in the service. To process these notifications, we recommend that you use instant triggers. You can recognize these easily in *`Adobe Workfront Fusion`* because of their tag:


![](assets/instant-350x256.png)




If the service does not provide webhooks, you need to use polling triggers to periodically poll the service.


## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> license**</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> <p data-mc-conditions="SnippetConditions.HIDE"><span class="mc-variable WFVariables.WFFusionAutomation variable varname">Workfront Fusion for Work Automation</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## View a webhook's queue {#view-a-webhooks-queue}

All messages from incoming webhooks are stored in the webhook's queue.



1. Click `Webhooks` in the menu on left.
1. Find the Webhook for which you want to view the queue.
1.  Click the button with a truck icon and the number of received webhooks.


   ![](assets/webhooks-truck-icon.png)




   >[!NOTE]
   >
   >Incoming webhook data is always stored in the queue regardless of how you have set the option Data is confidential (described in [Scenario settings panel](scenario-settings-panel.md)). As soon as the data is processed in a scenario, it is permanently deleted from the system.







## Schedule instant triggers  {#schedule-instant-triggers}

If your scenario contains an instant trigger, you can schedule the scenario to run immediately:


![](assets/schedule-setting-350x185.png)




In this case your scenario will run immediately when *`Workfront Fusion`* receives new data from the service. After the scenario executes, the total amount of pending webhooks waiting in the queue is counted and the scenario performs as many cycles as there are pending webhooks, processing one webhook per cycle. For more information, see [Scenario execution, cycles, and phases](scenario-execution-cycles-phases.md).


>[!NOTE]
>
>
>
>
>* A cycle is not the same as a scenario run. There can be multiple cycles within 1 scenario run. 
>* When you execute a scenario with an instant trigger scheduled to be immediate, the following exceptions apply:>
>    
>    
>    * The interval between two executions is not subject to the Minimum interval according to the pricing plan.
>    
>    
>      For example, once the scenario finishes its execution, the webhook's queue is checked again. If there are any pending webhooks, the scenario executes immediately again, processing all the pending webhooks once again.
>    
>    * The Maximum number of cycles scenario setting is ignored and set to 100, which means that no more than 100 pending webhooks will be processed during a single scenario execution (at the rate of 1 event per one cycle).
>    
>    
>
>



If you use any other schedule setting than Immediately, the scenario executes at the intervals you specify. As several webhooks can be gathered in the queue during the interval, it is recommended to set the [Maximum number of cycles](scenario-settings-panel.md#maximum) to a higher value than the default 1 to process more webhooks in one scenario run:



1. Click the Scenario settings icon ![](assets/gear-icon-settings.png) at the bottom of your scenario.
1.  In the `Scenario settings` box that appears, type a number in the `Max number of cycles` box to indicate the number of webhooks from the queue that you want to run each time you execute the scenario. 




## Rate limits {#rate-limits}

The current rate limit is 5 webhooks per second. If the limit is exceeded, 429 status code is returned.


## Expiration of inactive webhooks {#expiration-of-inactive-webhooks}

A webhook that has not been assigned to any scenario for more than 120 hours is removed.


## Error handling {#error-handling}

When there is an error in your scenario with an instant trigger, the scenario:



* Stops immediately - when the scenario is set to run Immediately.
* Stops after 3 unsuccessful attempts (3 errors) - when the scenario is set to run as scheduled.


If an error occurs during the scenario execution, the webhook is placed back into the queue during the instant trigger's rollback phase. In such a situation, you have the possibility to fix the scenario and rerun it again. For more information, see [Rollback](scenario-execution-cycles-phases.md#rollback) in the article [Scenario execution, cycles, and phases](scenario-execution-cycles-phases.md).


If there is a Webhook response module in your scenario, the error is sent to the Webhook response. The Webhook response module is always executed last (in the case where the Auto commit option in the Scenario settings is not enabled). For more information, see [Responding to webhooks](webhooks-updated.md#respondi) in the article [Webhooks](webhooks-updated.md).


## Custom webhooks {#custom-webhooks}

You can create your own webhooks. For more information, see [Webhooks](webhooks-updated.md).
