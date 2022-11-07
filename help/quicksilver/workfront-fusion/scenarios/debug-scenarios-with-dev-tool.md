---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Debug scenarios with the Adobe Workfront Fusion DevTool
description: The Adobe Workfront Fusion DevTool allows you to understand and troubleshoot scenarios. The DevTool adds an extra panel to the Chrome Developer Tools. Using this debugger panel, you can check all the manual runs of your scenario, review all the performed operations, and see the details of every API call performed. You can see which module, operation, or single response caused the error, and use that knowledge to refine your scenario.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
---
# Debug scenarios with the [!DNL Adobe Workfront Fusion] DevTool

The [!DNL Adobe Workfront Fusion] DevTool allows you to understand and troubleshoot scenarios. The DevTool adds an extra panel to the [!DNL Chrome Developer Tools]. Using this debugger panel, you can check all the manual runs of your scenario, review all the performed operations, and see the details of every API call performed. You can see which module, operation, or single response caused the error, and use that knowledge to refine your scenario.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Install the [!DNL Chrome] DevTool extension

To use the [!DNL Workfront Fusion] DevTool, you first need to install it.

1. Click [this link](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/workfront-fusion-devtool.zip) to download the extension.
1. When the files have downloaded, extract them to a folder of your choice.
1. Open a tab in [!DNL Chrome]
1. In the search bar of the tab, enter `chrome://extensions`.
1. Click the **[!UICONTROL Developer mode]** toggle at the upper-right of the screen to enable Developer mode. If the toggle to the right, developer mode is enabled.
1. Click **[!UICONTROL Load unpacked]**.
1. Select the folder containing the DevTool (where you extracted the files in step 2).

   Once unpacked, the DevTool appears among your other Chrome extensions.

## Locate the [!DNL Workfront Fusion] DevTool

