---
filename: connect-fusion-to-google-using-oauth
product: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connect Adobe Workfront Fusion to Google Services using a custom OAuth client
description: You must have the following access to use the functionality in this article:
---

# Connect *Adobe Workfront Fusion* to Google Services using a custom OAuth client

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
    <td> <p>Plan, Work</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront Fusion</em> license**</td> 
   <td> <p><em>Workfront Fusion for Work Automation and Integration</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <em>Adobe Workfront Fusion</em> as well as <em>Adobe Workfront</em> to use functionality described in this article.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

&#42;&#42;For information on *Adobe Workfront Fusion* licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

You need an existing Google account to make this connection.

## Create a project on Google Cloud Platform

>[!NOTE]
>
>The following procedure is intended for:
>
>* Personal use (@gmail.com and @googlemail.com users)
>* Internal use (G Suite users that prefer to use a custom OAuth client)
>

<ol> 
 <li value="1">Sign in to <a href="https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project">Google Cloud Platform</a> using your Google credentials.</li> 
 <li value="2">In the left panel, click <span class="bold">Dashboard</span>. </li> 
 <li value="3">Click <span class="bold">Create project</span> in the upper-right corner of the screen.</li> 
 <li value="4">Enter the <span class="bold">Project name</span>, then click <span class="bold">Create</span>.</li> 
 <li value="5">Click the <span class="bold">Enable APIs and services</span> tab near the top of the screen.</li> 
 <li value="6">In the <span class="bold">Search for APIs and Services</span> field at the top of the screen, type the name of the service you want to use (such as Gmail API or Google Drive API).</li> 
 <li value="7">When it displays, click the API or service you want to connect to <em>Workfront Fusion</em>.</li> 
 <li value="8">Click <span class="bold">Enable </span>to enable the selected API.</li> 
 <li value="9"> <p>Repeat steps 6-8 for each API you want to enable.</p> <note type="note">
   You must enable Google Drive API as well as the API of all Google apps you want to use (such as Google Sheets API).
  </note> </li> 
 <li value="10">On the screen that appears, click <span class="bold">Create credentials</span> in the upper-right corner.</li> 
 <li value="11">Continue to the section <a href="#configur" class="MCXref xref">Configure OAuth consent settings</a> in this article.</li> 
</ol>

## Configure OAuth consent settings

<ol> 
 <li value="1">In the left panel, click <span class="bold">OAuth consent screen</span>. </li> 
 <li value="2"> <p>Select <span class="bold">External</span>, then click <span class="bold">Create</span>.</p> <note type="note">
   You will not be charged when selecting this option. For more information, see Google's information about exceptions to verification requirements.
  </note> </li> 
 <li value="3"> <p>Fill the required fields as follows:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"> <p>App name</p> </td> 
     <td> <p>Enter the name of the app asking for consent.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><em>Adobe Workfront Fusion</em> </p> </td> 
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
  </table> </li> 
 <li value="4">Under Authorized domains, click <span class="bold">Add domain</span>, and enter <code>workfrontfusion.com</code>.</li> 
 <li value="5">Click <span class="bold">Save and continue</span>.</li> 
 <li value="6">Click <span class="bold">Add or remove scopes</span>.</li> 
 <li value="7"> <p>In the right panel, enable the following scopes:</p> 
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
  </table> <p>You may need to expand the list or go to the next page of the list to see them all.</p> </li> 
 <li value="8">Click <span class="bold">Update</span>.</li> 
 <li value="9">Click <span class="bold">Save and continue</span>.</li> 
 <li value="10">(Optional) Add any test users to the project.</li> 
 <li value="11">Click <span class="bold">Save and continue</span>.</li> 
 <li value="12"> <p>Examine your information for accuracy, then click <span class="bold">Back to dashboard</span>.</p> <note type="note">
   You don't need to submit your consent screen and application for verification by Google.
  </note> </li> 
 <li value="13">Continue to <a href="#create2" class="MCXref xref">Create OAuth Credentials</a>.</li> 
</ol>

## Create OAuth Credentials

<ol> 
 <li value="1"> <p>In the left panel, click <span class="bold">Credentials</span>.</p> <note type="note">
   If this is not the first API or service (Gmail or Google Drive) you have enabled, you don't have to create new credentials.
  </note> </li> 
 <li value="2">Click <span class="bold">Create credentials</span> near the top of the screen, then select <span class="bold">OAuth client ID</span> from the drop-down menu.</li> 
 <li value="3"> <p>Fill the required fields as follows:</p> 
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
     <td><em>Workfront Fusion</em> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4"> <p>Under Authorized redirect URIs, click <span class="bold">Add URI</span> and enter <span class="bold">one</span> of the following:</p> 
  <ul> 
   <li> <p>For Gmail or Google Drive: <code>https://app.workfrontfusion.com/oauth/cb/google-restricted</code></p> </li> 
   <li> <p>For other Google apps: <code>https://app.workfrontfusion.com/oauth/cb/google</code></p> </li> 
  </ul> </li> 
 <li value="5"> <p> Click <span class="bold">Create</span>.</p> <p>The Client ID and Client Secret display.</p> </li> 
 <li value="6"> <p>Copy the Client ID and Client Secret to a secure location. You will use them to make a connection in <em>Workfront Fusion</em>.</p> </li> 
 <li value="7"> <p>Continue to <a href="#connect" class="MCXref xref">Connect to Google in Workfront Fusion</a>.</p> </li> 
</ol>

## Connect to Google in *Workfront Fusion*

The process of creating a connection to Google differs depending on whether you are using a module from a Google service(such as Google Sheets or Google Docs), or if you are connecting to Google via the HTTP > Make an OAuth2.0 request module.

* [Connect to Google in a Google service module](#connect2) 
* [Connect to Google in the HTTP > Make an OAuth2.0 request module](#connect3)

### Connect to Google in a Google service module

1. In *Workfront Fusion*, locate the Google module that you need to create a connection for.
1. Click `Create a connection`, then click `Show advanced settings`.

1. Enter the Client ID and Client Secret you retrieved in [Create OAuth Credentials](#create2) in the respective fields, then click `Continue`.

1. Sign in with your Google account.

   The `This app isn't verified` window displays. Note that the “app” mentioned in the window title is the OAuth client that you created above.

1. Click `Advanced`, then click `Go to *Workfront Fusion* (unsafe)` to allow access using your custom OAuth client.

1. Click `Allow`to grant *Workfront Fusion* permission.

1. In the window that appears, click `Allow`again to confirm your choices.

   The connection to the desired Google service using a custom OAuth client is established.

### Connect to Google in the HTTP > Make an OAuth2.0 request module

For instructions on connecting to Google in the HTTP > Make an OAuth2.0 request module, see [Instructions for creating a connection to Google in the HTTP > Make an OAuth 2.0 request module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) in [HTTP > Make an OAuth 2.0 request module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Possible error message:[403] Access Not Configured

If the [403} Access Not Configured error message displays, you you need to enable the corresponding API in your Google Cloud Platform. To enable the API, follow the steps in the section [Create a project on Google Cloud Platform](#create) in this article.
