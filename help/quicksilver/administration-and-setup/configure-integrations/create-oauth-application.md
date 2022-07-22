---
title: Create OAuth2 applications for Workfront integrations
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: As an Adobe Workfront administrator, you can create OAuth2 applications for your instance of Workfront, which allow other applications to access Workfront. Your users can then give permission to those other applications to access their Workfront data. In this way, you can integrate Workfront with applications of your choice, including your own in-house applications.
feature: "System Setup and Administration, Workfront Integrations and Apps"
role: Admin
---

# Create OAuth2 applications for Workfront integrations

As an Adobe Workfront administrator, you can create OAuth2 applications for your instance of Workfront, which allow other applications to access Workfront. Your users can then give permission to those other applications to access their Workfront data. In this way, you can integrate Workfront with applications of your choice, including your own in-house applications.

When you create an OAuth2 application, you generate a Client ID and Client Secret. Your users can then use the Client ID in API calls to integrate with the application you have created.

>[!NOTE]
>
>In the context of OAuth2, "creating an app" refers to the process of creating this sort of access link between an app and a server such as Workfront.

* For instructions on configuring and using the OAuth2 application with user credentials (authorization code flow), see [Configure and use your organization's custom OAuth 2 applications using authorization code flow](../../wf-api/api/oauth-app-code-token-flow.md).
* For instructions on configuring and using the OAuth2 application using server authentication (JWT flow), see [Configure and use your organization's custom OAuth 2 applications using JWT flow](../../wf-api/api/oauth-app-jwt-flow.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> You must be a Workfront administrator. </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## OAuth2 overview

Imagine that an application needs to pull some specific information from Workfront. An application that requests information is called a client. For this example, the client name is ClientApp. ClientApp needs access to a particular user's information, and therefore needs to access Workfront as that user. If your user gives ClientApp their username and password, ClientApp could access all of the data that the user can access. This is a security risk, because ClientApp only needs a small, specific set of information.

When you create an OAuth2 app for ClientApp, you are essentially telling Workfront that ClientApp is allowed to access Workfront, but only if the user whose account ClientApp is accessing gives permission for the access.

## Create an OAuth2 application

When creating an OAuth2 application, choose the type of application that best meets the needs of your integration.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Application type</th> 
   <th>Best for</th> 
   <th>Authentication method</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Machine to Machine Application</p> </td> 
   <td> <p>Best for CLIs, daemons, or scripts running on your server</p> <p>Examples:</p> 
    <ul> 
     <li> <p>Shell </p> </li> 
     <li> <p>Python</p> </li> 
    </ul> </td> 
   <td> <p>Authentication through JSON Web Token with public/private key-pair encoding.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Single Page Web Application</p> </td> 
   <td> <p>Best for mobile or single-page web applications</p> <p>Examples:</p> 
    <ul> 
     <li> <p>Javascript</p> </li> 
     <li> <p>Angular</p> </li> 
     <li> <p> React</p> </li> 
     <li> <p>Vue</p> </li> 
    </ul> </td> 
   <td> <p>Authentication through OAuth 2.0 Authorization Code flow with Proof Key for Code Exchange (PKCE).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Web Application</p> </td> 
   <td> <p>Best for server-side applications that handle credentials and tokens on the server</p> <p>Examples:</p> 
    <ul> 
     <li> <p>Go</p> </li> 
     <li> <p>Java</p> </li> 
     <li> <p>ASP.Net</p> </li> 
     <li> <p>Node.js</p> </li> 
     <li> <p>PHP</p> </li> 
    </ul> </td> 
   <td> <p>Authentication through OAuth 2.0 Authorization Code flow.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>You can have up to ten OAuth2 Applications total at a time.

* [Create an OAuth2 application using server authentication (JWT flow)](#create-an-oauth2-application-using-server-authentication-jwt-flow) 
* [Create an OAuth2 application using user credentials (Authorization code flow)](#create-an-oauth2-application-using-user-credentials-authorization-code-flow) 
* [Create an OAuth2 single-page web application using PKCE](#create-an-oauth2-single-page-web-application-using-pkce)

### Create an OAuth2 application using server authentication (JWT flow) {#create-an-oauth2-application-using-server-authentication-jwt-flow}

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left navigation panel, click **System**, then select **OAuth Applications**.
1. Click **Create app integration**.
1. In the window that appears, select **Server Authentication**.
1. Enter a name for the new application, such as "Workfront for ClientApp."
1. Click **Create**.
1. Fill in the fields for the new app.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Client ID</td> 
      <td> <p>This field is automatically generated.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Client secret</td> 
      <td> <p>This field is automatically generated</p> <p><b>IMPORTANT</b>:  <p>Copy the contents of this field to another secure file before you close this page. You will not be able to see this secret key again.</p> <p>If you lose this key, delete it and create a new Client Secret.</p> 
        <ol> 
         <li value="1"> <p>Click the <b>Delete</b> icon <img src="assets/delete.png"> to delete the current Client Secret.</p> </li> 
         <li value="2"> <p>Click <b>Add client secret</b> to generate a new Client Secret.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Public Keys</td> 
      <td> <p>Server to server apps use public and private keys for authentication. Do one of the following:</p> 
       <ul> 
        <li> <p>Click <b>Add a public key</b> and enter the public key from the other application.</p> </li> 
        <li> <p>Click <b>Generate a public/private keypair</b>, then share the public key with the other application.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>This is the same name that you gave the app. This field cannot be empty.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Enter a description for the integration.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.

For instructions on configuring and using the OAuth2 application with user credentials (authorization code flow), see [Configure and use your organization's custom OAuth 2 applications using JWT flow](../../wf-api/api/oauth-app-jwt-flow.md).

### Create an OAuth2 application using user credentials (Authorization code flow) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).
1. In the left navigation panel, click **System**, then select **OAuth Applications**.
1. Click **Create app integration**.
1. In the window that apears, select **User Authentication**.
1. Enter a name for the new OAuth2 application, such as "Workfront for ClientApp."
1. Click **Create**.
1. Fill in the fields for the new app.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Client ID</td> 
      <td> <p>This field is automatically generated.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Client secret</td> 
      <td> <p>This field is automatically generated</p> <p><b>IMPORTANT</b>:  <p>Copy the contents of this field to another secure file before you close this page. You will not be able to see this secret key again.</p> <p>If you lose this key, delete it and create a new Client Secret.</p> 
        <ol> 
         <li value="1"> <p>Click the <b>Delete</b> icon <img src="assets/delete.png"> to delete the current Client Secret.</p> </li> 
         <li value="2"> <p>Click <b>Add client secret</b> to generate a new Client Secret.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Redirect URLs</td> 
      <td>Users will be redirected to this path after they have authenticated with Workfront. <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         The path will be appended with the authorization code for access, and must have a protocol.
        </MadCap:conditionalText>
       --></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Refresh token rotation</td> 
      <td>Enable this option to issue a new refresh token whenever the refresh token is used. Your application must store the new refresh token after every refresh.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Absolute refresh token expiration</td> 
      <td> <p>Select the amount of time you wish a refresh token to exist before it expires. When it expires, your users must log in to the integration again. Select "No expiration" if you do not want the refresh token to expire.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Inactivity refresh token expiration</td> 
      <td> <p>Select the amount of time after which, if the user has not been active in your system, their refresh token expires. </p> <p>For example, if the inactivity refresh token expiration is 6 months, and the user does not log in for six months, the refresh token expires even though the absolute refresh token expiration may be set for longer.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Logo</td> 
      <td>You can add a logo to make this app more identifiable. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>This is the same name that you gave the app. This field cannot be empty.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Enter a description for the integration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">App Description URL</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.

For instructions on configuring and using the OAuth2 application with user credentials (authorization code flow), see [Configure and use your organization's custom OAuth 2 applications using authorization code flow](../../wf-api/api/oauth-app-code-token-flow.md).

### Create an OAuth2 single-page web application using PKCE {#create-an-oauth2-single-page-web-application-using-pkce}

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).
1. In the left navigation panel, click **System**, then select **OAuth Applications**.
1. Click **Create app integration**.
1. In the window that apears, select **Single-page web application**.
1. Enter a name for the new OAuth2 application, such as "Workfront for ClientApp."
1. Click **Create**.
1. Fill in the fields for the new app.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Client ID</td> 
      <td> <p>This field is automatically generated.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Redirect URLs</td> 
      <td>Users will be redirected to this path after they have authenticated with Workfront. <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         The path will be appended with the authorization code for access, and must have a protocol.
        </MadCap:conditionalText>
       --></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Refresh token rotation</td> 
      <td>Enable this option to issue a new refresh token whenever the refresh token is used. Your application must store the new refresh token after every refresh.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Absolute refresh token expiration</td> 
      <td> <p>Select the amount of time you wish a refresh token to exist before it expires. When it expires, your users must log in to the integration again. Select "No expiration" if you do not want the refresh token to expire.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Inactivity refresh token expiration</td> 
      <td> <p>Select the amount of time after which, if the user has not been active in your system, their refresh token expires. </p> <p>For example, if the inactivity refresh token expiration is 6 months, and the user does not log in for six months, the refresh token expires even though the absolute refresh token expiration may be set for longer.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Logo</td> 
      <td>You can add a logo to make this app more identifiable. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>This is the same name that you gave the app. This field cannot be empty.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Enter a description for the integration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">App Description URL</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.

## Configure and use the created OAuth2 application

Further configuration and use of the created OAuth2 application requires some technical knowledge, including API calls.

* For instructions on configuring and using the OAuth2 application with user credentials (authorization code flow), see [Configure and use your organization's custom OAuth 2 applications using authorization code flow](../../wf-api/api/oauth-app-code-token-flow.md).
* For instructions on configuring and using the OAuth2 application using server authentication (JWT flow), see [Configure and use your organization's custom OAuth 2 applications using JWT flow](../../wf-api/api/oauth-app-jwt-flow.md).

## OAuth2 processes for authorization code flow

>[!NOTE]
>
>Your users access the OAuth2 application through the API. This section describes the functionality in general terms, and is provided for information only.
>
>For specific instructions on using the OAuth2 application, including specific API calls, see [Configure and use your organization's custom OAuth 2 applications using authorization code flow](../../wf-api/api/oauth-app-code-token-flow.md).

### Authorizing with an authorization code and access token {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp needs some information from Workfront, so it sends a request to the Workfront API `/authorize` endpoint. The request includes the response_type `code`, which indicates that the request should return an authorization code.
1. This triggers Workfront to send an authentication prompt to the user. The user can enter their credentials into the prompt, which gives Workfront permission to communicate with ClientApp. If the user is already logged into Workfront, this step may be skipped.
1. The Workfront API sends an authorization code to ClientApp.
1. ClientApp sends the following information in a request to the Workfront API `/token`   endpoint:

   * The authorization code sent to ClientApp in step 3. This identifies the specific instance of user permission.
   * The Client Secret that was generated when you set up the ClientApp OAuth2 app in Workfront. This allows Workfront to know that the request is coming from ClientApp.

1. If the authorization code and the client secret are correct, Workfront sends an access token to ClientApp. This access token is sent directly from Workfront to ClientApp, and cannot be viewed, copied, or used by any other user or client application. 
1. ClientApp sends the access token to Workfront along with the specific request for information.
1. Because the access token is correct, Workfront sends the information to ClientApp.

#### Refreshing access tokens

For security, access tokens expire after a short amount of time. To get new access tokens without having to enter credentials every time, OAuth2 uses refresh tokens. Refresh tokens are stored by the client.

The process for acquiring a refresh token is the same as the procedure discussed in the section [Authorizing with an authorization code and access token](#authorizing-with-an-authorization-code-and-access-token). The request for the authorization code includes the scope `offline_access`, which indicates that the request should return a request token along with the authorization code.

 
