---
filename: error-processing
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Error processing in Adobe Workfront Fusion
description: Sometimes an error can occur during the execution of a scenario. This usually happens if a service is unavailable due to a failure to connect to a service or if a validation fails. This article discusses the common errors that you may encounter.
---

# Error processing in&nbsp;Adobe Workfront Fusion

Sometimes an error can occur during the execution of a scenario. This usually happens if a service is unavailable due to a failure to connect to a service or if a validation fails. This article discusses the common errors that you may encounter.

Adobe Workfront Fusion distinguishes between several basic error types. It will react differently depending upon on the type of error that occurred.

## Access requirements

You must have the following access to use the functionality in this article:

<table> 
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
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
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

## Connection Error {#connection-error}

<pre>ConnectionError</pre>Connection error is one of the most common errors usually caused by unavailability of the third-party service for various reasons (overloading, maintenance, outage,and so on). The default handling of this error depends on which module it was encountered on:

* If the error occurs on the first module, the execution of the scenario is terminated with a warning message. Workfront Fusion then repeatedly attempts to rerun the scenario at increasing time intervals (these are explained below). If all attempts fail, Workfront Fusion deactivates the scenario.
* If the connection error occurs on another module than the first one, the subsequent steps depend on the [Allow storing incomplete executions](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) option in the scenario advanced settings:

   * If this option is enabled, the execution of the scenario is moved to the Incomplete executions folder where Workfront Fusion repeatedly attempts to rerun the scenario at increasing time intervals. If all attempts fail, the execution will remain in the [View and resolve incomplete executions in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) folder awaiting manual resolution by the user.
   * If the option is disabled, the execution of the scenario ends with an error followed by a rollback phase. Workfront Fusion then repeatedly attempts to rerun the scenario at increasing time intervals. If all attempts fail, Workfront Fusion deactivates the scenario.

### Increasing time intervals

The algorithm of multiplicatively increasing time intervals between attempts when an error occurs is known as exponential backoff. The increasing time intervals are set as follows:

1. 10 minutes
1. 1 hour
1. 3 hours
1. 12 hours
1. 24 hours

The main reason for employing the increasing time intervals in Workfront Fusion is to prevent frequently executed scenarios from consuming operations on repeatedly failing attempts.

**Example:** 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
Running this past Sam
</MadCap:conditionalText>
-->

A scenario contains the Google Sheets trigger Watch Rows. Google Sheets is unavailable for 30 minutes due to maintenance when Workfront Fusion starts the scenario, so it is unable to retrieve new rows. The scenario stops and tries again in 10 minutes. As the service continues to be unavailable within this time frame, Workfront Fusion is still unable to get information about new rows. The next run of the scenario is scheduled in 1 hour. Google Sheets is available again within this time and the scenario runs successfully.

## Data error

```
DataError
```

A data error is generated when an item is incorrectly mapped and does not pass the validation performed on the Workfront Fusion side or on the side of the third-party service being used. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

If this error occurs, the scenario, up to where the module failed, is moved to the [View and resolve incomplete executions in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) folder where you can troubleshoot the issue. However, the scenario does not stop and continues to run according to its schedule. To stop the execution of the scenario when Data error appears, enable the Sequential processing option in the [The scenario settings panel in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md). For information about schedules, see [Schedule a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

If you have not enabled the Allow storing incomplete executions option in the scenario settings, the execution of the scenario terminates with the error and a rollback is performed.

<!--
<p class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"><span class="autonumber"><span><b>Example: </b></span></span>If your scenario contains the action Create a tweet, the Twitter's 140-character limit for a tweet cannot be exceeded. If you try to tweet more than 140 characters, the execution of the scenario will terminate with a data error.</p>
-->

## Duplicate Data Error

<pre>DuplicateDataError</pre>If Workfront Fusion tries to insert the same bundle twice into a service that does not allow duplicate data, a duplicate data error is generated. If this error occurs, Workfront Fusion proceeds in the same way as as it does for the data error.

<!--
<p class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"><span class="autonumber"><span><b>Example: </b></span></span>A scenario containing the action Create a tweet will terminate with this error if Workfront Fusion tries to insert the same tweet twice.</p>
-->

## Invalid Access Token Error

<pre>InvalidAccessTokenError</pre>An invalid access token error occurs when Workfront Fusion cannot access your account registered with a third-party service. This mostly happens when you revoke access rights for Workfront Fusion in the administration of a given service but related scenarios keep running according to schedule.

If this error occurs, the execution of a scenario is stopped immediately. The rest of the scenario starting from the module where the error occurred is moved to the [View and resolve incomplete executions in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Rate Limit Error

```
RateLimitError
```

If a limit set by a given service is exceeded, a rate limit error is generated. If this error happens, Workfront Fusion proceeds in the same way as it does for the Connection Error. For more information, see [Connection Error](#connection-error).

<!--
<p class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"><span class="autonumber"><span><b>Example: </b></span></span>You will encounter this error if you try to send more than 1000 tweets within 24 hours. If this happens, wait until the limitation resets within the time frame.</p>
-->

## Incomplete Data Error

```
IncompleteDataError
```

An incomplete data error occurs only with triggers. This error is generated if a trigger fails to download required data from a given service.

If a scenario terminates with the IncompleteDataError, its further behavior will depend on its setting of Max number of consecutive errors. For more information, see [Number of consecutive errors](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) in the article [The scenario settings panel in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

**Example:** A scenario has the Workfront trigger Watch Record set to watch for documents. The scenario executes while you are uploading a large document, such as a long video. Because Workfront Fusion tries to download the video while it is still uploading to Workfront, the scenario terminates with the IncompleteDataError.

## Run time error

<pre>RuntimeError</pre>If any other error (not mentioned above) appears during scenario execution, it is reported as a RunTimeError.

If a scenario terminates with the RuntimeError, its further behavior will depend on its setting of Max number of consecutive errors. For more information, see [Number of consecutive errors](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) in the article [The scenario settings panel in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>If a scenario starts with an instant trigger, the setting of Max number of consecutive errors is ignored and the scenario is deactivated immediately once the first error has occurred. For more information, see [Instant triggers](../../workfront-fusion/modules/module-types.md#instant) in the article [Types of modules](../../workfront-fusion/modules/module-types.md).

## Inconsistency Error

<pre>InconsistencyError</pre>If any error described above occurs during the commit or rollback phase, a scenario will terminate with Inconsistency Error. For more information, see [Scenario execution, cycles, and phases in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

If this error appears in a scenario, the execution of the scenario is immediately stopped.

## Warning

While executing a scenario, you may receive a warning informing you about a problem. However, it does not prevent the scenario from being successfully completed.

For example, a warning can appear when the maximum allowed file size is exceeded and the Enable data loss option is disabled. For more information, see [Enable data loss](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in the article [The scenario settings panel in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
