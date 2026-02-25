---
product-area: documents
navigation-topic: approvals
title: Use Unified Approvals and proofing together
description: You can use Unified Approvals with proofing.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
---
# Use Unified Approvals and proofing together

Unified Approvals in Workfront introduces a new set of features to help you review and approve documents. You can use a Unified Approvals workflow with the existing proofing viewer to add comments and markup to documents in review.

There are some key differences in the workflow when using Unified Approvals and proofing together:

* Participants are shown in the document Summary, not the proofing workflow.

* Sent, Opened, Comment, Decision (SOCD) details in the document list is proofing related and does not reflect the decision status of the document.




<div class="preview">


## Use Unified Approvals and proofing together in your preview environment

### Upload a document and create a proof 

1. Go to the project, task, or issue where you want to add a new document.
1. Click the **Documents** tab, then click the **Add New** drop-down menu.
Or
Drag and drop the document into the document list.

   >[!NOTE]
   >
   >If you have **Automatically generate proofs when uploading documents** enabled in your user profile, the system automatically creates a simple proof.

1. Hover over the document, then click the **Create Proof** link that appears below the document name, and select **Simple Proof**. You need to create a simple proof because you will not use the proofing workflow for approvals. 

Users assigned as participants can use the proofing viewer to add comments and markup on the document. Continue to the next section to learn how to add review participants. 

### Open the document Summary and assign participants

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


### Create a new version as needed

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



### Review the proof and make a decision

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

</div>