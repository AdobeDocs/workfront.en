---
product-area: documents
navigation-topic: approvals
title: Create AI Reviewers
description: Once you have at least one brand set up in Workfront, you can create multiple AI Reviewers, which you can then assign to approval templates and individual review and approval requests.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
exl-id: 4673049e-119e-4315-95f0-f10d8b286856
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/sfM3OtA-DVqywr3Up8VGjcycLRs5WtF22dcpXzRlnvQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
    internal-label: Requests
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Create AI Reviewers

>[!NOTE]
>
>This feature is currently in beta. 

Once you have at least one brand set up in Workfront, you can create multiple AI Reviewers, which you can then assign to approval templates and individual review and approval requests. 


## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a system administrator.</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites

Before you begin, you must set up image brand guidelines in Workfront. For more information, see [Create and manage brands for the Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Add an AI Reviewer

>[!NOTE]
>
>The AI Reviewer is not designed to be a decision-maker in the review and approval workflow. It only provides a score and recommendations to align the asset with the specified brand requirements. 

To add a Content Reviewer:

{{step-1-to-setup}}

1. In the left panel, go to **Review and Approval** > **AI Reviewers**.
1. Click **Add new**.
1. Name the reviewer.
1. Select a **Brand**.
1. Select one of the following in the **Guideline Type** drop-down menu:
    * **Image**: The AI Reviewer will review the asset against the image brand guidelines you set up in Workfront.
    * **Brand voice**: The AI Reviewer will review the asset against brand voice guidelines you set up in Workfront.
1. Click **Create**.

    Once the AI Reviewer is created, users can add the AI Reviewer to approval templates or individual approvals. 

    For more information, see

    * [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
    * [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)
