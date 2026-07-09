---
product-area: documents
navigation-topic: approvals
title: Add additional approvers or reviewers to a document approval workflow
description: You can add additional approvers or reviewers to a document that already has pending approvals.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jo3N878hmvHRqo6kCepxPDk2-zlalLvqQbMjHHB8aGE
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
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Add additional approvers or reviewers to a document approval workflow

{{highlighted-preview}}

You can add additional approvers or reviewers to a document approval workflow that already has pending approvals.

>[!IMPORTANT]
>
>The content of this article refers to updated document approval functionality that is only available for specific accounts. For information on standard approval processes, see the articles listed in [Work approvals](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any Workfront package to manage approvals using legacy Workfront storage</p>
<p>Any Workflow package to manage approvals using Adobe cloud storage</p> </td> 
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
   <td> <p>View or higher access to the object associated with the request access or approval </p></td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++



## Add additional approvers or reviewers in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

To add additional approvers or reviewers from the Document Summary:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document will open.

1. Select the version of the document you would like to add an approver or reviewer to in the version drop-down menu. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Edit workflow**.

   ![edit approval workflow](assets/edit-approval-in-legacy.png)

1. Locate the stage you would like to add approvers or reviewers to, then add the user's name or email in the text box. You can also add an entire team if needed. 

1. Once their name is added, choose if they are an approver or reviewer. 

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
 Once you save, the participants added receive an email notification that their approval or review is needed on the document.

<div class="preview">

## Add additional approvers or reviewers in the legacy documents area in Preview

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

To add additional approvers or reviewers from the Document Summary:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need. The Document Summary panel for that document opens.

1. Select the version of the document you want to add an approver or reviewer to in the version drop-down menu. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Edit workflow**. The Request approval dialog opens in the mode the approval was last saved in: Basic for single-stage approvals, or Advanced for multi-stage approvals and approvals with parallel paths.

1. Add the user, team, or email:

   * In Basic mode, type the name or email in the **Add names or emails** field.
   * In Advanced mode, select the path that contains the stage you want to update, then type the name or email in the stage's **Add names or emails** field.

1. For each person you added, choose whether they're an approver or reviewer.

   ![approver or reviewer drop-down](assets/choose-reviewer-or-approver.png)

1. Click **Save**. The participants you added receive an email notification that their approval or review is needed on the document.

>[!TIP]
>
>To restructure a Basic-mode approval into a multi-stage or multi-path approval, click **Go to advanced** in the upper-right corner. Your existing participants are preserved as Path 1, Stage 1. After you save, you can't switch back to Basic mode. For details, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

</div>

## Add additional approvers or reviewers in the new Documents area in Production

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page. 

   ![Add approvers in document summary](assets/approvals-icon-new.png)


1. Click **Edit workflow**.

1. Locate the stage you would like to add approvers or reviewers to, then add the user's name or email in the text box. You can also add an entire team if needed. 

1. Once their name is added, choose if they are an approver or reviewer. 

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
 Once you save, the participants added receive an email notification that their approval or review is needed on the document.

<div class="preview">

## Add additional approvers or reviewers from the Document Summary in the new Documents area in Preview

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

To add additional approvers or reviewers from the Document Summary:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page.

   ![Add approvers in document summary](assets/approvals-icon-new.png)

1. Click **Edit workflow**. The Request approval dialog opens in the mode the approval was last saved in: Basic for single-stage approvals, or Advanced for multi-stage approvals and approvals with parallel paths.

1. Add the user, team, or email:

   * In Basic mode, type the name or email in the **Add names or emails** field.
   * In Advanced mode, select the path that contains the stage you want to update, then type the name or email in the stage's **Add names or emails** field.

1. For each person you added, choose whether they're an approver or reviewer.

   ![approver or reviewer drop-down](assets/choose-reviewer-or-approver.png)

1. Click **Save**. The participants you added receive an email notification that their approval or review is needed on the document.

>[!TIP]
>
>To restructure a Basic-mode approval into a multi-stage or multi-path approval, click **Go to advanced** in the upper-right corner. Your existing participants are preserved as Path 1, Stage 1. After you save, you can't switch back to Basic mode. For details, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

</div>