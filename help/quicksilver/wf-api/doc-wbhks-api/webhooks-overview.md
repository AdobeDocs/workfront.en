---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhooks Overview
description: Webhooks Overview
author: Becky
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
---

# Webhooks Overview

Adobe Workfront Document Webhooks defines a set of API endpoints through which Workfront makes authorized API calls to an External Document Provider. This allows anyone to create a middleware plugin for any document storage provider.

![](assets/mceclip0-350x262.png)

The user experience for webhook-based integrations will be similar to that of existing document integrations, such as Google Drive, Box, and Dropbox. For example, a Workfront user will be able to perform the following actions:

* Navigate the folder structure of the external document provider
* Search files
* Link files into Workfront
* Upload files to the external document provider
* View a thumbnail for the document

**Reference Implementation**

To help jumpstart the development of a new webhooks implementation, Workfront provides examples of a reference implementation. These exampless can be found at [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). The examples are Java-based and allow Workfront to connect documents on a network file system.&nbsp;

>[!NOTE]
>
>The resources on GitHub are examples only, and are not able to execute an implementation.

## Versions

* Version 1.0 (Release Date - May, 2015): Initial Specification

* Version 1.1 (Release Date - June, 2015). Updated /uploadInit - Added documentId and documentVersionId

* Version 1.2 (Release Date - October, 2015): Added /createFolder

* Upcoming versions (Release Date - TBD):

  * Added /delete
  * Added /rename
  * Added /serviceInfo
  * Added /customAction
  * Add pagination and parentId to /search
