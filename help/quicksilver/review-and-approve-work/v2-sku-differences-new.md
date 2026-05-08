---
product-area: documents
navigation-topic: approvals
title: Move to Workfront on Adobe enterprise storage
description: Plan your rollout of Workfront on Adobe enterprise storage. Learn what's different on Adobe enterprise storage objects, including the new Documents area and the Frame.io review experience, and decide how Adobe enterprise storage rolls out in your environment.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
---
# Move to Workfront on Adobe enterprise storage

Workfront on Adobe enterprise storage enables the full Unified Review and Approval experience: reviews in the Frame.io viewer, powerful approval workflows, cross-product visibility of assets, and more.

Your existing objects continue to work the way they do today. The new Documents area, the Frame.io viewer, and other Adobe enterprise storage behaviors apply to objects using Adobe enterprise storage only.

This article is for Workfront administrators preparing to roll out Workfront on Adobe enterprise storage. It covers major differences on Adobe enterprise storage objects, how to choose your rollout type, and what to think through before you enable Adobe enterprise storage for your users.


## Understand legacy Workfront storage and Adobe enterprise storage

After your contract is updated to include the new Unified Review and Approval Experience, your environment can contain two types of objects: objects on legacy Workfront storage (the objects you have today) and new objects on Adobe enterprise storage. At a high level, the two storage models differ in where the data lives and which Adobe products can see it:

| Capability | Object on legacy Workfront storage | Object on Adobe enterprise storage |
|---|---|---|
| Storage backend | Workfront only | Adobe enterprise storage |
| Cross-product visibility | Workfront only | Workfront, Frame.io, and Creative Cloud |

Objects created before Adobe enterprise storage is enabled in the Setup area remain on legacy Workfront storage. The new behaviors described in this article apply only to Adobe enterprise storage objects you and your users create once Adobe enterprise storage is enabled.

## What's different with Adobe enterprise storage 

The biggest day-to-day change with Adobe enterprise storage is the new Documents area and the Frame.io viewer that powers review and approval inside it. But there are other differences that impact how you manage objects, documents, and reviews. 

The following table summarizes the major differences when switching to Adobe enterprise storage. Each area in the table links to the detailed section below.

