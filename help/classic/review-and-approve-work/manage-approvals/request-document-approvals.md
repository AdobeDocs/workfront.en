---
filename: request-document-approvals
product-area: projects
navigation-topic: approvals
title: Request document approvals
description: You can request approval from managers or other users for a document in Adobe Workfront. You can also request document approvals from people without Workfront accounts if your Workfront administrator has enabled this capability, as described in Configure system security preferences.
---

# Request document approvals

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can request approval from managers or other users for a document in Adobe Workfront. You can also request document approvals from people without Workfront accounts if your Workfront administrator has enabled this capability, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, Templates, Portfolios, Programs, Reports, Dashboards, and Calendars, Documents</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher access to the object associated with the request access or approval </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Request a document approval

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. On the **Updates** tab in the right panel, click the **Start a new update** box.

1. (Optional)&nbsp;Type of message to explain how you want the approvers to approve the document.
1. In the **Notify** box, begin typing the name of a user who you want to approve the document, then click the name when it appears in the drop-down list.

   If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

   You cannot request approval from teams or groups.

1. Repeat the previous step to add other approvers.
1. Click **Ask for approval**, then click **Update**.

   The approvers receive a notification in which they are requested to make an approval decision on your document.   
   ![EmailNote.png](assets/emailnote-350x239.png)

## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show “changes” as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. On the **Details** tab in the Summary, under **Approvals**, click the ```More``` icon, then click ```Resubmit``` in the drop-down list that appears.

   ![](assets/classic-resubmit-approval-350x186.png)

## Delete a document approval request

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. On the **Details** tab in the Summary, under **Approvals**, click the approver's name, then click **Delete** in the drop-down list that appears. 
1. The approval request is removed and the approver receives a notification that their approval is no longer needed. Their approval-related share access is also removed.

## Send a reminder to an approver

You can send a message to remind document an approver that you're waiting for their feedback.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. On the **Details** tab in the Summary, under **Approvals**, click the approver's name, then click **Remind** in the drop-down menu that appears.
1. The approver receives a notification informing them the approval is still pending. They may also receive an email reminder if they have that enabled.

