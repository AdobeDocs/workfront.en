---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Operations in Adobe Workfront Fusion
description: An operation in Adobe Workfront Fusion is a task performed by a module. For tracking purposes, any successful action performed by a module is an operation.
author: Becky
feature: Workfront Fusion
exl-id: b6000f2d-8154-4402-9898-97f7350bfeac
---
# Operations in [!DNL Adobe Workfront Fusion]

An operation in [!DNL Adobe Workfront Fusion] is a task performed by a module. For tracking purposes, any successful action performed by a module is an operation.

## Considerations when counting the number of operations

* In general, any successful action-step execution is considered an operation.

* The first module in a scenario runs only once and is always counted as one operation, even if it does not return a bundle. 

* The number of times the rest of the modules run depends on the number of bundles they must process.  One run of a module for one bundle is one operation. An exception is the aggregator module, which is counted as one operation per set of bundles being processed.

* Operations are counted at the [!UICONTROL Finalization] stage of a scenario execution.

* The following are **not** counted as operations:

  * Any filter steps.

  * Any action that errors or halts.

  * Any route that does not run because the route's rules were not met, such as fallback or disabled routes.

  * Any action that does not run, either because a filter didn't allow data through or because the scenario stopped due to an error.

## Operation limits

Your organization may have a monthly operations limit. This is based on the [!DNL Workfront] plan that your organization purchased. The [!UICONTROL Ultimate] [!DNL Workfront] plan offers unlimited operations.

If your organization has a monthly limit, you will be notified when you near the limit. If you go over the limit, [!DNL Workfront] will contact your organization to ensure that your plan meets your needs.

## View the number of operations performed in the last 30 days

You can see a graphs showing the number of operations performed. These graphs are available in the following locations:

* **Organization dashboard**: Operations used by the entire organization
* **Team dashboard**: Operations used by scenarios owned by this team ([!DNL Adobe Experience Cloud] only)
* **Scenario details page**: Operations used by this scenario ([!DNL Adobe Experience Cloud] only)
