---
product-area: documents
navigation-topic: approvals
title: Move to the Workfront V2 SKU
description: Plan your rollout of the V2 Workfront SKU. Learn what's different on Adobe enterprise storage projects, including the new Documents area and the Frame.io review experience, and decide how Adobe enterprise storage rolls out in your environment.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
---
# Move to the Workfront V2 SKU

The V2 Workfront SKU brings a redesigned Documents area to your organization, powered by Adobe enterprise storage and unified review and approval with Frame.io. It also introduces a new project type, the Adobe enterprise storage project, that uses this storage and review experience.

Your existing projects continue to work the way they do today. The new Documents area, the Frame.io viewer, and other Adobe enterprise storage behaviors apply to Adobe enterprise storage projects only — projects you and your users create after the V2 Workfront SKU is in place. You decide how and when Adobe enterprise storage rolls out in your environment.

This article is for Workfront administrators preparing to roll out Adobe enterprise storage. It covers what's different on Adobe enterprise storage projects, how to choose your rollout shape, and what to think through before you enable Adobe enterprise storage for your users.

If your contract was signed before V2 Workfront SKUs were available, adding the V2 Workfront SKU requires a contracting event with Adobe at renewal or as an early recontract. Adobe Professional Services executes the contracting event, and there's no price increase when moving to an equivalent package. Contact your Adobe account representative to confirm your current SKU and the path that fits your organization. After your account is on the V2 Workfront SKU, you decide when to enable Adobe enterprise storage in your environment.

## Legacy projects and Adobe enterprise storage projects

After the V2 Workfront SKU is in place, your environment can contain two types of projects: legacy projects (the projects you have today) and Adobe enterprise storage projects (which use the new Documents area). The following table summarizes the main differences between the two:

| Capability | Legacy project | Adobe enterprise storage project |
|---|---|---|
| Storage backend | Workfront only | Adobe enterprise storage, shared with Frame.io and Creative Cloud |
| Documents experience | Legacy Documents area | New Documents area |
| Review viewer | Workfront Proofing viewer | Frame.io viewer |
| Document sharing | Share individual documents | Inherit permissions from the parent object |
| Cross-product visibility | Workfront only | Workfront, Frame.io, and Creative Cloud |
| Naming enforcement | Flexible | Strict |
| Object portability | Move between any projects | Adobe enterprise storage projects only |

Existing projects keep the storage model they were created with. After the V2 Workfront SKU is in place, all projects created before that point remain legacy projects and continue to use the legacy Documents area and the Workfront Proofing viewer. The new behaviors described in this article apply only to Adobe enterprise storage projects you and your users create going forward.

