---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: SharePoint modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use SharePoint, as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
---
# SharePoint modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use SharePoint, as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

To use [!DNL SharePoint] modules, you must have a SharePoint account.

## Connect SharePoint to [!DNL Workfront] Fusion {#connect-sharepoint-to-workfront-fusion}

* [Connect [!DNL SharePoint] to [!DNL Workfront Fusion] using a [!DNL Microsoft] account](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Connect [!DNL SharePoint] to [!DNL Workfront Fusion] using advanced settings](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Connect [!DNL SharePoint] to [!DNL Workfront Fusion] using a [!DNL Microsoft] account {#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account}

You can use your Microsoft account to create a connection to SharePoint. For instructions about connecting your Sharepoint account to Workfront Fusion, see [Create a connection to Adobe Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Connect [!DNL SharePoint] to [!DNL Workfront Fusion] using advanced settings {#connect-sharepoint-to-workfront-fusion-using-advanced-settings}

To connect [!DNL SharePoint] to [!DNL Workfront Fusion] without a [!DNL Microsoft] account, you need a Client ID, Client Secret, and Tenant ID.

1. Click **Add** near the top of the **SharePoint** box to open the **[!UICONTROL Create a connection]** box.

1. (Optional) Change the default **Connection name**.
1. Click **Show advanced settings**.
1. Enter the SharePoint **Client ID** and **Client Secret**.

1. Click **Continue**.
1. In the sign-in window that displays, enter your credentials to log in to the app if you haven't already done so.
1. (Conditional) If an **Allow** button displays, click the button to connect the app to Workfront Fusion.

## SharePoint modules and their fields

When you configure SharePoint modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional SharePoint fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Item](#item)
* [List](#list)
* [Page (Beta)](#page-beta)
* [Site](#site)
* [Other](#other)

### Item {#item}

* [Watch Items](#watch-items)
* [List Items](#list-items)
* [Get an Item](#get-an-item)
* [Create an item](#create-an-item)
* [Update an item](#update-an-item)
* [Delete an item](#delete-an-item)

#### Watch Items {#watch-items}

This trigger module starts a scenario when an item is created or modified.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Watch Lists</td> 
   <td>Select whether you want to watch lists by creation time (new items) or by modification time (updated items).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter Site and List ID</td> 
   <td> <p>Select how you want to identify the site and list that you want to watch.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Site ID</strong> and <strong>List ID</strong> in the fields that appear.</p> </li> 
     <li> <p><strong>Select from the list that you follow</strong> </p> <p>Select the site that you want to watch, then select the list. These drop-downs only retrieve followed sites.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of items you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Items {#list-items}

This action module retrieves a list of all items in a specified list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List Items</td> 
   <td> <p>Select how you want to identify the list that you want to retrieve items from.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Site ID</strong> and <strong>List ID</strong> in the fields that appear.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Select the site that contains the list you want to retrieve items from, then select the list. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of items you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get an Item {#get-an-item}

This action module returns the data of a specified item.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Get an Item</td> 
   <td> <p>Select how you want to identify the site and list that contain the item you want to get.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Site ID</strong>, <strong>List ID</strong>, and <strong>Item ID</strong> in the fields that appear.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Select the site that contains the list you want to retrieve an item from, then select the list, then select the item. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Create an item {#create-an-item}

This action module creates a new item in a SharePoint list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Create an Item</td> 
   <td> <p>Select how you want to identify the site and list where you want to create an item.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Site ID</strong> and <strong>List ID</strong> in the fields that appear.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Select the site that contains the list where you want to create an item, then select the list. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fields</td> 
   <td>For each field that you want to set for the new item, enter the field's key (identifies the field), and the value that you want the new item to have for that field.</td> 
  </tr> 
 </tbody> 
</table>

#### Update an item {#update-an-item}

This action module updates an existing item in a SharePoint list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Update an Item</td> 
   <td> <p>Select how you want to identify the site and list that contain the item you want to update.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Site ID</strong>, <strong>List ID</strong>, and <strong>Item ID</strong> in the fields that appear.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Select the site that contains the item you want to update, then select the list, then select the item. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fields</td> 
   <td>For each field that you want to update for the new item, enter the field's key (identifies the field), and the new value that you want the item to have for that field.</td> 
  </tr> 
 </tbody> 
</table>

#### Delete an item {#delete-an-item}

This action module deletes an existing item in a SharePoint list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Update an Item</td> 
   <td> <p>Select how you want to identify the site and list that contain the item you want to delete.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Site ID</strong>, <strong>List ID</strong>, and <strong>Item ID</strong> in the fields that appear.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Select the site that contains the item you want to delete, then select the list, then select the item. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### List {#list}

* [Watch Lists](#watch-lists)
* [List Lists](#list-lists)
* [Get a List](#get-a-list)
* [Create a List](#create-a-list)

#### Watch Lists {#watch-lists}

This trigger module starts a scenario when a list is created or modified.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Watch Lists</td> 
   <td>Select whether you want to watch lists by creation time (new items) or by modification time (updated items).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter Site and List ID</td> 
   <td> <p>Select how you want to identify the site and list that you want to watch.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Site ID</strong> where the list you want to watch is located.</p> </li> 
     <li> <p><strong>Select from the list that you follow</strong> </p> <p>Select the site that you want to watch. The drop-down only retrieves site you follow.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of lists you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Lists {#list-lists}

This action module retrieves a list of all items in a specified list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List Lists</td> 
   <td> <p>Select how you want to identify the site that you want to retrieve lists from.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Site ID</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Select the site that contains the lists you want to retrieve. The drop-down retrieves only sites you follow.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of lists you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a List {#get-a-list}

This action module returns the data of a specified list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Get a List</td> 
   <td> <p>Select how you want to identify the site and list that contain the item you want to get.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Site ID</strong> and <strong>List ID</strong> in the fields that appear.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Select the site that contains the list you want to retrieve, then select the list. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a List {#create-a-list}

This action module creates a new list in SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter a Site ID</td> 
   <td> <p>Select how you want to identify the site and list where you want to create a list.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Site ID</strong> where you want to create a list.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Select the site where you want to create a list. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Display Name</td> 
   <td>Enter or map a name for the new list.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Description</td> 
   <td>Enter or map a description for the new list.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Add Columns</td> 
   <td>For each column that you want to set for the new list, enter a <strong>Name</strong> for the field, and select the <strong>Type</strong> of value that you want the new column to have.</td> 
  </tr> 
 </tbody> 
</table>

### Page (Beta) {#page-beta}

>[!NOTE]
>
>APIs in the `beta` version in [!DNL Microsoft Graph] are subject to change. The use of these APIs in production applications is not supported.

#### Get a Page

This action module returns the data of a specified page.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Get a Page</td> 
   <td> <p>Select how you want to identify the page that you want to retrieve.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Site ID</strong>and <strong>Page ID</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Select the site that contains the page you want to retrieve, then select the page.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Site {#site}

* [Search Sites](#search-sites)
* [Get a Site](#get-a-site)

#### Search Sites {#search-sites}

This action module searches for sites by a parameter you specify.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Keyword of Display Name</td> 
   <td> <p>Enter or map the search term that you want to search the sites for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of sites you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Site {#get-a-site}

This action module returns the data of a specified site.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Get a Site</td> 
   <td> <p>Select how you want to identify the page that you want to retrieve.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Site ID</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Select the site that you want to retrieve.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Other {#other}

#### Make an API&nbsp;Call

This module allows you to perform a custom API call.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront] Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>URL</p> </td> 
   <td> <p>Enter a path relative to <code>https://graph.microsoft.com</code>. Example:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Method</p> </td> 
   td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.For example, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p> Add the query for the API call in the form of a standard JSON object.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type</td> 
   <td>Select the type of data that you want to send in your API call.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Add the body content for the API call in the form of a standard [!DNL JSON] object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<ul>
<li><a href="#watch-records" class="MCXref xref">Watch Records</a> </li>
<li><a href="#create-a-folder" class="MCXref xref">Create a folder</a> </li>
<li><a href="#create-an-item" class="MCXref xref">Create an item</a> </li>
<li><a href="#delete-an-item" class="MCXref xref">Delete an item</a> </li>
<li><a href="#download-a-file" class="MCXref xref">Download a file</a> </li>
<li><a href="#read-a-document" class="MCXref xref">Read a document</a> </li>
<li><a href="#read-an-item" class="MCXref xref">Read an item</a> </li>
<li><a href="#update-an-item" class="MCXref xref">Update an item</a> </li>
<li><a href="#upload-a-file" class="MCXref xref">Upload a file</a> </li>
<li><a href="#search-documents" class="MCXref xref">Search Documents</a> </li>
</ul>
<p><strong>Watch Records</strong></p>
<p>This trigger module executes a scenario when the scheduled poll shows that an object has been added or updated in SharePoint. The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses.You can map this information in subsequent modules in the scenario.This trigger module executes a scenario when an object is added or updated. The module returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario. This is a scheduled trigger module.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td> <p>For instructions about connecting your SharePoint account to Workfront Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Record Type</td>
<td>Select the type of SharePoint record that you want the module to watch.</td>
</tr>
<tr>
<td role="rowheader">Site</td>
<td>Select the site that you want the module to watch.</td>
</tr>
<tr>
<td role="rowheader">Event types</td>
<td>Select whether you want to watch for new records, updated records, or both.</td>
</tr>
<tr>
<td role="rowheader">Limit</td>
<td> <p>Enter or map the maximum number of records you want the module to watch during each scenario execution cycle.</p> </td>
</tr>
</tbody>
</table>
<p><strong>Create a folder</strong></p>
<p>This action module creates a new folder.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td> <p>For instructions about connecting your SharePoint account to Workfront Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Site</td>
<td>Select the location where you want to create a folder.</td>
</tr>
<tr>
<td role="rowheader">List</td>
<td>Select the list that you want to create a folder in.</td>
</tr>
<tr>
<td role="rowheader">Parent Folder</td>
<td>Select the folder that you want to create the new folder in.</td>
</tr>
<tr>
<td role="rowheader">Name</td>
<td>Enter or map a name for the new folder.</td>
</tr>
</tbody>
</table>
<p><strong>Create an item</strong></p>
<p>This action module creates a new item in a SharePoint list.</p>
<p>The module returns the ID of the new item and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td> <p>For instructions about connecting your SharePoint account to Workfront Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Site</td>
<td>Select the location where you want to create an item.</td>
</tr>
<tr>
<td role="rowheader">List</td>
<td>Select the list that you want to create a new item in.</td>
</tr>
<tr>
<td role="rowheader">Title</td>
<td>Enter or map a title for the new item.</td>
</tr>
</tbody>
</table>
<p><strong>Delete an item</strong></p>
<p>This action module deletes an item that you identify.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td> <p>For instructions about connecting your SharePoint account to Workfront Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Site</td>
<td>Select the location of the item you want to delete.</td>
</tr>
<tr>
<td role="rowheader">List</td>
<td>Select the list where the item you want to delete is located.</td>
</tr>
<tr>
<td role="rowheader">Item ID</td>
<td>Enter or map a the ID of the item you want to delete.</td>
</tr>
</tbody>
</table>
<p><strong>Download a file</strong></p>
<p>This action module downloads a file from a SharePoint drive.</p>
<p>You specify the ID of the file.</p>
<p>The module returns the file's content, filename, file extension, and file size. You can map this information in subsequent modules in the scenario.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td> <p>For instructions about connecting your SharePoint account to Workfront Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Site</td>
<td>Select the location of the file you want to download.</td>
</tr>
<tr>
<td role="rowheader">List</td>
<td>Select the list where the file you want to download is located.</td>
</tr>
<tr>
<td role="rowheader">File ID</td>
<td>Enter or map a the ID of the file you want to download .</td>
</tr>
</tbody>
</table>
<p><strong>Read a document</strong></p>
<p>This action module reads a single document and returns a bundle of the document's fields.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td> <p>For instructions about connecting your SharePoint account to Workfront Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Site</td>
<td>Select the location of the document you want to read.</td>
</tr>
<tr>
<td role="rowheader">List</td>
<td>Select the list where the document you want to read is located.</td>
</tr>
<tr>
<td role="rowheader">File ID</td>
<td>Enter or map the ID of the document you want to read.</td>
</tr>
</tbody>
</table>
<p><strong>Read an item</strong></p>
<p>This action module reads a single item and returns a bundle of the item's fields.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td> <p>For instructions about connecting your SharePoint account to Workfront Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Site</td>
<td>Select the location of the item you want to read.</td>
</tr>
<tr>
<td role="rowheader">List</td>
<td>Select the list where the item you want to read is located.</td>
</tr>
<tr>
<td role="rowheader">Item ID</td>
<td>Enter or map a the ID of the item you want to read.</td>
</tr>
</tbody>
</table>
<p><strong>Update an item</strong></p>
<p>This action module updates an existing item in a SharePoint list.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td> <p>For instructions about connecting your SharePoint account to Workfront Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Site</td>
<td>Select the location of the item you want to update.</td>
</tr>
<tr>
<td role="rowheader">List</td>
<td>Select the list where the item you want to update is located.</td>
</tr>
<tr>
<td role="rowheader">Item ID</td>
<td>Enter or map a the ID of the item you want to update.</td>
</tr>
</tbody>
</table>
<p><strong>Upload a file</strong></p>
<p>This action module uploads a file to SharePoint</p>
<p>You specify the location for the file, the file you want to upload, and an optional new name for the file.</p>
<p>The module returns the ID of the  file and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.</p>
<p>When you are configuring this module, the following fields display.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td> <p>For instructions about connecting your SharePoint account to Workfront Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Site</td>
<td>Select the location where you want to upload a file.</td>
</tr>
<tr>
<td role="rowheader">List</td>
<td>Select the list that you want to upload a file to.</td>
</tr>
<tr>
<td role="rowheader">Parent Folder</td>
<td>Select the folder that you want to upload a file to.</td>
</tr>
<tr>
<td role="rowheader">Source File</td>
<td>Select whether the source file is empty, link a source file from a previous module, or map the source file's name and data.</td>
</tr>
</tbody>
</table>
<p><strong>Search Documents</strong></p>
<p>This search module searches for a file or folder inside a SharePoint drive.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td> <p>For instructions about connecting your SharePoint account to Workfront Fusion, see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect SharePoint to Workfront Fusion</a> in this article.</p> </td>
</tr>
<tr>
<td role="rowheader">Site</td>
<td>Select the location where you want to search for documents.</td>
</tr>
<tr>
<td role="rowheader">List</td>
<td>Select the list where you want to search for documents.</td>
</tr>
<tr>
<td role="rowheader">Search query</td>
<td>Enter the search query that determines which documents the module will return. </td>
</tr>
<tr>
<td role="rowheader">Limit</td>
<td>Set the maximum number of results to be worked with during one execution cycle.</td>
</tr>
</tbody>
</table>
</div>
-->
