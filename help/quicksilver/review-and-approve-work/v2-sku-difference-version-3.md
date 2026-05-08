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
# Move to the Workfront on Adobe enterprise storage

Workfront on Adobe enterprise storage enables the full Unified Review and Approval experience: reviews in the Frame.io viewer, powerful approval workflows in  cross-product visibility of assets, and more. It also introduces a new project type, the Adobe enterprise storage project, that uses this storage and review experience.

Your existing projects continue to work the way they do today. The new Documents area, the Frame.io viewer, and other Adobe enterprise storage behaviors apply to Adobe enterprise storage projects only--projects you and your users create after the V2 Workfront SKU is in place. You decide how and when Adobe enterprise storage rolls out in your environment.

This article is for Workfront administrators preparing to roll out Workfront on Adobe enterprise storage. It covers what's different on Adobe enterprise storage projects, how to choose your rollout shape, and what to think through before you enable Adobe enterprise storage for your users.

## Legacy projects and Adobe enterprise storage projects

After the V2 Workfront SKU is in place, your environment can contain two types of projects: projects on legacy Workfront storage(the projects you have today) and new projects on Adobe enterprise storage. The following table summarizes the main differences between the two:

| Capability | Project on legacy Workfront storage | Project on Adobe enterprise storage |
|---|---|---|
| Storage backend | Workfront only | Adobe enterprise storage |
| Cross-product visibility | Workfront only | Workfront, Frame.io, and Creative Cloud |
| Documents experience | Legacy Documents area | New Documents area |
| Review viewer | Workfront Proofing viewer | Frame.io viewer |
| Document sharing | Share individual documents | Documents inherit permissions from the parent object |
| Naming enforcement | Flexible | Strict |
| Moving objects | Only projects on legacy Workfront storage | Only projects on Adobe enterprise storage |

Existing projects keep the storage model they were created with. After the V2 Workfront SKU is in place, all projects created before that point remain legacy projects and continue to use the legacy Documents area and the Workfront Proofing viewer. The new behaviors described in this article apply only to Adobe enterprise storage projects you and your users create going forward.

