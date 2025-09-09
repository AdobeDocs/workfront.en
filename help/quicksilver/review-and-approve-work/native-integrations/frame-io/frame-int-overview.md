---
product-area: documents
navigation-topic: approvals
title: Frame.io integration overview
description: Frame.io integration overview
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog

---

# Frame.io integration overview

The Workfront and Frame.io integration allows project coordinators to manage projects and plan work in Workfront while creatives, marketers, and stakeholders can review and approve assets in Frame.io.

## Built on Adobe Enterprise Storage Management

At the core of this integration is Adobe Enterprise Storage Management (ESM)—a cloud-based storage solution that serves as the central repository for assets across Adobe enterprise products, including Workfront and Frame.io.

Key benefits of Adobe Enterprise Storage Management include:

* Unified storage layer for creative and work management assets
* Centralized permissions via Adobe IMS for secure access control
* End-to-end asset visibility across Workfront, Frame.io, and Creative Cloud apps <!--coming soon?-->
* Scalable storage and quota management for enterprise needs

For more details, see [Adobe Enterprise Storage overview]. <!--coming soon?-->

## Unified review and approval 


### Unified approval management in Workfront

details about unified approvals 



### Use the Frame.io viewer

The integration supports a unified review and approval workflow with the Frame.io viewer. The Frame.io viewer provides

* Markup and commenting tools
* Version history and audit trails
* Mobile access for on-the-go reviews and approvals

For more information, see [Get started with the Frame.io integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

Documents experience

Documents must have unique names within the same project due to ESM hierarchy rules.
Auto-renaming is applied to prevent naming conflicts.

Document access is managed at the project level.


The Frame.io viewer supports all common video, image, audio, PDF, and MS Office types. For a detailed list of supported files, see [Types on Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

Video, image, audio, PDF, and Microsoft Office file types
→ https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io



## Powerful project management in Workfront

### naming

Naming conventions are specific and can't be duplicated
ESM requires unique names for peer objects with the same parent in  the hierarchy tree.
Documents can't have the same name if they belong to the same project
Solution: Auto renames the object or document

### Document management 

Naming conventions are specific and can't be duplicated
ESM requires unique names for peer objects with the same parent in  the hierarchy tree.
Documents can't have the same name if they belong to the same project
Solution: Auto renames the object or document

Document sharing
Share doc access at the project level

can't drag full folders

### Additional functionality available with Frame.io enterprise licenses

The Frame.io enterprise license includes additional functionality for organizations, such as:

* Accessing Frame.io from the Workfront interface
* Projects created in Workfront are also visible in Frame.io
* Assets uploaded in Frame.io are visible in Workfront







Maybe this needs to be a list in a separate doc when existing customers move over?

## Limitations/Considerations 

### Projects

stuff here 

### Documents 

* Documents can't have the same name if they belong to the same project
* Documents can't be added to tasks or issues
* Documents access is handled at the project level
* no external doc providers
* No favorite docs
* No requesting docs
* No sending to AEM
* No access to proofing
* No multi-stage approvals
* no uploading docs to comments or updates 















ESM Article: 

Key Features:
Unified Storage Layer:
ESM acts as a shared storage backend for Workfront, Frame.io, Document Cloud, and Creative Cloud. This enables seamless collaboration and asset management across these platforms.

Content Supply Chain (CSC) Enablement:
ESM is a foundational component for Adobe's Content Supply Chain vision, allowing teams to manage work-in-progress (WIP) assets without the need for manual downloads or reuploads.

Centralized Permissions & Access:
ESM supports enterprise-level access controls, integrating with Adobe IMS (Identity Management System) for secure and scalable user permissions.

End-to-End Asset Visibility:
Assets stored in ESM can be surfaced and managed directly in Workfront, Frame.io, and CC apps, providing consistent metadata, versioning, and audit trails.

Integration with Review & Approval Workflows:
ESM enables creative review and approval workflows by serving as the source of truth for all assets, ensuring that feedback and approvals are tracked centrally.

Scalable Storage & Quota Management:
ESM offers scalable storage options and unified quota tracking across Adobe products.