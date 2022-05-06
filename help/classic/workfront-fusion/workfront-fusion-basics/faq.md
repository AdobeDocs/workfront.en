---
filename: faq
content-type: faq
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Adobe Workfront Fusion FAQ
description: You must have the following access to use the functionality in this article:
---

# Adobe Workfront Fusion FAQ

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

## What is a scenario?

### Answer

A scenario defines a sequence of steps to be executed by Adobe Workfront Fusion. For each scenario, you specify the data source, how the data is to be processed, and what data is to be used and what is to be ignored. Workfront Fusion lets you create as complex of scenarios as you need; even the most sophisticated scenarios are possible.

For more information, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Can I use more than one module in a scenario? Or just a trigger and action?

### Answer

You can use as many modules as you want in a scenario. You can create independent routes and specify which data should flow through them. You can also use results returned by individual actions and then pass them on to the next action.

## Can Workfront Fusion work with files?

### Answer

Yes. Using Workfront Fusion, files can be received, saved, transformed, converted, encrypted, and so on. Moreover, Workfront Fusion provides a wide range of built-in features designed to enable users to work effectively and creatively with the data contained in the files.

For more information, see [About mapping files in Adobe Workfront Fusion](../../workfront-fusion/mapping/about-mapping-files.md).

## What happens if I let Workfront Fusion process an email containing more than one attachment?

### Answer

If you use the Email module Retrieve attachments, each attachment is sent individually through the rest of the modules in the scenario. Similar modules are also available in other apps that receive multiple files at once.

For more information, see [Email modules](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Some triggers allow scenarios to run instantly. What does "instantly" mean?

### Answer

Common scenarios are run at intervals according to the schedule you specify (for example, every hour, every 5 minutes, once a month, and the like). There are special triggers, called instant triggers (webhooks), that can start your scenario immediately after they receive data from a given service. Instant triggers can be extremely useful. We recommend to use them whenever possible. They help to reduce the number of operations. Received data is processed immediately without waiting for the next scheduled run. For example, the Google Sheets module Watch Changes starts a scenario immediately after a cell us updated.

## What are aggregators?

### Answer

An Aggregator merges data into one single collection. An example of this is files being compressed into a zip archive and sent as an email attachment.

For more information, see [Aggregator module in Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## What is an operation?

### Answer

An operation is any task performed by a module. An operation occurs, for example, every time a trigger runs and every time an action performs a task.

## What is data transfer?

### Answer

Data transfer refers to the amount of data transferred through your scenario. For example, suppose you have a scenario that retrieves a 100KB image from FTP and reduces its size to 50KB and saves both images to Dropbox. The amount of data used in this scenario is 150KB.

## What is a connection?

### Answer

A connection is the link between your Workfront Fusion account and the third-party service you want to use. The connection can be easily created when editing a scenario. To add a connection, click the **Add** button in the module setting and follow the step-by-step instructions.

For more information, see [About connecting Adobe Workfront Fusion to an app or service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
