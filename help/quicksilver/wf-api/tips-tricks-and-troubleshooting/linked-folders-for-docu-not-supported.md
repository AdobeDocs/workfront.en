---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Linked folders are not supported for DOCU object
description: Linked folders are not supported for DOCU object
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
---
# Using the API to add a linked folder is not supported

Using the API to add a linked folder to the folders array for a Document (DOCU) object is not supported. The request will be successful, but the document may be removed from the system by some external providers. This is because the external system will be used as the final source of truth. Therefore, if the document is removed from the external provider, the document is considered to no longer exist. Any documents not found in the linked (external) folder may be removed automatically from [!DNL Workfront] with no way to recover them.
