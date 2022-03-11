---
filename: servicenow-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: ServiceNow modules
description: In a Adobe Workfront Fusion scenario, you can connect your ServiceNow account to multiple third-party applications and services.
---

# ServiceNow modules

In a `Adobe Workfront Fusion` scenario, you can connect your `ServiceNow` account to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront Fusion</span> license**</td> 
   <td> <p><span>Workfront Fusion for Work Automation and Integration</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <span>Adobe Workfront Fusion</span> as well as <span>Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

&#42;&#42;For information on `Adobe Workfront Fusion` licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use ServiceNow modules, you must have a ServiceNow account.

## Connect ServiceNow to `Workfront Fusion`

To create a connection for your ServiceNow modules:

<ol> 
 <li value="1">Click <span class="bold">Add</span> next to the Connection box when you begin configuring the first ServiceNow module.</li> 
 <li value="2"> <p>Enter the following:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"> <p>Connection name</p> </td> 
     <td>Enter a name for the new ServiceNow connection</td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>Username</p> </td> 
     <td>Enter your ServiceNow username.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>Password</p> </td> 
     <td>Enter your ServiceNow password.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>Instance</p> </td> 
     <td> <p>Enter the address of your ServiceNow account without <code>https://</code> (usually <code><company>.service-now.com</code>).</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

## ServiceNow modules and their fields

When you configure `ServiceNow` modules, `Workfront Fusion` displays the fields listed below. Along with these, additional `ServiceNow` fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>If a custom record is selected in a "Record type" field, it may take some time to load the custom fields. 
>
>If there are no custom records, the dropdown will be empty.

* [Watch records](#watch) 
* [Custom API Call](#custom) 
* [Read a record](#read) 
* [Deactivate a User](#deactiva) 
* [Download an attachment](#download) 
* [Upload an attachment](#upload) 
* [Create a record](#create) 
* [Update a record](#update) 
* [Delete a record](#delete) 
* [Search for records](#search)

### Watch records

This trigger module activates a scenario when a record is created or updated.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your ServiceNow account to <span>Workfront Fusion</span>, see <a href="#connect" class="MCXref xref">Connect ServiceNow to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table type</td> 
   <td>Select whether the table you want to watch is a custom table or a standard table.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
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
   <td> <p>Enter or map the maximum number of <span>record</span>s you want the module to <span>return</span> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Custom API Call

This action module lets you make a custom authenticated call to the `ServiceNow` API. This way, you can create a data flow automation that can't be accomplished by the other `ServiceNow` modules.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your ServiceNow account to <span>Workfront Fusion</span>, see <a href="#connect" class="MCXref xref">Connect ServiceNow to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Relative URL</td> 
   <td> <p>Type the address on the web server that you want the module to interact with.</p> <p>You can type a relative URL, which means that you don’t have to include the protocol (such as <code>http://</code>) at the beginning. This suggests to the web server that the interaction is occurring on the server.</p> <p>For example: <code>/api/conversations.create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> </td> 
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

### Read a record

This action module reads a ServiceNow record by using the system ID.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your ServiceNow account to <span>Workfront Fusion</span>, see <a href="#connect" class="MCXref xref">Connect ServiceNow to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record System ID</td> 
   <td>Enter or map the unique ServiceNow ID of the record that you want the module to read.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table type</td> 
   <td>Select whether the record you want to read is in a custom table or a standard table.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select the type of <span>ServiceNow</span> record that you want the module to <span>read</span>.</td> 
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

### Deactivate a User

This action module deactivates a user in ServiceNow by using the system ID.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your ServiceNow account to <span>Workfront Fusion</span>, see <a href="#connect" class="MCXref xref">Connect ServiceNow to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">User System ID</td> 
   <td>Enter or map the unique ServiceNow ID of the user that you want the module to deactivate.</td> 
  </tr> 
 </tbody> 
</table>

### Download an attachment

This action module downloads an attachment in a ServiceNow record.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your ServiceNow account to <span>Workfront Fusion</span>, see <a href="#connect" class="MCXref xref">Connect ServiceNow to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Attachment System ID</td> 
   <td>Enter or map the unique ServiceNow ID of the attachment that you want the module to download.</td> 
  </tr> 
 </tbody> 
</table>

### Upload an attachment

This action module uploads an attachment to a ServiceNow record.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your ServiceNow account to <span>Workfront Fusion</span>, see <a href="#connect" class="MCXref xref">Connect ServiceNow to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table name</td> 
   <td>Enter or map the name of the table where you want to upload the attachment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">System ID</td> 
   <td>Enter or map the unique ServiceNow ID of the System where you want to upload the attachment.</td> 
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

### Create a record

This action module creates a new ServiceNow record.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your ServiceNow account to <span>Workfront Fusion</span>, see <a href="#connect" class="MCXref xref">Connect ServiceNow to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table type</td> 
   <td>Select whether you want to create a record in a custom table or a standard table.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select the type of <span>ServiceNow</span> record that you want the module to <span>create</span>. You can then fill in the available fields for this record type.</td> 
  </tr> 
 </tbody> 
</table>

### Update a record

This action module creates a new ServiceNow record.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your ServiceNow account to <span>Workfront Fusion</span>, see <a href="#connect" class="MCXref xref">Connect ServiceNow to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record System ID</td> 
   <td>Enter or map the unique ServiceNow ID of the record that you want the module to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table type</td> 
   <td>Select whether the record want to update is in a custom table or a standard table.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select the type of <span>ServiceNow</span> record that you want the module to <span>update</span>. You can then fill in the available fields for this record type.</td> 
  </tr> 
 </tbody> 
</table>

### Delete a record

This action module `deletes an incident or a user`.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your ServiceNow account to <span>Workfront Fusion</span>, see <a href="#connect" class="MCXref xref">Connect ServiceNow to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select whether you want to delete an incident or a user.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">System ID</td> 
   <td>Enter or map the unique ServiceNow ID of the record that you want the module to delete.</td> 
  </tr> 
 </tbody> 
</table>

### Search for records

This module searches for records using criteria you select.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map `this information` in subsequent modules in the scenario.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your ServiceNow account to <span>Workfront Fusion</span>, see <a href="#connect" class="MCXref xref">Connect ServiceNow to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table type</td> 
   <td>Select whether the table you want to search is a custom table or a standard table.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td>Select the type of record that you want to search for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Result set</td> 
   <td>Select whether you want the module to return all records that match the criteria, or only the first record to match it. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximal count of records</td> 
   <td> <p>Enter or map the maximum number of <span>record</span>s you want the module to <span>return</span> during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Search type</td> 
   <td> <p>Select what type of search you want the module to execute</p> 
    <ul> 
     <li> <p><span class="bold">Advanced query</span> </p> 
      <ul> 
       <li> <p>Search Query</p> <p>Enter the custom search query. For information on ServiceNow custom search queries, see the <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">ServiceNow query documentation</a>.</p> </li> 
      </ul> </li> 
     <li> <p><span class="bold">Simple</span> </p> 
      <ul> 
       <li> <p>Search Criteria</p> <p>Enter the criteria by which you want the module to search. For more information on setting up search filters, see <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Add a filter to a scenario</a>.</p> </li> 
       <li> <p>Sort by</p> <p>Indicate which field you want the module to sort results by, and whether they should be sorted ascending or descending.</p> </li> 
      </ul> </li> 
    </ul> <p>&nbsp;</p> </td> 
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

