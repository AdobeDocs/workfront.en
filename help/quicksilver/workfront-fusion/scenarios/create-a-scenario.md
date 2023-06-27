---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Create a scenario in Adobe Workfront Fusion
description: The following tasks explain how to create a [!DNL Adobe Workfront Fusion] scenario.
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
---
# Create a scenario in [!DNL Adobe Workfront Fusion]

The following tasks explain how to create a [!DNL Adobe Workfront Fusion] scenario.

For a practice exercise that walks you through creating an automation scenario, see [Create a practice automation scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

For a practice exercise that walks you through creating an integration scenario using data that we provide, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>To create a scenario from a template, see [Create scenarios with [!DNL Adobe Workfront Fusion] templates](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>    </td> 
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

## Begin creating a scenario

1. Click **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) in the left panel.

1. Click **[!UICONTROL Create a new scenario]** in the upper-right corner of the page.
1. In the screen that appears (the scenario editor), if you are creating a new scenario, click **[!UICONTROL New scenario]** in the upper-left corner and type a name for the scenario.
1. Continue on to [Add a module in a scenario](#add-a-module-in-a-scenario).

## Add a module in a scenario

1. To add the first module to the scenario, click the question mark icon. ![](assets/question-mark-icon.gif)

   Or

   To add additional modules to the scenario, click the handle on the right side of the module you want it to follow.

1. In the box that displays, find and click the app or service that you want to start with.

   Any previously selected apps are displayed in the box for easy access, and in the **[!UICONTROL Favorites]** section at the bottom of the screen.

   If you click **[!UICONTROL Add another module]**, the modules that display depend on where in the scenario you are adding the module. Some modules can be placed only in between other modules, and others only at the beginning of the scenario.

   >[!TIP]
   >
   >The two most common types of modules are actions and triggers. For more information, see [Types of modules](../../workfront-fusion/modules/module-types.md).

1. In the list of modules that displays, click the first module you want to add to the scenario.

   The modules that display depend on where you want to add a module in your scenario. Some modules can be placed only in between other modules, and others only at the beginning of the scenario.

   The two most common types of modules are actions and triggers. For more information, see [Types of modules](../../workfront-fusion/modules/module-types.md).

1. Continue on to [Connect the module's app or web service to [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## Connect the module's app or web service to [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Workfront Fusion modules that connect to an app (such as [!DNL Workfront], [!DNL Salesforce], or [!DNL Jira)] feature the [!UICONTROL Connection] field. Here, you can specify the connection that you want this module to use to connect to the app. You can select an existing connection from the dropdown, or create a new connection.

When you select or create a connection for an app in a scenario, other modules for that app automatically use the same connection unless you select a different one when setting up the later modules.

For more information, see [About connecting [!DNL Adobe Workfront Fusion] to an app or service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

To create a connection inside a [!DNL Workfront Fusion] module:

1. Click **[!UICONTROL Add]** to open the **[!UICONTROL Create a connection]** box.
1. (Optional) Change the default **[!UICONTROL Connection name]**.
1. (Conditional) If the app requires advanced connection settings, such as an ID, key, or [!UICONTROL secret], enter that information.

   You might need to click **[!UICONTROL Show advanced settings]** to display the fields where you can enter this kind of information.

1. Click **[!UICONTROL Continue]**.
1. In the sign-in window that displays, enter your credentials to log in to the app if you haven't already done so.
1. (Conditional) If an **[!UICONTROL Allow]** button displays, examine the actions that the connector will be able to take, then click the button to connect the app to [!DNL Workfront Fusion].
1. Continue on to [Configure the module](#configure-the-module).


## Configure the module

1. In the fields below the Connection field, configure the settings for the module, then click **[!UICONTROL OK]**.

   ![](assets/conf-settigs-mod-350x547.png)

   These settings are different for every module. A bolded title indicates a required setting.

   >[!TIP]
   >
   >As you work on your scenario, you can click the module to display this box of settings at any time.
   >
   >
   >If you see a black circle on a module, you haven't finished configuring its settings. Click the module to open it and continue configuring.
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. If you are adding the first module in your scenario, select an option to indicate where you want the scenario to start each time it runs.

   ![](assets/choose-where-start-350x194.png)

1. Repeat the steps in the sections [Add a module in a scenario](#add-a-module-in-a-scenario) and [Configure the module](#configure-the-module) to add other modules to the scenario.

1. (Optional) Copy and paste a module or group of modules.

   For more information, see [Copy modules or scenarios in Adobe Workfront Fusion](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Continue on to [Configure and work with your scenario](#configure-and-work-with-your-scenario).

## Configure and work with your scenario

1. Do any of the following to configure your scenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Specify when and how often the scenario will execute</td> 
      <td> <p>Click the clock icon. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>For more information, see <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Schedule a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Set up a route</td> 
      <td> <p>Click the wrench icon <img src="assets/wrench-icon.gif"> between the two modules and use any of the following options. For more information, see <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Add a filter to a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL Set up a filter]</strong>: Control which bundles are used at certain points in the scenario.</li> 
        <li><strong>[!UICONTROL Unlink]</strong>: Removes a route.</li> 
        <li><strong>[!UICONTROL Add a router]</strong>: Adds a router between modules. </li> 
        <li><strong>[!UICONTROL Add a module]</strong>: Adds a new module between modules.</li> 
        <li><strong>[!UICONTROL Add a note]</strong>: Adds a note to the route.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configure the scenario settings</td> 
      <td>Click the [!UICONTROL Scenario settings] icon. <img src="assets/gear-icon-settings.png"> These settings are intended primarily for advanced users. For more information, see <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">The scenario settings panel in [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configure Flow Control settings</td> 
      <td> <p>Click the [!UICONTROL Flow Control] icon. <img src="assets/flow-control-icon.gif"> You can set a task to repeat a given number of times, convert an array into a series of bundles, and merge several bundles into one single bundle. For more information, see <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Flow control in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enhance the scenario using advanced tools</td> 
      <td>Click the [!DNL Tools] icon. <img src="assets/tools-icon.gif"> You can create triggers, actions, aggregators, and transformers. For more information, see <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Tools</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">User text parsing tools</td> 
      <td>Click the [!DNL Text parser] icon <img src="assets/text-parser-icon.gif">. You can retrieve elements from HTML code, find and extract string elements matching a search pattern, search and replace text, and "scrape" data from a website. For more information, see <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Tools</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Do any of the following to work with your scenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">View a log of the events that occur when the scenario runs</td> 
      <td> <p>Click the [!UICONTROL Exit editing] arrow <img src="assets/exit-editing-arrow.png"> in the scenario editor to view the Scenario detail page. The log displays at the bottom of the window, or in the lower-right corner. It contains information about each phase and any errors encountered during the execution of the scenario.</p> <p>To return to working with your scenario in the [!DNL scenario editor], click anywhere on the Scenario detail page.</p> <p>For more information about the Scenario detail page, see <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Scenario details in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access your most commonly used apps and services</td> 
      <td> Click an icon in the <strong>[!UICONTROL Favorites]</strong> section at the bottom of the screen. Icons display in this section automatically as you add apps and services to your scenario. You can also click the [!UICONTROL Add] icon <img src="assets/add-icon.gif"> to add apps and services to this area manually.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">View an animation showing how data flows through the scenario</td> 
      <td>Click the [!UICONTROL Explain flow] icon <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Auto-align the layout of the modules </td> 
      <td>Click the [!UICONTROL Auto-align] icon <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type or view notes about the scenario</td> 
      <td>Click the [!UICONTROL Notes] icon <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Remove a module</td> 
      <td>Right-click the module, then click <strong>[!UICONTROL Delete module]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. To test-run the scenario, click **[!UICONTROL Run once]**.

   It's important to verify that the scenario runs as you expect before you activate it. Once activated, the scenario will execute according to its schedule. If everything does not run as expected, see [Error handling in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. When you finish editing the scenario (or at any time while you are editing), click the [!UICONTROL Save] icon at the bottom of the window ![](assets/save-icon.gif).

For information about activating a scenario, see [Activate or deactivate a scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Workfront Fusion scenario keyboard shortcuts

You can use the following keyboard shortcuts when creating or editing a scenario:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>Action</p> </th> 
   <th>[!DNL Windows]</th> 
   <th> <p>[!DNL MacOS]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Save] </td> 
   <td>Ctrl+Shift+S</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Run Once]</td> 
   <td>Ctrl+Shift+Enter</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+Enter</span> </td> 
  </tr> 
 </tbody> 
</table>
