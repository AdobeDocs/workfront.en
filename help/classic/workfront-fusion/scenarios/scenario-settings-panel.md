---
filename: scenario-settings-panel
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: The scenario settings panel in Adobe Workfront Fusion
description: You must have the following access to use the functionality in this article - EDIT ME.
---

# The scenario settings panel in Adobe Workfront Fusion

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

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

## Open the scenario settings

1. Open the scenario editor, as explained in [The scenario editor in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-editor.md).
1. Click the gear icon near the lower-left corner of the page.

   ![](assets/scenario-settings-350x221.png)

   In the Scenario settings panel that displays, you can configure various advanced settings for the scenario.

## Allow storing incomplete executions

This option determines how Adobe Workfront Fusion proceeds if an error occurs during the execution of a scenario. With this option enabled, the scenario is paused and moved to [View and resolve incomplete executions in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). This gives you the possibility to fix the issue and continue executing from where the scenario was stopped. If this option is disabled, the scenario run stops and a rollback phase is started.

## Sequential processing

This option determines how Workfront Fusion proceeds if an error occurs and the execution of a scenario is moved to the [View and resolve incomplete executions in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). If the Sequential processing option is enabled, Workfront Fusion stops processing the task sequence altogether until all incomplete executions are resolved. If the Sequential processing option is disabled, the scenario continues to run according to its schedule, accompanied by repeated attempts to rerun the incomplete executions.

For more information on scheduling, see [Schedule a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Data is confidential

Once a scenario has been executed, you can by default display information about which data was processed by modules in the scenario. If you do not want this information to be stored, enable the Data is confidential option.

For more information about displaying information, see [Scenario execution flow in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>If you enable this option, it is difficult to solve errors that may occur during the execution of a scenario.

## Enable data loss

This option has to do with enabling data loss if Workfront Fusion fails to save a bundle to the queue of [View and resolve incomplete executions in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (for example, due to a lack of free space). With this option enabled, the data is lost in order to prevent interruptions in the overall scenario execution. This is useful for scenarios where the highest priority is continuous execution and the incoming erroneous data is not that important.

Beyond that, when executing a scenario, a module can sometimes encounter a file that is larger than the maximum allowed size. In this case, Workfront Fusion proceeds in accordance with the setting of the Enable data loss option and a warning message is shown.

For more information about maximum file size, see [About mapping files in Adobe Workfront Fusion](../../workfront-fusion/mapping/about-mapping-files.md).

For more information on warnings, see [Error processing in Adobe Workfront Fusion](../../workfront-fusion/errors/error-processing.md).

## Auto commit

The Auto commit settings applies to transactions and defines the way to process a scenario. If the Auto commit option is on, the commit phase on each module starts immediately after completing the operation phase. With the Auto commit option disabled, no commit occurs until operations are executed for all modules (this is the default mode).

For more information on transactions, see [Scenario execution, cycles, and phases in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Maximum number of cycles

Setting more cycles can be useful when you want to prevent connection interruption to a third-party service and assure that all records are processed within the one scenario run.

* If the scenario starts with a polling trigger, the setting defines the maximum number of cycles allowed during the scenario execution.

  For more information on polling triggers, see [Polling triggers](../../workfront-fusion/modules/module-types.md#polling) in [Types of modules](../../workfront-fusion/modules/module-types.md).

* If the scenario starts with an instant trigger, the setting is ignored and all the pending events are processed during a single scenario execution, one event per one cycle.

  For more information on instant triggers, see [Instant triggers](../../workfront-fusion/modules/module-types.md#instant) in [Types of modules](../../workfront-fusion/modules/module-types.md).

* If the scenario does not start with a trigger (instant/polling), the specified maximum number of cycles is always performed.

``` ```**Examples: **`````` Workfront > Watch record watches for new issues that come in, and Workfront > Convert object converts the new request into a project and assigns it the appropriate template.

![](assets/scenario-settings-ex-1-350x157.png)

>[!NOTE]
>
>A more cycles setting is applied only when you schedule your scenario execution. When you use the Run once button, cycle settings are taken into account.

### Max number of cycles is set to 1 (default)

![](assets/max-number-cycles-1-350x201.png)

The Maximum number of returned files in the Dropbox > Watch files module is set to 

```
10
```

.

![](assets/max-number-cycles-10-350x175.png)

If 100 requests are submitted to Workfront, and the Limit field is set to 10, then 90 files are left unprocessed after one scenario run. The next 10 files are processed in the next scheduled scenario execution.

###  Max number of cycles is set to 10

The Maximum number of returned files in the Dropbox > Watch files module is set to 

```
10
```

.

If 100 files are added to the Dropbox folder and the Maximum number of returned files option is set to 10, then 10 files are processed during the first cycle, the next 10 files in the second cycle, the next 10 files in the third cycle and so on, until all files are processed.

All files are processed within 1 scenario run.

You can see the already-run cycles in the Scenario details:

![](assets/scenario-detail-350x207.png)

For more information about this page, see [Scenario details in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-detail.md).

## Number of consecutive errors

Defines the maximum number of consecutive execution attempts before the execution of a scenario is deactivated (excluding DataError, DuplicateDataError and ConnectionError).

For more information on errors, see [Error processing in Adobe Workfront Fusion](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>If a scenario starts with an instant trigger, the setting is ignored and the scenario is deactivated immediately once the first error has occurred.

