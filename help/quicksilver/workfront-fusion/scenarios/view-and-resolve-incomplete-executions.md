---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]
description: The [!UICONTROL Incomplete executions] folder stores scenario executions that were not successfully finalized due to an error. Each stored incomplete execution can be resolved either manually or automatically.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
---
# View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]

The [!UICONTROL Incomplete executions] folder stores scenario executions that were not successfully finalized due to an error. Each stored incomplete execution can be resolved either manually or automatically.

>[!NOTE]
>
>By default the storing of incomplete executions is disabled. To enable it, enable the [!UICONTROL Allow storing incomplete executions] option in the scenario advanced settings.
>
>For more information about scenario settings, see [The scenario settings panel in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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

## View incomplete executions

If a module encounters an error during its operation, a new incomplete execution is added to the Incomplete executions folder. Each incomplete execution contains the scenario's blueprint and all the bundles that can be mapped into the failed module. The list of incomplete executions can be opened by clicking on the [!UICONTROL Incomplete Executions] tab on the scenario detail page:

![](assets/incomplete-executions-tab-350x102.png)

For more information, see [Errors resulting into incomplete executions](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>The current size limit of the unresolved incomplete executions folder per organization is 500 MB. If your organization exceeds this limit, you may see the following error:
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>For more information, see [Enable data loss](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in [The scenario settings panel in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Resolve incomplete executions

When a new incomplete execution is stored, you can resolve it as follows:

1. Click the **[!UICONTROL Incomplete Executions]** tab.
1. Locate the incomplete execution you would like to resolve and click **[!UICONTROL Detail]**.


   If you want to see the log of all module's operations before you attempt to resolve the incomplete execution, you can resolve the incomplete execution from the [!UICONTROL History] folder:

1. Click the **[!UICONTROL History]** tab.
1. Locate the scenario's failed execution log and click **[!UICONTROL Details]**.
1. Open the module's log where all the module's operations are shown.
1. Locate the failed operation and click **[!UICONTROL Resolve]**:

   ![](assets/resolve-btn-350x188.png)

## Options related to incomplete executions

The following options in the [!UICONTROL Scenario settings] panel determine if and how the incomplete executions are stored:

* Allow storing incomplete executions
* Sequential processing
* Enable data loss

For more information about these options, see [The scenario settings panel in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Errors resulting into incomplete executions 

There are several categories of errors which result into storing of incomplete executions. These may include:

* Validation errors arising from incomplete or erroneous data, mostly because of a missing item that is expected in order to successfully process all data going through a module.
* Errors occurring from the final destination's unavailability because of temporary or long term connection failure (for example, during connection to email or remote FTP server).

If an error occurs on the first module in the scenario, the execution stops immediately and no incomplete execution is stored.

If an error occurs on any other module and there is no error handler route attached, one of the following occurs:

* If the error type is `ConnectionError`, `RateLimitError`, `OutOfSpaceError` or `ModuleTimeoutError`, an incomplete execution record with auto-retry is stored.
* If the error type is `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`, or `MaxResultsExceededError`, an incomplete execution record without auto-retry is stored.
* If the error type is anything other than the above, the execution fails.
