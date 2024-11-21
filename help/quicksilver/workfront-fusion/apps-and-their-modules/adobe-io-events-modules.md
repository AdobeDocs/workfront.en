---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe I/O Events modules
description: With the Adobe I/O Events modules, you can start an Adobe Workfront Fusion scenario based on events in your Adobe applications.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 18ad8098-9742-44d2-97cd-b0c2b5591538
---
# Adobe I/O Events modules

With the Adobe I/O Events modules, you can start an Adobe Workfront Fusion scenario based on events in Adobe accounts and services that do not have a dedicated Workfront Fusion connector. 

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

## Prerequisites

Before you can use the Adobe I/O Events connector, you must ensure that the following prerequisites are met:

* You must have an active Adobe account.

## Adobe I/O Events API information

The Adobe I/O Events connector uses the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Base URL</td> 
   <td>https://api.adobe.io/events</td> 
  </tr>
  <tr> 
   <td role="rowheader">API tag</td> 
   <td>v1.6.7</td> 
  </tr>
 </tbody> 
 </table>

## Create a connection to Adobe I/O Events

To create a connection for your Adobe I/O Events modules:

1. Click Add next to the Connection box.
    
1. Fill in the following fields:
    
    <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">Connection name</td>
        <td>
          <p>Enter a name for this connection.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Type</td>
        <td>
          <p>Select whether you want to connect to a service account or a personal account.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Additional scopes</td>
        <td>To add any additional scopes, click <b>Add item</b> and enter the scope.</td>
      </tr>
      <tr>
        <td role="rowheader">Client ID</td>
        <td>Enter your Adobe Client ID. This can be found in the Credentials details section of the Adobe Developer Console</td>
      </tr>
      <tr>
        <td role="rowheader">Client Secret</td>
        <td>Enter your Adobe Client Secret. This can be found in the Credentials details section of the Adobe Developer Console</td>
      </tr>
      </tr>
        <tr>
        <td role="rowheader">Consumer org ID</td>
        <td>Enter your Consumer org ID. This can be found in the credential URL of the project: <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">Credential ID</td>
        <td>Enter your Credential ID. This can be found in the credential URL of the project: <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">IMS organization ID</td>
        <td>Enter your Adobe Organization ID. This can be found in the Credentials details section of the Adobe Developer Console</td>
      </tr>
        <tr>
        <td role="rowheader">Project ID</td>
        <td>Enter your project ID. This can be found in the credential URL of the project: <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">Workspace ID</td>
        <td>To view your project's Workspace ID, download your project details from the project overview page in Adobe Developer Console. </td>
      </tr>
    </tbody>
    </table>
    
1. Click **Continue** to save the connection and return to the module.

## Adobe I/O Events modules and their fields

When you configure [!DNL Adobe I/O Events] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Adobe I/O Events] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Searches](#searches)

### Triggers

#### Create an event registration

This action module uses a webhook to create an event description. You can configure a webhook here. If you are using an existing webhook, the fields in this module are read-only.

To create a webhook:

1. Click **Add** next to the Webhook field.
1. Fill in the following fields:

   <table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[!UICONTROL Webhook name]</td>
        <td>Enter a name for this webhook.</td>
       </tr>
       <tr>
         <td role="rowheader">[!UICONTROL Connection]</td>
        <td>For instructions on creating a connection to [!DNL Adobe I/O Events], see <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Create a connection to [!DNL Adobe I/O Events]</a> in this article.</td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Webhook description]
         </td>
         <td>
           Enter a description for this webhook.
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Event provider]
         </td>
         <td>
           Select the product or account that you want to create events from.
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Event type]
         </td>
         <td>
           Select the events that you want the webhook to watch. The scenario will trigger when these events occur.
         </td>
       </tr>
     </tbody>
   </table>

1. Click Save to save the webhook and return to the module.

### Actions

#### Get all events from a journal

This search module retrieves all events for a registration from a journal.

   <table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[!UICONTROL Connection]</td>
        <td>For instructions on creating a connection to [!DNL Adobe I/O Events], see <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Create a connection to [!DNL Adobe I/O Events]</a> in this article.</td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Registration ID]
         </td>
         <td>
           Select the registration that you want to retrieve events for.
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Maximum number of returned records]
         </td>
         <td>
              Enter or map the maximum number of records you want the module to return during each scenario execution cycle. 
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Return events that occur after]
         </td>
         <td>
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Seek]
         </td>
         <td>
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Latest]
         </td>
         <td>
         Enable this option to return the latest event.
         </td>
       </tr>
     </tbody>
   </table>

#### Make a custom API call

This action module makes a custom API call to the [!DNL Adobe I/O Events] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
        <td>For instructions on creating a connection to [!DNL Adobe I/O Events], see <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Create a connection to [!DNL Adobe I/O Events]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Enter a path relative to <code>https://api.adobe.io/events</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
  <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p>  
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion adds authorization headers and x-api-key headers automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Enter the request query string.</p>
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

### Searches

#### Get provider and event IDs

This search module gets the Adobe I/O Events IDs for the specified provider and events.

   <table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[!UICONTROL Connection]</td>
        <td>For instructions on creating a connection to [!DNL Adobe I/O Events], see <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Create a connection to [!DNL Adobe I/O Events]</a> in this article.</td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Event provider]
         </td>
         <td>
           Select the provider that you want to retrieve the ID for.
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Event type]
         </td>
         <td>
              Select the events that you want to provide IDs for. Events are available based on the event provider. 
         </td>
       </tr>
     </tbody>
   </table>

<!--

Watch Events

This trigger module starts a scenario when an event occurs in the chosen Adobe product or service.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The source of the events you want to watch</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

-->
