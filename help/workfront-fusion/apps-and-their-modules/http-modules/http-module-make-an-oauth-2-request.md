---
filename: http-module-make-an-oauth-2-request
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
title: HTTP > Make an OAuth 2.0 request module
description: Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
---

# HTTP > Make an OAuth 2.0 request module

Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
In order to make an HTTP(S) request to servers that require an OAuth 2.0 authorization, you first need to create an OAuth connection. Adobe Workfront Fusion ensures that all calls made with this connection have the appropriate authorization headers and automatically refresh associated tokens when required.

Workfront Fusion supports the following OAuth 2.0 authentication flows:

* Authorization Code Flow
* Implicit Flow

Other flows, such as Resource Owner Password Credentials Flow and Client Credentials Flow, are not automatically supported through this module.

For more information on OAuth 2.0 authentication, see [The OAuth 2.0 Authorization Framework](https://tools.ietf.org/html/rfc6749).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Creating a connection for an OAuth request

* [General instructions for creating a connection in the HTTP > Make an OAuth 2.0 request module](#general) 
* [Instructions for creating a connection to Google in the HTTP > Make an OAuth 2.0 request module](#instruct) 
* [Instructions for connecting to Microsoft Graph API via the HTTP > Make an OAuth 2.0 request module](#instruct2)

### General instructions for creating a connection in the HTTP > Make an OAuth 2.0 request module

<ol> 
 <li value="1"> <p>Create an OAuth client in the target service with which you want Adobe Workfront Fusion to communicate. This option is most likely found in the Developer section of the given service. </p> 
  <ol style="list-style-type: lower-alpha;"> 
   <li value="1"> <p>When creating a client, enter the appropriate URL in the <code>Redirect URL</code> or <code>Callback URL</code> field:</p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">Americas / APAC</td> 
       <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
      </tr> 
      <tr> 
       <td role="rowheader">EMEA </td> 
       <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
      </tr> 
     </tbody> 
    </table> </li> 
   <li value="2"> <p>After you create the client, the given service displays 2 keys: <code>Client ID</code> and <code>Client Secret</code>. Some services call these <code>App Key</code> and <code>App Secret</code>. Save the key and secret in a secure location, so you can provide them when creating the connection in Workfront Fusion.</p> </li> 
  </ol> </li> 
 <li value="2"> <p>Find the <code>Authorize URI</code> and <code>Token URI</code> in the API documentation of the given service. These are URL addresses through which Workfront Fusion communicates with the target service. The addresses serve for OAuth authorization.</p> <note type="note">
    If the service uses Implicit flow, you will need only the 
   <code>Authorize URI</code>. 
  </note> 
  <div class="example" data-mc-autonum="<b>Example: </b>">
   <span class="autonumber"><span><b>Example: </b></span></span> 
   <p>Yahoo addresses:</p> 
   <ul> 
    <li>Authorize URI: <code>https://api.login.yahoo.com/oauth2/request_auth</code></li> 
    <li>Token URI: <code>https://api.login.yahoo.com/oauth2/get_token</code></li> 
   </ul> 
  </div> </li> 
 <li value="3">(Conditional) If the target service uses scopes (access rights), check how the service separates individual scopes and make sure you set the separator in the advanced settings accordingly. If the separator is not set correctly, Workfront Fusion fails to create the connection, and you receive an invalid scope error.</li> 
 <li value="4">After you complete the steps above, you can start to create the OAuth connection in Workfront Fusion. Add the OAuth 2.0 HTTP(S) request and response processing module to your scenario.</li> 
 <li value="5">In the module's Connection field, click <span class="bold">Add</span>.</li> 
 <li value="6"> <p>Fill in the following fields to create a connection: </p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Connection name </td> 
     <td> <p>Enter the name of the connection.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>Flow type</p> </td> 
     <td> <p>Select the flow for obtaining tokens.</p> 
      <ul> 
       <li><span class="bold">Authorization Code</span>: Enter the <code>Authorize URI</code> and <code>Token URI</code> from the service's API documentation.</li> 
       <li><span class="bold">Implicit</span>: Enter the <code>Authorize URI</code> from the service's API documentation.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Scope </td> 
     <td> <p>Add individual scopes. You can find this information in the given service's developer (API) documentation.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Scope separator </td> 
     <td> <p>Select what the scopes entered above should be separated by. You can find this information in the given service's developer (API) documentation.</p> <p class="warning" data-mc-autonum="<b>Warning: </b>"><span class="autonumber"><span><b>Warning: </b></span></span>If the separator is not set correctly, Workfront Fusion fails to create the connection and you receive an invalid scope error.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Client ID </td> 
     <td> <p>Enter the Client ID. You obtained the Client ID when you created an OAuth client in the service you want to connect.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Client Secret</td> 
     <td> <p> Enter the Client Secret. You obtained the Client Secret when you created an OAuth client in the service you want to connect.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>Authorize parameters</p> </td> 
     <td> <p>Add any parameters that you want to include in the authorization call. The following standard parameters are always automatically included and do not need to be added.</p> <p>Standard parameters:</p> 
      <ul> 
       <li> <p><span class="bold">response_type</span> </p> <p> <code>code </code>for Authorization Code flow and <code>token </code>for Implicit flow</p> </li> 
       <li> <p><span class="bold">redirect_uri</span> </p> 
        <table cellspacing="0"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader">Americas / APAC</td> 
           <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
          </tr> 
          <tr> 
           <td role="rowheader">EMEA </td> 
           <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
          </tr> 
         </tbody> 
        </table> </li> 
       <li> <p><span class="bold">client_id</span> </p> <p> The Client ID you received when creating the account</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>Access token parameters</p> </td> 
     <td> <p>Add any parameters that you want to include in the token call. The following standard parameters are always automatically included and do not need to be added.</p> <p>Standard parameters:</p> 
      <ul> 
       <li><span class="bold">grant_type</span>: <code>authorization_code</code></li> 
       <li> <p><span class="bold">redirect_uri:</span> </p> 
        <table cellspacing="0"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader">Americas / APAC</td> 
           <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
          </tr> 
          <tr> 
           <td role="rowheader">EMEA </td> 
           <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
          </tr> 
         </tbody> 
        </table> </li> 
       <li><span class="bold">client_id</span>: The Client ID you received when creating the account is automatically included in the request body</li> 
       <li><span class="bold">client_secret</span>: The Client Secret you received when creating the account is automatically included in the request body</li> 
       <li><span class="bold">code</span>: The code returned by the authorization request</li> 
      </ul> <note type="note"> 
       <p>The OAuth 2.0 standard supports at least 2 methods of client authentication during this step (<code>client_secret_basic</code> and <code>client_secret_post</code>). Workfront Fusion automatically sends the specified client ID and secret through the <code>client_secret_post</code> method. Therefore, these parameters are included as part of the token request body automatically. </p> 
       <p>For more information on OAuth 2.0 authentication, see <a href="https://tools.ietf.org/html/rfc6749">The OAuth 2.0 Authorization Framework</a>.</p> 
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>Refresh token parameters</p> </td> 
     <td> <p>Add any parameters that you want to include in the token call. The following standard parameters are always automatically included and do not need to be added.</p> <p>Standard parameters:</p> 
      <ul> 
       <li> <p><span class="bold">grant_type</span>: <code>refresh_token</code></p> </li> 
       <li> <p><span class="bold">refresh_token</span>: The most recent refresh token obtained by the service you are connecting to</p> </li> 
       <li> <p><span class="bold">client_id</span>: The Client ID you received when creating the account is automatically included in the request body</p> </li> 
       <li> <p><span class="bold">client_secret</span>: The Client Secret you received when creating the account is automatically included in the request body</p> </li> 
      </ul> <note type="note"> 
       <p>The OAuth 2.0 standard supports at least 2 methods of client authentication during this step (<code>client_secret_basic</code> and <code>client_secret_post</code>). Workfront Fusion automatically sends the specified client ID and secret through the <code>client_secret_post</code> method. Therefore, these parameters are included as part of the token request body automatically. </p> 
       <p>For more information on OAuth 2.0 authentication, see <a href="https://tools.ietf.org/html/rfc6749">The OAuth 2.0 Authorization Framework</a>.</p> 
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>Custom Headers</p> </td> 
     <td> <p>Specify any additional keys and values to include in the header of Token and Refresh Token steps.</p> <note type="note"> 
       <p>The OAuth 2.0 standard supports at least 2 methods of client authentication during this step (<code>client_secret_basic</code> and <code>client_secret_post</code>). Workfront Fusion does not automatically support the <code>client_secret_basic</code> method. If the service that you are connecting to expects the Client ID and Client Secret to be combined into a single string and then base64 encoded into the Authorization header, then you should add that header and key value here.</p> 
       <p> For more information on OAuth 2.0 authentication, see <a href="https://tools.ietf.org/html/rfc6749">The OAuth 2.0 Authorization Framework</a>.</p> 
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>Token placement</p> </td> 
     <td> <p>Select whether to send the token in the header, query string, or in both when connecting to the specified URL.</p> <p>Tokens are most commonly sent in the request header.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Header token name </td> 
     <td> <p>Enter the name of the authorization token in the header. Default: <code>Bearer</code>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Query string parameter name </td> 
     <td> <p>Enter the name of the authorization token in the query string. Default: <code>access_token</code>.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="7">Click <span class="bold">Continue </span>to save connection settings. </li> 
 <li value="8">Continue to <a href="#oauth" class="MCXref xref">OAuth 2.0 request module setup</a>.</li> 
</ol>

### Instructions for creating a connection to Google in the HTTP > Make an OAuth 2.0 request module

The following example shows how to use the HTTP > Make an OAuth 2.0 request module to connect to Google.

<ol> 
 <li value="1"> <p>Ensure that you have created a project, configured OAuth settings, and generated your credentials as described in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">Connect Adobe Workfront Fusion to Google Services using a custom OAuth client</a>.</p> </li> 
 <li value="2"> <p>Open the HTTP > Make an OAuth 2.0 request module.</p> </li> 
 <li value="3"> <p>Click <span class="bold">Add </span>next to the connection box.</p> </li> 
 <li value="4"> <p>Enter the following values:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Connection name </td> 
     <td> <p>Enter the name of the connection.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>Flow type</p> </td> 
     <td> <p>Authorization Code</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Authorize URI</td> 
     <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Token URI</td> 
     <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Scope </td> 
     <td> <p>Add individual scopes. For more information on scopes, see <a href="https://developers.google.com/identity/protocols/oauth2/scopes">OAuth 2.O Scopes for Google APIs</a> in the Google documentation.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Scope separator </td> 
     <td> <p>SPACE</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Client ID </td> 
     <td> <p>Enter your Google Client ID. </p> <p>To create a client ID, see <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Create OAuth Credentials</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">Connect Adobe Workfront Fusion to Google Services using a custom OAuth client</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Client Secret</td> 
     <td> <p>Enter your Google Client Secret. </p> <p>To create a client secret, see <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Create OAuth Credentials</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">Connect Adobe Workfront Fusion to Google Services using a custom OAuth client</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"> <p>Authorize parameters</p> </td> 
     <td> <p>Add <code>access_type</code> - <code>offline </code>key-value pair.</p> <p> <img src="assets/google-authentication-http.png"> </p> <note type="note">
       If you experience authentication issues, for example with token refreshing, try adding the 
       <code>prompt </code>- 
       <code>consent </code>key-value pair.
      </note> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5">Click <span class="bold">Continue </span>to save connection settings. </li> 
 <li value="6">Continue to <a href="#oauth" class="MCXref xref">OAuth 2.0 request module setup</a>.</li> 
</ol>

### Instructions for connecting to Microsoft Graph API via the HTTP > Make an OAuth 2.0 request module

For instructions regarding Microsoft Graph API, see [Call the MS Graph REST API via the HTTP > Make an OAuth 2.0 request module](../../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## OAuth 2.0 request module setup

When you have established an Oauth 2.0 connection as described in [Creating a connection for an OAuth request](#creating), continue setting up the module as desired. All authorization tokens are automatically included in this request, and in any other request that uses the same connection.

When you configure the HTTP > Make an OAuth 2.0 request module, Workfront Fusion displays the fields listed below. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--

-->

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> Connection For information on setting up a connection, see Creating a connection for an OAuth request in this article. 
  <tr> 
   <td role="rowheader">Evaluate all states as errors (except for 2xx and 3xx ) </td> 
   <td> <p>Use this option to set up error handling.</p> <p>For more information, see <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Error handling</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL </td> 
   <td> <p>Enter the URL you want to send a request to, such as an API endpoint, website, etc.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Method</p> </td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers </td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object. For example, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p> Enter the desired query key-value pairs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Body type</p> </td> 
   <td> <p>The HTTP Body is the data bytes transmitted in an HTTP transaction message immediately following the headers if there are any to be used.</p> 
    <ul> 
     <li> <p><span class="bold">Raw</span> </p> <p>The Raw body type is generally suitable for most HTTP body requests even in situations where developer documentation does not specify data to send.</p> <p>Specify a form of parsing the data in the Content type field.</p> <p>Despite the content type selected, data is entered in any format that is stipulated or required by the developer documentation.</p> </li> 
     <li> <p><span class="bold">Application/x-www-form-urlencoded</span> </p> <p>This body type is to POST data using <code>application/x-www-form-urlencoded</code>.</p> <p>For <code>application/x-www-form-urlencoded</code>, the body of the HTTP message sent to the server is essentially one query string. The keys and values are encoded in key-value pairs separated by <code>&amp;</code> and with an <code>=</code> between the key and the value. </p> <p>For binary data, <code>use multipart/form-data</code> instead.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Example: </b></span></span> 
       <p>Example of the resulting HTTP request format:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><span class="bold">Multipart/form-data</span> </p> <p>The Multipart/form-data is an HTTP multipart request used to send files and data. It is commonly used to upload files to the server.</p> <p>Add fields to be sent in the request. Each field must contain a key-value pair.</p> 
      <ul> 
       <li> <p><span class="bold">Text</span> </p> <p>Enter the key and value to be sent within the request body.</p> </li> 
       <li> <p><span class="bold">File </span> </p> <p>Enter the key and specify the source file you want to send in the request body.</p> <p>Map the file you want to upload from the previous module (such as HTTP &gt; Get a File or Google Drive &gt; Download a File), or enter the file name and file data manually.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Parse response</p> </td> 
   <td> <p>Enable this option to automatically parse responses and convert JSON and XML responses so you don't need to use JSON &gt; Parse JSON or XML &gt; Parse XML modules.</p> <p>Before you can use parsed JSON or XML content, run the module once manually so that the module can recognize the response content and allow you to map it in subsequent modules.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Timeout </td> 
   <td> <p>Enter the request timeout in seconds (1-300). The default is 40 seconds.</p> </td> 
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
   <td> <p> Enable this option to request a compressed version of the website.</p> <p>This adds an <code>Accept-Encoding</code> header to request compressed content.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Use Mutual TLS</td> 
   <td> <p>Enable this option to use Mutual TLS in the HTTP request.</p> <p>For more information on Mutual TLS, see <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Use Mutual TLS in HTTP modules</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