For a full description of Adobe enterprise storage, see [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

## What's different on Adobe enterprise storage projects

The biggest day-to-day change on Adobe enterprise storage projects is the new Documents area and the Frame.io viewer that powers review and approval inside it. The sections below cover that experience first, followed by the project, task, issue, and automation behaviors that change as a result of moving to Adobe enterprise storage.

### The new Documents area

The new Documents area is a unified documents experience designed for Adobe enterprise storage. It simplifies navigation, consolidates review and approval activity, and is the entry point for the Frame.io viewer.

The new Documents area is available on Adobe enterprise storage projects only. The global Documents area isn't part of the new experience. On Adobe enterprise storage projects, you access documents from a program, portfolio, project, task, or issue.

When you create an Adobe enterprise storage project, Workfront automatically creates a document folder with the same name as the project in the project's Documents section. After you add tasks or issues to the project, folders with the task or issue name are added to the Documents section of each task or issue. These system-generated folders inherit permissions from the task, issue, or project they're linked to, and any document uploaded to that object is stored in the matching folder.

For more information, see [The Documents area](/help/quicksilver/documents/managing-documents/documents-area.md).

### The Frame.io viewer for review and approval

On Adobe enterprise storage projects, the Frame.io viewer is the review and approval surface in place of Workfront Proof. The Frame.io viewer is included for all Workfront users with a paid license — no additional Frame.io license is required.

The Frame.io viewer provides:

* Markup and commenting tools, including freehand drawing and standard shapes such as circles, arrows, and squares
* Time-stamped comments with frame-accurate precision for video reviews
* Version history and version comparison
* Mobile access for on-the-go reviews and approvals
* Support for over 40 file formats, including all common video, image, audio, PDF, and Microsoft Office types, with native playback for professional video formats such as ProRes, H.265, and DNxHD, and support for files up to 500 GB

For a detailed list of supported files, see [Supported File Types on Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

<!-- COURTNEY-REVIEW START: AI-assisted review mention (placeholder per chat). Verify wording, expand or trim, and add a link to Content Reviewer AI Collaborator documentation if available. -->
**[REVIEWER PLACEHOLDER — Courtney to verify]** Adobe enterprise storage projects also support AI-assisted review through the Content Reviewer AI Collaborator.
<!-- COURTNEY-REVIEW END -->

The following capabilities aren't part of Adobe enterprise storage projects:

* Workfront Proofing
* The Workfront document viewer
* Favorite documents
* Request documents

Legacy projects retain access to Workfront Proofing and the legacy document capabilities listed above. Workfront Proofing doesn't receive new investment going forward and will be retired in a future release.

For more information, see the following:

* [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)

### Document permissions on Adobe enterprise storage projects

On Adobe enterprise storage projects, documents inherit permissions from the project, task, or issue they're linked to. You can't share or set permissions on individual documents.

* Tasks and issues inherit permissions from the project.
* System-generated folders inherit permissions from their linked task or issue.
* Subfolders inherit permissions from the parent folder.
* Subtasks don't inherit system-generated folder permissions from parent tasks. You must be added directly to a subtask to access its system-generated folder.

User permissions are set in Workfront and flow one direction through to Frame.io. You can't invite users to an Adobe enterprise storage project in Frame.io or modify user permissions in Frame.io. All access management for Adobe enterprise storage projects happens through the Project Share modal in Workfront.

>[!TIP]
>
>Train project coordinators that Frame.io access is a downstream reflection of Workfront permissions. If a stakeholder reports they can't access a review on an Adobe enterprise storage project, the fix is in Workfront — not Frame.io.

The following table maps Workfront permissions to Frame.io permissions:

| Workfront permission | Frame.io permission |
|---|---|
| Manage | Edit & Share |
| Contribute | Edit & Share |
| View | Comment Only |

<!-- COURTNEY-REVIEW START: permissions-collapse callout (placeholder per chat). Keep, edit, or remove. -->
>[!NOTE]
>
>**[REVIEWER PLACEHOLDER — Courtney to evaluate]** Both Manage and Contribute map to **Edit & Share** in Frame.io. As you review your sharing patterns for Adobe enterprise storage projects, consider whether contributors having the same review-side capabilities as managers — including external sharing — fits your governance model.
<!-- COURTNEY-REVIEW END -->

You can share assets externally. External users are notified by email when they're assigned to a review or approval, and they're prompted to create a Frame.io login to access the viewer and participate in the review. External users don't need a Workfront license to participate.

For more information, see [Object permissions and access level overview for the Adobe enterprise storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

### Naming rules

Adobe enterprise storage enforces strict naming and structural rules to keep the storage layer consistent across Adobe products. These rules apply to objects you create on Adobe enterprise storage projects. Existing legacy projects keep their current names.

The following rules apply on Adobe enterprise storage projects:

| Rule | Detail |
|---|---|
| Unique program and project names | Programs and projects can't have the same name if they belong to the same portfolio. |
| Unique document names | Documents can't have the same name if they belong to the same project. Document names must be unique within the same parent in the folder hierarchy. |
| Prohibited characters | Programs, portfolios, projects, templates, tasks, issues, document folders, and document names can't contain any of the following special characters: `\ / : * ? " \| < >` |
| Trailing characters | Programs, portfolios, projects, templates, tasks, issues, and document folders can't have names that end with a period or a space. |
| Name length limit | Object names are limited to 255 characters maximum. |

If a name conflicts with these rules, Workfront automatically renames the object to resolve the conflict.

If you create Adobe enterprise storage projects from templates, review your existing templates so the project names and structure they generate fit the rules above.

### Object portability

You can move, copy, and convert Workfront objects between like storage models. For example, you can move a task from one Adobe enterprise storage project to another Adobe enterprise storage project. You can't move or copy a task or issue from an Adobe enterprise storage project to a legacy project, or the reverse.

When you create or move an Adobe enterprise storage project to a legacy portfolio or program, the portfolio or program is automatically converted to an Adobe enterprise storage object.

### Storage quota and the annual video review cap

The V2 Workfront SKU changes how storage quota is reported and adds an annual cap on video review requests. Both apply at the organization level — they're not specific to Adobe enterprise storage projects.

#### Storage quota

When your contract moves to the V2 Workfront SKU, your storage quota is reported as a single pooled allocation that combines storage provisioned through your V2 Workfront SKU and any storage provisioned through a Frame.io Enterprise SKU or add-on. Each licensed user receives 60 GB of storage through the V2 Workfront SKU, up from 30 GB on the previous version.

Beginning with the May 2026 release, you can view your pooled storage quota and a usage breakdown on the Customer Info page in Setup.

There's no hard cap on storage usage. Workfront administrators receive email notifications when usage reaches 75%, 90%, and 100% of the quota.

For more information, see [Check document storage limits](/help/quicksilver/documents/managing-documents/check-document-storage.md).

#### Annual video review cap

There's an annual cap on video proof requests set at 10% of your organization's total paid Workfront user licenses (Standard and Light). This cap is applied at the organization level.

* Workfront administrators receive in-app notifications when usage reaches 80% and 100% of the cap.
* Once the cap is reached, you can't create new video review requests until the next annual period.
* This limit doesn't apply to Frame.io Enterprise customers. If your organization regularly reviews large volumes of video content, contact your Adobe account representative to learn about Frame.io Enterprise licensing.

For more information, see the Reviewing and approving assets and videos FAQ in [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

### Workfront Fusion on Adobe enterprise storage projects

Existing Workfront Fusion scenarios built on legacy proofing don't automatically work against Adobe enterprise storage projects. Proof-specific modules, webhooks, and API endpoints have direct equivalents in some cases and significant changes in others. Scenarios scoped to legacy projects continue to work as they do today.

For impact details by scenario type, classification guidance, and a recommended remediation approach, see [Update Workfront Fusion scenarios for unified review and approval](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).

## Choose how Adobe enterprise storage rolls out

You decide how Adobe enterprise storage appears to your users. There are two configurations, and either one can be applied to your entire organization or to specific Workfront groups.

* **Adobe enterprise storage only**: New projects use Adobe enterprise storage by default. Users can't create legacy projects.
* **Adobe enterprise storage and legacy Workfront storage**: When users create a project, they choose between Adobe enterprise storage (labeled "New project") and legacy Workfront storage (labeled "Legacy project").

To put Adobe enterprise storage in front of a smaller team first, apply either configuration to a single Workfront group. This lets you run a targeted pilot before rolling out more broadly. We recommend starting with a group-level rollout for controlled pacing, then expanding to the entire organization once the pilot group has validated the experience.

>[!NOTE]
>
>Existing projects keep the storage model they were created with. Changing the default storage preference doesn't change any existing project. For example, projects already created on Adobe enterprise storage continue to use Adobe enterprise storage after you change the preference, and projects already created on legacy Workfront storage continue to use legacy Workfront storage.

For more information, see [Enable Adobe enterprise storage for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

## Plan your rollout

Every Workfront environment is different. Before you enable Adobe enterprise storage for your users, take some time to plan what a successful rollout looks like for your organization. The considerations below aren't a checklist — they're a starting point for your own plan.

**Pick a pilot group.** A group-scoped rollout lets you put Adobe enterprise storage in front of a smaller team first, gather feedback, and adjust before broader rollout. Pick a group whose work patterns are representative enough to surface issues you want to know about early.

**Communicate the change to end users.** The biggest visible change for reviewers, approvers, and project owners is the new Documents area and the Frame.io viewer that powers review and approval on Adobe enterprise storage projects. Plan how you'll introduce these so users know what to expect when they encounter their first Adobe enterprise storage project. The [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) article is a useful starting point for end-user-facing material.

**Plan around Workfront Fusion connector availability.** Fusion connectors with native support for unified review and approval are expected to be available in Q3 2026. Existing proof-based Fusion scenarios continue to work on legacy projects. Before you bring teams that depend on those scenarios into your Adobe enterprise storage pilot, decide whether to wait for the new connectors, rebuild against the current API, or replace the scenario with native unified review and approval features. For impact details and remediation guidance, see [Update Workfront Fusion scenarios for unified review and approval](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).

**Stay aware of sync drift between Workfront and Frame.io.** It's possible for Workfront to become out of sync with Frame.io or Creative Cloud — for example, an asset can be deleted in Workfront but still appear in Frame.io. If you see this on an Adobe enterprise storage project, contact Workfront support to have your environment resynced.

## Related articles

* [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [Enable Adobe enterprise storage for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)
* [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [The Documents area](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Object permissions and access level overview for the Adobe enterprise storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)
* [Update Workfront Fusion scenarios for unified review and approval](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)