To use the [!DNL Workfront Fusion] DevTool, you must add the [!DNL Workfront Fusion] DevTool extension to your [!DNL Chrome] browser, as described in [Install the Chrome DevTool extension](#install-the-dnl-chrome-devtool-extension).

1. Open your [!DNL Workfront Fusion] scenario.
1. Open [!DNL Chrome Developer Tools]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Command + Option + I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Control + Shift + I</p> <p> Or </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >We recommend docking the [!DNL Chrome Developer Console] to the bottom to maintain a better view of your modules.

1. Click the **[!DNL Workfront Fusion]** tab in [!DNL Chrome Dev Tools].

## Use the [!DNL Workfront Fusion] DevTool

Workfront Fusion DevTool is divided into 3 main sections. You can find these in the left panel of your DevTool window.

* [Live Stream](#live-stream) 
* [Scenario Debugger](#scenario-debugger) 
* [Tools](#tools)

### Live Stream 

Live Stream displays what is happening in the background when you click Run once in your scenario.

1. Click the **[!UICONTROL Live Stream]** icon ![](assets/live-stream-icon.png) to open the Live Stream section.
1. Do any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Action</th> 
      <th>Instructions</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">View request information</td> 
      <td> <p>You can view the following information for each module in your scenario</p> 
       <ul> 
        <li> <p>Request Headers (API endpoint URL, http method, time and date the request was called, request headers, and query string)</p> </li> 
        <li> <p>Request Body</p> </li> 
        <li> <p>Response Headers</p> </li> 
        <li> <p>Response Body</p> </li> 
       </ul> <p>To view this information, click the appropriate tab in the right panel of the [!DNL Workfront Fusion] DevTool.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Search requests and responses</p> </td> 
      <td> <p>Enter the search term into the search field in the left panel of the [!DNL Workfront Fusion] DevTool to display only requests that contain the search term.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Remove list of requests </p> </td> 
      <td> <p>Click the trash bin icon in the top-right corner of the DevTool's left panel to clear the list of requests recorded by the [!DNL Workfront Fusion] DevTool. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Enable Console Logging</p> </td> 
      <td> <p>Click the computer icon <img src="assets/console-computer-icon.png"> in the top-right corner of the DevTool's left panel.</p> <p>Logging in the console is enabled when the computer icon is green.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Retrieve the Request in the Raw JSON Format or cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>Raw JSON</strong> </p> <p>Click <strong>[!UICONTROL Copy RAW]</strong> in the upper-right corner of the DevTool's right pane.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Click <strong>[!UICONTROL Copy cURL]</strong> in the upper-right corner of the DevTool's right pane.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Scenario Debugger 

The Scenario Debugger is useful for more complex scenarios. It displays the history of the scenario runs and enables you to search modules by their name or ID.

1. Click the **[!UICONTROL Scenario Debugger]** icon ![](assets/scenario-debugger-icon.png) to open the Scenario Debugger.
1. (Optional) Enter the search term (name or module ID) in the search field in the left pane of [!DNL Workfront Fusion] DevTool in the [!UICONTROL Scenario Debugger] section.
1. Double-click the module's name to open its settings in the scenario editor.
1. View request details by clicking the desired operation.

### Tools

The [!DNL Workfront Fusion] DevTool features tools that make setting up your scenario easier.

1. Click the **[!UICONTROL Tools]** icon ![](assets/console-tools-icon.png) to open the Tools. 
1. Select the tool you want to use
1. Configure the fields as detailed below.
1. Click **[!UICONTROL Run]**.

Tools and their fields:

* [Focus a Module](#uicontrol-focus-a-module) 
* [Find Modules by Mapping](#uicontrol-find-modules-by-mapping) 
* [Get App Metadata](#uicontrol-get-app-metadata) 
* [Copy Mapping](#uicontrol-copy-mapping) 
* [Copy Filter](#uicontrol-copy-filter) 
* [Swap Connection](#uicontrol-swap-connection) 
* [Swap Variable](#uicontrol-swap-variable) 
* [Swap App](#uicontrol-swap-app) 
* [Base 64](#uicontrol-base-64) 
* [Copy Module Name](#uicontrol-copy-module-name) 
* [Remap Source](#uicontrol-remap-source) 
* [Highlight App](#uicontrol-highlight-app) 
* [Migrate GS](#uicontrol-migrate-gs)

#### [!UICONTROL Focus a Module]

Opens settings of the specified module by ID.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Module ID]</td>
        <td>Enter the ID of the module for which you want to open settings.</td>
    </tr>
</table>

#### [!UICONTROL Find Modules by Mapping]

Allows you to search modules' values for a specified term. The output contains IDs of modules that contain the term you have searched for.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Keyword]</td> 
   <td> <p> Enter the term you want to search for. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Use Only Values]</p> </td> 
   <td> <p>Enable this option to only search in module fields' values.</p> <p>Disable this option to also search in module fields' names.</p> <p>The search is performed through the name and label parameters.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get App Metadata]

Retrieves metadata of the app by the app's module name or ID. This is useful, for example, when you need to know the version of the app used in your scenario.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Select the module for which you want to retrieve metadata.</td>
    </tr>
</table>

#### [!UICONTROL Copy Mapping]

Copies values from the source module to the target module.

>[!CAUTION]
>
>Make sure you set the correct source and target modules. If you select a different type of module, values in the target module will be deleted.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Select the module or enter the ID of the module from which you want to copy field values.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Select the module or enter the ID of the module into which you want to insert the source module values.</p> <p>Important: Values in the target module will be overwritten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copy Filter]

Copies the filter settings from the source module to the target module.

>[!NOTE]
>
>The copy action is performed on the filter placed on the left side of the selected module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Select the module or enter the ID of the module from which you want to copy filter values.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Select the module or enter the ID of the module into which you want to insert the filter values from the source module.</p> <p>Important: Values in the target module will be overwritten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Preserve Fallback Route setting]</p> </td> 
   <td> <p>The source filter is set as the fallback route. Enable this option to also set the the target filter is set as the fallback route.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Swap Connection]

Duplicates a connection from the source module to every module in the scenario of the same app.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Select the module or enter the ID of the module from which you want to duplicate the connection.</td>
    </tr>
</table>

#### [!UICONTROL Swap Variable]

Searches for specified variables in the scenario and replaces them with a new variable.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable to Find]</td> 
   <td> <p> Locate the variable pill that you want to replace from the module in your scenario and copy it to this ([!UICONTROL Variable to Find]) field. In the field, it appears with double curly brackets. Example: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace With]</p> </td> 
   <td> <p>Locate the variable pill that you want to replace the variable with from the module in your scenario and copy it to this ([!UICONTROL Variable to Find]) field. In the field, it appears with double curly brackets. Example: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module]</p> </td> 
   <td> <p>Select the module in which you want to replace the variable. If no module is selected, the variable will be replaced in the entire scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Swap App]

Replaces the selected app version in your scenario with another app version.

This can be used, for example, to upgrade Gmail and Email apps' modules to the latest version.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App to be Replaced]</td> 
   <td> <p> Select the app that you want to replace.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace with]</p> </td> 
   <td> <p>Select the app that you want to replace it with.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Allows you to encode the entered data to Base64 or to decode Base64. Some requests are encoded to Base64. This tool can be useful when you want to search for particular data in the encoded request.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>Select whether you want to encode the data from the [!UICONTROL Raw Data] field to Base64 or decode Base64 to Raw Data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Raw Data]</p> </td> 
   <td> <p> Enter the data you want to encode to Base64, or Base64 if you want to decode to raw data, depending on the option selected in the [!UICONTROL Operation] field above.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copy Module Name]

Copies the name of the selected module to your clipboard.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module] </td> 
   <td> <p>Select the module that you want to copy the name of.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remap Source]

Allows you to change the mapping source from one module to another.

You must first add the module you want to use as a source module to the route in your scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module] </td> 
   <td> <p> Select the module you want to be replaced as the mapping source for other modules in your scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Select the module you want to use as a new mapping source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module to Edit]</p> </td> 
   <td> <p>Select the module you want to change the mapping for if you don't want to change the mapping in the entire scenario. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Highlight App]

Highlights modules of the specified app in your scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App to be Highlighted] </td> 
   <td> <p> Select the app you want to be highlighted in your scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Version] </p> </td> 
   <td> <p>Select the version of the app you want to be highlighted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Highlight Color]</p> </td> 
   <td> <p> Enter the color hex you want to use for highlighting modules.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migrate GS] 

This tool is made especially to upgrade [!DNL Google Sheets] (legacy) modules to the latest [!DNL Google Sheets] version. It adds a new version of the module just after the legacy version of the module in the scenario route.

This module does not require that you set any parameters.
