---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: scenario,performance
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion performance guardrails
description: The Adobe Workfront Fusion documentation has moved to a new location. This article has been deprecated, but contains a link to the new article that covers this functionality.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
---
# [!DNL Adobe Workfront Fusion] performance guardrails

>[!IMPORTANT]
>
>The Adobe Workfront Fusion documentation has moved to a new location. 
>
>The information in this article can now be found in the article:
>
>* [Adobe Workfront Fusion performance guardrails](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/scenarios/fusion-performance-guardrails.html)
>
>Please update any bookmarks.
>
>This article is no longer being updated, and will be removed in the near future.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requires an [!DNL Adobe Workfront Fusion] license in addition to an [!DNL Adobe Workfront license].

Work automation requires rapid processing, so [!DNL Adobe Workfront Fusion] is designed for high performance. Because long-running scenarios can slow down the pace of your work, we've designed [!DNL Workfront Fusion] with performance-preserving guardrails that limit execution time, data size, and other scenario parameters. [!DNL Workfront Fusion] designers should be aware of these guardrails and incorporate them into their design practices.

## Browsers

* Workfront Fusion supports only Chrome based browsers.

## Scenarios

* The default scenario execution timeout is **40 minutes**. When the execution reaches this timeout, [!DNL Workfront Fusion] interrupts scenario execution after the next cycle or operation, depending on the scenario. This forces the scenario to stop shortly after the 40 minute limit is reached
* The maximum size of a scenario blueprint is **5 MB**, but we recommend keeping scenario size under **3 MB**.

  App modules that create or update data with large numbers of fields can cause very large blueprints.

  * When using the [!DNL Workfront] app, be sure to only select fields needed for your create or update use cases. 
  * When using other apps, use custom API modules to interact with any record type that has a large number of fields.

* While there is no cap for the number of modules in a scenario, scenarios with more than 150 modules negatively impact the performance of your [!DNL Workfront Fusion] system. For this reason, we do not recommend creating scenarios with over 150 modules.

## Operations

* The default operation timeout is typically **40 seconds**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Files

* Fusion's total processing capacity for files is **1 GB**. The limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.
* Organizations on the Workfront Ultimate plan have access to increased file processing beyond 1 GB. The Fusion platform can support individual files up to 15GB for a single action (e.g. upload file), but there are other factors that affect data transfer. The file size limit of single action depends on the web service Fusion connects to. Data transfer is the total processing for a single execution. This means multiple actions in a single execution contribute to the total data transfer. Fusion will process files until the execution limit of 40 minutes is reached. 

   For more information, see [Working with large files in Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/fusion-large-files.md).


## Server Memory Usage

* Server memory usage for a single execution is limited to **1 GB**.

  Many factors, such as large files or complex modules, can affect server memory usage in ways that are difficult to predict or control. Because of this, your scenario execution may exceed the 1 GB memory limit, even if the scenario follows all other performance guardrails. Exceeding the memory limit causes the execution to fail.

## Webhooks

* The default maximum size of a payload is **5 MB**.
* Webhooks are limited to **100 requests per second**. When this limit is reached, Workfront Fusion sends a 429 ([!UICONTROL Too Many Requests]) status.
* [!DNL Workfront Fusion] stores webhook payloads for 30 days. Accessing a webhook payload more than 30 days after it was received results in the error "[!UICONTROL Failed to read file from storage.]"
* Webhooks are deactivated automatically if either of the following applies:

  * The webhook has not been connected to any scenario for more than 5 days
  * The webhook is used only in inactive scenarios, which have been inactive for more than 30 days.

* Deactivated webhooks are deleted and unregistered automatically if they are not connected to any scenarios and have been in deactivated status for over 30 days.

## Execution history

* Execution history logs are limited to a size of **100 MB**. If the execution history exceeds this size, only the first 100 MB will be shown.
* If a scenario has multiple concurrent executions. only 5 executions display in the Executions area of the scenario details page. This is true even when more than 5 executions are running.

## Incomplete executions

* Incomplete executions are limited to a total size of **500 MB**. If the 500 MB limit is reached, no more incomplete executions will be stored.

## Retries

* When using the Break module and specifying the Retry directive, if a scenario fails consecutively 10 times within a 2-minute timeframe, the scenario will be automatically deactivated.
 