---
product-area: documents
navigation-topic: documents-navigation-topic
title: C2PA metadata in Adobe Workfront
description: Learn what C2PA metadata is and how Adobe Workfront preserves it on the documents you upload, store, and download.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---
# C2PA metadata in Adobe Workfront

C2PA metadata is secure, tamper-evident information that travels with a piece of content. When generative AI (GenAI) is used to create or alter an image, video, or audio file, C2PA metadata records that fact so that anyone who receives the file can see how it was made.

C2PA metadata is based on the open [C2PA](https://c2pa.org/) standard.

## Why C2PA metadata matters

New laws are emerging around generative AI transparency, and Adobe is working to meet applicable requirements across jurisdictions. Adobe automatically attaches C2PA metadata to GenAI-created image, video, and audio produced in its GenAI products so that this information stays with the content wherever it goes.

## What C2PA metadata contains

C2PA metadata includes:

* The name of the provider that supplied the GenAI tool.
* The name and version number of the GenAI system used to create or alter the content.
* The date and time the content was created or altered.
* A unique identifier.

C2PA metadata does not include any personally identifiable information (PII).

## How Workfront handles C2PA metadata

Adobe Workfront does not modify the metadata of the files you work with. When you upload a file that already carries C2PA metadata, Workfront preserves that information unchanged as the file is stored in and downloaded from Workfront.

Because the metadata is embedded in the file itself, it remains intact through your Workfront workflows, so the provenance information stays with the content when it leaves Workfront.
