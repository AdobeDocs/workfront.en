---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: ServiceNow modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL ServiceNow], as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
---
# ServiceNow modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL ServiceNow], as well as connect it to multiple third-party applications and services.

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
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

To use [!DNL ServiceNow] modules, you must have a [!DNL ServiceNow] account.

## Connect [!DNL ServiceNow] to [!DNL Workfront] Fusion {#connect-servicenow-to-workfront-fusion}

To create a connection for your [!DNL ServiceNow] modules:

1. Click **Add** next to the Connection box when you begin configuring the first [!DNL ServiceNow] module.
1. Enter the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Connection name</p> </td> 
      <td>Enter a name for the new [!DNL ServiceNow] connection</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Username</p> </td> 
      <td>Enter your [!DNL ServiceNow] username.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Password</p> </td> 
      <td>Enter your ServiceNow password.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Instance</p> </td> 
      <td> <p>Enter the address of your [!DNL ServiceNow] account without <code>https://</code> (usually <code>&lt;company>.service-now.com</code>).</p> </td> 
     </tr> 
    </tbody> 
   </table>

## ServiceNow modules and their fields

When you configure [!DNL ServiceNow] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL ServiceNow] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>If a custom record is selected in a "Record type" field, it may take some time to load the custom fields.
>
>If there are no custom records, the dropdown will be empty.

* [Watch records](#watch-records)
* [Custom API Call](#custom-api-call)
* [[!UICONTROL Read a record]](#read-a-record)
* [Deactivate a User](#deactivate-a-user)
* [Download an attachment](#download-an-attachment)
* [[!UICONTROL Upload an attachment]](#upload-an-attachment)
* [Create a record](#create-a-record)
* [Update a record](#update-a-record)
* [Delete a record](#delete-a-record)
* [[!UICONTROL Search for records]](#search-for-records)

### Watch records  {#watch-records}

This trigger module activates a scenario when a record is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your ServiceNow account to Workfront Fusion, see <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect ServiceNow] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table type</td> 
   <td>Select whether the table you want to watch is a custom table or a standard table.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td>Select the type of record that you want to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Display</td> 
   <td>Select the type of values that you want to display.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the fields that you want the module to output.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td>Select whether you want to watch new records or updated records.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Custom API Call {#custom-api-call}

This action module lets you make a custom authenticated call to the [!DNL ServiceNow] API. This way, you can create a data flow automation that can't be accomplished by the other [!DNL ServiceNow] modules.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your ServiceNow account to Workfront Fusion, see <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect ServiceNow] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Relative URL</td> 
   <td> <p>Type the address on the web server that you want the module to interact with.</p> <p>You can type a relative URL, which means that you don't have to include the protocol (such as <code>http://</code>) at the beginning. This suggests to the web server that the interaction is occurring on the server.</p> <p>For example: <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard [!DNL JSON] object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{“name”:“something-urgent”}</code></p> </td> 
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

### Read a record {#read-a-record}

This action module reads a [!DNL ServiceNow] record by using the system ID.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your ServiceNow account to Workfront Fusion, see <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect ServiceNow] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record System ID</td> 
   <td>Enter or map the unique [!DNL ServiceNow] ID of the record that you want the module to read.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table type</td> 
   <td>Select whether the record you want to read is in a custom table or a standard table.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select the type of [!DNL ServiceNow] record that you want the module to read.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Display</td> 
   <td>Select the type of values that you want to display.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the fields that you want the module to output.</td> 
  </tr> 
 </tbody> 
</table>

### Deactivate a User {#deactivate-a-user}

This action module deactivates a user in [!DNL ServiceNow] by using the system ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your ServiceNow account to Workfront Fusion, see <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect ServiceNow] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">User System ID</td> 
   <td> Enter or map the unique [!DNL ServiceNow] ID of the user that you want the module to deactivate.</td> 
  </tr> 
 </tbody> 
</table>

### Download an attachment {#download-an-attachment}

This action module downloads an attachment in a [!DNL ServiceNow] record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your ServiceNow account to Workfront Fusion, see <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect ServiceNow] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Attachment System ID</td> 
   <td> Enter or map the unique [!DNL ServiceNow] ID of the attachment that you want the module to download.</td> 
  </tr> 
 </tbody> 
</table>

### Upload an attachment {#upload-an-attachment}

This action module uploads an attachment to a [!DNL ServiceNow] record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your ServiceNow account to Workfront Fusion, see <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect ServiceNow] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table name</td> 
   <td>Enter or map the name of the table where you want to upload the attachment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">System ID</td> 
   <td>Enter or map the unique [!DNL ServiceNow] ID of the System where you want to upload the attachment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">File name</td> 
   <td>Enter or map a name for the attachment</td> 
  </tr> 
  <tr> 
   <td role="rowheader">File content</td> 
   <td>Enter or map the file that you want to upload to ServiceNow.</td> 
  </tr> 
 </tbody> 
</table>

### Create a record {#create-a-record}

This action module creates a new [!DNL ServiceNow] record.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your ServiceNow account to Workfront Fusion, see <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect ServiceNow] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table type</td> 
   <td>Select whether you want to create a record in a custom table or a standard table.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select the type of [!DNL ServiceNow] record that you want the module to create. You can then fill in the available fields for this record type.</td> 
  </tr> 
 </tbody> 
</table>

### Update a record {#update-a-record}

This action module creates a new [!DNL ServiceNow] record.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your ServiceNow account to Workfront Fusion, see <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect ServiceNow] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record System ID</td> 
   <td>Enter or map the unique [!DNL ServiceNow] ID of the record that you want the module to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table type</td> 
   <td>Select whether the record want to update is in a custom table or a standard table.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select the type of ServiceNow record that you want the module to update. You can then fill in the available fields for this record type.</td> 
  </tr> 
 </tbody> 
</table>

### Delete a record {#delete-a-record}

This action module deletes an incident or a user.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your ServiceNow account to Workfront Fusion, see <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect ServiceNow] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select whether you want to delete an incident or a user.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">System ID</td> 
   <td>Enter or map the unique [!DNL ServiceNow] ID of the record that you want the module to delete.</td> 
  </tr> 
 </tbody> 
</table>

### Search for records {#search-for-records}

This module searches for records using criteria you select.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your ServiceNow account to Workfront Fusion, see <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect ServiceNow] to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table type</td> 
   <td>Select whether the table you want to search is a custom table or a standard table.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td>Select the type of record that you want to search for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Result set</td> 
   <td>Select whether you want the module to return all records that match the criteria, or only the first record to match it. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximal count of records</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Search type</td> 
   <td> <p>Select what type of search you want the module to execute</p> 
    <ul> 
     <li> <p><strong>Advanced query</strong> </p> 
      <ul> 
       <li> <p>Search Query</p> <p>Enter the custom search query. For information on [!DNL ServiceNow] custom search queries, see the <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">ServiceNow query documentation</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>Simple</strong> </p> 
      <ul> 
       <li> <p>Search Criteria</p> <p>Enter the criteria by which you want the module to search. For more information on setting up search filters, see <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Add a filter to a scenario in Adobe Workfront Fusion</a>.</p> </li> 
       <li> <p>Sort by</p> <p>Indicate which field you want the module to sort results by, and whether they should be sorted ascending or descending.</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Display</td> 
   <td>Select the type of values that you want to display.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the fields that you want the module to output.</td> 
  </tr> 
 </tbody> 
</table>
