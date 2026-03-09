---
product-area: documents
navigation-topic: approvals
title: Adobe enterprise storage overview
description: Adobe enterprise storage overview
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
---
# Adobe enterprise storage overview

Adobe enterprise storage is a cloud-based storage solution that serves as the central repository for assets across Adobe enterprise products. The Workfront and Frame.io integration is built on Adobe enterprise storage, enabling seamless collaboration and asset management between these platforms. it also alters the existing workfront document experience.

This also paves the way for future asset management integrations with other Adobe products, such as Adobe Creative Cloud. 

## Key Features

* **Unified storage layer**: Adobe enterprise storage acts as a shared storage backend for Workfront, Frame.io, Document Cloud, and Creative Cloud. This enables seamless collaboration and asset management across these platforms.

* **Content supply chain enablement**: Adobe enterprise storage is a foundational component for Adobe's Content Supply Chain vision, allowing teams to manage work-in-progress assets without the need for manual downloads or reupload in various Adobe applications.

* **Centralized permissions and access**: Adobe enterprise storage supports enterprise-level access controls, integrating with Adobe IMS (Identity Management System) for secure and scalable user permissions.

* **End-to-end asset visibility**: Assets stored in Adobe enterprise storage can be surfaced and managed directly in Workfront, Frame.io, and Creative Cloud apps, providing consistent metadata, versioning, and audit trails.

* **Integration with review and approval workflows**: Adobe enterprise storage enables creative review and approval workflows by serving as the source of truth for all assets, ensuring that feedback and approvals are tracked centrally.

* **Scalable storage and quota management**: Adobe enterprise storage offers scalable storage options and unified quota tracking across Adobe products.

## Integration with review and approval workflows

The Workfront and Frame.io integration leverages Adobe enterprise storage to provide a unified review and approval experience. This integration allows project coordinators to manage projects and plan work in Workfront while creatives, marketers, and stakeholders can review and approve assets in Frame.io. This ensures that all stakeholders have access to the latest versions of assets, and feedback is centralized in one place.

For more information about the Workfront and Frame.io integration, see [Frame.io integration overview](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md).

## Differences between Adobe enterprise storage and legacy Workfront storage

Naming conventions for projects, tasks, and issues are different in Adobe enterprise storage than in legacy Workfront storage.

### Documents

#### New documents area

The new documents area is a unified documents area that allows users to manage and view documents across all projects, tasks, and issues. It is accessed by clicking **Documents** in the left panel while viewing a project, task, or issue.

For more information about the new documents area, see [The Documents area](/help/quicksilver/documents/managing-documents/documents-area.md).


#### New document permission model

In Adobe enterprise storage, document permissions work differently than in legacy Workfront storage. Documents use a binary permission model: you either have Manage access or no access. The traditional View and Contribute permission levels no longer apply to documents. Instead, the system automatically generates a folder for each task or issue and inherits permissions from the task or issue.

At the project level, system-generated folders display a linked object. This is usually the task or issue name and is how the system knows which task or issue the folder should be seen on.

For more information about the new document permission model, see [Object permissions and access level overview for the Adobe enterprise storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).


## Projects 

| Adobe enterprise storage | Legacy Workfront storage |
|---|---|
| <ul><li>Uses Adobe enterprise storage</li><li>Integrated with Frame.io</li><li>Uses the new Documents experience</li><li>Enforces strict naming conventions</li><li>Direct document sharing isn't available</li><li>Shares document storage between Frame.io and Creative Cloud</li></ul> | <ul><li>Uses Workfront storage</li><li>Uses the proofing viewer</li><li>Supports individual document sharing</li></ul> |



### move share copy

move/share/copy - can only do with like storage models
Linked folders dictate document sharing for tasks and issues


## Enable Adobe enterprise storage

Customers who meet xyz criteria can enable Adobe enterprise storage. they can choose between esm only or a combination of esm and legacy workfront storage.

All legacy workfront projects remain on legacy workfront storage and retain all their existing features and functionality.


Some environments can choose to use Adobe enterprise storage or legacy Workfront storage
Configure storage preferences in setup