---
product-area: documents
navigation-topic: approvals
title: Differences on the Workfront V2 SKU
description: Learn what changes for Workfront administrators when your organization moves to a V2 Workfront SKU, including Adobe enterprise storage, the Frame.io viewer, naming conventions, permissions, Fusion impact, and rollout options.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
---
# Differences on the Workfront V2 SKU

The V2 Workfront SKU is the contract package that unlocks Adobe enterprise storage and unified review and approval for your Workfront organization. If your contract was signed before V2 Workfront SKUs were available, adding the V2 Workfront SKU requires a contracting event with Adobe, either at renewal or as an early recontract. There's no price increase when moving to an equivalent package. Contact your Adobe account representative to confirm your current SKU and discuss the path that fits your organization.

This article is for Workfront administrators planning a move from a legacy Workfront SKU to the V2 Workfront SKU. It summarizes the categories of change you can expect and links to the detailed help for each one:

* Storage architecture (legacy Workfront storage to Adobe enterprise storage)
* Storage quotas and the annual video review cap
* Review and approval surface (Frame.io viewer in place of Workfront Proof)
* Workfront Fusion scenarios built on legacy proofing
* Enforced naming conventions and project structure
* Permissions and how access flows from Workfront to Frame.io
* Rollout options for enabling Adobe enterprise storage

We recommend reviewing every section before you enable Adobe enterprise storage so you can plan a controlled rollout and audit existing assets, automations, and naming conventions in advance.

## Storage: Legacy Workfront storage to Adobe enterprise storage

The V2 Workfront SKU shifts your storage layer from Workfront-only storage to Adobe enterprise storage. Adobe enterprise storage is a cloud-based storage solution that serves as the central repository for assets across Adobe enterprise products, including Workfront and Frame.io. It's also the foundation for future asset management integrations with other Adobe products, such as Adobe Creative Cloud.

