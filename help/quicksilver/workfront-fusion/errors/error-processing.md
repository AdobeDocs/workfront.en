---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Error processing in [!DNL Adobe Workfront Fusion]
description: Sometimes an error can occur during the execution of a scenario. This usually happens if a service is unavailable due to a failure to connect to a service or if a validation fails. This article discusses the common errors that you may encounter.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
---
# Error processing in [!DNL Adobe Workfront Fusion]

Sometimes an error can occur during the execution of a scenario. This usually happens if a service is unavailable due to a failure to connect to a service or if a validation fails. This article discusses the common errors that you may encounter.

[!DNL Adobe Workfront Fusion] distinguishes between several basic error types. It will react differently depending upon on the type of error that occurred.

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

## Connection Error 

`ConnectionError`

Connection error is one of the most common errors usually caused by unavailability of the third-party service for various reasons (overloading, maintenance, outage, and so on). The default handling of this error depends on which module it was encountered on:

* If the error occurs on the first module, the execution of the scenario is terminated with a warning message. [!DNL Workfront Fusion] then repeatedly attempts to rerun the scenario at increasing time intervals (these are explained below). If all attempts fail, [!DNL Workfront Fusion] deactivates the scenario.
* If the connection error occurs on another module than the first one, the subsequent steps depend on the [Allow storing incomplete executions](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) option in the scenario advanced settings:

    * If this option is enabled, the execution of the scenario is moved to the [!UICONTROL Incomplete executions] folder where [!DNL Workfront Fusion] repeatedly attempts to rerun the scenario at increasing time intervals. If all attempts fail, the execution will remain in the Incomplete executions folder awaiting manual resolution by the user.

      For more informationon incomplete executions, see [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
    * If this option is disabled, the execution of the scenario ends with an error followed by a rollback phase. [!DNL Workfront Fusion] then repeatedly attempts to rerun the scenario at increasing time intervals. If all attempts fail, [!DNL Workfront Fusion] deactivates the scenario.

### Increasing time intervals

The algorithm of multiplicatively increasing time intervals between attempts when an error occurs is known as exponential backoff. The increasing time intervals are set as follows:

1. 10 minutes
1. 1 hour
1. 3 hours
1. 12 hours
1. 24 hours

The main reason for employing the increasing time intervals in [!DNL Workfront Fusion] is to prevent frequently executed scenarios from consuming operations on repeatedly failing attempts.

>[!INFO]
>
>**Example:**
>
>A scenario contains the [!DNL Google Sheets] trigger [!UICONTROL Watch Rows]. [!DNL Google Sheets] is unavailable for 30 minutes due to maintenance when [!DNL Workfront Fusion] starts the scenario, so it is unable to retrieve new rows. The scenario stops and tries again in 10 minutes. Because [!DNL Google Sheets] is still unavailable, [!DNL Workfront Fusion] is still unable to get information about new rows. The next run of the scenario is scheduled in 1 hour. [!DNL Google Sheets] is available again at this time, and the scenario runs successfully.

## Data error

`DataError`

A data error is generated when an item is incorrectly mapped and does not pass the validation performed on the [!DNL Workfront Fusion] side or on the side of the third-party service being used. 

If this error occurs, the scenario, up to where the module failed, is moved to the incomplete executions folder where you can troubleshoot the issue. However, the scenario does not stop and continues to run according to its schedule. To stop the execution of the scenario when Data error appears, enable the Sequential processing option in the Scenario settings panel. 

If you have not enabled the [!UICONTROL Allow storing incomplete executions] option in the scenario settings, the execution of the scenario terminates with the error and a rollback is performed.

For more information on mapping, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

For information about incomplete executions, see [View and resolve incomplete executions in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

For imformation about the scenario setting panel, see [The scenario settings panel in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

For information about schedules, see [Schedule a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Duplicate Data Error

`DuplicateDataError`

If [!DNL Workfront Fusion] tries to insert the same bundle twice into a service that does not allow duplicate data, a duplicate data error is generated. If this error occurs, [!DNL Workfront Fusion] proceeds in the same way as as it does for the data error.

## Invalid Access Token Error

`InvalidAccessTokenError`

An invalid access token error occurs when [!DNL Workfront Fusion] cannot access your account registered with a third-party service. This usually happens when you revoke access rights for [!DNL Workfront Fusion] in the administration of a given service, but related scenarios keep running according to schedule.

If this error occurs, the execution of a scenario is stopped immediately. The rest of the scenario starting from the module where the error occurred is moved to the incomplete executions folder.

For information about incomplete executions, see [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Rate Limit Error

`RateLimitError`

If a limit set by a given service is exceeded, a rate limit error is generated. If this error happens, [!DNL Workfront Fusion] proceeds in the same way as it does for the Connection Error. 

For more information, see [Connection Error](#connection-error).

## Incomplete Data Error

`IncompleteDataError`

An incomplete data error occurs only with triggers. This error is generated if a trigger fails to download required data from a given service.

If a scenario terminates with the `IncompleteDataError`, its further behavior will depend on its setting of [!UICONTROL Max number of consecutive errors]. 

For more information, see [Number of consecutive errors](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) in the article [The scenario settings panel in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Example:** 
>
>A scenario has the [!DNL Workfront] trigger [!UICONTROL Watch Record] set to watch for documents. The scenario executes while you are uploading a large document, such as a long video. Because [!UICONTROL Workfront Fusion] tries to download the video while it is still uploading to Workfront, the scenario terminates with the `IncompleteDataError`.

## Run time error

`RuntimeError`

If any other error (not mentioned above) appears during scenario execution, it is reported as a `RunTimeError`.

If a scenario terminates with the `RuntimeError`, its further behavior will depend on its setting of [!UICONTROL Max number of consecutive errors]. For more information, see [Number of consecutive errors](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) in the article [The scenario settings panel in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>If a scenario starts with an instant trigger, the setting of [!UICONTROL Max number of consecutive errors] is ignored and the scenario is deactivated immediately once the first error has occurred. For more information, see [Instant triggers](../../workfront-fusion/modules/module-types.md#instant) in the article [Types of modules](../../workfront-fusion/modules/module-types.md).

## Inconsistency Error

`InconsistencyError`

If any error described above occurs during the commit or rollback phase, a scenario will terminate with Inconsistency Error. For more information, see [Scenario execution, cycles, and phases in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

If this error appears in a scenario, the execution of the scenario is immediately stopped.

## Warning

While executing a scenario, you may receive a warning informing you about a problem. However, it does not prevent the scenario from being successfully completed.

For example, a warning can appear when the maximum allowed file size is exceeded and the [!UICONTROL Enable data loss] option is disabled. For more information, see [Enable data loss](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in the article [The scenario settings panel in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
