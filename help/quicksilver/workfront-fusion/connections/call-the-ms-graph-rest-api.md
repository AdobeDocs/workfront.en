---
title: Call the MS Graph REST API via the [!DNL Adobe Workfront Fusion] HTTP &gt; Make an OAuth 2.0 request module
description: Call the MS Graph REST API via the [!DNL Adobe Workfront Fusion] HTTP &gt; Make an OAuth 2.0 request module
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
---
# Call the[!UICONTROL  MS Graph REST API] via the [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module

<!-- Audited: 3/2024-->

Many [!DNL Microsoft] web services are accessed through the [!DNL Microsoft Graph API]. You can create a connection to the [!DNL Microsoft Graph API], by using the [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: [!UICONTROL Standard]</p><p>Or</p><p>Current: [!UICONTROL Work] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy: Any </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>New:</p> <ul><li>[!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] Plan: Your organization must purchase [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] is included.</li></ul>
   <p>Or</p>
   <p>Current: Your organization must purchase [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Register [!DNL Workfront Fusion] in the [!DNL Microsoft Application Registration Portal] 

To create a connection to the [!DNL Microsoft Graph REST API], you must first register [!DNL Adobe Workfront Fusion].

1. Begin registering a new application as described in [Register your app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) in the [!DNL Microsoft] documentation.

   As part of the registration, [!DNL Microsoft] requires the following information:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Application name]</td>
        <td>Enter a name for the application, such as "My [!DNL Workfront Fusion] application."</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirect URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. When you have completed the app registration, make note of the [!UICONTROL Application ID].

   >[!IMPORTANT]
   >
   >You will need the Application ID to set up your connection in [!DNL Workfront Fusion].

1. Generate an [!UICONTROL Application Secret]. Make note of this secret.

   For instructions, see [Register your app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) in the [!DNL Microsoft] documentation.

   >[!IMPORTANT]
   >
   >You will need the [!UICONTROL Application Secret] to set up your connection in [!DNL Workfront Fusion].

1. Configure the permissions for your application.

   For specifics on locating and configuring these fields, see the "Configure permissions for Microsoft Graph" section in [Get access without a user](https://docs.microsoft.com/en-us/graph/auth-v2-service) in the [!UICONTROL Microsoft] documentation.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL What type of permissions does your application require?]</td> 
      <td>Select <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Select permissions]</td> 
      <td> <p>Select the following permissions:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Any other permissions required by your integrations (Example: <code>User.Read</code>)</p> </li> 
       </ul> <p><b>Important</b>: You will need the selected permissions to set up your connection in [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Proceed to [Configure your [!DNL MS Graph API] connection in [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configure your [!DNL MS Graph API] connection in [!DNL Workfront Fusion] 

After you register [!DNL Workfront Fusion] as discussed in [Register [!DNL Workfront Fusion] in the [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), you can configure your connection in the [!UICONTROL HTTP] > [!UICONTROL Make an Oauth 2.0] request module.

1. Add an [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 call] module to your scenario.
1. Click **[!UICONTROL Add]** next to the [!UICONTROL connection] field.
1. Configure the connection fields as follows:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name]</td> 
      <td>Enter a name for the connection.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Flow type]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Enter the permissions that you selected in step 4 of <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Register [!DNL Workfront Fusion] in the [!DNL Microsoft Application Registration Portal]</a>.</p> <p>For each scope, click <b>[!UICONTROL Add]</b> and type in the permission.</p> <p>Example: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>Enter the [!UICONTROL Application ID] from step 2 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Register [!DNL Workfront Fusion] in the [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Enter the [!UICONTROL Application Secret] that you generated in step 3 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Register [!DNL Workfront Fusion] in the [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize parameters]</td> 
      <td> <p>Add the following Authorize parameters:</p> 
       <ul> 
        <li> <p>[!UICONTROL Key]:<code> response_mode</code> [!UICONTROL Value]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Key]: <code>prompt </code>[!UICONTROL Value]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access token parameters]</td> 
      <td>You do not need to enter anything into this field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Refresh token parameters]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Click <b>[!UICONTROL Add]</b>.</p> </li> 
        <li value="2"> <p>In the <b>[!UICONTROL Key]</b> field, enter <code>scope</code>.</p> </li> 
        <li value="3"> <p>In the <b>[!UICONTROL Value]</b> field, enter all of the [!UICONTROL scope]s that you entered into the scope field, separated by spaces.</p> <p>Example: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Headers]</td> 
      <td>You do not need to enter anything into this field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Placement]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Continue]**.
1. In the window that appears, click **[!UICONTROL Accept]** to complete the connection and return to the module.
