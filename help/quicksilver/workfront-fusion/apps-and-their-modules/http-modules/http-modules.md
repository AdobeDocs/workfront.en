---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: HTTP &gt; Other modules
description: The [!DNL Adobe Workfront Fusion] HTTP app provides various modules for communication based on Hypertext Transfer Protocol (HTTP) protocol. HTTP is the foundation of data communication for the World Wide Web. You can use the modules to download web pages and files, call webhooks and API endpoints, and so on.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
---
# HTTP > Other modules

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] requires an [!UICONTROL Adobe Workfront Fusion] license in addition to an [!UICONTROL Adobe Workfront] license.

The [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] app provides various modules for communication based on Hypertext Transfer Protocol (HTTP) protocol. HTTP is the foundation of data communication for the World Wide Web. You can use the modules to download web pages and files, call webhooks and API endpoints, and so on.

The right choice of the module depends on the authentication/ authorization mechanism the resource you want to access employs. The following are examples of modules

* Make a request:universal module primarily intended for resources not employing any type of authentication/ authorization
* Make a Basic Auth request:for resources employing [!DNL HTTP] Basic authentication (BA)
* Make a OAuth 2.0 request: for resources employing OAuth 2.0 authorization protocol
* Make a Client Certificate Auth request: for resources employing authorization protocol that requires a client-side certificate.
* Make an API Key authorization request: for resources employing API Keys for authorization.

>[!NOTE]
>
>If you are connecting to an Adobe product that does not currently have a dedicated connector, we recommend using the Adobe Authenticator module.
>
>For more information, see [Adobe Authenticator module](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

## Request modules

See the following articles for specific request module instructions:

* [[!UICONTROL HTTP] >[!UICONTROL Make a request] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Make a Basic Authorization request] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Make a Client Certificate Authorization request] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Make an API Key Authorization request]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## Other action modules

* [[!UICONTROL Get a File]](#get-a-file)
* [[!UICONTROL Resolve a target URL]](#resolve-a-target-url)

### [!UICONTROL Get a File] 

This action module downloads a file from the specified URL. After the file is downloaded, you can further process the file (map the file data) using other modules in the scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Enter or map the URL of the file you want to download. </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Resolve a target URL] 

This action module resolves a chain of HTTP redirects and returns a target URL.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Enter or map the URL you want to resolve, such as a [!DNL bit.ly] URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method] </td> 
   <td> <p>Select whether you want to use the [!UICONTROL HEAD] method or the [!UICONTROL GET] method.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Iterator modules

### [!UICONTROL Retrieve headers]

This module returns each header (name and value) from the specified HTTP module in a separate bundle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Select the module you want to retrieve headers from.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Generating JSON Web Tokens (JWT)

It is possible to generate a JWT token with the help of built-in functions:

Header:

![](assets/jwt-header-350x19.png)

Code for copy&paste:

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Payload:

![](assets/jwt-payload-350x17.png)

Code for copy&paste:

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Token:

![](assets/jwt-token-350x15.png)

Code for copy&paste:

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
