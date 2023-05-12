---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Marketo modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Marketo], as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
---
# [!DNL Marketo] modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Marketo], as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] or higher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

## Prerequisites

To use [!DNL Marketo] modules, you must have a [!DNL Marketo] account.

## Connect [!DNL Marketo] to Workfront Fusion {#connect-marketo-to-workfront-fusion}

You can create a connection to your [!DNL Marketo] account directly from inside [!DNL Marketo] module.

1. In any [!DNL Marketo] module, click **[!UICONTROL Add]** next to the [!UICONTROL Connection] field.
1. Enter your [!DNL Marketo] account or [!DNL Marketo] [!UICONTROL Munchkin] ID. This is the unique part of the Base URL or Endpoint assigned to your account, that you use to access [!DNL Marketo] via its [!UICONTROL REST] API. For instructions on locating this, see [Base URL](https://developers.marketo.com/rest-api/base-url/) in the [!DNL Marketo] documentation.
1. Enter your [!UICONTROL Client ID] and [!UICONTROL Client secret]. For instructions on locating these, see [Authentication](https://developers.marketo.com/rest-api/authentication/) in the [!DNL Marketo] documentation.
1. Click **[!UICONTROL Continue]** to create the connection and go back to the module.

## [!DNL Marketo] Modules and their fields

When you configure [!DNL Marketo] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Marketo] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Searches](#searches)

### Triggers

* [[!UICONTROL Watch records]](#watch-records)
* [[!UICONTROL Watch events (Instant)]](#watch-events-instant)

#### [!UICONTROL Watch records]

This trigger module starts a scenario when a record is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of record that you want to create.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Activity]</strong> </p> <p>Select the activity type that you want to watch. </p> <p>The module watches only for new activities.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Lead]</strong> </p> <p>Select whether you want to watch for new records, updated records, both new and updated records, or specific field updates. If you select to watch specific field updates, select the field that you want the module to watch.</p> </li> 
     <li> <p><strong>[!UICONTROL Program]</strong> </p> <p>Select whether you want to watch for new records, updated records, or both new and updated records.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch events (Instant)]

This trigger module starts a scenario when a record is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>Enter the webhook that you want the module to use.</p> <p>For more information on webhooks, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant triggers (webhooks) in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions 

* [[!UICONTROL Custom API call]](#custom-api-call)
* [[!UICONTROL Create a record]](#create-a-record)
* [[!UICONTROL Update a record]](#update-a-record)
* [[!UICONTROL Download a File]](#download-a-file)
* [[!UICONTROL Upload a File]](#upload-a-file)
* [[!UICONTROL Read a record]](#read-a-record)
* [[!UICONTROL Add Leads to a List]](#add-leads-to-a-list)
* [[!UICONTROL Remove Leads from a List]](#remove-leads-from-a-list)
* [[!UICONTROL Schedule a Campaign]](#schedule-a-campaign)
* [[!UICONTROL Copy a Program]](#copy-a-program)

#### [!UICONTROL Custom API call]

This action module lets you make a custom authenticated call to the [!DNL Marketo] API. This way, you can create a data flow automation that can't be accomplished by the other [!DNL Marketo] modules.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Enter a path relative to <code>https://{your-base-url}.mktorest.com/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to work with during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a record]

This action module creates a new record in [!DNL Marketo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of record that you want to create.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Folder]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select fields to map]</td> 
   <td>If you are creating a Company or a Lead, select the fields that you want to set values for when the new record is created, then enter values for these fields.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Type]</td> 
   <td>If you are creating a Program, select the type of program that you want to create.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Channel] </td> 
   <td>If you are creating a Program, select the program channel where you want to create the program.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Program Name]</td> 
   <td>If you are creating a Folder or Program, enter or map a name for the new record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>If you are creating a Folder or Program, enter or map a description for the new record.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent Folder ID]</td> 
   <td>If you are creating a Folder or Program, enter or map the ID of the parent folder where you want to create the new record..</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs]</td> 
   <td>If you are creating a Program, add any costs.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>If you are creating a Program, add any tags</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a record]

This action module updates an existing record, using its ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of record that you want to create.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Company] / [!UICONTROL Lead] / [!UICONTROL Program ID]</td> 
   <td>Enter or map the ID of the record you want to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select fields to map]</td> 
   <td>If you are updating a Company or a Lead, select the fields that you want to update values for, then enter values for these fields.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Name]</td> 
   <td>If you are updating a Program, enter or map a new name for the program.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>If you are updating a Program, enter or map a new description for the program.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start Date]</td> 
   <td>If you are updating a Program, enter or map a new start date for the program.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End Date]</td> 
   <td>If you are updating a Program, enter or map a new end date for the program.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs]</td> 
   <td>If you are updating a Program, add any costs.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>If you are updating a Program, add any tags</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download a File]

