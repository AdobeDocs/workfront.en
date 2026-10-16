---
product-area: documents
navigation-topic: approvals
title: Manage grouped approvals
description: You can add or remove participants and documents in a grouped approval without disrupting the workflow for the rest of the group.
author: Courtney
feature: Work Management, Digital Content and Documents
---

# Manage grouped approvals

A grouped approval bundles multiple documents under a single approval workflow, so all the documents move through the same stages together instead of requiring a separate approval per document. You can add or remove participants and documents in an active grouped approval without recreating the workflow.

Grouped approvals support Basic and Advanced mode, multiple stages, and parallel paths the same way as single-asset approvals. For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. Grouped approvals are available only in the new Documents area. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront package</td>
   <td> <p>Any Workflow package to manage approvals using Adobe cloud storage</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license</td>
   <td>
   <p>Contributor or higher</p>
   <p>Review or higher</p>
   <p>If you are using the Frame.io integration, you must have a Standard license to create approval workflows.</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Access level configurations</td>
   <td> <p>View or higher access to Projects, Tasks, Issues, Templates, Portfolios, Programs, Reports, Dashboards, Calendars, and Documents</p></td>
  </tr>
  <tr>
   <td role="rowheader">Object permissions</td>
   <td> <p>Manage access to the object associated with the request or approval</p></td>
  </tr>
 </tbody>
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Add participants to an active grouped approval

You can add approvers or reviewers to a grouped approval while a stage is active, without interrupting the approvals already in progress.

To add participants to an active grouped approval:

1. Go to the project, task, or issue that contains the grouped approval, then select **Documents** in the left panel.

1. Click any document in the group, then click the **Approvals** icon on the right side of the page.

   ![Add approvers in document summary](assets/approvals-icon-new.png)

1. Click **Edit workflow**.

1. Type the user, team, or email in the active stage's **Add names or emails** field.

1. For each person you add, choose whether they're an approver or reviewer.

1. Click **Save**.

   New participants see every open approval in the group in their queue. They don't see decisions that were made before they were added, so they still need to complete all currently open approvals themselves.

## Remove participants from an active grouped approval

You can remove approvers or reviewers from a grouped approval while a stage is active. Removed participants immediately stop seeing the group's approvals in their queue, but decisions they already made are kept and aren't reset.

To remove participants from an active grouped approval:

1. Go to the project, task, or issue that contains the grouped approval, then select **Documents** in the left panel.

1. Click any document in the group, then click the **Approvals** icon on the right side of the page.

   ![Remove approvers in document summary](assets/approvals-icon-new.png)

1. Click **Edit workflow**.

1. Locate the participant you want to remove from the active stage, then click the **Remove** icon next to their name.

1. Click **Save**.

## Add documents to a grouped approval

You can add documents to a grouped approval until its first stage is locked. Once the first stage locks, you can no longer add documents.

To add a document to a grouped approval:

1. Go to the project, task, or issue that contains the grouped approval, then select **Documents** in the left panel.

1. Click any document in the group, then click the **Approvals** icon on the right side of the page.

1. Click **Edit workflow**, then click the **Documents** tab.

1. Select the document or documents you want to add to the group.

1. Click **Save**.

   All participants in the group are notified that an additional document was added for them to review.

## Remove documents from a grouped approval

You can remove a document from a grouped approval at any point in the workflow. The removed document becomes its own standalone approval and keeps all of its existing decisions, comments, and history without restarting. Because the document already carries an approval decision, you can't add it back to a grouped approval afterward.

To remove a document from a grouped approval:

1. Go to the project, task, or issue that contains the grouped approval, then select **Documents** in the left panel.

1. Click the document you want to remove, then click the **Approvals** icon on the right side of the page.

1. Click **Edit workflow**, then click the **Documents** tab. The document you selected is pinned at the top of the list and already checked.

1. Clear the selection for the document you want to remove from the group.

1. Click **Save**.

   >[!NOTE]
   >
   >The document's approval status stays visible and unchanged from the moment it was removed. The grouped approval view updates to reflect the remaining documents in the group.


## Resolve a "Needs work" decision on a single document in a multi-stage grouped approval

In a multi-stage grouped approval, all the documents in a stage must reach a decision before the group can advance to the next stage. If a document is marked **Needs work**, it can't move forward with the rest of the group, so it must be manually removed from the group for the stage to progress. 

When you remove the document from the group, it becomes its own standalone approval and keeps all of its existing decisions, comments, and history without restarting. You can add the revised document as a new version to the standalone approval or create a new grouped approval with it.

To resolve a "Needs work" decision:

1. Remove the document that was marked **Needs work** from the group. For more information, see [Remove documents from a grouped approval](#remove-documents-from-a-grouped-approval). The removed document becomes its own standalone approval and keeps its existing decisions, comments, and history.

1. After the document is updated, upload it as a new version and request approval on it again or add it as part of a new group. 

   For more information, see 
   
   * [Upload a new document version and request an approval](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md)
   * [Create a document approval workflow](create-a-document-approval.md)
   * [Create a grouped approval](create-a-grouped-approval.md)


## Known limitations

There is a temporary syncing issue with Frame.io when you add or remove documents in a grouped approval. The changes will not be reflected in Frame.io until the next time the document is synced.