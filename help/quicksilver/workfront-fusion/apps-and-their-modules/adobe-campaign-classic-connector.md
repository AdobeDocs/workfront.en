---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Campaign Classic modules
description: With the Adobe Campaign Classic modules, you can start an Adobe Workfront Fusion scenario based on events in your Adobe Campaign Classic account, create, read, or update agreements and other records, search for records using criteria you set, and upload documents.
author: Becky
feature: Workfront Fusion
---
# Adobe Campaign Classic modules

With the Adobe Campaign Classic modules, you can start an Adobe Workfront Fusion scenario based on events in your Adobe Campaign Classic account, create, read, or update records, search for records using criteria you set, and perform custom API calls.

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
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Connect Adobe Campaign Connector to Adobe Workfront Fusion

1. In any Adobe Campaign Classic module, click **Add** next to the Connection field.
1. Enter the base URL that you use to connect to your Adobe Campaign Classic instance.
1. Enter your Username and Password.
1. Click **Continue** to create the connection and go back to the module.

## Adobe Campaign Classic modules and their fields

When you configure Adobe Campaign Classic modules, Workfront Fusion displays the fields listed below. Along with these, additional Adobe Campaign Classic fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Create a record

This action module creates a new record in Adobe Campaign Classic.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe Campaign Classic, see <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to Adobe Campaign Classic</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Resource</td> 
   <td>Select the type of Adobe Campaign Classic record you want to create.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fields </td> 
   <td>Select the fields that you want to set values for when the record is created, then fill in the values for those fields. Fields vary based on the type of record you select.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Custom fields</td> 
   <td> For each custom field that you want to add to the new record, click <b>Add item</b> and enter or map the field's name and value. </td> 
  </tr> 
 </tbody> 
</table>

#### Make a custom API call

This module makes a custom API call to the Adobe Campaign Classic API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
   <td>For instructions on creating a connection to Adobe Campaign Classic, see <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to Adobe Campaign Classic</a> in this article.</td> 
    </tr>
    <tr>
      <td role="rowheader">Action</td>
      <td><p>Select the action that you want the API call to perform.</p>
      <p>Execute query</p>
      <p>Write</p>
      <p>Get entity if more recent</p>
      <p>Select all</p>
      <p>Push event</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Path</p>
      </td>
      <td>
        <p>Enter a path relative to {baseURL}/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Method</p>
      </td>
      <td>
        <p>Select the HTTP request method you need to configure the API call. For more information, see HTTP request methods.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Headers</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion adds authorization headers and x-api-key headers automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Query String  </td>
      <td>
        <p>Enter the request query string.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Body</td>
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>







