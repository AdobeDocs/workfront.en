---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Linked folders are not supported for DOCU object
description: Linked folders are not supported for DOCU object
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
TQID: https://experienceleague.adobe.com/iPjiffn9QLDldjWRdxMyf8RTaZaB9X6axc7UVY1B3Bg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
    internal-label: APIs
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
---
# Using the API to add a linked folder is not supported

Using the API to add a linked folder to the folders array for a Document (DOCU) object is not supported. The request will be successful, but the document may be removed from the system by some external providers. This is because the external system will be used as the final source of truth. Therefore, if the document is removed from the external provider, the document is considered to no longer exist. Any documents not found in the linked (external) folder may be removed automatically from [!DNL Workfront] with no way to recover them.
