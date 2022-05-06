---
filename: anaplan-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Anaplan Modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Anaplan, as well as connect it to to multiple third-party applications and services.
---

# Anaplan Modules

In an Adobe Workfront Fusion scenario, you can automate workflows that use Anaplan, as well as connect it to to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

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
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
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

## Prerequisites

Before you can use the Anaplan connector, you must ensure that the following prerequisites are met:

* You must have an active Anaplan account.
* You must configure Workspaces, Models, and other Anaplan objects in your Anaplan account before Workfront Fusion can interact with them.

## Connect Anaplan to Workfront Fusion {#connect-anaplan-to-workfront-fusion}

To create a connection for your Anaplan modules:

1. Click **Add** next to the Connection box.
1. Select the connection type.

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anaplan Basic</td> 
      <td> <p>An Anaplan Basic connection requires only an email address and password to create the connection. </p> <p>Enter a name for the connection, then enter your email address and the password of your Anaplan account.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anaplan CA Certificate</td> 
      <td> <p>An Anaplan CA Certificate connection requires a Certificate Key, Encoded Data, and Encoded Signed Data. You can generate these in your Anaplan account. For instructions, see the Anaplan documentation.</p> <p>Enter a name for the connection, then enter the connection requires a Certificate Key, Encoded Data, and Encoded Signed Data that you generated in your Anaplan account.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Continue** to save the connection and return to the module.

## Anaplan modules and their fields

When you configure Anaplan modules, Workfront Fusion displays the fields listed below. Along with these, additional Anaplan fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions)

### Triggers {#triggers}

#### Watch records

