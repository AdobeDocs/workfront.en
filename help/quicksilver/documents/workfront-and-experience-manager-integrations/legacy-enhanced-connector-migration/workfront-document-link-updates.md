---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrate linked folders and documents
description: text
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
---

# Migrate linked folders and documents

To migrate linked folders and documents:

1. Using the API, identify all documents and folders linked with the previous external document storage provider, noting their Workfront internal document or folder identifiers as well as the folder ID of any containing folder:

    1. **Documents**

        Find All Documents (DOCU) Linked to Document Provider of providerType with documentProviderID

        ```
        Http Method: GET
        
        Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}

        ```

        API DOCS: https://developer.workfront.com/documents.html#get-/docu/search

    1. **Folders** 

        Find All Document Folders (DOCFDR) Linked to Document Provider of providerType with documentProviderID

        ```
        Http Method: GET
        
        Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}

        ```

        API DOCS: (Document Folder Endpoints Not Currently Covered at developer.workfront.com )

1. In the new repository, locate the discovered documents and folders by path and lookup their identity in that external system. 

1. Create a mapping of the internal Workfront ID, to the ID in the new external store. You need this to create a new link.

1. Create a new document or document folder link in Workfront that points to the resource in its new location, via its new external id.

    1. **Documents**: Add a new version of the existing document with the new external document provider:

        Link **Documents (DOCU)** from **External Document Provider** of **providerType** with **documentProviderID**.

        >[!IMPORTANT]
        >
        >Documents are temporally stored. Meaning, you have all versions of the document. When you link from, we can specify the existing document ID, so that we are simply writing a new version to that document, with the data being hosted externally, in the new provider. This document id would be the same as the document id found on the document link we are replacing. It's the same conceptual document. We are simply indicating that the bytes for this new version are stored with a different provider.

        ```
        Http Method: POST
        
        Endpoint: {host}/internal/documents/linkExternalObjects
        
        Http Body:
        refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}

        ```

        API DOCS: (Internal Link Endpoints Not Currently Covered at developer.workfront.com)

    1. **Folders**: Create a new folder in the same place with the same name, then disable the old Workfront provider to filter out old links once complete.
        Link **Document Folders (DOCFDR)** from **External Document Provider** of **providerType** with **documentProviderID**.

        

        >[!IMPORTANT]
        >
        >For folder links , unlike Document links, we need the 'documentFolderId' of the folder in workfront we want to place our new link into. This would be the same parent folder, most likely as the linked folder we are copying. Also of note, folders are not temporally stored. We will create a new folder and then simply disable the old folder when we disable the prior document provider.

        ```
        Http Method: POST
        
        Endpoint: {host}/internal/document/version/linkExternal
        
        Http Body:
        providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}

        ```

        API DOCS: (Internal Link Endpoints Not Currently Covered at developer.workfront.com)

>[!IMPORTANT]
>
>When changing folder links, it's not advisable to delete the old linked folder, in an automated way after linking as this would not be recoverable. If done at scale, the loss of data could be significant. Simply disable the old provider to remove the old folder links from the Workfront application view.

Also, for documents, we are adding a new version to the existing document, so there again, a delete would not be part of the process.

## Example process for migrating links

![simplified-link-flow](assets/links-flow-simplified.png)

## APIs involved

For more information on the Workfront APIs in this section, see [Developer Documentation:Documents](https://developer.workfront.com/documents.html).

### Find all documents

Find All **Documents (DOCU)** Linked to **Document Provider** of **providerType** with **documentProviderID**.

[API DOCS reference](https://developer.workfront.com/documents.html#get-/docu/search)

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}

```

### Find all folders

Find All **Document Folders (DOCFDR)** Linked to Document Provider of **providerType** with **documentProviderID**.

API DOCS: (Document Folder Endpoints Not Currently Covered at developer.workfront.com )

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}

```

### Link documents

Link **Documents (DOCU)** from **External Document Provider** of **providerType** with **documentProviderID**.

API DOCS: (Internal Link Endpoints Not Currently Covered at developer.workfront.com)

>[!IMPORTANT]
>
>Documents are temporally stored. Meaning we have all versions of the document. When we do the link from, we can specify the existing document id, so that we are simply writing a new version to that document, with the data being hosted externally, in the new provider.  This document id would be the same as the document id found on the document link we are replacing. It's the same conceptual document. We are simply indicating that the bytes for this new version are stored with a different provider.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}

```

### Link folders

Link **Document Folders (DOCFDR)** from **External Document Provider** of **providerType** with **documentProviderID**.

API DOCS: (Internal Link Endpoints Not Currently Covered at developer.workfront.com)

>[!IMPORTANT]
>
>For folder links , unlike Document links, we need the 'documentFolderId' of the folder in workfront we want to place our new link into. This would be the same parent folder, most likely as the linked folder we are copying. Also of note, folders are not temporally stored. We will create a new folder and then simply disable the old folder when we disable the prior document provider.

```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}

```

## Important terms

* **Document**: A digital asset within Workfront

* **Document Folder**: A container for digital assets within Workfront

* **Document ID**: Workfront internal id for a digital asset

* **Document Folder ID**: Workfront internal id for a digital asset folder

* **Document Provider ID**

   This is important to note. For any given Document Provider Type, a customer may have multiple connected instances. They may have multiple AEM Repositories linked for example. Or multiple Google One Drive instances linked.  The id indicates the specific instance of the connection type we want to replace or switch to.

* **Document Storage Provider Type (also "External Integration Type")**: This is a type of document storage provider integration that we support. Either via a dedicated integration or a "custom integration". 

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

* **Linked Document**: A digital asset hosted externally, in an external document storage provider. Workfront will have its own internal "Document Id' for the asset, but the bytes are stored externally. To facilitate this, Workfront also stores an "external document id" to assist with locating the externally referenced resource within the remote repository or store.

* **Linked Document Folder**: A container for digital assets hosted externally, in an external document storage provider. Workfront will have its own internal "Document Folder Id' for the asset, but the bytes are stored externally. To facilitate this, Workfront also stores an "external document id" to assist with locating the externally referenced resource within the remote repository or store.

* **External Document ID**: When assets are stored outside of workfront. Workfront maps its internal identifier, to the identifier used to locate the asset in the external system, via this "external document identifier" field. Therefore, when linking the document or folder from a new external store, a new external document identifier must be composed, in the appropriate format for the external document provider to identify the document in the new repository or store. 

    >[!NOTE]
    >
    > It's important to note that workfront does not yet have a standard for external document identifiers. A new spec is being used for AEM ids, but for other ids the external document id may take on different forms depending on the provider type.


* **Object Type**: This is an API only term for the purposes of this document. it's a type of generic object within workfront that we wish to interact with. In our cases we'll be interacting with documents and folders having the types "DOCU" and "DOCFDR" respectively. 

* **Object ID**: The internal Workfront identifier for the generic object we wish to interact with. Again in this case we will be interacting with documents and folders so this will be either the document ID or document folder ID respectively.