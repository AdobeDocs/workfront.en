---
filename: throw
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Throw
description: In some cases you may want to forcibly stop the scenario execution followed by Rollback or Commit phase or to stop the processing of a route and optionally store it in the queue of View and resolve incomplete executions.
---

# Throw

In some cases you may want to forcibly stop the scenario execution followed by [Rollback](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) or [Commit](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) phase or to stop the processing of a route and optionally store it in the queue of [View and resolve incomplete executions](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Currently the [Directives for error handling](../../workfront-fusion/errors/directives-for-error-handling.md) cannot be used out of the scope of an [Error handler route](../../workfront-fusion/errors/error-handling.md#error) and `Adobe Workfront Fusion` does not offer a module that would enable you to easily conditionally generate (throw) errors.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront Fusion</span> license**</td> 
   <td> <p><span>Workfront Fusion for Work Automation and Integration</span> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <span>Adobe Workfront Fusion</span> as well as <span>Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

&#42;&#42;For information on `Adobe Workfront Fusion` licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Workaround for Throw

To conditionally throw an error, you may configure a module to make it optionally purposely fail during its operation. One possibility is to employ the JSON >&nbsp;Parse JSON module (see [JSON modules](../../workfront-fusion/apps-and-their-modules/json-modules.md)), configured to optionally throw an error (BundleValidationError in this case):

<!--

-->

You can then attach one of the [Directives for error handling](../../workfront-fusion/errors/directives-for-error-handling.md) to the error handling route to:

* force the scenario execution to stop and perform the rollback phase: Rollback
* force the scenario execution to stop and perform the commit phase: Commit
* stop the processing of a route: Ignore
* stop the processing of a route and store it in the queue of [View and resolve incomplete executions](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md): Break

The following example shows the use of the Rollback directive:

![](assets/rollback-directive-350x175.png)

