---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Adobe Journey Optimizer, as well as connect it to multiple third-party applications and services. 
author: Becky
---

# Adobe Journey Optimizer Modules

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

In an Adobe Workfront Fusion scenario, you can automate workflows that use Adobe Journey Optimizer, as well as connect it to multiple third-party applications and services. Adobe Journey Optimizer modules allow you to ,reate, read, update, or delete records,list all records of a given type, search records based on criteria you specify, or perform a custom API call to the Adobe Journey Optimizer API.


If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Adobe Workfront plan*</td>
      <td>
        <p>Pro or higher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Adobe Workfront license*</td>
      <td>
        <p>Plan, Work</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Adobe Workfront Fusion license**</td>
      <td >
        <p>Workfront Fusion for Work Automation and Integration</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">Access level configurations*</td>
      <td>
        <p>You must be a Workfront Fusion administrator for your organization.</p>
        <p>You must be a Workfront Fusion administrator for your team.</p>
      </td>
    </tr>
  </tbody>
</table>


&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

Before you can use the Adobe Journey Optimizer connector, you must ensure that the following prerequisites are met:

*   You must have an active Adobe Journey Optimizer account.

## Adobe Journey Optimizer modules and their fields

When you configure Adobe Journey Optimizer modules, Workfront Fusion displays the fields listed below. Along with these, additional Adobe Journey Optimizer fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

#### Make a custom API call

This module makes a custom API call to the Adobe Journey Optimizer API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
      <td>Connection</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Path</p>
      </td>
      <td>
        <p>Enter a path relative to {baseURL} starting with<code>/</code></p>
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
     <tr>
      <td role="rowheader">Limit  </td>
      <td>
        <p>Enter the maximum number of results that you want the module to return in one execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>
