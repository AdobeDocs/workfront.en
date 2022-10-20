---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Campaign Classic modules
description: With the Adobe Campaign Classic modules, you can start an [!DNL Adobe Workfront Fusion] scenario based on events in your Adobe Campaign Classic account, create, read, or update agreements and other records, search for records using criteria you set, and upload documents.
author: Becky
feature: Workfront Fusion
---
# Adobe Campaign Classic modules

With the Adobe Campaign Classic modules, you can start an [!DNL Adobe Workfront Fusion] scenario based on events in your Adobe Campaign Classic account, create, read, or update records, search for records using criteria you set, and perform custom API calls.

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
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Connect Adobe Campaign Connector to Adobe Workfront Fusion

1. In any Adobe Campaign Classic module, click **Add** next to the [!UICONTROL Connection] field.
1. Enter the base URL that you use to connect to your Adobe Campaign Classic instance.
1. Enter your Username and Password.
1. Click **[!UICONTROL Continue]** to create the connection and go back to the module.

## Adobe Campaign Classic modules and their fields

When you configure Adobe Campaign Classic modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional Adobe Campaign Classic fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Searches](#searches)

### Triggers

#### Watch records

This scheduled trigger module starts a scenario when a record changes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe Campaign Classic, see <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to Adobe Campaign Classic</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td>Select whether you want to watch for new records, updated records, or both.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Resource</td> 
   <td>Select the resource that you want to watch for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fields to inlcude in output</td> 
   <td>Select the fields that you want to include in the module's output.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Custom fields to inlcude in output</td> 
   <td>For each custom field that you want to include in output, click <b>Add</b> and enter the name of the custom field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned results</td> 
   <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>


### Actions

* [Create a record](#create-a-record)
* [Custom API call](#make-a-custom-api-call)
* [Delete a record](#delete-record)
* [Misc action](#misc-action)
* [[!UICONTROL Read a record]](#read-a-record)
* [Subscription](#subscription)
* [Update a record](#update-record)

#### Create a record

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
   <td> For each custom field that you want to add to the new record, click <b>[!UICONTROL Add item]</b> and enter or map the field's name and value. </td> 
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
      <td role="rowheader">Headers</td>
      <td>
        <p>Add the headers of the request in the form of a standard [!DNL JSON] object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion adds the x-security token header automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">XML Body</td>
   <td> <p>Add the body content for the API call in XML, without the session element. </td>     </tr>
  </tbody>
</table>

#### Delete Record

This action module deletes a single record from Adobe Campaign Classic.

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
   <td>Select the type of resource that you want to delete.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter or map the ID of the resourece you want to delete.</td> 
  </tr> 
 </tbody> 
</table>


#### Perform an action

This action module performs a selected action on an object in the Adobe Campaign Classic API.

For information on specific actions and fields, see [Adobe Campaign - API Documentation](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).
[test](#delete-record)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe Campaign Classic, see <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to Adobe Campaign Classic</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Action</td> 
   <td><p>Select the action to perform on the object.</p>
   <ul>
   <li><p><b>List</b></p><p> For available fields, see <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in this article. </p></li>
     <li><p><b>Get</b></p><p> For available fields, see <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in this article. </p></li> 
   <li><p><b>Create</b></p><p> For available fields, see <a href="#create-a-record" class="MCXref xref" >Create a record</a> in this article. </p></li>
   <li><p><b>Update</b></p><p> For available fields, see <a href="#update-record" class="MCXref xref" >Update a record</a> in this article. </p></li>
   <li><p><b>Delete</b></p><p> For available fields, see <a href="#delete-record" class="MCXref xref" >[!UICONTROL Delete] a record</a> in this article. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### Read a record

This action module reads a record from Adobe Campaign Classic.

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
   <td>Select the type of Adobe Campaign Classic record you want to read.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">ID </td> 
   <td>Enter of map the ID of the record you want to read.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">Fields to include in output </td> 
   <td>Select the fields that you want to include in the module's output.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Custom fields to include in output</td> 
   <td>For each custom field that you want to include in output, click <b>Add</b> and enter the name of the custom field.</td> 
  </tr> 
 </tbody> 
</table>


#### Subscribe or unsubscribe

This action module subscribes a user to or unsubscribes a user from an information service.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions on creating a connection to Adobe Campaign Classic, see <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >Create a connection to Adobe Campaign Classic</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subscribe or unsubscribe</td> 
   <td>Select whether you want to subscribe or unsubscribe to the information service.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Service name</td> 
   <td>Select the service that you want to subscribe to or unsubscribe from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Recipient email address </td> 
   <td>Enter or map the email address of the user you want to subscribe or unsubscribe to the information service.</td> 
  </tr> 
 </tbody> 
</table>

#### Update record

This action module updates a single record in Adobe Campaign Classic.

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
   <td role="rowheader">ID </td> 
   <td>Enter of map the ID of the record you want to update.</td> 
  </tr> 
<tr> 
   <td role="rowheader">Fields </td> 
   <td>Select the fields that you want to update values for, then fill in the values for those fields. Fields vary based on the type of record you select.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Custom fields</td> 
   <td> For each custom field that you want to update, click <b>[!UICONTROL Add item]</b> and enter or map the field's name and value. </td> 
  </tr> 
 </tbody> 
</table>

### Searches

#### Search

This search module returns records based on the specified criteria.

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
   <td role="rowheader">Limit </td> 
   <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