For a full description of Adobe enterprise storage, see [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

## What's different on Adobe enterprise storage projects

The biggest day-to-day change on Adobe enterprise storage projects is the new Documents area and the Frame.io viewer that powers review and approval inside it. But there are other differences that impact how you manage projects, documents, and reviews on Adobe enterprise storage projects. The sections below cover the key differences to be aware of as you prepare to roll out Adobe enterprise storage.

## Hybrid draft: What's different on Adobe enterprise storage projects

The biggest day-to-day change on Adobe enterprise storage projects is the new Documents area and the Frame.io viewer that powers review and approval inside it. The table below summarizes the differences to be aware of as you prepare to roll out Adobe enterprise storage. The subsections that follow cover the three areas that have reference detail worth keeping inline.

<table>
  <thead>
    <tr>
      <th>Area</th>
      <th>What's different</th>
      <th>What to know</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>The new Documents area</td>
      <td>A redesigned, unified Documents area replaces the legacy Documents area.</td>
      <td>
      <ul>
        <li>Users can access documents from a program, portfolio, project, task, or issue.</li>
        <li>There is no longer a global Documents area. </li>
      </ul>
        <p>For more information, see <a href="/help/quicksilver/documents/managing-documents/documents-area.md">The Documents area</a> article.</p>
      </td>
    </tr>
     <tr>
      <td>Access level permissions</td>
      <td>Projects, programs, portfolios, and templates that use Adobe enterprise storage follow Adobe enterprise storage access level logic in other Adobe products.</td>
      <td>
      <ul>
        <li>When an access level has <strong>No access</strong> selected for projects, programs, portfolios, and templates but the object is shared with them, users are unable to see the object in Workfront, but they can still view the object name and any associated documents in other Adobe tools, such as Frame.io and Adobe Creative Cloud. </li>
        <li>When an access level has <strong>No access</strong> selected for documents, users are unable to see documents on projects in Workfront, but they can still view and manage documents for projects shared with them in other Adobe tools, such as Frame.io and Adobe Creative Cloud.</li>
      </ul>
      <p>For more information, see <a href="/help/quicksilver/review-and-approve-work/esm-access-permissions.md">Object permissions and access level overview for the Adobe enterprise storage model</a>.</p>
      </td>
    </tr>
    <tr>
      <td>Document permissions</td>
      <td>Documents inherit permissions from the project, task, or issue they're linked to.</td>
      <td>
      <ul>
        <li>Users can't share or set permissions on individual documents.</li>
        <li>Document access is managed through the project, task, or issue Share modal in Workfront.</li>
        <li>Subtasks don't inherit folder permissions from parent tasks.</li>
        <li>External users are supported on approval workflows — see below.</li>
      </ul>
      <p>For more information, see <a href="/help/quicksilver/review-and-approve-work/external-users.md">External users on approval workflows</a>.</p>
      </td>
    </tr>
    <tr>
      <td>Permissions flow</td>
      <td>Permissions flow from Workfront to Frame.io. </td>
      <td>
      <ul>
        <li>Workfront's Manage and Contribute permissions both map to Edit &amp; Share in Frame.io. View maps to Comment Only.</li>
        <li>Both Manage and Contribute users gain external sharing capability in Frame.io. See <a href="/help/quicksilver/review-and-approve-work/esm-access-permissions.md">Object permissions and access level overview for the Adobe enterprise storage model</a>.</li>
      </ul></td>
    </tr>
    <tr>
      <td>Review and approval viewer</td>
      <td>The Frame.io viewer replaces the Workfront Proofing viewer.</td>
      <td>
      <ul>
        <li>Included for all Workfront users with a paid license.</li>
        <li>Supports markup, time-stamped comments, version history, mobile, 40+ formats, files up to 500 GB.</li>
        <li>AI-assisted review through the Content Reviewer AI Collaborator available for Adobe Enterprise storage projects.</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>Capabilities not available</td>
      <td>Workfront Proofing, the Workfront document viewer, favorite documents, and request documents aren't part of the experience.</td>
      <td>
      <ul>
        <li>Legacy projects retain these capabilities. </li>
        <li>Workfront Proofing won't receive new investment and will be retired in a future release.</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>Naming rules</td>
      <td>Strict naming rules apply: unique names within a portfolio or project, no special characters, no trailing period or space, 255-character limit.</td>
      <td>Workfront auto-renames objects when conflicts arise. Audit templates that generate new project names and structure. See the full rule set below.</td>
    </tr>
    <tr>
      <td>Object portability</td>
      <td>You can move, copy, and convert objects only between like storage models.</td>
      <td>Adobe enterprise storage objects can't move to legacy projects, or the reverse. Moving an Adobe enterprise storage project to a legacy portfolio or program converts the parent to Adobe enterprise storage.</td>
    </tr>
    <tr>
      <td>Storage quota</td>
      <td>Pooled allocation that combines V2 Workfront SKU storage and any Frame.io Enterprise SKU or add-on storage. 60 GB per licensed user. No hard cap.</td>
      <td>View on the Customer Info page (May 2026 release). Email notifications at 75%, 90%, and 100% of the quota. See <a href="/help/quicksilver/documents/managing-documents/check-document-storage.md">Check document storage limits</a>.</td>
    </tr>
    <tr>
      <td>Annual video review cap</td>
      <td>Org-level cap on video proof requests at 10% of paid Workfront user licenses (Standard + Light combined).</td>
      <td>Once reached, no new video reviews until the next annual period. In-app notifications at 80% and 100%. Doesn't apply to Frame.io Enterprise customers.</td>
    </tr>
    <tr>
      <td>Workfront Fusion</td>
      <td>Existing proof-based Fusion scenarios don't automatically work against Adobe enterprise storage projects.</td>
      <td>Scenarios scoped to legacy projects continue to work. Each affected scenario gets one of three paths: edit, rebuild, or retire. New connectors expected Q3 2026. See the Workfront Fusion subsection below.</td>
    </tr>
  </tbody>
</table>

### External users on approval workflows

Users can add external users to approval workflows on Adobe enterprise storage projects. External users are notified by email when they're assigned to a review or approval, and they're prompted to create a Frame.io login to access the viewer and participate in the review. External users don't need a Workfront license to participate.

### Naming rules (full rule set)

Adobe enterprise storage enforces strict naming and structural rules to keep the storage layer consistent across Adobe products. These rules apply to objects you create on Adobe enterprise storage projects. Existing legacy projects keep their current names.

| Rule | Detail |
|---|---|
| Unique program and project names | Programs and projects can't have the same name if they belong to the same portfolio. |
| Unique document names | Documents can't have the same name if they belong to the same project. Document names must be unique within the same parent in the folder hierarchy. |
| Prohibited characters | Programs, portfolios, projects, templates, tasks, issues, document folders, and document names can't contain any of the following special characters: `\ / : * ? " \| < >` |
| Trailing characters | Programs, portfolios, projects, templates, tasks, issues, and document folders can't have names that end with a period or a space. |
| Name length limit | Object names are limited to 255 characters maximum. |

If a name conflicts with these rules, Workfront automatically renames the object to resolve the conflict. If you create Adobe enterprise storage projects from templates, review your existing templates so the project names and structure they generate fit the rules above.

### Workfront Fusion on Adobe enterprise storage projects (hybrid)

Existing Workfront Fusion scenarios built on legacy proofing don't automatically work against Adobe enterprise storage projects. Scenarios scoped to legacy projects continue to work as they do today. Each affected scenario falls into one of three remediation paths:

* **Edit or update**: The existing proof-related action has a direct equivalent in unified approvals and can be updated to use the new action.
* **Rebuild**: The underlying steps have changed significantly, or new capabilities exist, so the scenario needs to be rebuilt from scratch.
* **Retire**: Native unified approvals functionality, such as multi-stage approval templates with deadline reminders, replaces what the scenario was built to do.

Fusion connectors with native support for unified review and approval are expected to be available in Q3 2026.

For scenario-by-scenario impact, the legacy-proofing-to-unified-approvals scenario type mapping, and detailed remediation guidance, see [Update Workfront Fusion scenarios for unified review and approval](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).

---

**If you adopt this hybrid structure, the project-coordinator TIP currently in the Object permissions subsection moves to `## Plan your rollout` as a fifth bullet:**

**5. Train project coordinators on permissions troubleshooting.** Frame.io access on Adobe enterprise storage projects is a downstream reflection of Workfront permissions. If a stakeholder reports they can't access a review on an Adobe enterprise storage project, the fix is in Workfront — not Frame.io. Make sure project coordinators know to start their troubleshooting in the Project Share modal.
