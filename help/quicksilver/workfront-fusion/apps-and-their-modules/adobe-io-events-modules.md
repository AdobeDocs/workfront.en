---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe IO Events modules
description: With the Adobe IO Events modules, you can start an Adobe Workfront Fusion scenario based on events in your Adobe applications.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 01158218-31a6-4c68-a9b7-6a678a8f40c9
---
# Adobe IO Events modules

With the Adobe IO Events modules, you can start an Adobe Workfront Fusion scenario based on events in your Adobe IO Events account, create, read, or update agreements and other records, search for records using criteria you set, and upload documents.

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

Before you can use the Adobe IO Events connector, you must ensure that the following prerequisites are met:

*   You must have an active Adobe account.

## Create a connection to Adobe IO Events

To create a connection for your Adobe IO Events modules:

1.  Click Add next to the Connection box.
    
2.  Fill in the following fields:
    
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
        <td role="rowheader">Client ID</td>
        <td>Enter your Adobe Client ID. This can be found in the Credentials details section of the Adobe Developer Console</td>
      </tr>
      <tr>
        <td role="rowheader">Client Secret</td>
        <td>Enter your Adobe Client Secret. This can be found in the Credentials details section of the Adobe Developer Console</td>
      </tr>
      <tr>
        <td role="rowheader">Organization ID</td>
        <td>Enter your Adobe Organization ID. This can be found in the Credentials details section of the Adobe Developer Console</td>
      </tr>
      <tr>
        <td role="rowheader">Technical account ID</td>
        <td>Enter your Adobe Technical account ID. This can be found in the Credentials details section of the Adobe Developer Console</td>
      </tr>
      <tr>
        <td role="rowheader">Tenant</td>
        <td>
          <p> To locate your Tenant, log in to the Adobe Experience Cloud, open IO Events, and click the IO Events card. Use the Tenant ID value as noted in the URL subdomain.</p>
          <p>For example, if your URL when logged in to Adobe IO Events is <code>&lt;https://mycompany.experiencecloud.adobe.com/...&gt;</code> then your Tenant ID is "mycompany."</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Private key</td>
        <td>
          <p>Enter the private key that was generated when your credentials were created in the Adobe Developer Console. </p>
          <p>To extract your private key or certificate:</p>
          <ol>
            <li value="1">
              <p>Click <b>Extract</b>.</p>
            </li>
            <li value="2">
              <p>Select the type of file you are extracting.</p>
            </li>
            <li value="3">
              <p>Select the file that contains the private key or certificate.</p>
            </li>
            <li value="4">
              <p>Enter the password for the file.</p>
            </li>
            <li value="5">
              <p>Click <b>Save</b> to extract the file and return to the connection setup.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
  </table>
    
1.  Click **Continue** to save the connection and return to the module.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for build status changes</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>
