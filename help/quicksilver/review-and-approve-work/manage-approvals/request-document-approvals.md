---
product-area: documents
navigation-topic: approvals
title: Request a legacy document approval
description: You can request approval from managers or other users for a document in Adobe Workfront. You can also request document approvals from people without Workfront accounts if your Workfront administrator has enabled this capability, as described in Configure system security preferences.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
TQID: https://experienceleague.adobe.com/NQgXFcbc-4DiObeNE2nRgaW9iKeCKRD5v7J1PRfHkHU
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
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Request a legacy document approval

You can request approval from managers or other users for a document in Adobe Workfront. You can also request document approvals from people without Workfront accounts if your Workfront administrator has enabled this capability, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

>[!NOTE]
>
>The information in this article refers to legacy document approvals. <br>
>For information about new Unified Review and Approval, see [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).


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
   <td>
   <p>Contrbute or higher</p>
   <p>Review or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, Templates, Portfolios, Programs, Reports, Dashboards, and Calendars, Documents</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the object associated with the request access or approval </p></td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Request a document approval

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, and begin typing in the **Add Approver** text box. You can add Workfront users by name or external users by email.

1. If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

   You cannot request approval from teams or groups.

1. Repeat the previous step to add other approvers.

## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)

## Delete a document approval request

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, then click the **More** menu inline with the approver's name and select **Delete**.

   The approval request is removed and the approver receives a notification that their approval is no longer needed. Their approval-related share access is also removed.

## Send a reminder to an approver

You can send a message to remind document an approver that you're waiting for their feedback.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, then click the **More** menu inline with the approver's name and select **Remind**.

   The approver receives a notification informing them the approval is still pending. They may also receive an email reminder if they have that enabled.
