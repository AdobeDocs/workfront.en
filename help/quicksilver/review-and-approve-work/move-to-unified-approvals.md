---
product-area: documents
navigation-topic: approvals
title: Move from legacy document approvals to Unified Approvals
description: Understand what happens to your existing document approval workflows when your organization moves to a version of Workfront that supports Unified Approvals.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
---
# Move from legacy document approvals to Unified Approvals

Moving to a version of Workfront that supports Adobe cloud storage also moves your organization from Legacy Document Approvals to Unified Approvals—for every object, regardless of storage model. This article provides information on which functionality will be available in Unified Approvals as well as recommendations for Workfront administrators moving users off legacy document approvals.


>[!IMPORTANT]
>
>This change applies organization-wide as soon as you're on a version of Workfront that supports Adobe cloud storage. There's no pilot group or gradual rollout option for the move from Legacy Document Approvals to Unified Approvals.<br>
>For the full picture of what changes with Adobe cloud storage, see [Move to Workfront on Adobe cloud storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Understand what is changing from legacy document approvals to Unified Approvals

|  | Legacy document approvals | Unified Approvals |
| --- | --- | --- |
| Approvers and reviewers | Individual users only, as approvers | Individual users and teams, as approvers or reviewers |
| Deadlines and reminders | No built-in deadline reminders | Due dates with automated reminders at 72 hours, 24 hours, and on the deadline |
| Approval stages and paths | Single round of approval | [Multi-stage approvals and parallel review paths](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| Approval templates | Not supported—each approval is configured individually | [Reusable approval templates](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) configured in Workfront Setup |
| Review and markup | Proofing viewer | [Proofing viewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md) on legacy Workfront storage, or the [Frame.io viewer](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) on Adobe cloud storage |
| AI-assisted review | Not available | [Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md) for automated brand compliance checks |
| Reporting | Legacy reporting | Home KPI widgets and [Canvas Dashboards](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |
| Workfront Fusion | N/A | Existing scenarios may need to be [edited, rebuilt, or retired](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md) |


### What happens to approvals already in progress

>[!NOTE]
>
>PLACEHOLDER — confirm with Product/PM: What happens to legacy document approvals that are in progress (not yet fully approved) at the moment an org upgrades? Are they automatically migrated, closed/withdrawn and requiring re-creation, or left to complete on the legacy system?

## Prepare for the upgrade

* Share the [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) article with your end users.
* Review your existing Workfront Fusion scenarios against [Update Workfront Fusion scenarios for unified review and approval](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md) before your organization upgrades.
* PLACEHOLDER — confirm: Should admins export or archive legacy approval reports before cutover, since they don't carry over to Canvas Dashboards?
* PLACEHOLDER — confirm: Is there a recommended way to close out in-flight legacy approvals before upgrading?

### Help articles for end users

* [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Available functionality for document approvals](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Review and approve with the Frame.io viewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [Use Unified Approvals and proofing together](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [Document decision status overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Get started with the Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)
