---
filename: http-request-methods
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: HTTP request methods in Adobe Workfront Fusion
description: When you are configuring an API call in a module, you need to fill in the field for the HTTP request method.
---

# HTTP request methods in Adobe Workfront Fusion

When you are configuring an API call in a module, you need to fill in the field for the HTTP request method.

## Access requirements

You must have the following access to use the functionality in this article:

<table> 
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
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## HTTP methods

Use one of the following HTTP methods.

* **GET**: Retrieves data from a web server based on your parameters. GET requests a representation of the specified resource, and receives a 200 OK response message with the requested content if successful.
* **POST**: Sends data to a web server based on your parameters. POST requests include actions like uploading a file. Multiple POSTs may result in a different outcome than a single POST, so be cautious about unintentionally sending multiple POSTs. If a POST is successful, you receive a 200 OK response message.
* **PUT**: Sends data to a location in the web server based on your parameters. PUT requests include actions like uploading a file. The difference between a PUT and POST is that PUT is idempotent, meaning that the result of a single successful PUT is the same as many identical PUTs. If a PUT is successful, you receive a 200 response message (usually 201 or 204).
* **PATCH**: (Not available for some API call modules) Applies partial modifications to a resource on a web server based on your parameters. PATCH is not idempotent, meaning that the result of multiple PATCH’s could have unintended consequences. If a PUT is successful, you will receive a 200 response message (usually 204).
* **DELETE**: Deletes the specified resource from the web server based on your parameters (if the resource exists). If a DELETE is successful, you receive a 200 OK response message.

