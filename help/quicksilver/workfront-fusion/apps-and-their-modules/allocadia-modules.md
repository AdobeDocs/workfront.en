---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Allocadia modules
description: In an [!DNL Adobe Workfront] Fusion scenario, you can automate workflows that use Allocadia, as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
---
# Allocadia modules

In an [!DNL Adobe Workfront] Fusion scenario, you can automate workflows that use Allocadia, as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Allocadia modules, you must have an Allocadia account.

## Connect Allocadia to Workfront Fusion {#connect-allocadia-to-workfront-fusion}

You can create a connection to your [!DNL Allocadia] account directly from inside an [!DNL Allocadia] module.

1. In any Allocadia module, click **Add** next to the Connection field.
1. Select whether you want to use the North America server or the Europe server.
1. Enter your Username and Password.
1. Click **[!UICONTROL Continue]** to create the connection and go back to the module.

## Allocadia modules and their fields

When you configure Allocadia modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional Allocadia fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Searches](#searches)

### Triggers {#triggers}

#### Watch Record

This trigger module executes a scenario when objects of a specific type are added, updated, or both. The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Allocadia account to [!DNL Workfront] Fusion, see <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td> <p>Select whether you want the scenario to watch New Records Only, [!UICONTROL Updated Records Only], or New and Updated Records.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entity Type</td> 
   <td>Select the Allocadia record type that you want the module to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td> <p>Select the fields that you want to include in the module's output. Available fields depend on the Entity Type you selected.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to watch during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Custom API Call](#custom-api-call)
* [Read Record](#read-record)
* [Create Record](#create-record)
* [Delete Record](#delete-record)
* [Update Record](#update-record)

#### Custom API Call {#custom-api-call}

This action module lets you make a custom authenticated call to the [!DNL Allocadia] API. This way, you can create a data flow automation that can't be accomplished by the other [!DNL Allocadia] modules.

The action is based on the entity type (Allocadia object type) you specify.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Allocadia account to [!DNL Workfront] Fusion, see <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Enter a path relative to <code>https://api-na.allocadia.com/{version}</code> or <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard [!DNL JSON] object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{“name”:“something-urgent”}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard [!DNL JSON] object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Read Record {#read-record}

This action module reads data from a single record in Allocadia.

You specify the ID of the record.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Allocadia account to [!DNL Workfront] Fusion, see <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entity Type</td> 
   <td>Select the type of Allocadia record that you want the module to read.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td> <p>Select the fields that you want to include in the module's output. Available fields depend on the Entity Type you selected.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter or map the unique Allocadia ID of the record that you want the module to read.</td> 
  </tr> 
 </tbody> 
</table>

#### Create Record {#create-record}

This action module creates a record.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Allocadia account to [!DNL Workfront] Fusion, see <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entity Type</td> 
   <td>Select whether you want to create a new record based on line item or column choice.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Budgets</td> 
   <td> <p>Select the budget where you want to create a record.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Column choices</td> 
   <td>Select the column that you want to use to create a new record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Label</td> 
   <td>Enter or map a label for the new record</td> 
  </tr> 
 </tbody> 
</table>

#### Delete Record {#delete-record}

This action module deletes a particular record.

You specify the ID of the record.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Allocadia account to [!DNL Workfront] Fusion, see <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entity Type</td> 
   <td> <p>Select the type of entity that you want to delete.</p> 
    <ul> 
     <li> <p><strong>Line item</strong> </p> <p>Enter the Line Item ID</p> </li> 
     <li> <p><strong>Column Choice</strong> </p> <p>Select the budget that you want to delete a record from, then enter the Column ID and Choice ID.</p> </li> 
     <li> <p><strong>Forecast Tags</strong> </p> <p>Select the budget that you want to delete a record from, then enter the Tag ID.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Update Record {#update-record}

This action module updates a record, such as a line item, user, or column choice,.

You specify the ID of the record.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Allocadia account to [!DNL Workfront] Fusion, see <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entity Type</td> 
   <td>Select the type of Allocadia record that you want the module to update. Other fields appear based on the entity type you select.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Budgets</td> 
   <td> <p>Select the budget where you want to update a record. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Searches {#searches}

#### Search Record

This search module looks for records in an object in Allocadia that match the search query you specify.

You can map this information in subsequent modules in the scenario.

You specify the type of the records you want.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Allocadia account to [!DNL Workfront] Fusion, see <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entity Type</td> 
   <td>Select the type of Allocadia record that you want the module to search for. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Budgets</td> 
   <td> <p>Select the budget that you want to search. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Result set</td> 
   <td>Select whether you want the module to return All Matching Records, or the First Matching Record only.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximal count of records</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Search criteria</td> 
   <td>Select the field you want to search for, select the operation, and enter or map the value you want to search for. You can add AND or OR rules to further filter your search.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td> <p>Select the fields that you want to include in the module's output. Available fields depend on the Entity Type you selected.</p> </td> 
  </tr> 
 </tbody> 
</table>
