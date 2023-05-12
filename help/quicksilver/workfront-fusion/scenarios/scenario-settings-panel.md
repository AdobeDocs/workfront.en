---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: The scenario settings panel in Adobe Workfront Fusion
description: This article describes the settings available in the [!UICONTROL scenario settings] panel in your [!DNL Adobe Workfront Fusion] scenarios.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
---
# The scenario settings panel in [!DNL Adobe Workfront Fusion]

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

## Open the scenario settings

1. Open the scenario editor, as explained in [The scenario editor in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Click the gear icon near the lower-left corner of the page.

   ![](assets/scenario-settings-350x221.png)

   In the [!UICONTROL Scenario settings] panel that displays, you can configure various advanced settings for the scenario.

## [!UICONTROL Allow storing incomplete executions]

This option determines how [!DNL Adobe Workfront Fusion] proceeds if an error occurs during the execution of a scenario. With this option enabled, the scenario is paused and moved to [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). This gives you the possibility to fix the issue and continue executing from where the scenario was stopped. If this option is disabled, the scenario run stops and a rollback phase is started.

## [!UICONTROL Sequential processing]

This option determines how [!DNL Workfront Fusion] proceeds if an error occurs and the execution of a scenario is moved to the [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). If the [!UICONTROL Sequential processing] option is enabled, Workfront Fusion stops processing the task sequence altogether until all incomplete executions are resolved. If the [!UICONTROL Sequential processing] option is disabled, the scenario continues to run according to its schedule, accompanied by repeated attempts to rerun the incomplete executions.

For more information on scheduling, see [Schedule a scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Data is confidential

Once a scenario has been executed, you can by default display information about which data was processed by modules in the scenario. If you do not want this information to be stored, enable the [!UICONTROL Data is confidential] option.

For more information about displaying information, see [Scenario execution flow in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>If you enable this option, it may be difficult to solve errors that may occur during the execution of a scenario.

## Enable data loss

This option has to do with enabling data loss if [!DNL Workfront Fusion] fails to save a bundle to the queue of [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (for example, due to a lack of free space). With this option enabled, the data is lost in order to prevent interruptions in the overall scenario execution. This is useful for scenarios where the highest priority is continuous execution and the incoming erroneous data is not that important.

Beyond that, when executing a scenario, a module can sometimes encounter a file that is larger than the maximum allowed size. In this case, [!DNL Workfront Fusion] proceeds in accordance with the setting of the [!UICONTROL Enable data loss] option and a warning message is shown.

For more information about maximum file size, see [About mapping files in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

For more information on warnings, see [Error processing in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Auto commit]

The [!UICONTROL Auto commit] settings applies to transactions and defines the way to process a scenario. If the Auto commit option is on, the commit phase on each module starts immediately after completing the operation phase. With the Auto commit option disabled, no commit occurs until operations are executed for all modules (this is the default mode).

For more information on transactions, see [Scenario execution, cycles, and phases in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Maximum number of cycles

Setting more cycles can be useful when you want to prevent connection interruption to a third-party service and assure that all records are processed within the one scenario run.

* If the scenario starts with a polling trigger, the setting defines the maximum number of cycles allowed during the scenario execution.

   For more information on polling triggers, see [Polling triggers](../../workfront-fusion/modules/module-types.md#polling) in [Types of modules](../../workfront-fusion/modules/module-types.md).

* If the scenario starts with an instant trigger, the setting is ignored and all the pending events are processed during a single scenario execution, one event per one cycle.

   For more information on instant triggers, see [Instant triggers](../../workfront-fusion/modules/module-types.md#instant) in [Types of modules](../../workfront-fusion/modules/module-types.md).

* If the scenario does not start with a trigger (instant/polling), the specified maximum number of cycles is always performed.

>[!INFO]
>
>**Examples:**  [!DNL Workfront] > [!UICONTROL Watch record] watches for new issues that come in, and [!DNL Workfront] >[!UICONTROL Convert object] converts the new request into a project and assigns it the appropriate template.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL more cycles] setting is applied only when you schedule your scenario execution. When you use the [!UICONTROL Run once] button, cycle settings are taken into account.
>
>### Max number of cycles is set to 1 (default)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>The [!UICONTROL Maximum number of returned files] in the [!UICONTROL Dropbox] >[!UICONTROL Watch files] module is set to `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>If 100 requests are submitted to [!DNL Workfront], and the [!UICONTROL Limit] field is set to 10, then 90 files are left unprocessed after one scenario run. The next 10 files are processed in the next scheduled scenario execution.
>
>### Max number of cycles is set to 10
>
>The [!UICONTROL Maximum number of returned files] in the [!UICONTROL Dropbox] >[!UICONTROL Watch files] module is set to `10`.
>
>If 100 files are added to the Dropbox folder and the [!UICONTROL Maximum number of returned files] option is set to 10, then 10 files are processed during the first cycle, the next 10 files in the second cycle, the next 10 files in the third cycle and so on, until all files are processed.
>
>All files are processed within 1 scenario run.
>
>You can see the already-run cycles in the Scenario details:
>
>![](assets/scenario-detail-350x207.png)
>
>For more information about this page, see [Scenario details in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Number of consecutive errors

Defines the maximum number of consecutive execution attempts before the execution of a scenario is deactivated (excluding [!UICONTROL DataError], [!UICONTROL DuplicateDataError] and [!UICONTROL ConnectionError]).

For more information on errors, see [Error processing in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>If a scenario starts with an instant trigger, the setting is ignored and the scenario is deactivated immediately once the first error has occurred.