This trigger module starts a scenario when a record of the chosen type is created or updated.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Anaplan, see <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect Anaplan to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type of object to watch</td> 
   <td>Select the type of item that you want to watch. The scenario begins when this type of record is created or updated.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;Object&gt; ID</td> 
   <td>Enter the ID of the object in Anaplan, such as a Model or Module, that is associated with the objects you want to watch</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to [action] during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Create a list item](#create-a-list-item) 
* [Make a custom API Call](#make-a-custom-api-call) 
* [Delete a record](#delete-a-record) 
* [Export data](#export-data) 
* [Get record](#get-record) 
* [Import Data](#import-data) 
* [Read a record](#read-a-record) 
* [Update a record](#update-a-record)

#### Create a list item {#create-a-list-item}

This action module adds a new item to a list in Anaplan.

| Connection |For instructions on creating a connection to Anaplan, see [Connect Anaplan to Workfront Fusion](#connect-anaplan-to-workfront-fusion) in this article. |
|---|---|
| Workspace ID |Select or map the ID&nbsp;of the Anaplan Workspace that contains the list where you want to add an item. |
| Model ID |Select or map the ID of the Model that contains the list where you want to add an item. |
| List ID |Select or map the ID of the List where you want to create an item. |
| Name |Enter a name for the new item. |
| Code |Enter the code for the new item. Codes are user-generated codes that enable you to distinguish between line items with the same name. |
| Parent |Enter the name of the parent item that you want to create the new item under. |
| Properties |If the list you want to add an item to has custom properties, select the properties you want to add values for, then add the values. |
| Subsets |If the list you want to add items to has custom subsets, select the subsets you want to add the item to, then select **Yes** to add the new item to that subset. |

#### Make a custom API Call {#make-a-custom-api-call}

This module allows you to perform a custom API call to the Anaplan API.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Anaplan, see <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect Anaplan to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>URL</p> </td> 
   <td> <p>Enter a path relative to <code>https://api.anaplan.com/2/0/</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Method</p> </td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds authorization headers automatically.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String </td> 
   <td> <p>Enter the request query string.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a record  {#delete-a-record}

This action module deletes an existing record.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Anaplan, see <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect Anaplan to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the ID of the Anaplan Workspace that contains the object you want to delete.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Model ID</td> 
   <td>Enter or map the ID of the Model that contains the object you want to delete.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Delete</td> 
   <td> <p>Select the type of object to delete.</p> 
    <ul> 
     <li> <p><b>Action</b> </p> <p>Select or map the action to delete.</p> </li> 
     <li> <p><b>List item</b> </p> <p>Select the list that you want to delete an item from, then enter or map the ID or the code of the item that you want to delete</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Enter or map the ID of the list that you want to delete an item from, then enter or map the ID or the code of the item that you want to delete</p>
      --> </li> 
     <li> <p><b>File</b> </p> <p>Select or map the file to delete.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Export data {#export-data}

This action module exports data from Anaplan. You can export into the following file formats:

* XLS
* XLSX
* CSV

| Connection |For instructions on creating a connection to Anaplan, see [Connect Anaplan to Workfront Fusion](#connect-anaplan-to-workfront-fusion) in this article. |
|---|---|
| Workspace ID |Select or map the ID of the Anaplan Workspace that contains the object you want to export. |
| Model ID |Enter or map the ID of the Model that contains the object you want to export. |
| Export ID |Enter or map the ID&nbsp;of the export definition that you want to use. |

#### Get record {#get-record}

This action module returns all accessible records of the selected type.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Anaplan, see <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect Anaplan to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record types</td> 
   <td> <!--
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <p>Select the type of record that you want to retrieve.</p> 
      <ul> 
       <li> <p><b>Workspaces</b> </p> </li> 
       <li> <p><b>Models</b> </p> </li> 
       <li> <p><b>Line items</b> </p> <p>Select or map the ID of the Model that contains the line items you want to retrieve.</p> </li> 
       <li> <p><b>Model lists</b> </p> <p>Select or map the ID of the Workspace and Model ID that contain the Model lists you want to retrieve.</p> </li> 
       <li> <p><b>Model calendar</b> </p> <p>Select or map the ID of the Workspace that contains the Model calendar you want to retrieve.</p> </li> 
       <li> <p><b>Model versions</b> </p> </li> 
       <li> <p>Select or map the ID of the Model that contains the Model versions you want to retrieve.</p> </li> 
       <li> <p><b>Users</b> </p> </li> 
       <li> <p><b>Views</b> </p> <p>Select whether you want to choose the view by Module or by Model, then select or map the ID&nbsp;of the Module or Model that contains the view you want to retrieve.</p> </li> 
      </ul> 
     </div>
    --> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Return workspace size</td> 
   <td>Enable this option to return an estimate of the current size of the workspace. This estimate is based on the sizes of all of the modules contained in the workspace.</td> 
  </tr> 
 </tbody> 
</table>

#### Import Data {#import-data}

This action module imports data into Anaplan using the Anaplan API. For example, you can import a file that you have uploaded.

| Connection |For instructions on creating a connection to Anaplan, see [Connect Anaplan to Workfront Fusion](#connect-anaplan-to-workfront-fusion) in this article. |
|---|---|
| Workspace ID |Select or map the ID of the Anaplan Workspace where you want to import data. |
| Model ID |Select or map the ID of the Model where you want to import data. |
| Import ID |Enter or map the ID&nbsp;of the import definition that you want to use. |

#### Read a record  {#read-a-record}

This action module reads a single record.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Anaplan, see <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect Anaplan to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td> <p>Select the type of record to read.</p> 
    <ul> 
     <li> <p><b>Model</b> </p> <p>Select or map the ID&nbsp;of the Model you want to read</p> </li> 
     <li> <p><b>Model list</b> </p> <p>Select or map the IDs of the Workspace and Model that contain the List you want to read, then select the List. In the Data type field, select whether you want to read data or metadata.</p> </li> 
     <li> <p><b>Model version</b> </p> <p>Select or map the ID of the Model you want to read.</p> </li> 
     <li> <p><b>User</b> </p> <p>Select whether you want to return data about the owner of the account being used, or another user. If you select another user, select the name of the user.</p> </li> 
     <li> <p><b>Workspace</b> </p> <p>Select or map the ID of the Workspace you want to read.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a record  {#update-a-record}

This action module updates a single record in Anaplan.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Anaplan, see <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect Anaplan to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td> <p>Select the type of record you want to update.</p> 
    <ul> 
     <li> <p><b>List item</b> </p> <p>For fields, see <a href="#create-a-list-item" class="MCXref xref">Create a list item</a> in this article.</p> </li> 
     <li> <p><b>Module cell data</b> </p> <p>When you update cell data, all downstream calculations that use that data are also updated.</p> <p>Fill in the following fields:</p> 
      <ul> 
       <li> <p><b>Model ID</b> </p> <p>Select or map the Model that contains the cell you want to update.</p> </li> 
       <li> <p><b>Module ID</b> </p> <p>Select or map the Module that contains the cell you want to update</p> </li> 
       <li> <p><b>Line item name</b> </p> <p style="font-weight: bold;">Select or map the line item of the cell you want to update</p> </li> 
       <li> <p style="font-weight: bold;">Dimension ID</p> <p>Select or map the dimension that is on the line item.</p> <p>For information on dimensions, search for Dimensions in the Anaplan Anapedia.</p> </li> 
       <li> <p><b>Value</b> </p> <p>Enter or map the new value for the cell.</p> </li> 
      </ul> </li> 
     <li> <p><b>Model current fiscal year</b> </p> <p>Enter the Workspace ID and Model ID of the Model for which you want to update the fiscal year, then enter or map the new year for the model.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h4>Upload a file</h4>
<p>This action module uploads a file to Anaplan. The file must have already been uploaded to Anaplan. You can use this module to upload it to additional locations within Anaplan.</p>
<table cellspacing="0">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Connection</td>
<td>For instructions on creating a connection to Anaplan, see <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect Anaplan to Workfront Fusion</a> in this article.</td>
</tr>
<tr>
<td role="rowheader">Workspace ID</td>
<td>Select or map the ID of the Anaplan Workspace<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
where you want to upload a file
</MadCap:conditionalText>
-->.</td>
</tr>
<tr>
<td role="rowheader">Model ID</td>
<td>Select or map the ID of the Model<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
where you want to upload a file
</MadCap:conditionalText>
-->.</td>
</tr>
<tr>
<td role="rowheader">File ID</td>
<td>Select or map the ID&nbsp;of the file you want to upload.</td>
</tr>
</tbody>
</table>
</div>
-->

