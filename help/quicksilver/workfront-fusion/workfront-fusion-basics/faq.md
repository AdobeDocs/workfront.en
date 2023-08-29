---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Adobe Workfront Fusion FAQ
description: This article addresses common questions related to [!DNL Adobe Workfront Fusion], including information about object commonly used in Fusion workflows
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
---
# Adobe Workfront Fusion FAQ

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

## What is a scenario?

### Answer

A scenario defines a sequence of steps to be executed by [!DNL Adobe Workfront Fusion]. For each scenario, you specify the data source, how the data is to be processed, and what data is to be used and what is to be ignored. [!DNL Workfront Fusion] lets you create as complex of scenarios as you need; even the most sophisticated scenarios are possible.

For more information, see [Create a practice integration scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Can I use more than one module in a scenario? Or just a trigger and action?

### Answer

You can use as many modules as you want in a scenario. You can create independent routes and specify which data should flow through them. You can also use results returned by individual actions and then pass them on to the next action.

## Can [!DNL Workfront Fusion] work with files?

### Answer

Yes. Using [!DNL Workfront Fusion], files can be received, saved, transformed, converted, encrypted, and so on. Moreover, [!DNL Workfront Fusion] provides a wide range of built-in features designed to enable users to work effectively and creatively with the data contained in the files.

For more information, see [About mapping files in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## What happens if I let [!DNL Workfront Fusion] process an email containing more than one attachment?

### Answer

If you use the [!UICONTROL Email] module [!UICONTROL Retrieve attachments], each attachment is sent individually through the rest of the modules in the scenario. Similar modules are also available in other apps that receive multiple files at once.

For more information, see [[!UICONTROL Email] modules](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Some triggers allow scenarios to run instantly. What does "instantly" mean?

### Answer

Common scenarios are run at intervals according to the schedule you specify (for example, every hour, every 5 minutes, once a month, and the like). There are special triggers, called instant triggers (webhooks), that can start your scenario immediately after they receive data from a given service. Instant triggers can be extremely useful. We recommend to use them whenever possible. They help to reduce the number of operations. Received data is processed immediately without waiting for the next scheduled run. For example, the [!DNL Google Sheets] module [!UICONTROL Watch Changes] starts a scenario immediately after a cell is updated.

## What are aggregators?

### Answer

An [!UICONTROL Aggregator] merges data into one single collection. An example of this is files being compressed into a zip archive and sent as an email attachment.

For more information, see [[!UICONTROL Aggregator] module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## What is an operation?

### Answer

An operation is any task performed by a module. An operation occurs, for example, every time a trigger runs and every time an action performs a task.

## What is data transfer?

### Answer

Data transfer refers to the amount of data transferred through your scenario. For example, suppose you have a scenario that retrieves a 100KB image from FTP and reduces its size to 50KB and saves both images to [!DNL Dropbox]. The amount of data used in this scenario is 250KB.

## What is a connection?

### Answer

A connection is the link between your [!DNL Workfront Fusion] account and the third-party service you want to use. The connection can be easily created when editing a scenario. To add a connection, click the **[!UICONTROL Add]** button in the module setting and follow the step-by-step instructions.

For more information, see [About connecting [!DNL Adobe Workfront Fusion] to an app or service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