| Area | What's different | What to know |
|---|---|---|
| [The new Documents area](#the-new-documents-area) | A redesigned, unified Documents area replaces the legacy Documents area. | No global Documents area. Access documents from a program, portfolio, project, task, or issue.|
| [Document permissions](#document-permissions) | Documents inherit permissions from the project, task, or issue they're linked to. | You can't share or set permissions on individual documents. Users manage all access through the object Share modal in Workfront, which cascades to system-generated documentfolders.|
| [Object permissions mapping](#object-permissions-mapping) | Workfront's Manage and Contribute permissions both map to Edit & Share in Frame.io. View maps to Comment Only. | Permissions are managed in Workfront. Both Manage and Contribute users gain external sharing capability in Frame.io. |
| [Review and approval viewer](#review-and-approval-viewer) | The Frame.io viewer replaces the Workfront Proofing viewer. | Included for all Workfront users with a paid license. Supports markup, time-stamped comments, version history, mobile, 40+ formats, files up to 500 GB. |
| [Object naming rules](#object-naming-rules) | Strict naming rules apply: unique names within a portfolio or project, no special characters, no trailing period or space, 255-character limit. | Workfront auto-renames objects when conflicts arise. Audit templates that generate new project names and structure. |
| [Object portability](#object-portability) | You can move, copy, and convert objects only between like storage models. | Adobe enterprise storage objects can't move to legacy projects, or the reverse. Moving an Adobe enterprise storage project to a legacy portfolio or program converts the parent to Adobe enterprise storage. |
| [Capabilities not available](#capabilities-not-available-on-adobe-enterprise-storage-objects) | Workfront Proof, the Workfront document viewer, favorite documents, and request documents aren't part of the experience. | Legacy objects retain these capabilities. Workfront Proof won't receive new investment and will be retired in a future release. |
| [Storage quota](#storage-quota) | Storage is pooled for legacy Workfront projects and Adobe enterprise projects. 60 GB per licensed user. No hard cap. | System admins can view storage usage on the Customer Info page in Setup.|
| [Annual video review cap](#annual-video-review-cap) | Organizational-level cap on video proof requests at 10% of paid Workfront user licenses (Standard + Light combined). | Once reached, no new video reviews until the next annual period. In-app notifications at 80% and 100%. Doesn't apply to Frame.io Enterprise customers. |
| [Workfront Fusion](#workfront-fusion-on-adobe-enterprise-storage-projects) | Existing proof-based Fusion scenarios don't automatically work against Adobe enterprise storage projects. | Scenarios scoped to legacy projects continue to work. Each affected scenario gets one of three paths: edit, rebuild, or retire. New connectors expected Q3 2026. |

### The new Documents area

The new Documents area is a unified documents experience designed for Adobe enterprise storage. It simplifies navigation, consolidates review and approval activity, and is the entry point for the Frame.io viewer.

The global Documents area isn't part of the new experience. On Adobe enterprise storage projects, you access documents from a program, portfolio, project, task, or issue.

For more information, see [The Documents area](/help/quicksilver/documents/managing-documents/documents-area.md).

### Document permissions

Document permissions are fundamentally different on Adobe enterprise storage projects: 

* You can't share or set permissions on individual documents. Instead, permissions are applied to system-generated document folders that contain the documents.
* System-generated document folders inherit permissions from their parent project, task, or issue.
* Subfolders inherit permissions from the parent system-generated document folder.
* Subtasks don't inherit permissions from parent tasks. You must be added directly to a subtask to access its system-generated document folder.


For more information about how document permissions work, see [Object permissions and access level overview for the Adobe enterprise storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).


### Object permissions mapping

Permissions are set in Workfront and flow in one direction through to Frame.io. You can't invite users to an Adobe enterprise storage project in Frame.io or modify user permissions in Frame.io.

>[!TIP]
>
>Train project coordinators that Frame.io access is a downstream reflection of Workfront permissions. If a stakeholder reports they can't access a review on an Adobe enterprise storage project, the fix is in Workfront — not Frame.io.

The following table maps Workfront object permissions to Frame.io permissions:

| Workfront permission | Frame.io permission |
|---|---|
| Manage | Edit & Share |
| Contribute | Edit & Share |
| View | Comment Only |

Both Manage and Contribute map to **Edit & Share** in Frame.io. As you review your sharing patterns for Adobe enterprise storage projects, consider whether contributors having the same review-side capabilities as managers, including external sharing, fits your governance model.

For more information, see [Object permissions and access level overview for the Adobe enterprise storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio).


### Review and approval viewer

On Adobe enterprise storage objects, the Frame.io viewer is the review and approval surface in place of Workfront Proof. The Frame.io viewer is included for all Workfront users with a paid license.

The Frame.io viewer provides:

* Markup and commenting tools, including freehand drawing and standard shapes such as circles, arrows, and squares
* Time-stamped comments with frame-accurate precision for video reviews
* Version history and version comparison
* Mobile access for on-the-go reviews and approvals
* Support for over 40 file formats, including all common video, image, audio, PDF, and Microsoft Office types, with native playback for professional video formats such as ProRes, H.265, and DNxHD, and support for files up to 500 GB


### Object naming rules

Adobe enterprise storage enforces strict naming and structural rules to keep the storage layer consistent across Adobe products. These rules apply to objects you create on Adobe enterprise storage projects. Existing legacy projects keep their current names.

The following rules apply on Adobe enterprise storage projects:

| Rule | Detail |
|---|---|
| Unique program and project names | Programs and projects can't have the same name if they belong to the same portfolio. |
| Unique document names | Documents can't have the same name if they belong to the same project. Document names must be unique within the same parent in the folder hierarchy. |
| Prohibited characters | Programs, portfolios, projects, templates, tasks, issues, document folders, and document names can't contain any of the following special characters: `\ / : * ? " \| < >` |
| Trailing characters | Programs, portfolios, projects, templates, tasks, issues, and document folders can't have names that end with a period or a space. |
| Name length limit | Object names are limited to 255 characters. |

If a name conflicts with these rules, Workfront automatically renames the object to resolve the conflict.

>[!TIP]
>
>If you create Adobe enterprise storage projects from templates, review your existing templates so the project names and structure they generate fit the rules above.


### Object portability

You can move, copy, and convert Workfront objects between like storage models. For example, you can move a task from one Adobe enterprise storage project to another Adobe enterprise storage project. You can't move or copy a task or issue from an Adobe enterprise storage project to a legacy project, or the reverse.

Today, when you create or move an Adobe enterprise storage project to a legacy portfolio or program, the portfolio or program is automatically converted to an Adobe enterprise storage object. This functionality is being updated to provide more control for the system administrator over which objects can be automatically converted and will be available in a future release. 

### Capabilities not available on Adobe enterprise storage objects

The following capabilities aren't part of Adobe enterprise storage objects:

* Workfront Proof
* The Workfront document viewer
* Favorite documents
* Request documents

Legacy projects retain access to Workfront Proof and the legacy document capabilities listed above. Workfront Proof will not receive new investment going forward and will be retired in a future release.

### Storage quota

Storage is pooled for legacy Workfront objects and Adobe enterprise storage objects. Each licensed user receives 60 GB of storage. There's no hard cap on storage usage, but Workfront administrators receive email notifications when usage reaches 75%, 90%, and 100% of the quota.

System admins can go to **Setup** > **System** > **Customer Info** to view current storage usage and quota. 

For more information, see [Check document storage limits](/help/quicksilver/documents/managing-documents/check-document-storage.md).


### Annual video review cap

There's an annual cap on video proof requests set at 10% of your organization's total paid Workfront user licenses (Standard and Light). This cap is applied at the organization level.

* Workfront administrators receive in-app notifications when usage reaches 80% and 100% of the cap.
* Once the cap is reached, you can't create new video review requests until the next annual period.
* This limit doesn't apply to Frame.io Enterprise customers. If your organization regularly reviews large volumes of video content, contact your Adobe account representative to learn about Frame.io Enterprise licensing.

For more information, see the Reviewing and approving assets and videos FAQ in [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

### Workfront Fusion on Adobe enterprise storage projects

Existing Workfront Fusion scenarios built on legacy proofing don't automatically work against Adobe enterprise storage projects. Proof-specific modules, webhooks, and API endpoints have direct equivalents in some cases and significant changes in others. Scenarios scoped to legacy projects continue to work as they do today.

Fusion connectors with native support for unified review and approval are expected to be available in Q3 2026.

For detailed information about the impact on common scenario types and how to classify each scenario as Edit, Rebuild, or Retire based on its functionality, see [Update Workfront Fusion scenarios for unified review and approval](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).


## Choose how Adobe enterprise storage rolls out

You decide how Adobe enterprise storage appears to your users. There are two configurations, and either one can be applied to your entire organization or to specific Workfront groups.

* **Adobe enterprise storage only**: New projects use Adobe enterprise storage by default. Users can't create legacy projects.
* **Adobe enterprise storage and legacy Workfront storage**: When users create a project, they choose between Adobe enterprise storage (labeled "New project") and legacy Workfront storage (labeled "Legacy project").

For step-by-step instructions, see [Enable Adobe enterprise storage for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

>[!TIP]
>
>To put Adobe enterprise storage in front of a smaller team first, apply either configuration to a single Workfront group. This lets you run a targeted pilot before rolling out more broadly. We recommend starting with a group-level rollout for controlled pacing, then expanding to the entire organization once the pilot group has validated the experience.

Existing objects keep the storage model they were created with. Changing the default storage preference doesn't change any existing object. 

## Plan your rollout

Every Workfront environment is different. Before you enable Adobe enterprise storage for your users, take some time to plan what a successful rollout looks like for your organization. The suggestions below aren't a checklist, but a starting point for your own plan.

**1. Pick a pilot group.** A group-scoped rollout lets you put Adobe enterprise storage in front of a smaller team first, gather feedback, and adjust before broader rollout. Pick a group whose work patterns are representative enough to surface issues you want to know about early.

**2. Communicate the change to end users.** The biggest visible change for reviewers, approvers, and project owners is the new Documents area and the Frame.io viewer that powers review and approval on Adobe enterprise storage projects. Plan how you'll introduce these so users know what to expect when they encounter their first Adobe enterprise storage project. The [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) article is a useful starting point for end-user-facing material.

**3. Plan around Workfront Fusion connector availability.** Fusion connectors with native support for unified review and approval are expected to be available in Q3 2026. Existing proof-based Fusion scenarios continue to work on legacy projects. Before you bring teams that depend on those scenarios into your Adobe enterprise storage pilot, decide whether to wait for the new connectors, rebuild against the current API, or replace the scenario with native unified review and approval features. 

For detailed information about the impact on common scenario types and how to classify each scenario as Edit, Rebuild, or Retire based on its functionality, see [Update Workfront Fusion scenarios for unified review and approval](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).


## Related articles

* [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [Enable Adobe enterprise storage for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)
* [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [The Documents area](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Object permissions and access level overview for the Adobe enterprise storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)