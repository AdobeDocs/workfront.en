---
filename: disable-document-integrations
title: Disable document integrations
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Disable document integrations
description: As anAdobe Workfront administrator, you can disable the connection between Workfront and any of the third-party document providers.
---

# Disable document integrations

As anAdobe Workfront administrator, you can disable the connection between Workfront and any of the third-party document providers.&nbsp;

When you disable the connection between Workfront and a document provider, the links to the documents disappear from Workfront. Users can no longer see the linked documents, they cannot make any changes to the documents through the Workfront links, and they cannot add more documents to that provider.&nbsp;

## Access requirements

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a Workfront administrator. For information on Workfront administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Disable cloud provider integrations

To disable document integrations for Workfront DAM, Workfront Library, Box, Dropbox, Google Drive, Microsoft&nbsp;OneDrive, WebDAM:

1. Log in to Workfront as a Workfront administrator.
1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Documents** > **Cloud Providers**.

1. Deselect any of the cloud providers you want to disconnect from Workfront.
1. Click **Save**.

   Users are not able to connect to the specific cloud provider you disabled, and they can no longer link documents from that cloud provider to Workfront.

## Disable the SharePoint integration

1. Log in to Workfront as a Workfront administrator.
1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Expand **Documents**, then click **SharePoint Integration**.
1. Select the SharePoint integration you want to disable.
1. Click **Disable**.  
   Users are not able to connect to the SharePoint site you disabled, and they can no longer link documents from SharePoint&nbsp;to Workfront.&nbsp;

## Disable custom integrations

1. Log in to Workfront as the administrator.
1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Documents** > **Custom Integration**.
1. Select the custom&nbsp;integration you want to disable.
1. Click **Disable**.

   Users are not able to connect to the third-party document provider you disabled, and they can no longer link documents from that cloud provider to Workfront.

