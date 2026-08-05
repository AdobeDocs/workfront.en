---
product-area: documents
navigation-topic: approvals
title: Update Workfront Fusion scenarios for unified review and approval
description: Inventory, classify, and remediate Workfront Fusion scenarios built on legacy Workfront Proofing as your organization adopts Adobe cloud storage and unified review and approval.
author: Courtney
feature: Work Management, Digital Content and Documents
role: Admin
---
# Update Workfront Fusion scenarios for unified review and approval

Workfront Fusion scenarios built on legacy Workfront Proofing don't automatically work against Adobe cloud storage projects. Proof-specific modules, webhooks, and API endpoints have direct equivalents in some cases and significant changes in others. This article helps you inventory affected scenarios, classify them, and decide on a remediation path before you bring teams that depend on those scenarios into your Adobe cloud storage rollout.

Scenarios scoped to legacy Workfront projects continue to work as they do today. The remediation work described in this article applies to scenarios you intend to run against Adobe cloud storage projects.

>[!IMPORTANT]
>
>The Adobe Workfront Unified Review and Approvals connector is now available in Workfront Fusion. We recommend using this connector for simpler and more reliable scenarios when using Fusion with Adobe cloud storage.
>
>For information and instructions, see [Adobe Workfront Unified Review and Approvals modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-review-and-approvals-modules) in the Workfront Fusion documentation.

Use this article to inventory and classify scenarios to understand the best way to upgrade your Fusion scenarios to account for Adobe cloud storage.

For a high-level summary of what changes when your organization moves to Workfront on Adobe cloud storage, see [Move to Workfront on Adobe cloud storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).


## What changes for Fusion on Adobe cloud storage projects

Existing Fusion scenarios built on Workfront Proof rely on proof-specific modules, webhook triggers, and API endpoints that aren't part of the unified review and approval data model. The table below maps common scenario types to their expected impact and path forward:

| Scenario type | Impact | Path forward |
|---|---|---|
| Proof creation and routing | Breaks | Rebuild using the unified approvals API in Q3 2026 |
| Proof status webhooks | Breaks | Rebuild with new approval event triggers in Q3 2026 |
| Document upload triggers | Partial: retest required | Audit and retest after migration in Q3 2026 |
| Approval reminder notifications | Breaks | Replace with approval template deadlines |
| Approval decision routing | Breaks | Rebuild using new decision status fields |
| Custom approval reporting | Partial: field names may change | Map legacy fields to the new schema |


## Classify each scenario as Edit, Rebuild, or Retire

The work each scenario requires depends on what it does and what's available in unified review and approval. Use the following classifications:

* **Edit**: The existing proof-related action has a direct equivalent in unified review and approval, and you can update the scenario to use the new action.
* **Rebuild**: The underlying steps have changed significantly, or new capabilities exist that the scenario should use, so the scenario needs to be rebuilt from scratch.
* **Retire**: Native unified review and approval functionality, such as multi-stage approval templates with deadline reminders, replaces what the scenario was built to do.

Review each scenario against your specific business logic to decide its classification.

## Remediation approach

Use the following approach to plan and execute Fusion remediation:

1. **Inventory now.** Pull a full list of active Fusion scenarios and tag every one that references proof creation, proof status, document approvals, or approval routing. Don't wait until after Adobe cloud storage is enabled.
1. **Classify each scenario** as Edit, Rebuild, or Retire based on the criteria in the previous section.
1. **Pause proof-dependent scenarios** before you bring teams that depend on them into your Adobe cloud storage pilot. Running stale proof-based automations against the new model can produce silent failures or duplicate actions.
1. **Use approval templates to replace simple routing logic.** Native multi-stage approval templates with deadline automation can handle many use cases that previously required Fusion. For more information, see [Create an Approval Template for assets and documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).
1. **Use the Adobe Workfront Unified Review and Approvals connector when rebuilding.** The updated connectors expose modules built specifically for unified review and approval and make rebuilds significantly simpler and more reliable. We don't recommend rebuilding against Workfront API version 22 beforehand. 
1. **Test rebuilt scenarios end-to-end in a sandbox instance** before enabling them in production. Pay particular attention to event subscription payloads — field names and schema differ from legacy proof events.

>[!TIP]
>
>Many organizations have accumulated Fusion scenarios that were workarounds for gaps in legacy proofing. Native unified review and approval features — including approval templates, deadline reminders, and multi-stage routing — eliminate the need for some of these scenarios entirely. As you classify each scenario, evaluate whether a native feature can replace it. Retiring a scenario is often a cleaner long-term outcome than rebuilding it.

## Related articles

* [Move to Workfront on Adobe cloud storage](/help/quicksilver/review-and-approve-work/workfront-storage.md)
* [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Create an Approval Template for assets and documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
