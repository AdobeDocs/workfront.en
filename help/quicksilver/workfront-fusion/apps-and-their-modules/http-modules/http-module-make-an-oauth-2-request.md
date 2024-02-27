---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
title: HTTP &gt; Make an OAuth 2.0 request module
description: In order to make an [!DNL Adobe Workfront Fusion] HTTP(S) request to servers that require an OAuth 2.0 authorization, you first need to create an OAuth connection. [!DNL Adobe Workfront Fusion] ensures that all calls made with this connection have the appropriate authorization headers and automatically refresh associated tokens when required.
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
---
# [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requires an [!DNL Adobe Workfront Fusion] license in addition to an [!DNL Adobe Workfront] license.

In order to make an [!DNL Adobe Workfront Fusion] HTTP(S) request to servers that require an OAuth 2.0 authorization, you first need to create an OAuth connection. [!DNL Adobe Workfront Fusion] ensures that all calls made with this connection have the appropriate authorization headers and automatically refresh associated tokens when required.

[!DNL Workfront Fusion] supports the following OAuth 2.0 authentication flows:

* Authorization Code Flow
* Implicit Flow

Other flows, such as Resource Owner Password Credentials Flow and Client Credentials Flow, are not automatically supported through this module.

For more information on OAuth 2.0 authentication, see [The OAuth 2.0 Authorization Framework](https://tools.ietf.org/html/rfc6749).

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

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Creating a connection for an [!DNL OAuth] request 

* [General instructions for creating a connection in the HTTP > Make an OAuth 2.0 request module](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [Instructions for creating a connection to Google in the HTTP >[!UICONTROL Make] an OAuth 2.0 request module](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [Instructions for connecting to Microsoft Graph API via the HTTP > Make an OAuth 2.0 request module](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### General instructions for creating a connection in the [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module 

1. Create an OAuth client in the [!DNL target] service with which you want [!DNL Adobe Workfront Fusion] to communicate. This option is most likely found in the [!UICONTROL Developer] section of the given service.

   1. When creating a client, enter the appropriate URL in the `[!UICONTROL Redirect URL]` or `[!UICONTROL Callback URL]` field:

      | Americas / APAC | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | EMEA | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. After you create the client, the given service displays 2 keys: `[!UICONTROL Client ID]` and `[!UICONTROL Client Secret]`. Some services call these `[!UICONTROL App Key]` and `[!UICONTROL App Secret]` . Save the key and secret in a secure location, so you can provide them when creating the connection in Workfront Fusion.

1. Find the `[!UICONTROL Authorize URI]` and `[!UICONTROL Token URI]` in the API documentation of the given service. These are URL addresses through which [!DNL Workfront Fusion] communicates with the [!DNL target] service. The addresses serve for OAuth authorization.

   >[!NOTE]
   >
   >If the service uses Implicit flow, you will need only the `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**Example:** Yahoo addresses:
   >
   >* Authorize URI:
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* Token URI:
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. (Conditional) If the target service uses scopes (access rights), check how the service separates individual scopes and make sure you set the separator in the advanced settings accordingly. If the separator is not set correctly, [!DNL Workfront Fusion] fails to create the connection, and you receive an invalid scope error.
1. After you complete the steps above, you can start to create the OAuth connection in [!DNL Workfront Fusion]. Add the OAuth 2.0 HTTP(S) request and response processing module to your scenario.
1. In the module's Connection field, click **[!UICONTROL Add]**.

1. Fill in the following fields to create a connection:

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name] </td> 
      <td> <p>Enter the name of the connection.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Flow type]</p> </td> 
      <td> <p>Select the flow for obtaining tokens.</p> 
       <ul> 
        <li><strong>[!UICONTROL Authorization Code]</strong>: Enter the <code>[!UICONTROL Authorize URI]</code> and <code>[!UICONTROL Token URI]</code> from the service's API documentation.</li> 
        <li><strong>[!UICONTROL Implicit]</strong>: Enter the <code>[!UICONTROL Authorize URI]</code> from the service's API documentation.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope] </td> 
      <td> <p>Add individual scopes. You can find this information in the given service's developer (API) documentation.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator] </td> 
      <td> <p>Select what the scopes entered above should be separated by. You can find this information in the given service's developer (API) documentation.</p> <p>Warning: If the separator is not set correctly, [!DNL Workfront Fusion] fails to create the connection and you receive an invalid scope error.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID] </td> 
      <td> <p>Enter the Client ID. You obtained the Client ID when you created an OAuth client in the service you want to connect.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p> Enter the Client Secret. You obtained the Client Secret when you created an OAuth client in the service you want to connect.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Authorize parameters]</p> </td> 
      <td> <p>Add any parameters that you want to include in the authorization call. The following standard parameters are always automatically included and do not need to be added.</p> <p>Standard parameters:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL response_type]</strong> </p> <p> <code>code </code>for [!UICONTROL Authorization Code flow] and <code>token </code>for [!UICONTROL Implicit flow]</p> </li> 
        <li> <p><strong>[!UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
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
        <li> <p><strong>[!UICONTROL client_id]</strong> </p> <p> The Client ID you received when creating the account</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Access token parameters]</p> </td> 
      <td> <p>Add any parameters that you want to include in the token call. The following standard parameters are always automatically included and do not need to be added.</p> <p>Standard parameters:</p> 
       <ul> 
        <li><strong>[!UICONTROL grant_type]</strong>: <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL redirect_uri]:</strong> </p> 
         <table style="table-layout:auto">  
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
        <li><strong>[!UICONTROL client_id]</strong>: The Client ID you received when creating the account is automatically included in the request body</li> 
        <li><strong>client_secret</strong>: The Client Secret you received when creating the account is automatically included in the request body</li> 
        <li><strong>code</strong>: The code returned by the authorization request</li> 
       </ul> <p>Note:  <p>The OAuth 2.0 standard supports at least 2 methods of client authentication during this step (<code>[!UICONTROL client_secret_basic]</code> and <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] automatically sends the specified client ID and secret through the <code>[!UICONTROL client_secret_post]</code> method. Therefore, these parameters are included as part of the token request body automatically. </p> <p>For more information on OAuth 2.0 authentication, see <a href="https://tools.ietf.org/html/rfc6749">The OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Refresh token parameters]</p> </td> 
      <td> <p>Add any parameters that you want to include in the token call. The following standard parameters are always automatically included and do not need to be added.</p> <p>Standard parameters:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL grant_type]</strong>: <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong>: The most recent refresh token obtained by the service you are connecting to</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong>: The Client ID you received when creating the account is automatically included in the request body</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong>: The Client Secret you received when creating the account is automatically included in the request body</p> </li> 
       </ul> <p>Note:  <p>The OAuth 2.0 standard supports at least 2 methods of client authentication during this step (<code>[!UICONTROL client_secret_basic]</code> and <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] automatically sends the specified client ID and secret through the <code>[!UICONTROL client_secret_post]</code> method. Therefore, these parameters are included as part of the token request body automatically. </p> <p>For more information on OAuth 2.0 authentication, see <a href="https://tools.ietf.org/html/rfc6749">The OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Custom Headers]</p> </td> 
      <td> <p>Specify any additional keys and values to include in the header of [!UICONTROL Token] and R[!UICONTROL efresh Token] steps.</p> <p>Note:  <p>The OAuth 2.0 standard supports at least 2 methods of client authentication during this step (<code>[!UICONTROL client_secret_basic]</code> and <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] does not automatically support the <code>[!UICONTROL client_secret_basic]</code> method. If the service that you are connecting to expects the Client ID and Client Secret to be combined into a single string and then base64 encoded into the Authorization header, then you should add that header and key value here.</p> <p> For more information on OAuth 2.0 authentication, see <a href="https://tools.ietf.org/html/rfc6749">The OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Token placement]</p> </td> 
      <td> <p>Select whether to send the token in the [!UICONTROL header], [!UICONTROL query string], or in both when connecting to the specified URL.</p> <p>Tokens are most commonly sent in the request header.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Header token name] </td> 
      <td> <p>Enter the name of the authorization token in the header. Default: <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Query string parameter name] </td> 
      <td> <p>Enter the name of the authorization token in the query string. Default: <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Continue]** to save connection settings.
1. Continue to [OAuth 2.0 request module setup](#oauth-20-request-module-setup).

### Instructions for creating a connection to [!DNL Google] in the [!UICONTROL HTTP] >[!UICONTROL Make an OAuth 2.0 request module]  

The following example shows how to use the [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0] request module to connect to [!DNL Google].

1. Ensure that you have created a project, configured OAuth settings, and generated your credentials as described in [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] using a custom OAuth client](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).
1. Open the [!UICONTROL HTTP] >[!UICONTROL Make an OAuth 2.0 request] module.
1. Click **[!UICONTROL Add]** next to the connection box.
1. Enter the following values:

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name] </td> 
      <td> <p>Enter the name of the connection.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Flow type]</p> </td> 
      <td> <p>[!UICONTROL Authorization Code]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize URI]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope] </td> 
      <td> <p>Add individual scopes. For more information on scopes, see <a href="https://developers.google.com/identity/protocols/oauth2/scopes">OAuth 2.O Scopes for [!DNL Google] APIs</a> in the [!DNL Google] documentation.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator] </td> 
      <td> <p>[!UICONTROL SPACE]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID] </td> 
      <td> <p>Enter your [!DNL Google] Client ID. </p> <p>To create a client ID, see <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Create OAuth Credentials</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] to [!DNL Google Services] using a custom OAuth client</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p>Enter your [!DNL Google] Client Secret. </p> <p>To create a client secret, see <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Create OAuth Credentials</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] to [!DNL Google] Services using a custom OAuth client</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Authorize parameters]</p> </td> 
      <td> <p>Add <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code>key-value pair.</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>Note: If you experience authentication issues, for example with token refreshing, try adding the <code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code>key-value pair.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Continue]** to save connection settings.
1. Continue to [OAuth 2.0 request module setup](#oauth-20-request-module-setup).

### Instructions for connecting to [!DNL Microsoft Graph API] via the [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module 

For instructions regarding [!DNL Microsoft Graph API], see [Call the [!DNL MS Graph REST API] via the [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module](../../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## OAuth 2.0 request module setup 

When you have established an [!DNL Oauth 2].0 connection as described in [Creating a connection for an [!DNL OAuth] request](#creating-a-connection-for-an-oauth-request), continue setting up the module as desired. All authorization tokens are automatically included in this request, and in any other request that uses the same connection.

When you configure the [!UICONTROL HTTP] >[!UICONTROL Make an OAuth 2.0 request] module, [!DNL Workfront Fusion] displays the fields listed below. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For information on setting up a connection, see <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">Creating a connection for an OAuth request</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Evaluate all states as errors (except for 2xx and 3xx]) </td> 
   <td> <p>Use this option to set up error handling.</p> <p>For more information, see <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Error handling in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>The Raw body type is generally suitable for most HTTP body requests even in situations where developer documentation does not specify data to send.</p> <p>Specify a form of parsing the data in the [!UICONTROL Content type] field.</p> <p>Despite the content type selected, data is entered in any format that is stipulated or required by the developer documentation.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>This body type is to POST data using <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>For <code>[!UICONTROL application/x-www-form-urlencoded]</code>, the body of the HTTP message sent to the server is essentially one query string. The keys and values are encoded in key-value pairs separated by <code>&amp;</code> and with an <code>=</code> between the key and the value. </p> <p>For binary data, <code>use [!UICONTROL multipart/form-data]</code> instead.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Example: </b></span></span> 
       <p>Example of the resulting HTTP request format:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>The [!UICONTROL Multipart/form-data] is an HTTP multipart request used to send files and data. It is commonly used to upload files to the server.</p> <p>Add fields to be sent in the request. Each field must contain a key-value pair.</p> 
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
   <td> <p>Enter the request timeout in seconds (1-300). The default is 40 seconds.</p> </td> 
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
   <td> <p> Enable this option to request a compressed version of the website.</p> <p>This adds an <code>[!UICONTROL Accept-Encoding]</code> header to request compressed content.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Use Mutual TLS]</td> 
   <td> <p>Enable this option to use Mutual TLS in the HTTP request.</p> <p>For more information on Mutual TLS, see <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Use Mutual TLS in HTTP modules in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
