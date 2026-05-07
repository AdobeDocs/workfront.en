---
product-area: documents
navigation-topic: approvals
title: Update Workfront Fusion scenarios for unified review and approval
description: Inventory, classify, and remediate Workfront Fusion scenarios built on legacy Workfront Proofing as your organization adopts Adobe enterprise storage and unified review and approval.
author: Courtney
feature: Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
---
# Update Workfront Fusion scenarios for unified review and approval

Workfront Fusion scenarios built on legacy Workfront Proofing don't automatically work against Adobe enterprise storage projects. Proof-specific modules, webhooks, and API endpoints have direct equivalents in some cases and significant changes in others. This article helps you inventory affected scenarios, classify them, and decide on a remediation path before you bring teams that depend on those scenarios into your Adobe enterprise storage rollout.

Scenarios scoped to legacy Workfront projects continue to work as they do today. The remediation work described in this article applies to scenarios you intend to run against Adobe enterprise storage projects.

Fusion connectors with native support for unified review and approval are expected to be available in Q3 2026. Until those connectors are available, edits and rebuilds use the current Fusion API.

For a high-level summary of what changes when your organization moves to the V2 Workfront SKU, see [Move to the Workfront V2 SKU](/help/quicksilver/review-and-approve-work/v2-sku-differences-new.md).

## What changes for Fusion on Adobe enterprise storage projects

Existing Fusion scenarios built on Workfront Proof rely on proof-specific modules, webhook triggers, and API endpoints that aren't part of the unified review and approval data model. The table below maps common scenario types to their expected impact and path forward:

| Scenario type | Impact | Path forward |
|---|---|---|
| Proof creation and routing | Breaks | Rebuild using the unified approvals API |
| Proof status webhooks | Breaks | Rebuild with new approval event triggers |
| Document upload triggers | Partial: retest required | Audit and retest after migration |
| Approval reminder notifications | Breaks | Replace with approval template deadlines |
| Approval decision routing | Breaks | Rebuild using new decision status fields |
| Custom approval reporting | Partial: field names may change | Map legacy fields to the new schema |

## Classify each scenario as Edit, Rebuild, or Retire

The work each scenario requires depends on what it does and what's available in unified review and approval. Use the following classifications:

* **Edit**: The existing proof-related action has a direct equivalent in unified review and approval, and you can update the scenario to use the new action.
* **Rebuild**: The underlying steps have changed significantly, or new capabilities exist that the scenario should use, so the scenario needs to be rebuilt from scratch.
* **Retire**: Native unified review and approval functionality, such as multi-stage approval templates with deadline reminders, replaces what the scenario was built to do.

Use the impact table in the previous section as a starting point, and review each scenario against your specific business logic.

## Remediation approach

Use the following approach to plan and execute Fusion remediation:

1. **Inventory now.** Pull a full list of active Fusion scenarios and tag every one that references proof creation, proof status, document approvals, or approval routing. Don't wait until after Adobe enterprise storage is enabled.
1. **Classify each scenario** as Edit, Rebuild, or Retire based on the criteria in the previous section.
1. **Pause proof-dependent scenarios** before you bring teams that depend on them into your Adobe enterprise storage pilot. Running stale proof-based automations against the new model can produce silent failures or duplicate actions.
1. **Use approval templates to replace simple routing logic.** Native multi-stage approval templates with deadline automation can handle many use cases that previously required Fusion. For more information, see [Create an Approval Template for assets and documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).
1. **Wait for the Q3 2026 connector updates before rebuilding complex scenarios** if your timeline allows. The updated Fusion connectors will expose modules built specifically for unified review and approval, which will make rebuilds significantly easier.
1. **Test rebuilt scenarios in a sandbox instance end-to-end** before enabling them in production. Pay particular attention to event subscription payloads — field names and schema differ from legacy proof events.

>[!TIP]
>
>Many organizations have accumulated Fusion scenarios that were workarounds for gaps in legacy proofing. Native unified review and approval features — including approval templates, deadline reminders, and multi-stage routing — eliminate the need for some of these scenarios entirely. As you classify each scenario, evaluate whether a native feature can replace it. Retiring a scenario is often a cleaner long-term outcome than rebuilding it.

## Related articles

* [Move to the Workfront V2 SKU](/help/quicksilver/review-and-approve-work/v2-sku-differences-new.md)
* [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Create an Approval Template for assets and documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
