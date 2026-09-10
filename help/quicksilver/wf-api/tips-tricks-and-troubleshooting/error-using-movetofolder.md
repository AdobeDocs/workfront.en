---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Document moveToFolder action does not work
description: When using the Document moveToFolder action, a 422 error is returned.
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
TQID: https://experienceleague.adobe.com/UV4VnQEs-jGJau1UqXTLnp7Ak-cmKRpjuJqxgNTF5z8
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
# Document moveToFolder action does not work

## Problem

When using the Document object's `moveToFolder` action, a 422 error is returned.

Or

If using this action through the Adobe Authenticator module in Workfront Fusion, the document is not moved but there is no indication of the error. The error is the same, but the Adobe Authenticator module does not display it.

## Solution

One possible cause of a 422 error for this action is that the action is attempting to move a Document in one Linked Folder into another Linked Folder.

Check to ensure that the document you want to move is not already in a linked folder.
