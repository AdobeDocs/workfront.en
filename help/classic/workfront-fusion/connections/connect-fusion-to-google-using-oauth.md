---
filename: connect-fusion-to-google-using-oauth
product: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connect Adobe Workfront Fusion to Google Services using a custom OAuth client
description: You must have the following access to use the functionality in this article:
---

# Connect Adobe Workfront Fusion to Google Services using a custom OAuth client

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
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
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
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

## Prerequisites

You need an existing Google account to make this connection.

## Create a project on Google Cloud Platform {#create-a-project-on-google-cloud-platform}

>[!NOTE]
>
>The following procedure is intended for:
>
>* Personal use (@gmail.com and @googlemail.com users)
>* Internal use (G Suite users that prefer to use a custom OAuth client)
>

1. Sign in to [Google Cloud Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) using your Google credentials.
1. In the left panel, click **Dashboard**. 
1. Click **Create project** in the upper-right corner of the screen.
1. Enter the **Project name**, then click **Create**.

1. Click the **Enable APIs and services** tab near the top of the screen.
1. In the **Search for APIs and Services** field at the top of the screen, type the name of the service you want to use (such as Gmail API or Google Drive API).
1. When it displays, click the API or service you want to connect to Workfront Fusion.
1. Click **Enable**to enable the selected API.
1. Repeat steps 6-8 for each API you want to enable.

   >[!NOTE]
   >
   >You must enable Google Drive API as well as the API of all Google apps you want to use (such as Google Sheets API).

1. On the screen that appears, click **Create credentials** in the upper-right corner.
1. Continue to the section [Configure OAuth consent settings](#configure-oauth-consent-settings) in this article.

## Configure OAuth consent settings {#configure-oauth-consent-settings}

1. In the left panel, click **OAuth consent screen**. 
1. Select **External**, then click **Create**.

   >[!NOTE]
   >
   >You will not be charged when selecting this option. For more information, see Google's information about exceptions to verification requirements.

1. Fill the required fields as follows:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>App name</p> </td> 
      <td> <p>Enter the name of the app asking for consent.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>Adobe Workfront Fusion </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">User support email</td> 
      <td>Enter an email address for users to contact you with questions about their consent when connecting to this app.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Email addresses</td> 
      <td>Enter one or more email addresses that Google can use to notify you about any changes to your project.</td> 
     </tr> 
    </tbody> 
   </table>

1. Under Authorized domains, click **Add domain**, and enter 

   ```
   workfrontfusion.com
   ```

   .

1. Click **Save and continue**.
1. Click **Add or remove scopes**.
1. In the right panel, enable the following scopes:

   <table cellspacing="15"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Service/API</th> 
      <th>Required scopes</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>Gmail</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Google Drive</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

   You may need to expand the list or go to the next page of the list to see them all.

1. Click **Update**.
1. Click **Save and continue**.
1. (Optional) Add any test users to the project.
1. Click **Save and continue**.
1. Examine your information for accuracy, then click **Back to dashboard**.

   >[!NOTE]
   >
   >You don't need to submit your consent screen and application for verification by Google.

1. Continue to [Create OAuth Credentials](#create-oauth-credentials).

## Create OAuth Credentials {#create-oauth-credentials}

1. In the left panel, click **Credentials**.

   >[!NOTE]
   >
   >If this is not the first API or service (Gmail or Google Drive) you have enabled, you don't have to create new credentials.

1. Click **Create credentials** near the top of the screen, then select **OAuth client ID** from the drop-down menu.

1. Fill the required fields as follows:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Application type</td> 
      <td> <p> Web application</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Workfront Fusion </td> 
     </tr> 
    </tbody> 
   </table>

1. Under Authorized redirect URIs, click **Add URI** and enter **one** of the following:

   * For Gmail or Google Drive:    
   
     ```   
     https://app.workfrontfusion.com/oauth/cb/google-restricted
     ```

   * For other Google apps:    
   
     ```   
     https://app.workfrontfusion.com/oauth/cb/google
     ```

1. Click **Create**.

   The Client ID and Client Secret display.

1. Copy the Client ID and Client Secret to a secure location. You will use them to make a connection in Workfront Fusion.
1. Continue to [Connect to Google in Workfront Fusion](#connect-to-google-in-workfront-fusion).

## Connect to Google in Workfront Fusion {#connect-to-google-in-workfront-fusion}

The process of creating a connection to Google differs depending on whether you are using a module from a Google service(such as Google Sheets or Google Docs), or if you are connecting to Google via the HTTP > Make an OAuth2.0 request module.

* [Connect to Google in a Google service module](#connect-to-google-in-a-google-service-module) 
* [Connect to Google in the HTTP > Make an OAuth2.0 request module](#connect-to-google-in-the-http-make-an-oauth2-0-request-module)

### Connect to Google in a Google service module {#connect-to-google-in-a-google-service-module}

1. In Workfront Fusion, locate the Google module that you need to create a connection for.
1. Click **Create a connection**, then click**Show advanced settings**.

1. Enter the Client ID and Client Secret you retrieved in [Create OAuth Credentials](#create-oauth-credentials) in the respective fields, then click **Continue**.

1. Sign in with your Google account.

   The **This app isn't verified** window displays. Note that the “app” mentioned in the window title is the OAuth client that you created above.

1. Click **Advanced**, then click **Go to Workfront Fusion (unsafe)** to allow access using your custom OAuth client.

1. Click **Allow**to grant Workfront Fusion permission.
1. In the window that appears, click **Allow**again to confirm your choices.

   The connection to the desired Google service using a custom OAuth client is established.

### Connect to Google in the HTTP > Make an OAuth2.0 request module {#connect-to-google-in-the-http-make-an-oauth2-0-request-module}

For instructions on connecting to Google in the HTTP > Make an OAuth2.0 request module, see [Instructions for creating a connection to Google in the HTTP > Make an OAuth 2.0 request module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) in [HTTP > Make an OAuth 2.0 request module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Possible error message:[403] Access Not Configured

If the [403} Access Not Configured error message displays, you you need to enable the corresponding API in your Google Cloud Platform. To enable the API, follow the steps in the section [Create a project on Google Cloud Platform](#create-a-project-on-google-cloud-platform) in this article.
