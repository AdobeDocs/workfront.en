---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Basic terms in Adobe Workfront Fusion
description: Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
---
# Basic terms in [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requires an [!DNL Adobe Workfront Fusion] license in addition to an [!UICONTROL Adobe Workfront] license.


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Action</p> </td> 
   <td>A module that allows you to read or write bundles from or into a selected app or service.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Aggregator]</p> </td> 
   <td> <p>A type of module that merges together multiple bundles (multiple arrays of data) into one single bundle. For more information, see <a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">[!UICONTROL Aggregator] module in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API Key</td> 
   <td>A unique code that identifies the user, developer, or program that is calling a software's API, used for authentication. Since [!DNL Adobe Workfront Fusion] modules work by connecting APIs, API keys are sometimes necessary. API keys are distributed by the app that requires them. For example, if you need an API key for [!DNL ActiveCampaign], you would request it though your [!DNL ActiveCampaign] account.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">App or service</td> 
   <td> <p>A software application, most commonly.</p> <p>An app can also be a special function that manipulates data, such as an iterator or an aggregator. </p> <p>A service is a source of bundles that might include a web API, web page, different types of servers (FTP, SMTP, IMAP), and so on. </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">App connector</td> 
   <td>An app that connects to another system.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bundle</p> </td> 
   <td> <p>A bundle is a basic unit that is returned or received by modules. A bundle consists of items.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>When adding an app or service to a scenario, most likely you will have to first create a connection between [!DNL Workfront Fusion] and the app or service in order to retrieve or send the selected data. For more information, see <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">About connecting [!DNL Adobe Workfront Fusion] to an app or service</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Cycle</p> </td> 
   <td> <p>A cycle refers to two phases of the scenario run: operation and commit. The scenario may consists of one or more cycles. For more detailed information, see <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Scenario execution, cycles, and phases in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Data Store</p> </td> 
   <td> <p>A tool that stores data from scenarios or allows you to transfer data between individual scenarios or scenario runs. For more information, see <a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">Data Stores in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Data Transfer</p> </td> 
   <td> <p>The amount of data transferred through your scenario. For more information, see <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Scenario details in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Filter</p> </td> 
   <td> <p>Additional features that can be applied between two modules. A filter allows you to then only work with bundles that fit certain criteria. There are a number of different filters you can apply. For more information, see <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Add a filter to a scenario in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID</p> </td> 
   <td> <p>A name that is used to uniquely identify a bundle. An ID is usually used to differentiate a bundle that is to be updated or deleted from a given service.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Items</p> </td> 
   <td> <p>A part of a bundle. Bundles can consist of multiple items. There are several different types of items: text, number, boolean (yes/no), date, time, buffer (binary data), collections, select menu, array, and validation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Iterator]</p> </td> 
   <td> <p>A type of module that allows you to take one bundle of data (an array of data) and divide into separate bundles. For more information, see <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator] module in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Module</p> </td> 
   <td> <p>A single step within a scenario that performs a function, such as creating a record, within the associated app or service.</p> <p>Each app or service has various modules that define the way it responds to a request.</p> <p>There are 4 types of modules: actions, triggers, iterators, and aggregators.</p> <p> <img src="assets/module.jpg"> </p> <p>For more information, see <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Types of modules</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Operation</p> </td> 
   <td> <p>A task performed by a module.</p><p>For more information, see <a href="../../workfront-fusion/get-started/operations-in-workfront-fusion.md" class="MCXref xref">Operations in [!DNL Adobe Workfront Fusion]</a>.</p>
  </tr> 
  <tr> 
   <td role="rowheader">Public/Private Keys</td> 
   <td>Public and private keys are used to encrypt and decrypt data. The public key can be distributed, and anyone with the public key can encrypt data, but only the private key can decrypt it. Similarly, a user with a private key can encrypt data that anyone with the public key can decrypt. The private key encryption assures that the data came from the owner of the private key and serves as validation of the data's source.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Router]</p> </td> 
   <td>Allows you to duplicate data or add new routes to a scenario, so to re-route data and handle different groups of data separately. For more information, see <a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">[!UICONTROL Router] module in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Scenario</p> </td> 
   <td> <p>A user-created series of automated steps, each represented and performed by a module. The purpose of a scenario is to move and manipulate data.</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> For more information, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in[!UICONTROL  Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transactions</p> </td> 
   <td> <p>[!DNL Workfront Fusion] uses transactional processing to capture the scenario lifecycle. A transaction consists of several phases during which data is transformed from one consistent state into another consistent state. There are 4 phases: initalization, operation (reading or writing), commit/rollback, and finalization.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Trigger</p> </td> 
   <td> <p>A module that allows you to grab bundles that were added or updated since the last run of a scenario. There are 2 types of triggers: polling and instant (webhooks). For more information, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant triggers (webhooks) in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>A special type of trigger that allows you to run a scenario immediately after a new bundle is available. For more information, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant triggers (webhooks) in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
