---
filename: link-documents-from-external-apps
product-area: documents
navigation-topic: add-documents-to-workfront
title: Link documents from external applications
description: You can link documents and folders to Adobe Workfront from the following sources:
---

# Link documents from external applications

You can link documents and folders to Adobe Workfront from the following sources:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Existing third party cloud document providers</td> 
   <td>These include the following: 
    <ul> 
     <li>Box</li> 
     <li>Dropbox</li> 
     <li>Dropbox Business</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>Google Drive</li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Proof </td> 
   <td>You can make proofs that were originally created within Workfront Proof available within Workfront. A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see <a href="https://www.workfront.com/plans">Workfront Plans</a>.</td> 
  </tr> Experience Manager Assets Essentials You can link documents to Workfront from Experience Manager Assets Essentials. For more information, see Adobe Workfront for Experience Manager Assets Essentials. 
  <tr> 
   <td role="rowheader">Workfront DAM </td> 
   <td>This requires an additional purchase. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Microsoft SharePoint</td> 
   <td>This requires an additional purchase. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Other document providers (through custom document integrations)</td> 
   <td> <p class="workfront_plans">A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see <a href="https://www.workfront.com/plans">Workfront Plans</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Before you link documents or folders, your Workfront administrator must enable this functionality for each document provider, or for a custom document integration,&nbsp;as described in [Configure document integrations](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

You can proof and approve documents linked to an external cloud provider the same way you do so with documents uploaded directly to Workfront.&nbsp;

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Document storage

Documents that are linked to Workfront from an external application are stored with the external cloud provider, not within Workfront.

The following exceptions apply:

* When provided by the document service, thumbnails and preview images might be stored on Workfront servers.
* When you use proofing in Workfront, the document is copied and added to the proofing servers.&nbsp;

## Link a document from an external application to Workfront

You can link&nbsp;existing documents with an external cloud&nbsp;provider. This includes any shared documents.

* [Prerequisites](#prerequi) 
* [Link an external document to Workfront](#linking-existing-documents) 
* [Add a new version of a linked document](#add) 
* [Link Workfront Proof documents](#linking-existing-documents-from-workfront-proof) 
* [Create a Google document from within Workfront](#creating-new-linked-google-documents)

### Prerequisites

Before you link documents or folders, your Workfront administrator must enable this functionality for each document provider, or for a custom document integration,&nbsp;as described in [Configure document integrations](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

### Link an external document to Workfront

You can link documents to Workfront from an external application such as Google and Microsoft OneDrive.

>[!IMPORTANT]
>
>Dropbox stores documents based on the&nbsp;file path. Because of this, if a&nbsp;file linked from Dropbox is moved, renamed, or deleted, it becomes inaccessible in Workfront.

1. Go to the `Documents` area in Workfront where you want the document.
1. Click `Add New`, then click the external document provider&nbsp;where you want to link&nbsp;documents to Workfront.

   For example, to link documents from Dropbox, click `From Dropbox`.

   External providers that you have already authorized appear at the top of the list.

1. (Conditional) If you are prompted to log into the external service, type your login credentials for the service in the box that appears, then click `Sign in`.
1. (Conditional) If you are prompted to authorize the external application, click the `Authorize` button.

   You need to do this only once.

1. In the search box of the `Link External Files and Folders` box that appears, type the name of the item you want to search for, then press `Enter` to see all results&nbsp;from the external application, regardless of which folder they are storied in.

   Or

   Browse to and select the documents you want to link.

   Though you can select multiple documents, only documents that are selected in&nbsp;the current view are linked. For example, if you select a document, then go into a folder, the document&nbsp;you originally selected is not linked.

1. (Conditional) If you are a Workfront DAM customer, click the `Thumbnail`&nbsp;icon to display files as thumbnail images.

   >[!NOTE]
   >
   >Workfront DAM customers can view thumbnails when linking&nbsp;documents from Workfront DAM. Thumbnails might also be displayed for Workfront DAM customers for other services such as Dropbox and Box. However, viewing thumbnails for&nbsp;services other than Workfront DAM within Workfront is not supported, and thumbnails are never displayed when linking&nbsp;documents from SharePoint or Google Drive.

1. Click `Link`.

   In Workfront, the cloud provider's icon appears next to the documents.

   >[!NOTE]
   >
   >For documents that are linked&nbsp;to Box, the link&nbsp;to the document in Box does not display until you refresh the page.

### Add a new version of a linked document

You can add a new version of a document linked to Workfront from an external application.

1. Go to the `Documents` area where the document is linked, then select the linked document.

   >[!IMPORTANT]
   >
   >The document must be outside of a linked folder to create a new version.

1. Click `Add New` > `Version`, then click the external document provider.

   For example, to link a new version of a document from Dropbox, click `From Dropbox`.

   External providers that you have already authorized appear at the top of the list.

1. (Conditional) If you are prompted to log into the external service, type your login credentials for the service in the box that appears, then click `Sign in`.
1. (Conditional) If you are prompted to authorize the external application, click `Authorize`.

   You need to do this only once.

1. In the search box of the `Link External Files and Folders` box that appears, type the name of the item you want to search for, then press `Enter` to see all results&nbsp;from the external application, regardless of which folder they are storied in.

   Or

   Browse to and select the documents you want to link.

   You can select multiple documents; however, only documents that are selected in&nbsp;the current&nbsp;view are linked.&nbsp;For example, if you select a document, then go into a folder, the document&nbsp;you originally selected is not linked.

1. (Conditional) If you are a Workfront DAM customer, click the `Thumbnail`&nbsp;icon to display files as thumbnail images.

   >[!NOTE]
   >
   >Workfront DAM customers can view thumbnails when linking&nbsp;documents from Workfront DAM. Thumbnails might also be displayed for Workfront DAM customers for other services such as Dropbox and Box. However, viewing thumbnails for&nbsp;services other than Workfront DAM within Workfront is not supported, and thumbnails are never displayed when linking&nbsp;documents from SharePoint or Google Drive.

1. Click `Link`.

   In Workfront, the cloud provider's icon appears next to the documents, indicating that&nbsp;they are linked&nbsp;to the external&nbsp;cloud&nbsp;provider.

   >[!NOTE]
   >
   >For documents that are linked&nbsp;to Box, the link&nbsp;to the document in Box does not display until you refresh the page.

For information about adding new version of a document you have uploaded to Workfront from your file system, see [Add documents to Adobe Workfront from your file system](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#adding-new-versions-of-documents) in [Add documents to Adobe Workfront from your file system](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### Link Workfront Proof documents

You can link proofs to Workfront that originally existed in Workfront Proof. When you link a proof from Workfront Proof, all comments and other metadata associated with the proof are available in Workfront.&nbsp;

You can link only those proofs for which you have View access in Workfront Proof. (For more information about rights within Workfront Proof, see [Configure a user's proofing access](../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md)).

1. Go to the `Documents` area in Workfront where you want the document.
1. Click `Add New`, then click `From Workfront Proof`.

   >[!NOTE]
   >
   >The options in this menu may vary depending on what third party providers are configured in your environment.

1. In the `Link` proofs `from` Workfront Proof box that appears, begin typing the name of the proof you want to make available in Workfront.

   The list is filtered as you type.

1. Select up to 10 proofs to link.

   Any proof name that is dimmed is not available to link, because the proof is already associated with a document in Workfront.

1. Click `Link`.

   The most current version of the proof is linked to Workfront. When you open the proof, all versions are available in the proofing viewer.

### Create a Google document from within Workfront

You can create a new Google document from within Workfront. You cannot create new documents from within Workfront for other cloud providers.

1. Go to the `Documents` area in Workfront where you want the document.
1. Click `Add New` > `Google File`, then select the type of Google document you want to create.  

1. Select the type of Google Doc that you want to create.
1. If the `Add Google Drive Account` box appears, click `Authorize Googe Drive`.

   A Google Document is added to the `Documents` tab.

   >[!NOTE]
   >
   >&nbsp;My Drive and Shared with Me&nbsp;display two different results. If you are unable to locate a file in My Drive, check in the Shared with Me&nbsp;folder.

## Update and link a document from Workfront to an external cloud provider

You can upload and link a document from Workfront to an external cloud provider. This moves storage of the document from Workfront to the external cloud provider. When the document is changed in the external application, it updates automatically in Workfront.

Users without Workfront access can see the document in the external application if they have access to the application.

1. Select a document that is uploaded in Workfront.
1. Click `More` > `Send to`, then select the cloud provider that you want to store the linked document.
   You can also use the More menu on the Document Details page to do this. 
1. Select the folder in the provider's application where you want to store the document.

   This can be any folder in the provider's application, including a shared folder. 

1. Click `Save`.

   The external provider's logo appears next to the document name to indicate that the document is now linked to Workfront and stored by the external cloud provider.

   ![doc_with_google_drive_link_highlight__1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

   You can also send documents from Workfront to Workfront Library. For information, see in [Send documents from Workfront to Workfront Library](../../workfront-library/content-management/send-documents-from-wf-to-library.md).

## Link folders

When you link a folder between Workfront and an external cloud&nbsp;provider, the folder and all of its contents are linked. If users without Workfront access add, remove, and modify files from the external&nbsp;document application, their changes are synchronized to Workfront. The following sections describe how to link&nbsp;folders and subfolders:

* [Folder access rights](#folder-access-rights) 
* [Link one or more external folders](#linking-a-folder) 
* [Add subfolders to a linked folder](#creating)

### Folder access rights

When synchronizing folder content from an external document application, Workfront uses the credentials of the user who originally linked the folder. This results in the following user experience:

* If users do not have access to view files and folders in the external application, but do have access to view the linked folder via Workfront, they can view only the names of the files and folders in Workfront, not their contents. 
* When someone accesses content inside a linked folder in Workfront (such as a subfolder in a linked folder) that was linked to Workfront by another user, the content synchronizes to Workfront using the Workfront login credentials of the user who originally linked the folder, not the credentials of the user accessing the content.

>[!IMPORTANT]
>
>* If the user who originally linked the folder is removed from the Workfront system, users are no longer able to access content on the linked folder&nbsp;via Workfront. In this case, the folder must be relinked by an active Workfront user who has rights to the folder in the external&nbsp;application. 
>* If the user who linked a folder no longer has access to the external application, Workfront can no longer access the contents of the folder. This may happen, for example, if the user who originally linked the folder leaves the company. To ensure continued access, a user with access to the folder must re-link the folder.

>

### Link one or more external folders

1. Go to the area in Workfront where you want the folder, then click Documents in the left panel.
1. Click `Add New`, then click the external document provider from which you want to link&nbsp;a folder to Workfront.
1. (Conditional) If you have not yet authorized the external service, specify your login credentials for the external provider, then click `Sign in`.

   External providers that you have already authorized appear at the top of the list.

1. In the `Link External Files and Folders` box that appears, browse to and select the folders you want to link.

   Or

   Type the name of the folder you want to search for, then press `Enter`.

   You can select multiple folders; however, only folders that are selected in&nbsp;the current&nbsp;view are linked. For example, if you select a folder, then go into a folder, the folder you originally selected is not linked.

   >[!NOTE]
   >
   >When linking folders from Google Drive, you can only link folders that are within your personal drive (My Drive) and Team Drive. You cannot link folders from the Shared with Me area.

1. Click `Link`.

   In Workfront, the cloud provider's logo displays next to the folder, indicating that&nbsp;it is linked&nbsp;to the external&nbsp;cloud&nbsp;provider.

1. (Optional) To rename the folder so that the folder name in Workfront is different from the folder name in the external document application, select the folder in the `Folders` section, click the More menu that displays next to the folder name, then click `Rename`.

This does not rename the folder in the external&nbsp;application.

### Add subfolders to a linked&nbsp;folder

You can create a new folder inside an existing linked folder. You can also drag another folder into an existing linked folder.

1. To create a new folder within an existing linked folder, go to the existing folder, then create the new folder as described in [Create document folders](../../documents/organizing-documents/create-documents-folder.md).

   Or

   To drag an existing folder into an existing linked folder, go to the&nbsp;Documents&nbsp;area where you want the subfolder, then drag it into the linked folder.

   >[!NOTE]
   >
   >The following limitations apply when dragging an existing Workfront&nbsp;folder into a linked&nbsp;folder:
   >
   >  
   >  
   >  * The folder that you are dragging can't already be linked&nbsp;and can't contain any content that is already linked.
   >  * The folder (including its contents)&nbsp;that you are dragging can't exceed 50 MB.
   >  
   >

## Add a document to a linked folder

When you add a document to a linked&nbsp;folder via Workfront, it is automatically added as a linked&nbsp;document.

1. In the `Documents` area where you want the document, drag the document into a linked&nbsp;folder.  

   Selection box is wonky on the left 

   Or

   Select the linked folder where you want the document, click `Add New > Document`, then browse to the document and add it to the folder.

   A new version of your document is automatically created in the external&nbsp;application and linked to Workfront.

## Delete a linked document or folder

When you delete a linked&nbsp;document or folder from the external application, the document or folder remains in the Workfront system until you also delete it from Workfront.

1. Select the linked document or folder, then click `Delete`.
1. In the confirmation box that appears, click `Yes, Unlink it`.

   The document is unlinked from the Workfront site. It is not affected in the external application.

## About renaming linked documents and folders

When you rename a linked document or folder, the change is visible only in the application where you make it. For example, if you rename a linked document in Workfront, the new name is visible only in Workfront.

If you want the name to match in Workfront and in the external application, you must rename it in both places.

>[!IMPORTANT]
>
>Do not rename a document in Workfront that is linked&nbsp;to Dropbox; doing so renders the file in Workfront inaccessible. Instead, rename the file in Dropbox, then re-synchronize the file, as described in [Link documents from external applications](#synchronizing-changes-made-on-a-linked-document).

