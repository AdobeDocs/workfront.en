---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Manage locked scenarios in [!DNL Adobe Workfront Fusion]
description: Manage locked scenarios in [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 5fccf336-d904-43fe-ad4a-c3ce76dbcad0
---
# Manage locked scenarios in [!DNL Adobe Workfront Fusion]

In some cases, a scenario might be temporarily locked in [!DNL Workfront Fusion]. Locked executions will be automatically unlocked within 2-4 hours. You can also unlock scenarios manually.

>[!IMPORTANT]
>
>Unlocking a scenario manually can cause errors in a scenario's executions. 

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Understanding locked scenarios

Scenarios may be locked for a number of reasons. 

Workfront Fusion does not support parallel processing of scheduled scenarios. These scenarios are locked at the beginning of the scenario execution and unlocked when it completes. If the execution is interrupted, the scenario may not unlock. This may occur when a user manually force-stops the scenario, or when there is a system issue.

In addition, the Workfront Fusion engineering team may lock a scenario because it is causing performance or other issues.

Regardless of the cause of a locked scenario, the scenario will unlock automatically 2-4 hours after it is locked.

## Unlock a locked scenario

Locked scenarios will unlock 2-4 hours from the time they were locked. You can unlock a scenario manually before it is scheduled to unlock automatically. 

Unlocking a scenario manually can cause errors in a scenario's executions. We recommend manually unlocking scenarios only when a scenario is locked due to running and stopping executions as part of designing the scenario. In other circumstances, we recommend that you wait for the scenario to be unlocked automatically.

>[!IMPORTANT]
>
>Unlocking a scenario manually can cause errors in a scenario's executions. 

1. Go the Scenario details page of the locked scenario.
1. Click **[!UICONTROL Options]** in the upper-right corner of the screen.
1. Select **[!UICONTROL Unlock execution]**.
1. Click **[!UICONTROL Unlock]**.
