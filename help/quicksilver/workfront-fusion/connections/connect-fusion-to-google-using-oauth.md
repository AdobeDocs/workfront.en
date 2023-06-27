---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] using a custom OAuth client
description: You can use [!DNL Adobe Workfront Fusion] to connect to [!DNL Google Services] using a custom OAuth client. This procedure requires an existing [!DNL Google] account.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
---
# Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] using a custom OAuth client

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

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisites

You need an existing [!DNL Google] account to make this connection.

## Create a project on [!DNL Google Cloud Platform] 

The following procedure is intended for:

* Personal use ([!DNL @gmail.com] and [!DNL @googlemail.com] users)
* Internal use ([!DNL G Suite] users that prefer to use a custom OAuth client)

To create a project on [!DNL Google Cloud] Platform:

1. Sign in to [[!DNL Google Cloud] Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) using your [!DNL Google] credentials.
1. In the left panel, click **[!UICONTROL Dashboard]**.
1. Click **[!UICONTROL Create project]** in the upper-right corner of the screen.
1. Enter the **[!UICONTROL Project name]**, then click **[!UICONTROL Create]**.

1. Click the **[!UICONTROL Enable APIs and services]** tab near the top of the screen.
1. In the **[!UICONTROL Search for APIs and Services]** field at the top of the screen, type the name of the service you want to use (such as [!DNL Gmail] API or [!DNL Google Drive] API).
1. When it displays, click the API or service you want to connect to [!DNL Workfront Fusion].
1. Click **[!UICONTROL Enable]** to enable the selected API.
1. Repeat steps 6-8 for each API you want to enable.

   >[!NOTE]
   >
   >You must enable [!DNL Google Drive] API as well as the API of all [!DNL Google] apps you want to use (such as [!DNL Google Sheets] API).

1. On the screen that appears, click **[!UICONTROL Create credentials]** in the upper-right corner.
1. Continue to the section [Configure OAuth consent settings](#configure-oauth-consent-settings) in this article.

## Configure [!UICONTROL OAuth consent] settings 

1. In the left panel, click **[!UICONTROL OAuth consent screen]**.
1. Select **[!UICONTROL External]**, then click **[!UICONTROL Create]**.

   >[!NOTE]
   >
   >You will not be charged when selecting this option. For more information, see [!DNL Google]'s information about exceptions to verification requirements.

1. Fill the required fields as follows:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App name]</p> </td> 
      <td> <p>Enter the name of the app asking for consent.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL User support email]</td> 
      <td>Enter an email address for users to contact you with questions about their consent when connecting to this app.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email addresses]</td> 
      <td>Enter one or more email addresses that Google can use to notify you about any changes to your project.</td> 
     </tr> 
    </tbody> 
   </table>

1. Under [!UICONTROL Authorized domains], click **[!UICONTROL Add domain]**, and enter `workfrontfusion.com`.

1. Click **[!UICONTROL Save and continue]**.
1. Click **[!UICONTROL Add or remove scopes]**.
1. In the right panel, enable the following scopes:

<table style="table-layout:auto">
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
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

You may need to expand the list or go to the next page of the list to see them all.

1. Click **[!UICONTROL Update]**.
1. Click **[!UICONTROL Save and continue]**.
1. (Optional) Add any test users to the project.
1. Click **[!UICONTROL Save and continue]**.
1. Examine your information for accuracy, then click **[!UICONTROL Back to dashboard]**.

   >[!NOTE]
   >
   >You don't need to submit your consent screen and application for verification by [!DNL Google].

1. Continue to [Create OAuth Credentials](#create-oauth-credentials).

## Create OAuth Credentials 

1. In the left panel, click **[!UICONTROL Credentials]**.

   >[!NOTE]
   >
   >If this is not the first API or service ([!DNL Gmail] or [!DNL Google Drive]) you have enabled, you don't have to create new credentials.

1. Click **[!UICONTROL Create credentials]** near the top of the screen, then select **[!UICONTROL OAuth client ID]** from the drop-down menu.

1. Fill the required fields as follows:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Application type]</td> 
      <td> <p> [!UICONTROL Web application]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. Under [!UICONTROL Authorized redirect URIs], click **[!UICONTROL Add URI]** and enter **one** of the following:

   * For [!DNL Gmail] or [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * For other [!DNL Google] apps: `https://app.workfrontfusion.com/oauth/cb/google`

1. Click **[!UICONTROL Create]**.

   The [!UICONTROL Client ID] and [!UICONTROL Client Secret] display.

1. Copy the [!UICONTROL Client ID] and [!UICONTROL Client Secret] to a secure location. You will use them to make a connection in [!DNL Workfront Fusion].
1. Continue to [Connect to [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

## Connect to [!DNL Google] in [!DNL Workfront Fusion] 

The process of creating a connection to [!DNL Google] differs depending on whether you are using a module from a [!DNL Google] service(such as [!DNL Google Sheets] or [!DNL Google Docs]), or if you are connecting to [!DNL Google] via the [!UICONTROL HTTP] >[!UICONTROL Make an OAuth2.0] request module.

* [Connect to [!DNL Google] in a [!DNL Google] service](#connect-to-google-in-a-google-service)
* [Connect to [!DNL Google] in the [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] module](#connect-to-google-in-the-http--make-an-oauth20-request-module)

### Connect to [!DNL Google] in a [!DNL Google] service

1. In [!DNL Workfront Fusion], locate the [!DNL Google] module that you need to create a connection for.
1. Click **[!UICONTROL Create a connection]**, then click **[!UICONTROL Show advanced settings]**.

1. Enter the [!UICONTROL Client ID] and [!UICONTROL Client Secret] you retrieved in [[!UICONTROL Create OAuth Credentials]](#create-oauth-credentials) in the respective fields, then click **[!UICONTROL Continue]**.

1. Sign in with your [!DNL Google] account.

   The **[!UICONTROL This app isn't verified]** window displays. Note that the "app" mentioned in the window title is the OAuth client that you created above.

1. Click **[!UICONTROL Advanced]**, then click **[!UICONTROL Go to [!DNL Workfront Fusion] (unsafe)]** to allow access using your custom OAuth client.

1. Click **[!UICONTROL Allow]** to grant [!DNL Workfront Fusion] permission.
1. In the window that appears, click **[!UICONTROL Allow]** again to confirm your choices.

   The connection to the desired [!DNL Google] service using a custom OAuth client is established.

### Connect to [!DNL Google] in the [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] module {#connect-to-google-in-the-http--make-an-oauth20-request-module}

For instructions on connecting to [!DNL Google] in the [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] module, see [Instructions for creating a connection to [!DNL Google] in the [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) in [[!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Possible error message:[!UICONTROL [403] Access Not Configured]

If the [!UICONTROL [403] Access Not Configured] error message displays, you you need to enable the corresponding API in your Google Cloud Platform. To enable the API, follow the steps in the section [Create a project on [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) in this article.
