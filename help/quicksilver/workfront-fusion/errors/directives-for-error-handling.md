---
filename: directives-for-error-handling
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Directives for error handling in Adobe Workfront Fusion
description: You must have the following access to use the functionality in this article - EDIT ME.
---

# Directives for error handling in Adobe Workfront Fusion

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

## Directives for error handling

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Rollback</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>Scenario execution is stopped immediately and a <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">Rollback</a> phase is started on all the modules in an attempt to revert them all to their initial state. The subsequent modules are not processed.</p> <p>Barring a few error types, the scenario is deactivated after the number of consecutive errors specified under Scenario settings. For more information, see <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Number of consecutive errors</a>.</p> <p>The scenario execution status is marked as "error."</p> <p>Note: This is the default behavior if no error handler route is attached to the module and the <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Allow storing incomplete executions</a> setting under Scenario settings is not checked.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Commit</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>Scenario execution is stopped immediately and a commit phase is started on all modules. The subsequent modules are not processed.</p> <p>All unprocessed bundles are ignored.</p> <p>The scenario execution status is marked as "success." For information about commit phases, see <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Commit</a> in the article <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Scenario execution, cycles, and phases in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Resume</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>A substitute output is specified and supplied to the module that encounters an error.</p> <p>The subsequent modules are processed.</p> <p>The scenario execution status is marked as "success."</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ignore</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>The error is ignored and the subsequent modules are not processed.</p> <p>If there are unprocessed bundles, the scenario execution continues normally.</p> <p>The scenario execution status is marked as "success."</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Break</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>The state of the scenario execution is stored in the queue of incomplete executions where the error can be resolved manually. For more information, see <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">View and resolve incomplete executions in Adobe Workfront Fusion</a>. </p> <p>There are, however, some exceptions. For more information, see <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Allow storing incomplete executions</a> in the article <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">The scenario settings panel in Adobe Workfront Fusion</a>.</p> <p>The subsequent modules are not processed.</p> <p>If there are unprocessed bundles, the scenario execution continues normally.</p> <p>The scenario execution status is marked as "warning" when the Automatically complete execution option is disabled.</p> <p>See the <a href="#break" class="MCXref xref">Break</a> section below for further information.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Retry</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>In some cases it could be useful to re-execute a failing module for a couple of times when there is a chance that the reason for the failure might pass over time.</p> <p>Workfront Fusion currently does not offer the Retry directive, though several workarounds can be employed to mimic its functionality. For more information, see <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Retry error handling in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Currently the error handling directives cannot be used out of the scope of an error handling route and Workfront Fusion currently does not offer a Throw module that would enable you to easily conditionally generate (throw) errors, though a workaround can be employed to mimic its functionality. For more information, see [Error handler route](../../workfront-fusion/errors/error-handling.md#error) in the article [Error handling in Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md). Also see [Workaround for Throw](../../workfront-fusion/errors/throw.md#workarou) in the article [Throw error handling in Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).

## Break {#break}

When an error is handled by the Break directive, a record is created in the [View and resolve incomplete executions in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) folder which stores the state of the scenario execution along with data from the prior modules. For each bundle of data that causes the error, a separate record is created.

The record references the module where the error originated and contains information regarding what data was received by the module as input. For more information, see [View and resolve incomplete executions in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Here, you may resolve the error manually by updating the scenario (if needed) and running it once.

On the other hand, by enabling the Automatically complete execution option under the Break directive settings, it can be configured to automatically process an incomplete execution by re-executing the scenario after the specified number of minutes.

With this option enabled, when an error takes place, the incomplete execution is retrieved (after the time specified in the Interval between attempts field) and executed with the original input data. This will repeat until the execution of the module completes without an error or until the Number of attempts specified is reached.

When "Automatically complete execution" is turned on, the scenario run is marked as "Success" because the Break error handler's auto-retry is handling the issue automatically. In this case, users do not receive an email about the failed run.

When "Automatically complete execution" is turned off, the run is marked as "Warning". ![](assets/break-directive-350x241.png)

However, there are some exceptions to executions being stored under Incomplete Executions and with some error types, the auto-retry of a scenario execution is not possible. For more information, see [Allow storing incomplete executions](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) in the article [The scenario settings panel in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

For additional information, see [Advanced error handling in Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