For a full description of Adobe enterprise storage, see [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

### Legacy Workfront storage compared to Adobe enterprise storage

The following table summarizes the main differences between the two storage models:

| Capability | Legacy Workfront storage | Adobe enterprise storage |
|---|---|---|
| Storage backend | Workfront only | Shared across Workfront, Frame.io, and Creative Cloud |
| Review viewer | Workfront Proofing viewer | Frame.io viewer |
| Document sharing | Share individual documents | Inherit from parent object only |
| Documents experience | Legacy Documents area | New Documents area |
| Cross-product visibility | Workfront only | Workfront, Frame.io, and Creative Cloud |
| Naming enforcement | Flexible | Strict |
| Object portability | Move between any projects | Adobe enterprise storage projects only |

### How projects, tasks, and issues behave differently

Once Adobe enterprise storage is enabled, your environment can contain both Adobe enterprise storage projects and legacy Workfront storage projects. Any objects created before Adobe enterprise storage was enabled remain on legacy Workfront storage. Net new environments have Adobe enterprise storage enabled by default and don't have a legacy Workfront storage option.

When you create an Adobe enterprise storage project, Workfront automatically creates a document folder with the same name as the project in the project's Documents section. After you add tasks or issues to the project, folders with the task or issue name are added to the Documents section of each task or issue. These system-generated folders inherit permissions from the task, issue, or project they're linked to, and any document uploaded to that object is stored in the matching folder.

### You can't move or copy objects between storage models

You can move, copy, and convert Workfront objects between like storage models. For example, you can move a task from one Adobe enterprise storage project to another Adobe enterprise storage project. You can't move or copy a task or issue from an Adobe enterprise storage project to a legacy Workfront storage project, or the reverse.

When you create or move an Adobe enterprise storage project to a legacy Workfront storage portfolio or program, the portfolio or program is automatically converted to an Adobe enterprise storage object.

### Document permissions move from document-level to object-level

In Adobe enterprise storage, document permissions work differently than in legacy Workfront storage. Documents inherit permissions from the project, task, or issue they're linked to, and you can't share or set permissions on individual documents.

* Tasks and issues inherit permissions from the project.
* System-generated folders inherit permissions from their linked task or issue.
* Subfolders inherit permissions from the parent folder.
* Subtasks don't inherit system-generated folder permissions from parent tasks. You must be added directly to a subtask to access its system-generated folder.

For more information, see [Object permissions and access level overview for the Adobe enterprise storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

### The new Documents area

The new Documents area is a unified documents experience redesigned for Adobe enterprise storage. It simplifies navigation, improves clarity, and consolidates review and approval activity.

The new Documents area is only available if your organization is on Adobe enterprise storage. The global Documents area isn't available in the new experience. Instead, you access documents from a program, portfolio, project, task, or issue.

For more information, see [The Documents area](/help/quicksilver/documents/managing-documents/documents-area.md).

### Sync caveats between Workfront and Frame.io

It's possible for Workfront to become out of sync with Frame.io or Creative Cloud. For example, an asset can be deleted in Workfront but still appear in Frame.io. If this happens, contact Workfront support to have your environment resynced.

## Storage quotas

The V2 Workfront SKU changes how storage quota is reported and adds an annual cap on video review requests.

### Document storage quota

With the V2 Workfront SKU, each licensed user receives 60 GB of storage, up from 30 GB on the previous version. The Customer Info page shows a Storage Overview section that breaks usage into legacy Workfront storage, Adobe enterprise storage, and Frame.io. Workfront also applies a soft cap to uploads when usage exceeds your quota, so users can still upload documents.

Workfront administrators automatically receive email notifications when storage usage reaches 75%, 85%, and 100% of the quota.

For more information, see [Check document storage limits](/help/quicksilver/documents/managing-documents/check-document-storage.md).

### Annual video review cap

There's an annual cap on video proof requests set at 10% of your organization's total paid Workfront user licenses (Standard and Light). This cap is applied at the organization level.

* Workfront administrators receive in-app notifications when usage reaches 80% and 100% of the cap.
* Once the cap is reached, you can't create new video review requests until the next annual period.
* This limit doesn't apply to Frame.io Enterprise customers. If your organization regularly reviews large volumes of video content, contact your Adobe account representative to learn about Frame.io Enterprise licensing.

For more information, see the Reviewing and approving assets and videos FAQ in [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Review and approvals: the Frame.io viewer replaces the Proofing viewer

When unified review and approval is enabled, the Frame.io viewer becomes the primary review surface in Workfront, replacing Workfront Proof. The Frame.io viewer is the default viewer for all Workfront review and approval workflows on Adobe enterprise storage projects, and it's automatically included for all Workfront users with a paid license. No additional Frame.io license is required.

### What's new in the Frame.io viewer

The Frame.io viewer provides:

* Markup and commenting tools, including freehand drawing and standard shapes such as circles, arrows, and squares
* Time-stamped comments with frame-accurate precision for video reviews
* Version history and version comparison
* Mobile access for on-the-go reviews and approvals
* Support for over 40 file formats, including all common video, image, audio, PDF, and Microsoft Office types, with native playback for professional video formats such as ProRes, H.265, and DNxHD, and support for files up to 500 GB

For a detailed list of supported files, see [Supported File Types on Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

### What's removed in Workfront

The following document capabilities aren't included on Adobe enterprise storage projects:

* Access to Proofing in Workfront
* Document viewer in Workfront
* Favorite documents
* Request documents

>[!NOTE]
>
>Existing customers retain access to Workfront Proofing functionality for any projects created before the integration was enabled.

For more information, see the following:

* [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)

## Fusion scenario changes

Existing Workfront Fusion scenarios built on legacy Workfront proofing won't automatically work with unified review and approval. Proof-specific modules, webhooks, and API endpoints have direct equivalents in some cases and significant changes in others. The impact varies depending on how each scenario is built:

* **Edit or update**: Scenarios where the existing proof-related action has a direct equivalent in unified approvals can be updated to use the new action.
* **Rebuild**: Scenarios where the underlying steps have changed significantly, or where new capabilities exist, may need to be rebuilt from scratch.
* **Retire**: Scenarios where native unified approvals functionality, such as multi-stage approval templates with deadline reminders, replaces what the scenario was built to do.

Fusion actions for unified review and approval are currently in development and are expected to be available in Q3 2026. A clearer picture of how each scenario maps to unified approvals will emerge once those Fusion APIs are available.

### Common scenario types and their expected impact

The following table maps common legacy proofing scenario types to their expected impact and path forward:

| Scenario type | Impact | Path forward |
|---|---|---|
| Proof creation and routing | Breaks | Rebuild using the unified approvals API |
| Proof status webhooks | Breaks | Rebuild with new approval event triggers |
| Document upload triggers | Partial: retest required | Audit and retest after migration |
| Approval reminder notifications | Breaks | Replace with approval template deadlines |
| Approval decision routing | Breaks | Rebuild using new decision status fields |
| Custom approval reporting | Partial: field names may change | Map legacy fields to the new schema |

### Recommended remediation approach

1. Inventory every Fusion scenario that touches Workfront proofing modules, webhooks, or proof-related API endpoints.
1. Classify each scenario as Edit, Rebuild, or Retire based on whether the new unified approvals capabilities can replace it.
1. Pause proof-dependent scenarios before you enable unified review and approval in production. Running stale proof-based automations against the new model can produce silent failures or duplicate actions.
1. Audit your scenarios against the new unified approvals capabilities once the Fusion connectors are available, and rebuild what's needed.

>[!TIP]
>
>Where a Fusion scenario exists only to route reviewers and approvers, evaluate whether a native Workfront approval template can replace it. Approval templates support reviewers, approvers, due dates, and multi-stage workflows directly in Workfront, with no automation to maintain.

For more information, see the following:

* Fusion and automation FAQ in [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Create an Approval Template for assets and documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

## Naming conventions and project structure

Because the V2 Workfront SKU is built on Adobe enterprise storage, Workfront enforces strict naming and structural rules. Audit your portfolios, programs, projects, templates, tasks, issues, document folders, and document names before you enable Adobe enterprise storage so you can resolve conflicts in advance.

The following rules apply on Adobe enterprise storage:

| Rule | Detail |
|---|---|
| Unique program and project names | Programs and projects can't have the same name if they belong to the same portfolio. |
| Unique document names | Documents can't have the same name if they belong to the same project. Document names must be unique within the same parent in the folder hierarchy. |
| Prohibited characters | Programs, portfolios, projects, templates, tasks, issues, document folders, and document names can't contain any of the following special characters: `\ / : * ? " \| < >` |
| Trailing characters | Programs, portfolios, projects, templates, tasks, issues, and document folders can't have names that end with a period or a space. |
| Name length limit | Object names are limited to 255 characters maximum. |

Workfront automatically renames objects or documents as needed to prevent conflicts.

For more information, see [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Permissions

User permissions are set and controlled in Workfront and flow one direction, through to Frame.io. You can't invite users to a project in Frame.io or modify user permissions in Frame.io. All access management for unified review and approval happens through the Project Share modal in Workfront.

### Workfront-to-Frame.io permission mapping

| Workfront permission | Frame.io permission |
|---|---|
| Manage | Edit & Share |
| Contribute | Edit & Share |
| View | Comment Only |

### External users

You can share assets externally. External Workfront users are notified by email when they're assigned to a review or approval, and they're prompted to create a Frame.io login to access the viewer and participate in the review.

For more information, see the following:

* [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Object permissions and access level overview for the Adobe enterprise storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)

## Rollout options

You can roll out Adobe enterprise storage in one of two configurations, and you can scope either configuration to specific Workfront groups for a controlled rollout.

* **Adobe enterprise storage only**: All new projects use Adobe enterprise storage by default.
* **Adobe enterprise storage and legacy Workfront storage**: Users can choose the storage provider when they create a project. Adobe enterprise storage is labeled as "New project" and legacy Workfront storage is labeled as "Legacy project."

>[!NOTE]
>
>Existing projects keep the storage model they were created with. For example, projects that use Adobe enterprise storage continue to use Adobe enterprise storage after you change the default storage preference.

### Group-scoped rollout

You can apply the default storage provider to your entire organization or to specific Workfront groups. To limit exposure during rollout, you can enable Adobe enterprise storage for a specific group within your Workfront production environment. This lets you run a targeted pilot with a smaller set of users before rolling out more broadly.

We recommend starting with a group-level rollout for controlled pacing, then expanding to the entire organization once the pilot group has validated the experience.

### Configure the storage preference

To configure the default storage provider:

{{step-1-to-setup}}

1. Select **System** in the left navigation, then select **Preferences**.
1. Scroll down to the **Storage preferences** section.
1. In the Default drop-down menu, select **Adobe enterprise storage**.
1. (Optional) To allow a combination of Adobe enterprise storage and legacy Workfront storage, select the **Allow user to select storage provider** checkbox.
1. In the Applies to drop-down menu, select one of the following:
    * **Entire organization**: Applies the default storage provider to your entire Workfront environment.
    * **Specific groups**: Applies the default storage provider only to specific groups within your organization.
1. Click **Save**.

For more information, see [Enable Adobe enterprise storage for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).
