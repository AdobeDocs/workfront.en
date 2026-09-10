---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Remove links between Adobe Workfront and external document storage providers
description: When uploading a document from any service for the first time, Adobe Workfront requests permission from the user to access their document service. When the user provides their document service credentials to log in, the document service links itself to Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: fce8e8aa-fc48-49e1-a71d-c3933a179cf5
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wDii-Gr-3a0NfMhc9VPfbiUNSTyJaJuFHeXACI26NxU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Remove links between Adobe Workfront and external document storage providers

When uploading a document from any service for the first time, Adobe Workfront requests permission from the user to access their document service. When the user provides their document service credentials to log in, the document service links itself to Workfront.

For information about linking external document services to Workfront, see [Linking Documents from External Applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Since the document service is the one allowing permission to link to Workfront, it is not possible for Workfront&nbsp;to remove the permission granted by the document service. You must remove the permission from within the document service application or you must call our Support Team to remove this link from our servers.

>[!NOTE]
>
>This functionality is not available in the new Documents area.<br>
>If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> 
   <p>Contributor or higher</p>
   <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Documents</p>  </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Remove the link between Workfront and Dropbox

1. Log in to Dropbox.
1. Click your profile picture in the upper right corner, then click **Settings**.
1. Click the&nbsp;**Connected apps** tab, then scroll down to **Linked apps**.

1. Click the **X** next to Workfront.

## Remove the link between Workfront and Box

1. Log in to your Box account.
1. Click your profile picture in the upper right corner.
1. Click **Account Settings**, then the **Security** tab.

1. Find **MyWorkfront** and click the **X** under Forget App.

## Remove the link between Workfront and Google Drive

1. Log in to your Google Drive.
1. Click the gear icon in the upper right corner, then click **Settings**.
1. Click **Manage Apps** on the left&nbsp;side and find **Workfront** in the list.

1. Under the Options drop-down menu, click **Disconnect from Drive**.

## Remove the links between Workfront and Other Document Storage Providers

You must call our Support Team to disconnect Microsoft One Drive or WebDAM from Workfront.

For information about contacting our Support Team, see [Contact Customer Support](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
