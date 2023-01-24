---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: HTTP request methods in [!DNL Adobe Workfront Fusion]
description: When you are configuring an API call in a module, you need to fill in the field for the HTTP request method.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
---
# HTTP request methods in [!DNL Adobe Workfront Fusion]

When you are configuring an API call in a module, you need to fill in the field for the HTTP request method.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
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

## HTTP methods

Use one of the following HTTP methods.

* **[!UICONTROL GET]**: Retrieves data from a web server based on your parameters. [!UICONTROL GET] requests a representation of the specified resource, and receives a [!UICONTROL 200 OK] response message with the requested content if successful.
* **[!UICONTROL POST]**: Sends data to a web server based on your parameters. [!UICONTROL POST] requests include actions like uploading a file. Multiple [!UICONTROL POST]s may result in a different outcome than a single [!UICONTROL POST], so be cautious about unintentionally sending multiple [!UICONTROL POST]s. If a [!UICONTROL POST] is successful, you receive a [!UICONTROL 200 OK] response message.
* **[!UICONTROL PUT]**: Sends data to a location in the web server based on your parameters. [!UICONTROL PUT] requests include actions like uploading a file. The difference between a [!UICONTROL PUT] and [!UICONTROL POST] is that PUT is idempotent, meaning that the result of a single successful [!UICONTROL PUT] is the same as many identical [!UICONTROL PUT]s. If a PUT is successful, you receive a 200 response message (usually 201 or 204).
* **[!UICONTROL PATCH]**: (Not available for some API call modules) Applies partial modifications to a resource on a web server based on your parameters. [!UICONTROL PATCH] is not idempotent, meaning that the result of multiple [!UICONTROL PATCH]'s could have unintended consequences. If a [!UICONTROL PATCH] is successful, you will receive a 200 response message (usually 204).
* **[!UICONTROL DELETE]**: Deletes the specified resource from the web server based on your parameters (if the resource exists). If a [!UICONTROL DELETE] is successful, you receive a 200 OK response message.
