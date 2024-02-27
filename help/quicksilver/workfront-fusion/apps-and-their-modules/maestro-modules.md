---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Maestro modules
description: With the [!DNL Adobe Maestro] modules, you can start an [!DNL Adobe Workfront Fusion] scenario based on events in your [!DNL Adobe] Maestro account, create, read, or update agreements and other records, search for records using criteria you set, and upload documents.
author: Becky
feature: Workfront Fusion
hide: yes
hidefromtoc: yes
---
# [!DNL Adobe Maestro] modules

With the [!DNL Adobe Maestro] modules, you can trigger a scenario when events occur in Maestro. You can also create, read, update, and delete records, or perform a custom API call to your [!DNL Adobe Maestro] account.

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

## Create a connection to [!DNL Adobe Maestro]

You can create a connection to your [!DNL Maestro] account directly from inside a [!DNL Workfront Fusion] module.

1. In any [!DNL Maestro] app module, click **[!UICONTROL Add]** next to the [!UICONTROL Connection] box.
1. Enter a name for this connection.
1. Select whether you want to connect to a production environment, or a non-production environment.
1. Select whether you are connecting to a service account or a personal account.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

## [!DNL Adobe Maestro] modules and their fields

### Watch Events

This trigger module starts a scenario when a record, record type, or workspace is created, updated, or deleted in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>Select the webhook that you want to use, or click Add to create a new one.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Object type]</td>
      <td>Select whether you want to watch records, record types, or workspaces.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Objects to watch]</td>
      <td>Select whether you want to watch for new. updated, new and updated, or deleted records.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Exclude updates made by this connection]</p>
      </td>
      <td>Enable this option to prevent the scenario from triggering when a change is made by the connection used by this module. This prevents another instance of the scenario being triggered if this scenario performs a triggering action.</td> 
      </tr>
  </tbody>
</table>

### Delete a record type

This action module deletes a single record type in Maestro by its ID.

>[!WARNING]
>
>Deleting a record type in Maestro also deletes all records in the record type table. 

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record type ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Make a custom API call

This module makes a custom API call to the [!DNL Adobe Maestro] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Enter a path relative to https://&ltWORKFRONT_DOMAIN&gt/attask/api/&ltAPI_VERSION&gt/</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API version]</p>
      </td>
      <td>
        <p>Select the API version that you want to use. If you do not select a version, the most recent version will be used by default.</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API Path override]</p>
      </td>
      <td>
        <p>Enter a path relative to https://&ltWORKFRONT_DOMAIN&gt/attask/api/&ltAPI_VERSION&gt/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] adds authorization headers automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>For each key/value pair that you want to add to the query string, click <b>Add item</b> and enter the key and value.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Maestro by its ID.

>[!WARNING]
>
>Deleting a field in Maestro deletes it and any data in it from every object of that record type in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the record type you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Get a field 


This action module retrieves a single field in Maestro by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

-->

### Create a record

This action creates a single record in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record type ID]</p>
      </td>
      <td>Enter or map the type of record you want to create. Available record types are based on your Maestro account.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Other fields</p>
      </td>
      <td>These fields are based on the record type you selected.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Delete a record

This action module deletes the specified record in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>Enter or map the ID of the record you want to delete.</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Maestro] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### Get a record

This action module retrieves a single record from [!DNL Adobe Maestro], specified by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record ID]</td>
      <td>Enter or map the ID of the record you want to retrieve.</td>
    </tr>
  </tbody>
</table>

### Get records by record type

This action module retrieves all records of the specified type.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Select or map the workspace that contains the records you want to retrieve.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>Select the type of record that you want to retrieve.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
  </tbody>
</table>

### Get record types

This action module retrieves a list of record types in an [!DNL Adobe Maestro] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
  </tbody>
</table>

### Update record

This action updates a single record in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>Enter or map the type of record you want to update . Available record types are based on your Maestro account.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Other fields</p>
      </td>
      <td>These fields are based on the record type you selected.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Search records

This action module retrieves a list of records based on criteria you specify.

>[!NOTE]
>
>This module is under construction.

