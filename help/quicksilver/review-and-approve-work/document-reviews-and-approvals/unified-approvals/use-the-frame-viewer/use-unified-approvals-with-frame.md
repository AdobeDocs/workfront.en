---
product-area: documents
navigation-topic: approvals
title: Use Unified Approvals and proofing together
description: You can use Unified Approvals with proofing.
author: Courtney
feature: Work Management, Digital Content and Documents

---

# Use Unified Approvals and frame.io together

Unified Approvals in Workfront introduces a new set of features to help you review and approve documents. You can use a Unified Approvals workflow with the frame.io viewer to add comments and markup to documents in review.

## Upload a document

1. Go to the project where you want to add a new document.
1. Click the **Documents** tab, then click the **Add New** drop-down menu.


## Open the document Summary and assign participants

You have the option to assign reviewers, approvers, or a mix of both:

* **Reviewers** can add comments and mark up assets. Once finished, they can mark their review as complete. Marking the review as complete is not required for the document to move forward in the approval process.
* **Approvers** can add comments and mark up assets. They must make a decision to move the approval process forward. 

To assign participants:

1. Select the document you uploaded and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the Approvals section, then click **Add**.

1. (Optional) Choose an existing approval template. Users with a Standard license can create resuable Approval Templates from the Setup area. For more information, see [Create an Approval Template for assets and documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Optional) Set a deadline for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified deadline.

1. To add an approver, click the Approver button and begin typing in a user or team name.

1. To add a reviewer, click the Reviewer button and begin typing in a user or team name.

    ![Add approvers](assets/add-approvers.png)
 
1. Once you've added all reviewers and approvers, click **Submit Request**. Participants are notified via email.

## Create a new version as needed

If you need another round of review and approval, you can create a new version and add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants in the document Summary.

To add a new version:

1. Drag and drop the new file on top of the previous document in Workfront. This automatically creates a new version. 

1. Once the document finishes uploading, select the document, then click **Create proof** > **Simple proof**. 

1. Select the document again, and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the Approvals section, then click **Add**.

1. (Optional) Choose an existing approval template. Users with a Standard license can create resuable Approval Templates from the Setup area. For more information, see [Create an Approval Template for assets and documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Optional) Set a deadline for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified deadline.

1. To add an approver, click the Approver button and begin typing in a user or team name, or choose an approver from the previous version.

1. To add a reviewer, click the Reviewer button and begin typing in a user or team name, choose a reviewer from the previous version.

    ![Add approvers](assets/add-approvers.png)
 
1. Once you've added all reviewers and approvers, click **Submit Request**. Participants are notified via email.
 
<!-- add info about reusing previous participants once released -->


## Review the docuement and make a decision

The document does not move to an approved status until all assigned approvers choose "approved".

If any one approver chooses "needs work", the status of the document immediately changes to Needs work. The document needs to be revised and uploaded as a new version with a new approval workflow. 

To review and approve a document:

1. Go to your review email notification, and click to **Go to review**.

1. Once you're in Workfront, click **Go to review**.

1. Review the content, and add any comments or markup. For more information about how to use the frame.io viewer, see [FIO link](FIO-link).

1. Choose one of the following decisions:

    * **Approve**: The document does not need changes and is ready for use.
    * **Needs work**: The document needs changes and is not ready for use. Once the specified changes are made, the document must be uploaded as a new version and go through another round of approvals. For more information on uploading a new version, see [ Create a new version as needed](#create-a-new-version-as-needed) in this article.

Once you make a decision, the document owner is notified via email.

