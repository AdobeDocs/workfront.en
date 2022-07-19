---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365 modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Microsoft Dynamics 365, as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
---

# Microsoft Dynamics 365 modules

In an Adobe Workfront Fusion scenario, you can automate workflows that use Microsoft Dynamics 365, as well as connect it to multiple third-party applications and services.

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

To use Microsoft Dynamics 365, you must have a Microsoft Dynamics 365 account.

## Connect Microsoft Dynamics 365 to Workfront Fusion {#connect-microsoft-dynamics-365-to-workfront-fusion}

You can create a connection to your Microsoft Dynamics 365 account directly from inside an Allocadia module.

1. In any Microsoft Dynamics 365 module, click **Add** next to the Connection field.
1. Enter a name for the connection.
1. In the **Resource** field, enter the address of your Dynamics 365 account, without `https://`.
1. Click **Continue** to create the connection and go back to the module.

>[!NOTE]
>
>When registering Workfront Fusion in your Microsoft Azure portal, use the following redirect URI:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`&nbsp;

## Microsoft Dynamics 365 modules and their fields

When you configure Microsoft Dynamics 365 modules, Workfront Fusion displays the fields listed below. Along with these, additional Microsoft Dynamics 365 fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Watch Records (Scheduled)](#watch-records-scheduled) 
* [Watch Records (Real Time)](#watch-records-real-time) 
* [Create Record](#create-record) 
* [Make an API Call](#make-an-api-call) 
* [Delete Record](#delete-record) 
* [Read Records](#read-records) 
* [Update Record](#update-record) 
* [Search Records](#search-records)

### Watch Records (Scheduled) {#watch-records-scheduled}

This scheduled trigger module executes a scenario when a record in the object you specify is created or updated after the last scheduled run in Dynamics 365.

The module's output indicates whether the record that it found is new or updated (if it was both added and updated in the time period, it's marked as new). You can map this information in subsequent modules in the scenario.

This happens on a regularly scheduled interval that you specify.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Microsoft Dynamics 365 account to Workfront Fusion, see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect Microsoft Dynamics 365 to Workfront Fusion</a> in this article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Include</td> 
   <td>Select whether you want the module to watch <strong>Only new records</strong>, <strong>Updated records only</strong>, or <strong>New records and all changes</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entity Type</td> 
   <td>Choose the Microsoft Dynamics 365 record type that you want the scenario to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Max Records</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Watch Records (Real Time) {#watch-records-real-time}

This instant trigger module executes a scenario when a record (object) you specify is created or updated in Dynamics 365.

A webhook is required in this module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook</td> 
   <td> <p>Select the webhook that you want to use for this module. </p> <p>To add a new webhook:</p> 
    <ol> 
     <li value="1"> <p>Click <strong>Add</strong> to the right of the Webhook field</p> </li> 
     <li value="2"> <p>In the <strong>Webhook</strong> name field, type a descriptive name for the webhook.</p> </li> 
     <li value="3"> <p>In the <strong>Connection</strong> field, select the Connection that you want to use selected</p> <p>For instructions about connecting your Microsoft Dynamics 365 account to Workfront Fusion, see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect Microsoft Dynamics 365 to Workfront Fusion</a> in this article. </p> </li> 
     <li value="4"> <p>Click <strong>Save</strong> to save your webhook and return to the module.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Create Record {#create-record}

This action module creates an entity, such as an appointment or task,.

You specify information about the entity that you want to create.

The module returns the ID of the new entity and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Microsoft Dynamics 365 account to Workfront Fusion, see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect Microsoft Dynamics 365 to Workfront Fusion</a> in this article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entity Type</td> 
   <td>Select the type of entity that you want the module to create.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Property fields</td> 
   <td>In these fields, enter the value that you want the work item to have for a given property. Available fields depend on the entity type.</td> 
  </tr> 
 </tbody> 
</table>

### Make an API Call {#make-an-api-call}

This action module lets you make a custom authenticated call to the Microsoft Dynamics 365 API. This way, you can create a data flow automation that can't be accomplished by the other Microsoft Dynamics 365 modules.

The module returns information about the status code, headers, and body. You can map this information in subsequent modules in the scenario.

To learn more, see the Microsoft documentation about using the Dynamics 365 Customer Engagement Web API.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Microsoft Dynamics 365 account to Workfront Fusion, see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect Microsoft Dynamics 365 to Workfront Fusion</a> in this article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Enter a path relative to <code>&lt;Instance URL&gt;/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in Adobe Workfront Fusion</a>.</p> <p>For more in</p> </td> 
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
 </tbody> 
</table>

### Delete Record {#delete-record}

This action module deletes an entity.

You specify the ID of the entity.

The module returns the ID of the  entity and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Microsoft Dynamics 365 account to Workfront Fusion, see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect Microsoft Dynamics 365 to Workfront Fusion</a> in this article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entity Type</td> 
   <td> <p>Select the type of entity that you want the module to delete.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td> <p>Enter or map the unique Microsoft Dynamics 365 ID of the record that you want the module to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Read Records {#read-records}

This action module reads data from a single entity in Microsoft Dynamics 365.

You specify the ID of the entity.

The module returns the ID of the entity and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Microsoft Dynamics 365 account to Workfront Fusion, see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect Microsoft Dynamics 365 to Workfront Fusion</a> in this article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entity Type</td> 
   <td>Select the type of entity that you want the module to read.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter or map the unique Microsoft Dynamics 365 ID of the record that you want the module to read.</td> 
  </tr> 
 </tbody> 
</table>

### Update Record {#update-record}

This action module updates an entity.

You specify the ID of the entity.

The module returns the ID of the updated record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Microsoft Dynamics 365 account to Workfront Fusion, see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect Microsoft Dynamics 365 to Workfront Fusion</a> in this article. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Entity Type</td> 
   <td>Select the type of entity that you want the module to update.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Property fields</td> 
   <td>In these fields, enter the value that you want the work item to have for a given property. Available fields depend on the entity type.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">ID</td> 
   <td>Enter or map the unique Microsoft Dynamics 365 ID of the record that you want the module to update.</td> 
  </tr> 
 </tbody> 
</table>

### Search Records {#search-records}

This search module looks for records in an object in Microsoft Dynamics 365 that match the search query you specify. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Microsoft Dynamics 365 account to Workfront Fusion, see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect Microsoft Dynamics 365 to Workfront Fusion</a> in this article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entity Type</td> 
   <td>Select the type of entity that you want the module to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filters</td> 
   <td> <p>Select the filter that you want to use for this search.</p> 
    <ul> 
     <li> <p><strong>Standard Filters</strong> </p> <p>Set up the filter by selecting a field and operator, and entering or mapping the value that you want to search for. You can use AND or OR rules to your filter.</p> </li> 
     <li> <p><strong>Query Functions</strong> </p> <p>Enter the Dynamics 365 web API query function that you want to use to search. </p> <p>For more information on query functions, see <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Web API Query Function Reference</a> in the Microsoft documentation.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sort</td> 
   <td> <p>Specify the order in which items are returned. You can add multiple sorts.</p> 
    <ul> 
     <li> <p><strong>Field</strong> </p> <p>Specify the field by which you want to sort results.</p> </li> 
     <li> <p><strong>Direction</strong> </p> <p>Specify the direction of the sort (ascending or descending).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Max Records</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