This action module downloads a file by using the file ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Map the ID of the file you want to download.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload a File]

This action module uploads a new file to [!UICONTROL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>Enter or map the ID of the folder where you want the new file to be located.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter a description for the uploaded file.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read a record]

This action module reads information about a record by using its ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of record that you want to create.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaign]</p> </li> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL List]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Select the information you want included in the output bundle for this module. Fields are available based on the [!UICONTROL Record Type] you selected.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;Object> ID]</td> 
   <td>Enter or map the ID of the object you want to retrieve information about.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add Leads to a List]

This action module adds one or more leads to a list, by using the lead ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Enter or map the ID of the list where you want to add leads.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lead IDs]</td> 
   <td> <p>For each lead that you want to add to the list, click <b>[!UICONTROL Add]</b>, then enter or map the ID of the lead you want to add. You can add up to 300 leads for the module to add to the list.</p> <p>Click the map toggle to map an existing collection of leads that you want to add to the list.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove Leads from a List]

This action module removes one or more leads from a list, by using the lead ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Enter or map the ID of the list where you want to remove leads.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lead IDs]</td> 
   <td> <p>For each lead that you want to remove from the list, click <b>[!UICONTROL Add]</b>, then enter or map the ID of the lead you want to remove. You can add up to 300 leads for the module to remove from the list. </p> <p>Click the map toggle to map an existing collection of leads that you want to remove from the list.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Schedule a Campaign]

This action module schedules an existing campaign for a certain date.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign ID]</td> 
   <td>Enter or map the ID of the campaign that you want to schedule.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Schedule for Date]</p> </td> 
   <td>Select the date that you want the campaign to run. If this field is left blank, the campaign runs five minutes after the scenario began.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copy a Program]

This action module makes a copy of a program using the existing program's ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Existing Program ID]</td> 
   <td>Enter or map the ID of the program that you want to copy.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL New Program Name]</p> </td> 
   <td> <p>Enter or map a name for the new program</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>Enter or map the ID of the folder where you want the new program to be located.</td> 
  </tr> 
 </tbody> 
</table>

### Searches 

* [[!UICONTROL List records]](#list-records)
* [[!UICONTROL Search Records]](#update-a-record)

#### [!UICONTROL List records]

This action module retrieves all records of a specific type.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of record that you want to list.</p> 
    <ul> 
     <li> <p>[!UICONTROL Read all campaigns]</p> </li> 
     <li> <p>[!UICONTROL Read all programs]</p> </li> 
     <li> <p>[!UICONTROL Read all leads] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field]</td> 
   <td>If you have selected to retrieve leads, select whether you want to retrieve leads from a list or from a program.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Select the information you want included in the output bundle for this module. Fields are available based on the [!UICONTROL Record Type] you selected.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search Records]

This search module retrieves a list of records that match specific search criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>For instructions about connecting your [!DNL Marketo] account to [!DNL Workfront Fusion], see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Select the type of record you want to search.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaigns]</p> </li> 
     <li> <p>[!UICONTROL Leads]</p> </li> 
     <li> <p>[!UICONTROL Programs]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Field]</p> </td> 
   <td> <p>Select whether you want to search by name, program name, or workspace name.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td>For each value you want to search for, click <b>[!UICONTROL Add item]</b> and enter the value.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>
