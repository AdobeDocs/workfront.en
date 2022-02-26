---
filename: http-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: HTTP > Other modules
description: Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
---

# HTTP > Other modules

*Adobe Workfront Fusion* requires an *Adobe Workfront Fusion* license in addition to an *Adobe Workfront* license.
The HTTP app provides various modules for communication based on Hypertext Transfer Protocol (HTTP) protocol. HTTP is the foundation of data communication for the World Wide Web. You can use the modules to download web pages and files, call webhooks and API endpoints, and so on.

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

* [Get a File](#get) 
* [Resolve a target URL](#resolve)

### Get a File

This action module downloads a file from the specified URL. After the file is downloaded, you can further process the file (map the file data) using other modules in the scenario.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>URL </td> 
   <td> <p>Enter or map the URL of the file you want to download. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Resolve a target URL

This action module resolves a chain of HTTP redirects and returns a target URL.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>URL </td> 
   <td> <p>Enter or map the URL you want to resolve, such as a bit.ly URL.</p> </td> 
  </tr> 
  <tr> 
   <td>Method </td> 
   <td> <p>Select whether you want to use the HEAD method or the GET method.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Iterator modules

### Retrieve headers

This module returns each header (name and value) from the specified HTTP module in a separate bundle.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Source Module</td> 
   <td> <p> Select the module you want to retrieve headers from.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="Advanced"></a>Advanced information</h2>
<ul>
<li><a href="#standard" class="MCXref xref">Standard authorization parameters</a> </li>
<li><a href="#requesti" class="MCXref xref">Requesting Access tokens - standard parameters</a> </li>
<li><a href="#requesti2" class="MCXref xref">Requesting Refresh tokens - standard parameters</a> </li>
<li><a href="#authoriz" class="MCXref xref">Authorized request made to a service</a> </li>
</ul>
<h3><a name="Standard"></a>Standard authorization parameters</h3>
<ul>
<li>response_type: <code>code</code> for Authorization Code flow and <code>token</code> for Implicit flow</li>
<li>redirect_uri: <code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></li>
<li>client_id: The Client ID you entered when creating the account</li>
</ul>
<h3><a name="Requesti"></a>Requesting Access tokens - standard parameters</h3>
<ul>
<li>grant_type: <code>authorization_code</code></li>
<li>redirect_uri: <code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></li>
<li>client_id: The Client ID you entered when creating the account</li>
<li>client_secret: The Client Secret you entered when creating the account</li>
<li>code: The code returned by authorization request</li>
</ul>
<h3><a name="Requesti2"></a>Requesting Refresh tokens - standard parameters</h3>
<ul>
<li>grant_type: <code>refresh_token</code></li>
<li>refresh_token: The Refresh token obtained together with the Access token</li>
<li>client_id: The Client ID you entered when creating the account</li>
<li>client_secret: The Client Secret you entered when creating the account</li>
</ul>
<h3><a name="Authoriz"></a>Authorized request made to a service</h3>
<p>After the connection is established, the module uses by default the bearer token which is sent in the request header field. The bearer token has the following format: <code>Authorization: Bearer <access token></code></p>
<p>When creating a connection, it is possible to adjust where the token shall be located, whether in the header in the <code>Authorization</code> parameter or in the URL in the query string.</p>
<h2><a name="HTTP"></a>HTTP message body type and when to use it.</h2>
<p>HTTP Message Body is the data bytes transmitted in an HTTP transaction message immediately following the headers if there are any to be used.</p>
<ul>
<li><a href="#raw" class="MCXref xref">Raw</a> </li>
<li><a href="#multipar" class="MCXref xref">Multipart/Form-Data</a> </li>
<li><a href="#applicat" class="MCXref xref">Application/form-urlencoded</a> </li>
</ul>
<h3><a name="Raw"></a>Raw</h3>
<p class="PinkDraftNote">Screenshot</p>
<p>The Raw body type is generally suitable for most HTTP body requests even is situations where developer documentation does not specify data to send, with the following field option of specifying content type as a form of parsing data.</p>
<p class="PinkDraftNote">Screenshot</p>
<p>Despite the content type selected, data is entered in any format that is stipulated or required by the developer documentation.</p>
<h3><a name="Multipar"></a>Multipart/Form-Data</h3>
<p>Multipart/form-data is an HTTP multipart request that HTTP clients construct to send files and data over to an HTTP module. It is commonly used to upload files to your desired server.</p>
<p class="PinkDraftNote">Screenshot</p>
<p>You will notice that when you select application form the input method changes and this entails that from the developer documentation you will have the relevant fields required, same also applies to Multipart/form-data whereby in order to receive files encoded with <code>multipart/form-data</code>, it is necessary to configure a data structure with a <code>collection </code>type field that contains the nested fields <code>name</code>, <code>mime </code>and <code>data</code>. So as you can see the way the information is received is different.</p>
<h3><a name="Applicat"></a>Application/form-urlencoded</h3>
<p>This body type is to POST data using <code>application/x-www-form-urlencoded</code></p>
<p class="PinkDraftNote">Screenshot</p>
<p>For <code>application/x-www-form-urlencoded</code>, the body of the HTTP message sent to the server is essentially one giant query string -- name/value pairs are separated by the ampersand (<code>&</code>), and names are separated by the fields name and value for easy use to you and replacing the equals symbol (=) used in coding. However, after you have configured the above it will look like the example shown below:</p>
<pre>MyVariableOne=ValueOne&MyVariableTwo=ValueTwo</pre>
<h2><a name="Tutorial"></a>Tutorials</h2>
<p>How to connect <em>Workfront Fusion</em> with any web service using OAuth2 authorization<draft-comment>
<MadCap:conditionalText style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
- drafted out until I fix that article
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
- drafted out until I fix that article
</MadCap:conditionalText></p>
</div>
-->

## Advanced information

* [Standard authorization parameters](#standard) 
* [Requesting Access tokens - standard parameters](#requesti) 
* [Requesting Refresh tokens - standard parameters](#requesti2) 
* [Authorized request made to a service](#authoriz)

### Standard authorization parameters

* response_type: 

  ```
  code
  ```

  for Authorization Code flow and 

  ```
  token
  ```

  for Implicit flow

* redirect_uri: 

  ```
  https://app.workfrontfusion.com/oauth/cb/oauth2
  ```

* client_id: The Client ID you entered when creating the account

### Requesting Access tokens - standard parameters

* grant_type: 

  ```
  authorization_code
  ```

* redirect_uri: 

  ```
  https://app.workfrontfusion.com/oauth/cb/oauth2
  ```

* client_id: The Client ID you entered when creating the account
* client_secret: The Client Secret you entered when creating the account
* code: The code returned by authorization request

### Requesting Refresh tokens - standard parameters

* grant_type: 

  ```
  refresh_token
  ```

* refresh_token: The Refresh token obtained together with the Access token
* client_id: The Client ID you entered when creating the account
* client_secret: The Client Secret you entered when creating the account

### Authorized request made to a service

After the connection is established, the module uses by default the bearer token which is sent in the request header field. The bearer token has the following format: 

```
Authorization: Bearer <access token>
```

When creating a connection, it is possible to adjust where the token shall be located, whether in the header in the 

```
Authorization
```

parameter or in the URL in the query string.

## HTTP message body type and when to use it.

HTTP Message Body is the data bytes transmitted in an HTTP transaction message immediately following the headers if there are any to be used.

* [Raw](#raw) 
* [Multipart/Form-Data](#multipar) 
* [Application/form-urlencoded](#applicat)

### Raw

Screenshot

The Raw body type is generally suitable for most HTTP body requests even is situations where developer documentation does not specify data to send, with the following field option of specifying content type as a form of parsing data.

Screenshot

Despite the content type selected, data is entered in any format that is stipulated or required by the developer documentation.

### Multipart/Form-Data

Multipart/form-data is an HTTP multipart request that HTTP clients construct to send files and data over to an HTTP module. It is commonly used to upload files to your desired server.

Screenshot

You will notice that when you select application form the input method changes and this entails that from the developer documentation you will have the relevant fields required, same also applies to Multipart/form-data whereby in order to receive files encoded with 

```
multipart/form-data
```

, it is necessary to configure a data structure with a 

```
collection
```

type field that contains the nested fields 

```
name
```

, 

```
mime
```

and 

```
data
```

. So as you can see the way the information is received is different.

### Application/form-urlencoded

This body type is to POST data using 

```
application/x-www-form-urlencoded
```

Screenshot

For 

```
application/x-www-form-urlencoded
```

, the body of the HTTP message sent to the server is essentially one giant query string -- name/value pairs are separated by the ampersand (

```
&
```

), and names are separated by the fields name and value for easy use to you and replacing the equals symbol (=) used in coding. However, after you have configured the above it will look like the example shown below:
<pre>MyVariableOne=ValueOne&MyVariableTwo=ValueTwo</pre>

## Tutorials

How to connect *Workfront Fusion* with any web service using OAuth2 authorization`<MadCap:conditionalText style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">  - drafted out until I fix that article </MadCap:conditionalText>`

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