---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrate linked folders and documents
description: You can use the API to migrate linked folders and documents to Adobe Experience Manager Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
---
# Migrate linked folders and documents

You can use the API to migrate linked folders and documents to Adobe Experience Manager Assets.

## Procedure

1. Identify all documents and folders linked with the previous external document storage provider, noting their Workfront internal document or folder identifiers as well as the folder id of any containing folder.

    >[!NOTE]
    >
    > You should check for all discovered folders or documents to verify they have not already created a link for them with the new provider.

1. Locate the documents and folders in the new repository by path, then look up their identity in the external system. 

1. Create a mapping of the internal Workfront ID, to the ID in the new external store. You need this to create a new link in the following step.

1. Create a new document or document folder link in Workfront, pointing to the resource in its new location via its new external ID.

    1. **Documents**: Add a new version of the existing document with the new external document provider.
    1. **Folders**: Create a new folder in the same place with the same name.

>[!CAUTION]
>
>   Do not delete the existing linked folders. This could result in data loss. To remove old folder links from the Workfront application, disable the custom document integration in the Setup area. 


## Example process for migrating links

![simplified-link-flow](assets/links-flow-simplified.png)

## API information

For more information on the Workfront APIs in this section, see [Developer Documentation:Documents](https://developer.workfront.com/documents.html).

### Find all documents

Find All **Documents (DOCU)** Linked to **Document Provider** of **providerType** with **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}

```

[API DOCS reference](https://developer.workfront.com/documents.html#get-/docu/search)

### Find all folders

Find All **Document Folders (DOCFDR)** Linked to Document Provider of **providerType** with **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}

```

API DOCS: (Document Folder Endpoints Not Currently Covered at developer.workfront.com)

### Link documents

Link **Documents (DOCU)** from **External Document Provider** of **providerType** with **documentProviderID**.

>[!IMPORTANT]
>
>Documents are temporarily stored. Meaning, you have access to all versions of the document. When you create the link, you can specify the existing document ID, so you are simply writing a new version to that document, with the data being hosted externally in the new provider. This document ID is the same as the document ID found on the document link you are replacing. It's the same conceptual document. You are simply indicating that the bytes for this new version are stored with a different provider.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}

```

API DOCS: (Internal Link Endpoints Not Currently Covered at developer.workfront.com)

### Link folders

Link **Document Folders (DOCFDR)** from **External Document Provider** of **providerType** with **documentProviderID**.

>[!IMPORTANT]
>
>For folder links, unlike Document links, you need the 'documentFolderId' of the folder in Workfront you want to place your new link into. This is the same parent folder, most likely, as the linked folder we are copying. 

>[!CAUTION]
>
>Folders are not temporally stored. Do not delete the old folders. Disable the custom document integration in the setup area to remove old folders.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}

```

API DOCS: (Internal Link Endpoints Not Currently Covered at developer.workfront.com)

## Important terms

* **Document**: A digital asset within Workfront

* **Document Folder**: A container for digital assets within Workfront

* **Document ID**: Workfront internal ID for a digital asset

* **Document Folder ID**: Workfront internal ID for a digital asset folder

* **Document Provider ID**: ID associated with specific doc providers

>[!IMPORTANT]
>
> For any given Document Provider Type, a customer may have multiple connected instances. They may have multiple AEM Repositories linked for example. Or multiple Google Drive instances linked. The Document Provider ID indicates the specific instance of the connection type we want to replace or switch to.

* **Document Storage Provider Type (also "External Integration Type")**: The type of document storage provider integration that Workfront supports. Either via a dedicated integration or a "custom integration". 

* **Current Document Storage Provider Types ( providerType)**:

    ```
    ATTASK
    BOX
    GOOGLE
    SHAREPOINT
    WEBDAM
    WORKFRONTDAM
    INFERNO
    WIDEN
    DROPBOX
    DROPBOX_BUSINESS
    ONEDRIVE
    QUIP
    WEBHOOKS
    AEM
    MOCK
    ```

* **Linked Document**: A digital asset hosted in an external document storage provider. Workfront will have its own internal "Document ID' for the asset, but the bytes are stored externally. To facilitate this, Workfront also stores an "external document ID" to assist with locating the externally referenced resource within the remote repository or store.

* **Linked Document Folder**: A container for digital assets hosted in an external document storage provider. Workfront will have its own internal "Document Folder ID' for the asset, but the bytes are stored externally. To facilitate this, Workfront also stores an "external document ID" to assist with locating the externally referenced resource within the remote repository or store.

* **External Document ID**: ID assigned when assets are stored outside of Workfront. Workfront maps its internal identifier, to the identifier used to locate the asset in the external system, via this "external document identifier" field. Therefore, when linking the document or folder from a new external store, a new external document identifier must be composed, in the appropriate format for the external document provider to identify the document in the new repository or store. 

    >[!NOTE]
    >
    > Workfront does not yet have a standard for external document identifiers. A new spec is being used for AEM IDs, but for other IDs, the external document ID may take on different forms depending on the provider type.


* **Object Type**: This is an API only term for the purposes of this document. It's a type of generic object within Workfront that you wish to interact with. In this cases, you'll interact with documents and folders having the types "DOCU" and "DOCFDR" respectively.

* **Object ID**: The internal Workfront identifier for the generic object you wish to interact with. You'll interact with documents and folders so this will be either the document ID or document folder ID respectively.
