---
product-area: documents
navigation-topic: documents-navigation-topic
title: Content credentials in Adobe Workfront
description: Learn what content credentials are and how Adobe Workfront preserves them on the documents you upload, store, and download.
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
# Content credentials in Adobe Workfront

Content credentials are secure, tamper-evident metadata that travel with a piece of content. When generative AI (GenAI) is used to create or alter an image, video, or audio file, content credentials record that fact so that anyone who receives the file can see how it was made.

Content credentials are based on the open [C2PA](https://c2pa.org/) standard.

## Why content credentials matter

Regulations such as California's AI Transparency Act (SB 942) and the European Union's AI Act require that content created or altered with GenAI be labeled with this kind of provenance information. Adobe automatically attaches content credentials to GenAI-created image, video, and audio produced in its GenAI products so that this information stays with the content wherever it goes.

## What a content credential contains

A content credential includes:

* The name of the provider that supplied the GenAI tool.
* The name and version number of the GenAI system used to create or alter the content.
* The date and time the content was created or altered.
* A unique identifier.

Content credentials do not include any personally identifiable information (PII).

## How Workfront handles content credentials

Adobe Workfront does not modify the metadata of the documents you work with. When you upload a document that already carries content credentials, Workfront preserves that information unchanged as the document is stored in and downloaded from Workfront.

Because the credentials are embedded in the file itself, they remain intact through your Workfront workflows, so the provenance information stays with the content when it leaves Workfront.