---
product-area: documents
navigation-topic: approvals
title: What's different on Adobe cloud storage
description: Understand the major differences on Adobe cloud storage objects, including the new Documents area, the Frame.io viewer, document permissions, object naming rules, storage quota, and Workfront Fusion.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
---
# What's different on Adobe cloud storage

With Adobe cloud storage, your environment can contain two types of objects: objects on legacy Workfront storage (the objects you have today) and objects created using Adobe cloud storage. The new Documents area, the Frame.io viewer, and the other behaviors described here apply only to objects that use Adobe cloud storage.

For an orientation to the move, see [Move to Workfront on Adobe cloud storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Understand legacy Workfront storage and Adobe cloud storage

At a high level, the two storage models differ in where the data lives, which Adobe products can see it, and what functionality is available:

|  | Object on legacy Workfront storage | Object on Adobe cloud storage |
|---|---|---|
| Storage backend | Workfront only | Adobe cloud storage |
| Cross-product visibility | Workfront only | Workfront, Frame.io, and Creative Cloud |
| Functionality | Legacy functionality | New functionality |

Objects created before Adobe cloud storage is the default remain on legacy Workfront storage. The behaviors described in this article apply only to Adobe cloud storage objects that you and your users create once Adobe cloud storage is the default.

## Summary of differences

The biggest day-to-day change with Adobe cloud storage is the new Documents area and the Frame.io viewer that powers review and approval inside it. There are other differences that affect how you manage objects, documents, and reviews. Each area in the following table links to the detailed section below.

| Area | What's different | What to know |
|---|---|---|
| [The new Documents area](#the-new-documents-area) | A redesigned, unified Documents area replaces the legacy Documents area. | There's no global Documents area. You access documents from a program, portfolio, project, task, or issue.|
| [Document permissions](#document-permissions) | Documents inherit permissions from the project, task, or issue they're linked to. | You can't share or set permissions on individual documents. You manage all access through the object Share modal in Workfront, which cascades to system-generated document folders.|
| [Object permissions mapping](#object-permissions-mapping) | Manage and Contribute permissions both map to Edit & Share in Frame.io. View maps to Comment Only. | You manage permissions in Workfront. Both Manage and Contribute users gain external sharing capability in Frame.io. |
| [Review and approval viewer](#review-and-approval-viewer) | The Frame.io viewer replaces the Workfront Proofing viewer. | It's included for all Workfront users, including External users assigned to a review or approval. It supports markup, time-stamped comments, version history, mobile, 40+ formats, and files up to 500 GB. |
| [Object naming rules](#object-naming-rules) | Strict naming rules apply: unique names within a portfolio or project, no special characters, no trailing period or space, and a 255-character limit. | Workfront automatically renames objects when conflicts arise. Audit the templates that generate new project names and structure. |
| [Object portability](#object-portability) | In most scenarios, you can move, copy, and convert objects only between like storage models. | You can convert a legacy object to Adobe cloud storage in three specific cases. Documents and document folders don't move from legacy storage during conversion. |
| [Capabilities not available](#capabilities-not-available-on-adobe-cloud-storage-objects) | Workfront Proof, the Workfront document viewer, favorite documents, and request documents aren't part of the experience. | Legacy objects retain these capabilities. Workfront Proof won't receive new investment and will be retired in a future release. |
| [Storage quota](#storage-quota) | Storage is pooled for legacy Workfront projects and Adobe cloud storage projects, at 60 GB per licensed user with no hard cap. | System administrators can view storage usage on the Customer Info page in Setup.|
| [Annual video review cap](#annual-video-review-cap) | There's an organization-level cap on video proof requests at 10% of paid Workfront user licenses (Standard and Light). | Once you reach the cap, you can't create new video reviews until the next annual period. You receive in-app notifications at 80% and 100%. The cap doesn't apply to Frame.io Enterprise customers. |
| [Workfront Fusion](#workfront-fusion-on-adobe-cloud-storage-projects) | Existing proof-based Fusion scenarios don't automatically work against Adobe cloud storage projects. | Scenarios scoped to legacy projects continue to work. Each affected scenario takes one of three paths: edit, rebuild, or retire. |

## The new Documents area

The new Documents area is a unified documents experience designed for Adobe cloud storage. It simplifies navigation, consolidates review and approval activity, and is the entry point for the Frame.io viewer.

The global Documents area isn't part of the new experience. On Adobe cloud storage projects, you access documents from a program, portfolio, project, task, or issue.

For more information, see [The Documents area](/help/quicksilver/documents/managing-documents/documents-area.md).

## Document permissions

Document permissions are fundamentally different on Adobe cloud storage projects:

* You can't share or set permissions on individual documents. Instead, permissions are applied to the system-generated document folders that contain the documents.
* System-generated document folders inherit permissions from their parent project, task, or issue.
* Subfolders inherit permissions from the parent system-generated document folder.
* Subtasks don't inherit permissions from parent tasks. You must be added directly to a subtask to access its system-generated document folder.

For more information about how document permissions work, see [Object permissions and access level overview for the Adobe cloud storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Object permissions mapping

Permissions are set in Workfront and flow in one direction through to Frame.io. You can't invite users to an Adobe cloud storage project in Frame.io or modify user permissions in Frame.io.

>[!TIP]
>
>Train project coordinators that Frame.io access is a downstream reflection of Workfront permissions. If a stakeholder reports they can't access a review on an Adobe cloud storage project, the fix is in Workfront, not Frame.io.

The following table maps Workfront object permissions to Frame.io permissions:

| Workfront permission | Frame.io permission |
|---|---|
| Manage | Edit & Share |
| Contribute | Edit & Share |
| View | Comment Only |

Both Manage and Contribute map to Edit & Share in Frame.io. As you review your sharing patterns for Adobe cloud storage projects, consider whether it fits your governance model for contributors to have the same review-side capabilities as managers, including external sharing.

For more information, see [Object permissions and access level overview for the Adobe cloud storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio).

## Review and approval viewer

On Adobe cloud storage objects, the Frame.io viewer is the review and approval surface in place of Workfront Proof. The Frame.io viewer is included for all Workfront users at no additional cost, including External users who are assigned to a review or approval.

The Frame.io viewer provides:

* Markup and commenting tools, including freehand drawing and standard shapes such as circles, arrows, and squares
* Time-stamped comments with frame-accurate precision for video reviews
* Version history and version comparison
* Mobile access for on-the-go reviews and approvals
* Support for over 40 file formats, including all common video, image, audio, PDF, and Microsoft Office types, with native playback for professional video formats such as ProRes, H.265, and DNxHD, and support for files up to 500 GB

## Object naming rules

Adobe cloud storage enforces strict naming and structural rules to keep the storage layer consistent across Adobe products. These rules apply to objects you create on Adobe cloud storage projects. Existing legacy projects keep their current names.

The following rules apply to Adobe cloud storage projects:

| Rule | Detail |
|---|---|
| Unique program and project names | Programs and projects can't have the same name if they belong to the same portfolio. |
| Unique document names | Documents can't have the same name if they belong to the same project. Document names must be unique within the same parent in the folder hierarchy. |
| Prohibited characters | Programs, portfolios, projects, templates, tasks, issues, document folders, and documents can't contain any of the following special characters: `\ / : * ? " \| < >` |
| Trailing characters | Programs, portfolios, projects, templates, tasks, issues, and document folders can't have names that end with a period or a space. |
| Name length limit | Object names are limited to 255 characters. |

If a name conflicts with these rules, Workfront automatically renames the object to resolve the conflict.

>[!TIP]
>
>If you create Adobe cloud storage projects from templates, review your existing templates so the project names and structure they generate fit the rules above.

## Object portability

In most scenarios, you can move, copy, and convert Workfront objects only between like storage models. For example, you can move a task from one Adobe cloud storage project to another Adobe cloud storage project. In three specific cases, you can convert a legacy Workfront storage object to Adobe cloud storage.

For more information, see [Convert legacy objects to Adobe cloud storage](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md).

## Capabilities not available on Adobe cloud storage objects

The following capabilities aren't part of Adobe cloud storage objects:

* Workfront Proof
* The Workfront document viewer
* Favorite documents
* Request documents

Legacy projects retain access to Workfront Proof and the legacy document capabilities listed above. Workfront Proof won't receive new investment going forward and will be retired in a future release.

## Storage quota

Storage is pooled for legacy Workfront objects and Adobe cloud storage objects. Each licensed user receives 60 GB of storage. There's no hard cap on storage usage, but Workfront administrators receive email notifications when usage reaches 75%, 90%, and 100% of the quota.

To view current storage usage and quota, go to **Setup** > **System** > **Customer Info**.

For more information, see [Check document storage limits](/help/quicksilver/documents/managing-documents/check-document-storage.md).

## Annual video review cap

There's an annual cap on video proof requests set at 10% of your organization's total paid Workfront user licenses (Standard and Light). This cap is applied at the organization level.

* Workfront administrators receive in-app notifications when usage reaches 80% and 100% of the cap.
* Once you reach the cap, you can't create new video review requests until the next annual period.
* This limit doesn't apply to Frame.io Enterprise customers. If your organization regularly reviews large volumes of video content, contact your Adobe account representative to learn about Frame.io Enterprise licensing.

For more information, see the Reviewing and approving assets and videos FAQ in [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Workfront Fusion on Adobe cloud storage projects

Existing Workfront Fusion scenarios built on legacy proofing don't automatically work against Adobe cloud storage projects. Proof-specific modules, webhooks, and API endpoints have direct equivalents in some cases and significant changes in others. Scenarios scoped to legacy projects continue to work as they do today.

For detailed information about the impact on common scenario types and how to classify each scenario as Edit, Rebuild, or Retire based on its functionality, see [Update Workfront Fusion scenarios for unified review and approval](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).
