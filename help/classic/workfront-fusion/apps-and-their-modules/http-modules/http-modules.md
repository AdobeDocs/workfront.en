---
filename: http-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
title: HTTP > Other modules
description: HTTP > Other moduleshow to", it is an overview; and according to the style guide the overview articles are titled "HTTP modules overview". Would this fit the bill for that title?)"
---

# HTTP > Other modules

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: from&nbsp;Alina: Just a suggestion: I think when an article is not a "how to", it is an overview; and according to the style guide the overview articles are titled "HTTP modules overview". Would this fit the bill for that title?)</p>
-->

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
The Adobe Workfront Fusion HTTP app provides various modules for communication based on Hypertext Transfer Protocol (HTTP) protocol. HTTP is the foundation of data communication for the World Wide Web. You can use the modules to download web pages and files, call webhooks and API endpoints, and so on.

The right choice of the module depends on the authentication/ authorization mechanism the resource you want to access employs.&nbsp;The following are examples of modules

* Make a request:universal module primarily intended for resources not employing any type of authentication/ authorization
* Make a Basic Auth request:for resources employing HTTP Basic authentication (BA)
* Make a OAuth 2.0 request: for resources employing OAuth 2.0 authorization protocol
* Make a Client Certificate Auth request: for resources employing authorization protocol that requires a client-side certificate.
* Make an API Key authorization request: for resources employing API Keys for authorization.

## Request modules

See the following articles for specific request module instructions:

* [HTTP > Make a request module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md) 
* [HTTP > Make a Basic Authorization request module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md) 
* [HTTP > Make an OAuth 2.0 request module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md) 
* [HTTP > Make a Client Certificate Authorization request module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md) 
* [HTTP > Make an API Key Authorization request](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## Other action modules

* [Get a File](#get-a-file) 
* [Resolve a target URL](#resolve-a-target-url)

### Get a File {#get-a-file}

This action module downloads a file from the specified URL. After the file is downloaded, you can further process the file (map the file data) using other modules in the scenario.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL </td> 
   <td> <p>Enter or map the URL of the file you want to download. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Resolve a target URL {#resolve-a-target-url}

This action module resolves a chain of HTTP redirects and returns a target URL.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL </td> 
   <td> <p>Enter or map the URL you want to resolve, such as a bit.ly URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method </td> 
   <td> <p>Select whether you want to use the HEAD method or the GET method.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Iterator modules

### Retrieve headers

This module returns each header (name and value) from the specified HTTP module in a separate bundle.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Source Module</td> 
   <td> <p> Select the module you want to retrieve headers from.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Generating JSON Web Tokens (JWT)

It is possible to generate a JWT token with the help of built-in functions:

Header:

![](assets/jwt-header-350x19.png)

Code for copy&paste:
<pre>{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}</pre>Payload:

![](assets/jwt-payload-350x17.png)

Code for copy&paste:
<pre>{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}</pre>Token:

![](assets/jwt-token-350x15.png)

Code for copy&paste:
<pre>{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}</pre>