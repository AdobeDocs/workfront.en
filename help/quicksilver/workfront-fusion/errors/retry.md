---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Retry error handling in [!DNL Adobe Workfront Fusion]
description: In some cases it is useful to re-execute a failing module for a couple of times if there is a chance that the reason for the failure might pass over time.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
---
# Retry error handling in [!DNL Adobe Workfront Fusion]

In some cases it is useful to re-execute a failing module if there is a chance that the reason for the failure might pass over time.

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

## Workarounds to the [!UICONTROL Retry] error handling directive

[!UICONTROL Adobe Workfront Fusion] currently does not offer the [!UICONTROL Retry] error handling directive, though two workarounds can be employed to mimic its functionality. For more information, see [Directives for error handling in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Use the [!UICONTROL Break] directive

1. In the scenario settings panel, enable the **[!UICONTROL Allow storing of Incomplete Executions]** option.
   
   For more information, see [The scenario settings panel in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Attach an error handler route to the module, as described in [Error handling in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Link the [!UICONTROL Break] directive to the error handler route  and configure it.

   For more information, see [Directives for error handling in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Drawbacks

* The minimum retry interval is one minute.
* If the module is processing multiple bundles and the processing of a bundle fails, the partial execution (only the bundle that caused the error) is moved to the incomplete executions folder and scheduled for retries according to the [!UICONTROL Break] directive settings. However, the current execution continues and the module continues to process the subsequent bundles. You can enable the "[!UICONTROL Sequential processing]" option in the [!UICONTROL Scenario settings] to prevent the scenario from executing again until the execution stored in the the Incomplete executions folder has been successfully resolved.

    For more information on incomplete executions, see [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Use the [!UICONTROL Repeater] module

1. Employ the **[!UICONTROL Repeater]** module and set its **[!UICONTROL Repeats]** field to the maximum number of attempts.
1. Link the potentially failing module to the **[!UICONTROL Repeater]** module.
1. Attach an error handler route to this module (see [Error handling in [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Link the **[!UICONTROL Tools] > [!UICONTROL Sleep]** module to the error handler route and set its **[!UICONTROL Delay]** field to the number of seconds between the attempts.

1. Link the **[!UICONTROL Ignore]** directive after the **[!UICONTROL Tools] > [!UICONTROL Sleep]** module (see [Directives for error handling in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Link the **[!UICONTROL Tools] > [!UICONTROL Set variable]** module after the the potentially failing module and configure it to store the module's result in a variable named, for example, `Result`.

1. Link the **[!UICONTROL Array aggregator]** module after the **[!UICONTROL Tools] > [!UICONTROL Set variable]** and choose the **[!DNL Repeater]** module in its Source Module field.

1. Link the **[!UICONTROL Tools] > [!UICONTROL Get variable]** module to the **[!UICONTROL Array aggregator]** module and configure it to obtain the value of the `Result` variable.

1. Insert the **[!UICONTROL Tools] > [!UICONTROL Get variable]** module between the **[!UICONTROL Repeater]** module and the potentially failing module and configure it obtain the value of the `Result` variable.

1. Insert a filter between this **[!UICONTROL Tools] > [!UICONTROL Get variable]** module and the potentially failing module to continue only if the `Result` variable does not exist.

>[!INFO]
>
>**Example:** Here is a sample scenario where the [!UICONTROL HTTP] >[!UICONTROL Make a request] module represents the potentially failing module:
>
>![](assets/http-make-request-350x116.png)
>
>If the result of the potentially failing module is too complex to be stored in a simple variable, you can employ a data store to store/retrieve the result. The data store would contain just one record. The record's key can be, for example, `Result`.
>
>For more information on data stores, see [Data Stores in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Drawback

This workaround might appear a bit too complex, and  is also more demanding in terms of operations.
