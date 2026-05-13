---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Document name changed after upload and contains an invalid character
description: Certain documents cannot be converted to proofs.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
TQID: https://experienceleague.adobe.com/bE5iUIG7rFpIIa3zXt-5pO0sgfbEO-3QDVFVLwkayIo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
---
# Document name changed after upload and contains an invalid character

## Problem

Certain documents cannot be converted to proofs.

## Cause

Files that are uploaded to Workfront cannot contain certain characters in file names. If a file contains any of the following characters in the file name, the characters are removed from the file name when the file is uploaded: `! # % * \ | ' " / ? < > { } [ ]`.

If a Document name is updated to include an invalid character after the initial upload, the proof generation will fail. 

## Solution

Remove the invalid character from the document name:

1. Select the document, then click **Document Details**.
1. Click on the document name and remove the invalid character, and press Enter.
    
    Invalid charaters: `! # % * \ | ' " / ? < > { } [ ]`

    ![Document name](assets/doc-name.png)

1. Refresh the page, and generate the proof.
