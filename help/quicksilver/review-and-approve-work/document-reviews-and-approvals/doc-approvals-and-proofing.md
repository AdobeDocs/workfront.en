---
product-area: documents
navigation-topic: approvals
title: Use Unified Approvals and proofing together
description: You can use Unified Approvals with proofing.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UBrLQv-1DRwZ-TO3c1SAUn8OF0yOAYnKPGrf-lSS0xM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---
# Use Unified Approvals and proofing together

{{highlighted-preview}}

Unified Approvals in Workfront introduces a new set of features to help you review and approve documents. You can use a Unified Approvals workflow with the existing proofing viewer to add comments and markup to documents in review.

There are some key differences in the workflow when using Unified Approvals and proofing together:

* Participants are shown in the document Summary, not the proofing workflow.

* Sent, Opened, Comment, Decision (SOCD) details in the document list is proofing related and does not reflect the decision status of the document.

## Upload a document and create a proof 

1. Go to the project, task, or issue where you want to add a new document.
1. Click the **Documents** tab, then click the **Add New** drop-down menu.
Or
Drag and drop the document into the document list.

   >[!NOTE]
   >
   >If you have **Automatically generate proofs when uploading documents** enabled in your user profile, the system automatically creates a simple proof.

1. Hover over the document, then click the **Create Proof** link that appears below the document name, and select **Simple Proof**. You need to create a simple proof because you will not use the proofing workflow for approvals. 

Users assigned as participants can use the proofing viewer to add comments and markup on the document. Continue to the next section to learn how to add review participants. 

## Open the document Summary and assign participants in Production

You have the option to assign reviewers, approvers, or a mix of both:

* **Reviewers** can add comments and mark up assets. Once finished, they can mark their review as complete. Marking the review as complete is not required for the document to move forward in the approval process.
* **Approvers** can add comments and mark up assets. They must make a decision to move the approval process forward. 

To assign participants:

1. Select the document you uploaded and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.

<div class="preview">

## Open the document Summary and assign participants in Preview

The Request approval dialog opens in Basic mode by default for a single-stage approval. Switch to Advanced mode to configure multi-stage approvals or parallel paths.

To assign participants:

1. Select the document you uploaded and open the document Summary.

   ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**. The **Request approval** dialog opens in Basic mode.

1. Configure the approval workflow. For field descriptions, the Advanced mode toggle, and the parallel paths flow, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Click **Request approval**. Participants are notified via email.

</div>

## Create a new version as needed in Production

If you need another round of review and approval, you can create a new proof version and add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants in the document Summary.

To add a new version:

1. Drag and drop the new file on top of the previous document in Workfront. This automatically creates a new version. 

1. Once the document finishes uploading, select the document, then click **Create proof** > **Simple proof**. 

1. Select the document again, and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.

<div class="preview">

## Create a new version as needed in Preview

If you need another round of review and approval, you can create a new proof version and add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants in the document Summary.

The Request approval dialog opens in Basic mode by default for a single-stage approval. Switch to Advanced mode to configure multi-stage approvals or parallel paths.

To add a new version:

1. Drag and drop the new file on top of the previous document in Workfront. Workfront automatically creates a new version.

1. Once the document finishes uploading, select the document, then click **Create proof** > **Simple proof**.

1. Select the document again, then open the document Summary.

   ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**. The **Request approval** dialog opens in Basic mode.

1. Configure the approval workflow. For field descriptions, the Advanced mode toggle, and the parallel paths flow, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Click **Request approval**. Participants are notified via email.

</div>

## Review the proof and make a decision

The document does not move to an approved status until all assigned approvers choose "approved".

To review and approve a document:

1. Go to your review email notification, and click to **Go to review**.

1. Once you're in Workfront, click **Go to proof**.

1. Review the content, and add any comments or markup. For more information about how to use the proofing viewer, see [Review proofs within Adobe Workfront: article index](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Choose one of the following decisions:

    * **Approve**: The document does not need changes and is ready for use.
    * **Approve with changes**: The document needs changes and is ready for use once they are made. Additional approval is not required. 
    * **Needs work**: The document needs changes and is not ready for use. Once the specified changes are made, the document must be uploaded as a new version and go through another round of approvals. For more information on uploading a new version, see [Create a new version as needed](#create-a-new-version-as-needed) in this article.

Once you make a decision, the document owner is notified via email.