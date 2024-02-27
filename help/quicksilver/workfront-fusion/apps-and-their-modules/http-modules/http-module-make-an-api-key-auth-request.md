---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
title: HTTP &gt; Make an API Key Authorization request
description: This [!DNL Adobe Workfront Fusion] action module sends an HTTPS request to a specified URL that requires an API Key Auth authorization, and processes the response.
author: Becky
feature: Workfront Fusion
exl-id: 70bf87c7-6d51-4ef4-9dce-80ad004e613f
---
# HTTP >[!UICONTROL Make an API Key Authorization request]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requires an [!DNL Adobe Workfront Fusion] license in addition to an Adobe Workfront license.

This [!DNL Adobe Workfront Fusion] action module sends an HTTPS request to a specified URL that requires an API Key Auth authorization, and processes the response.

>[!NOTE]
>
>If you are connecting to an Adobe product that does not currently have a dedicated connector, we recommend using the Adobe Authenticator module.
>
>For more information, see [Adobe Authenticator module](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

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

For information on [!UICONTROL Adobe Workfront Fusion] licenses, see [Adobe Workfront Fusion licenses](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL Make an API Key Authorization request] module configuration

When you configure the [!UICONTROL HTTP] >[!UICONTROL Make an API Key Authorization request] module, [!DNL Adobe Workfront Fusion] displays the fields listed below. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Credentials]</td> 
   <td> <p>Select the key that contains your API Key authentication credentials. To add a new key, click <strong>[!UICONTROL Add]</strong> and configure the following information:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key name]</strong></p> <p>Enter a name for this set of API credentials.</p> </li> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Enter the API Key.</p> </li> 
     <li> <p><strong>[!UICONTROL API Key placement]</strong> </p> <p>Select whether to place the API Key in the header or in the query of the API call.</p> </li> 
     <li> <p><strong>[!UICONTROL API Key parameter name]</strong> </p> <p>Enter the name by which the API call identifies the API Key, such as "apiKey" or "X-API-Key." You can find this information in the documentation of the web service the module is connecting to.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Evaluate all states as errors (except for 2xx and 3xx)] </td> 
   <td> <p>Use this option to set up error handling.</p> <p>For more information, see <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Error handling in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Enter the URL you want to send a request to, such as an API endpoint, website, etc.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object. For example, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Enter the desired query key-value pairs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Body type]</p> </td> 
   <td> <p>The HTTP Body is the data bytes transmitted in an HTTP transaction message immediately following the headers if there are any to be used.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>The Raw body type is generally suitable for most HTTP body requests even in situations where developer documentation does not specify data to send.</p> <p>Specify a form of parsing the data in the [!UICONTROL Content type] field.</p> <p>Despite the content type selected, the module enters data in any format that is stipulated or required by the developer documentation.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>This body type is to [!UICONTROL POST] data using <code>application/x-www-form-urlencoded</code>.</p> <p>For <code>[!UICONTROL application/x-www-form-urlencoded]</code>, the body of the HTTP message sent to the server is essentially one query string. The keys and values are encoded in key-value pairs separated by <code>&amp;</code> and with a <code>=</code> between the key and the value. </p> <p>For binary data, use <code>[!UICONTROL multipart/form-data]</code> instead.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Example: </b></span></span> 
       <p>Example of the resulting HTTP request format:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>The [!UICONTROL Multipart/form-data] is an HTTP multipart request used to send files and data. It is commonly used to upload files to the server.</p> <p>Add fields to be sent in the request. Each field must contain Key-Value pair.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Text]</strong> </p> <p>Enter the key and value to be sent within the request body.</p> </li> 
       <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Enter the key and specify the source file you want to send in the request body.</p> <p>Map the file you want to upload from the previous module (such as [!UICONTROL HTTP] >[!UICONTROL Get a File] or [!UICONTROL Google Drive] >[!UICONTROL Download a File)], or enter the file name and file data manually.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse response]</p> </td> 
   <td> <p>Enable this option to automatically parse responses and convert JSON and XML responses so you don't need to use [!UICONTROL JSON] > [!UICONTROL Parse JSON] or [!UICONTROL XML] > [!UICONTROL Parse XML] modules.</p> <p>Before you can use parsed JSON or XML content, run the module once manually so that the module can recognize the response content and allow you to map it in subsequent modules.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeout] </td> 
   <td> <p>Specify the request timeout in seconds (1-300). The default is 40 seconds.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Share cookies with other HTTP modules]</td> 
   <td> <p> Enable this option to share cookies from the server with all HTTP modules in your scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-signed certificate]</td> 
   <td> <p> Upload your certificate if you want to use TLS using your self-signed certificate.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reject connections that are using unverified (self-signed) certificates] </td> 
   <td> <p>Enable this option to reject connections that are using unverified TLS certificates.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow redirect]</td> 
   <td> <p> Enable this option to follow the URL redirects with 3xx responses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow all redirects] </td> 
   <td> <p>Enable this option to follow the URL redirects with all response codes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Disable serialization of multiple same query string keys as arrays]</p> </td> 
   <td> <p>By default, [!DNL Workfront Fusion] handles multiple values for the same URL query string parameter key as arrays. For example, <code>www.test.com?foo=bar&amp;foo=baz</code> will be converted to <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Activate this option to disable this feature. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Request compressed content]</td> 
   <td> <p> Enable this option to request a compressed version of the website.</p> <p>Adds an <code>[!UICONTROL Accept-Encoding]</code> header to request compressed content.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Use Mutual TLS]</td> 
   <td> <p>Enable this option to use Mutual TLS in the HTTP request.</p> <p>For more information on Mutual TLS, see <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Use Mutual TLS in HTTP modules in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
