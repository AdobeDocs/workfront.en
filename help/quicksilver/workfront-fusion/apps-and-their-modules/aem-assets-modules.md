---
filename: aem-assets-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets modules
description: With the Adobe Experience Manager Assets connector for Adobe Workfront Fusion, you can start a scenario based on events in your Adobe Experience Manager Assets account, create, upload, and update assets, and copy or move folders and assets.
---

# Adobe Experience Manager Assets modules

With the Adobe Experience Manager Assets connector for Adobe Workfront Fusion, you can start a scenario based on events in your Adobe Experience Manager Assets account, create, upload, and update assets, and copy or move folders and assets.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

* You must have an Adobe Experience Manager Assets account to use these modules.
* You must set up Server-to-server flow in the Adobe Developer console.

  For instructions on setting up Server-to-server flow on the Adobe Developer Console, see [Generating Access Tokens for Server Side APIs](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## Connect Adobe Experience Manager Assets to Workfront Fusion

To create a connection for your Adobe Experience Manager Assets modules:

1. Click `Add` next to the Connection box.
1. Fill in the following fields.

   >[!NOTE]
   >
   >The information for these fields is generated as part of setting up Server-to-server flow on the Adobe Developer Console. You can find these values in the service credentials JSON file generated as part of that setup.
   >
   >
   >For instructions on setting up Server-to-server flow on the Adobe Developer Console, see [Generating Access Tokens for Server Side APIs](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Connection name</td> 
      <td> <p>Enter a name for this connection</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instance URL without a trailing slash</td> 
      <td>Enter the URL for your Adobe Experience Manager instance. Do not include a slash <code>/</code> at the end of the URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Client ID</td> 
      <td>Enter the Client ID generated in the Server-to-server setup.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Client Secret</td> 
      <td>Enter the Client Secret generated in the Server-to-server setup.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Technical account ID</td> 
      <td>Enter the ID&nbsp;of the technical account. This is the "id" field in the client credentials JSON file.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Org ID</td> 
      <td>Enter the ID&nbsp;of your organization. This is the "org" field in the client credentials JSON file.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meta Scopes</td> 
      <td>Enter the Meta Scopes generated in the service-to-service setup.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Private key</td> 
      <td>Enter the Private Key generated win the Server-to-server setup. To extract the private key, click Extrace, then enter the</td> 
     </tr> 
    </tbody> 
   </table>

## Adobe Experience Manager Assets modules and their fields

When you configure Adobe Experience Manager Essentials modules, Workfront Fusion displays the fields listed below. Along with these, additional Adobe Experience Manager Essentials fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Create a record

This action module creates a folder or an asset comment.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Experience Manager Assets account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Adobe Experience Manager Assets to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object type</td> 
   <td> <p>Select whether you want to create a folder or a comment on an asset.</p> 
    <ul> 
     <li> <p>Folder</p> <p>Fill in the following fields:</p> 
      <ul> 
       <li> <p>Name</p> <p>Enter a name for the folder. This name will appear in the file path, so it must not include spaces or other characters. </p> </li> 
       <li> <p>Title</p> <p>Enter a title for the folder, which can be displayed instead of the name.</p> </li> 
      </ul> </li> 
     <li> <p>Asset comment</p> <p>Select or map the ID of the asset you want to add a comment to, and enter the text of the comment.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Get folder listing

This action module retrieves a representation of an existing folder and of its child entities (folders or assets).

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Experience Manager Assets account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Adobe Experience Manager Assets to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder</td> 
   <td>Select or map the folder that you want to retrieve. To add subfolders to the path, click the plus icon and select the subfolder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned records</td> 
   <td> <p>Enter or map the maximum number of records you want the module to [action] during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Make a custom API call

This action module makes a custom API call to the Adobe Experience Manager Assets API.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Adobe Experience Manager Assets account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Adobe Experience Manager Assets to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>URL</p> </td> 
   <td> <p>Enter a path relative to </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Method</p> </td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods</a>.</p> </td> 
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

&nbsp;
