---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: "Adobe I/O Events modules"
description: "With the Adobe I/O Events modules, you can start an Adobe Workfront Fusion scenario based on events in your Adobe applications."
author: Becky
feature: Workfront Fusion, Digital Content and Documents
---
# Adobe I/O Events module

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

*   You must have an active Adobe account.

## Create a connection to Adobe I/O Events

To create a connection for your Adobe I/O Events modules:

1.  Click Add next to the Connection box.
    
1.  Fill in the following fields:
    
    <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">Connection type</td>
        <td>
          <p>Select whether you want to connect using a service account or using OAuth.</p>
        </td>
      </tr>
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
        <td role="rowheader">Technical account ID</td>
        <td>Enter your Adobe Technical account ID. This can be found in the Credentials details section of the Adobe Developer Console</td>
      </tr>
      <tr>
        <td role="rowheader">Organization ID</td>
        <td>Enter your Adobe Organization ID. This can be found in the Credentials details section of the Adobe Developer Console</td>
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
        <tr>
        <td role="rowheader">Consumer Org ID</td>
        <td>Enter your Consumer Org ID. This can be found in the credential URL of the project: <code>https://developer.adobe.com/console/projects/{consumerOrgId}/ {projectId}/credentials/{credentialId}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">Credential ID</td>
        <td>Enter your Adobe Technical account ID. This can be found in the credential URL of the project: <code>https://developer.adobe.com/console/projects/{consumerOrgId}/ {projectId}/credentials/{credentialId}/details</code></td>
      </tr>
    </tbody>
    </table>
    
1.  Click **Continue** to save the connection and return to the module.

## Adobe I/O Events module and its fields

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
