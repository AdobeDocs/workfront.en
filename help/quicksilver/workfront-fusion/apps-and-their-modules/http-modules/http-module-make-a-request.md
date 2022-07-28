---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
title: HTTP &gt; Make a request module
description: The Adobe Workfront Fusion HTTP &gt; Make a request module is a universal module that enables you to configure an HTTP request and submit it to a server. The received HTTP response is then contained in the output bundle.
author: Becky
feature: Workfront Fusion
exl-id: 7857c395-ce84-480e-8fa2-065035ac5b95
---
# HTTP > Make a request module

Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
The Adobe Workfront Fusion HTTP > Make a request module is a universal module that enables you to configure an HTTP request and submit it to a server. The received HTTP response is then contained in the output bundle.

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

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## HTTP > Make a request module configuration

When you configure the HTTP > Make a request module, Adobe Workfront Fusion displays the fields listed below. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Evaluate all states as errors (except for 2xx and 3xx ) </td> 
   <td> <p>Use this option to set up error handling.</p> <p>For more information, see <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Error handling in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL </td> 
   <td> <p>Enter the URL you want to send a request to, such as an API endpoint, website, etc.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Method</p> </td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers </td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.For example, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p> Enter the desired query key-value pairs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Body type</p> </td> 
   <td> <p>The HTTP Body is the data bytes transmitted in an HTTP transaction message immediately following the headers if there are any to be used.</p> 
    <ul> 
     <li> <p><strong>Raw</strong> </p> <p>The Raw body type is generally suitable for most HTTP body requests even in situations where developer documentation does not specify data to send.</p> <p>Specify a form of parsing the data in the Content type field.</p> <p>Despite the content type selected, data is entered in any format that is stipulated or required by the developer documentation.</p> </li> 
     <li> <p><strong>Application/x-www-form-urlencoded</strong> </p> <p>This body type is to POST data using <code>application/x-www-form-urlencoded</code>.</p> <p>For <code>application/x-www-form-urlencoded</code>, the body of the HTTP message sent to the server is essentially one query string. The keys and values are encoded in key-value pairs separated by <code>&amp;</code> and with a <code>=</code> between the key and the value. </p> <p>For binary data, <code>use multipart/form-data</code> instead.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Example: </b></span></span> 
       <p>Example of the resulting HTTP request format:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>Multipart/form-data</strong> </p> <p>The Multipart/form-data is an HTTP multipart request used to send files and data. It is commonly used to upload files to the server.</p> <p>Add fields to be sent in the request. Each field must contain Key-Value pair.</p> 
      <ul> 
       <li> <p><strong>Text</strong> </p> <p>Enter the key and value to be sent within the request body.</p> </li> 
       <li> <p><strong>File</strong> </p> <p>Enter the key and specify the source file you want to send in the request body.</p> <p>Map the file you want to upload from the previous module (such as HTTP &gt; Get a File or Google Drive &gt; Download a File), or enter the file name and file data manually.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Parse response</p> </td> 
   <td> <p>Enable this option to automatically parse responses and convert JSON and XML responses so you don't need to use JSON &gt; Parse JSON or XML &gt; Parse XML modules.</p> <p>Before you can use parsed JSON or XML content, run the module once manually so that the module can recognize the response content and allow you to map it in subsequent modules.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>User name</p> </td> 
   <td> <p> Enter the user name if you want to send a request using basic authorization.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Password </td> 
   <td> <p>Enter the password if you want to send a request using basic authorization.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Timeout </td> 
   <td> <p>Specify the request timeout in seconds (1-300). The default is 40 seconds.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Share cookies with other HTTP modules</td> 
   <td> <p> Enable this option to share cookies from the server with all HTTP modules in your scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Self-signed certificate</td> 
   <td> <p> Upload your certificate if you want to use TLS using your self-signed certificate.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reject connections that are using unverified (self-signed) certificates </td> 
   <td> <p>Enable this option to reject connections that are using unverified TLS certificates.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Follow redirect</td> 
   <td> <p> Enable this option to follow the URL redirects with 3xx responses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Follow all redirects </td> 
   <td> <p>Enable this option to follow the URL redirects with all response codes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Disable serialization of multiple same query string keys as arrays</p> </td> 
   <td> <p>By default, Workfront Fusion handles multiple values for the same URL query string parameter key as arrays. For example, <code>www.test.com?foo=bar&amp;foo=baz</code> will be converted to <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Activate this option to disable this feature. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Request compressed content</td> 
   <td> <p> Enable this option to request a compressed version of the website.</p> <p>Adds an <code>Accept-Encoding</code> header to request compressed content.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Use Mutual TLS</td> 
   <td> <p>Enable this option to use Mutual TLS in the HTTP request.</p> <p>For more information on Mutual TLS, see <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Use Mutual TLS in HTTP modules in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Example:** This example shows how to set up the module to submit a POST request with JSON payload:
>
>![](assets/make-a-request-example-350x522.png)

>[!NOTE]
>
>To make sure your JSON is valid, you can use one of the available online services such as [https://jsonlint.com/](https://jsonlint.com/). You can also use JSON > Create JSON module to create the JSON dynamically and take care of all the necessary escaping.
>
>Mixing JSON pieces with expressions and items directly in the Request content field is not recommended as it can result in invalid JSON.
