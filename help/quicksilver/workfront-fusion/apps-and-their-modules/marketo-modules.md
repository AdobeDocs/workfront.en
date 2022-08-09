---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Marketo modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Marketo, as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
---
# Marketo modules

In an Adobe Workfront Fusion scenario, you can automate workflows that use Marketo, as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
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
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Marketo modules, you must have a Marketo account.

## Connect Marketo to Workfront Fusion {#connect-marketo-to-workfront-fusion}

You can create a connection to your Marketo account directly from inside Marketo module.

1. In any Marketo module, click **Add** next to the Connection field.
1. Enter your Marketo account or Marketo Munchkin ID. This is the unique part of the Base URL or Endpoint assigned to your account, that you use to access Marketo via its REST API. For instructions on locating this, see [Base URL](https://developers.marketo.com/rest-api/base-url/) in the Marketo documentation.
1. Enter your Client ID and Client secret. For instructions on locating these, see [Authentication](https://developers.marketo.com/rest-api/authentication/) in the Marketo documentation.
1. Click **Continue** to create the connection and go back to the module.

## Marketo Modules and their fields

When you configure Marketo modules, Workfront Fusion displays the fields listed below. Along with these, additional Marketo fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches)

### Triggers {#triggers}

* [Watch records](#watch-records) 
* [Watch events (Instant)](#watch-events-instant)

#### Watch records  {#watch-records}

This trigger module starts a scenario when a record is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record that you want to create.</p> 
    <ul> 
     <li> <p><strong>Activity</strong> </p> <p>Select the activity type that you want to watch. </p> <p>The module watches only for new activities.<br></p> </li> 
     <li> <p><strong>Lead</strong> </p> <p>Select whether you want to watch for new records, updated records, both new and updated records, or specific field updates. If you select to watch specific field updates, select the field that you want the module to watch.</p> </li> 
     <li> <p><strong>Program</strong> </p> <p>Select whether you want to watch for new records, updates records, or both new and updated records.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch events (Instant) {#watch-events-instant}

This trigger module starts a scenario when a record is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>Enter the webhook that you want the module to use.</p> <p>For more information on webhooks, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant triggers (webhooks) in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Custom API call](#custom-api-call) 
* [Create a record](#create-a-record) 
* [Update a record](#update-a-record) 
* [Download a File](#download-a-file) 
* [Upload a File](#upload-a-file) 
* [Read a record](#read-a-record) 
* [Add Leads to a List](#add-leads-to-a-list) 
* [Remove Leads from a List](#remove-leads-from-a-list) 
* [Schedule a Campaign](#schedule-a-campaign) 
* [Copy a Program](#copy-a-program)

#### Custom API call {#custom-api-call}

This action module lets you make a custom authenticated call to the Marketo API. This way, you can create a data flow automation that can't be accomplished by the other Marketo modules. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Enter a path relative to <code>https://{your-base-url}.mktorest.com/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{“name”:“something-urgent”}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to work with during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a record {#create-a-record}

This action module creates a new record in Marketo

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record that you want to create.</p> 
    <ul> 
     <li> <p>Company</p> </li> 
     <li> <p>Folder</p> </li> 
     <li> <p>Lead</p> </li> 
     <li> <p>Program</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Select fields to map</td> 
   <td>If you are creating a Company or a Lead, select the fields that you want to set values for when the new record is created, then enter values for these fields.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Program Type</td> 
   <td>If you are creating a Program, select the type of program that you want to create.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Program Channel </td> 
   <td>If you are creating a Program, select the program channel where you want to create the program.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder / Program Name</td> 
   <td>If you are creating a Folder or Program, enter or map a name for the new record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Description</td> 
   <td> <p>If you are creating a Folder or Program, enter or map a description for the new record.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Parent Folder ID</td> 
   <td>If you are creating a Folder or Program, enter or map the ID of the parent folder where you want to create the new record..</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Costs</td> 
   <td>If you are creating a Program, add any costs.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tags</td> 
   <td>If you are creating a Program, add any tags</td> 
  </tr> 
 </tbody> 
</table>

#### Update a record  {#update-a-record}

This action module updates an existing record, using its ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record that you want to create.</p> 
    <ul> 
     <li> <p>Company</p> </li> 
     <li> <p>Lead</p> </li> 
     <li> <p>Program</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Company / Lead / Program ID</td> 
   <td>Enter or map the ID&nbsp;of the record you want to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Select fields to map</td> 
   <td>If you are updating a Company or a Lead, select the fields that you want to update values for, then enter values for these fields.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Program Name</td> 
   <td>If you are updating a Program, enter or map a new name for the program.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Description</td> 
   <td> <p>If you are updating a Program, enter or map a new description for the program.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Start Date</td> 
   <td>If you are updating a Program, enter or map a new start date for the program.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">End Date</td> 
   <td>If you are updating a Program, enter or map a new end date for the program.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Costs</td> 
   <td>If you are updating a Program, add any costs.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tags</td> 
   <td>If you are updating a Program, add any tags</td> 
  </tr> 
 </tbody> 
</table>

#### Download a File {#download-a-file}

This action module downloads a file by using the file ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">File ID</td> 
   <td>Map the ID of the file you want to download.</td> 
  </tr> 
 </tbody> 
</table>

#### Upload a File {#upload-a-file}

This action module uploads a new file to Marketo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Source file</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder ID</td> 
   <td>Enter or map the ID&nbsp;of the folder where you want the new file to be located.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Description</td> 
   <td>Enter a description for the uploaded file.</td> 
  </tr> 
 </tbody> 
</table>

#### Read a record {#read-a-record}

This action module reads information about a record by using its ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record that you want to create.</p> 
    <ul> 
     <li> <p>Campaign</p> </li> 
     <li> <p>Company</p> </li> 
     <li> <p>Lead</p> </li> 
     <li> <p>List</p> </li> 
     <li> <p>Program</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the information you want included in the output bundle for this module. Fields are available based on the Record Type you selected.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;Object&gt; ID</td> 
   <td>Enter or map the ID&nbsp;of the object you want to retrieve information about.</td> 
  </tr> 
 </tbody> 
</table>

#### Add Leads to a List {#add-leads-to-a-list}

This action module adds one or more leads to a list, by using the lead ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID</td> 
   <td>Enter or map the ID of the list where you want to add leads.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Lead IDs</td> 
   <td> <p>For each lead that you want to add to the list, click Add, then enter or map the ID of the lead you want to add. You can add up to 300 leads for the module to add to the list.</p> <p>Click the map toggle to map an existing collection of leads that you want to add to the list.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Remove Leads from a List {#remove-leads-from-a-list}

This action module removes one or more leads from a list, by using the lead ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID</td> 
   <td>Enter or map the ID of the list where you want to remove leads.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Lead IDs</td> 
   <td> <p>For each lead that you want to remove from the list, click Add, then enter or map the ID of the lead you want to remove. You can add up to 300 leads for the module to remove from the list. </p> <p>Click the map toggle to map an existing collection of leads that you want to remove from the list.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Schedule a Campaign {#schedule-a-campaign}

This action module schedules an existing campaign for a certain date.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campaign ID</td> 
   <td>Enter or map the ID of the campaign that you want to schedule.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Schedule for Date</p> </td> 
   <td>Select the date that you want the campaign to run. If this field is left blank, the campaign runs five minutes after the scenario began.</td> 
  </tr> 
 </tbody> 
</table>

#### Copy a Program {#copy-a-program}

This action module makes a copy of a program using the existing program's ID. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Existing Program ID</td> 
   <td>Enter or map the ID of the program that you want to copy.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>New Program Name</p> </td> 
   <td> <p>Enter or map a name for the new program</p> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder ID</td> 
   <td>Enter or map the ID&nbsp;of the folder where you want the new program to be located.</td> 
  </tr> 
 </tbody> 
</table>

### Searches {#searches}

* [List records](#list-records) 
* [Search Records](#search-records)

#### List records {#list-records}

This action module retrieves all records of a specific type.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td> <p>Select the type of record that you want to list.</p> 
    <ul> 
     <li> <p>Read all campaigns</p> </li> 
     <li> <p>Read all programs</p> </li> 
     <li> <p>Read all leads </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Field</td> 
   <td>If you have selected to retrieve leads, select whether you want to retrieve leads from a list or from a program.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the information you want included in the output bundle for this module. Fields are available based on the Record Type you selected.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Records {#search-records}

This search module retrieves a list of records that match specific search criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Marketo account to Workfront Fusion, see <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect Marketo to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td> <p>Select the type of record you want to search.</p> 
    <ul> 
     <li> <p>Campaigns</p> </li> 
     <li> <p>Leads</p> </li> 
     <li> <p>Programs</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Field</p> </td> 
   <td> <p>Select whether you want to search by name, program name, or workspace name.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Values</td> 
   <td>For each value you want to search for, click Add item and enter the value.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Output</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>
