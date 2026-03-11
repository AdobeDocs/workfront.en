---
product-area: documents
navigation-topic: approvals
title: Remove approvers or reviewers from a document approval workflow
description: You can remove individual approvers or reviewers from a document.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
---
# Remove approvers or reviewers from a document approval workflow

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span>

You can remove individual approvers or reviewers from an asset or document after they have been assigned.

>[!IMPORTANT]
>
>The content of this article refers to updated document approval functionality that is only available for specific accounts. For information on standard approval processes, see the articles listed in [Work approvals](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

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
   <p>Contributor or higher</p>
   <p>Review or higher</p>
   <p>If you are using the Frame.io integration, you must have a Standard license to create approval workflows.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, Templates, Portfolios, Programs, Reports, Dashboards, and Calendars, Documents</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the object associated with the request access or approval </p>  </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Remove approvers or reviewers from the Document Details page in your production environment

1. Go to the document page by clicking on the name of the document, then select the version of the document you would like to remove an approval for in the version dropdown. The latest version is selected by default.

1. Select **Approvals** in the left panel.

1. Hover over the name of the approver or reviewer you would like to remove, then click on the **Delete** icon ![Delete icon](../assets/delete.png) that appears after their name.

    The approval or review request is removed and the approver receives a notification that their approval is no longer needed. Their approval-related share access is also removed.

1. (Optional) To demote an approver to a reviewer rather than remove them entirely, uncheck the **Approver** checkbox in line with their name.

1. Repeat the previous step to remove any additional approvers or reviewers.

## Remove approvers or reviewers from the Document Summary in your production environment

1. Go to the project, task, or issue that contains the document, then select **Documents**.

1. Click on the document you need and the Document Summary panel for that document opens.

1. Select the version of the document you would like to remove an approver or reviewer for in the version dropdown. The latest version is selected by default.

1. Scroll down to the **Approvals** section in the Document Summary panel. Hover over the name of the approver or reviewer you would like to remove, then click on the **Delete** icon ![Delete icon](../assets/delete.png) that appears after their name.

    The approval or review request is removed and the approver receives a notification that their approval is no longer needed. Their approval-related share access is also removed.

1. (Optional) To demote an approver to a reviewer rather than remove them entirely, uncheck the **Approver** checkbox in line with their name.

1. Repeat the previous step to remove any additional approvers or reviewers.


<div class="preview">

## Remove approvers or reviewers from an approval workflow in your preview environment<!--in the legacy documents area-->

<!--If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Workfront Storage vs. Adobe enterprise storage](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).-->

To remove approvers or reviewers from an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document opens.

1. Scroll down to the **Approvals** section in the Document Summary panel. 

1. Click **Edit workflow**.

1. Locate the participant you want to remove, then click the **Remove** icon next to their name.

    The approval or review request is removed and the approver receives a notification that their approval is no longer needed. Their approval-related share access is also removed.

    ![edit approval workflow](assets/edit-approval-in-legacy.png)

1. (Optional) To change the role of an approver to a reviewer, or vice versa, click the drop-down menu next to the username, and select the new role.

1. Repeat the previous step to remove any additional approvers or reviewers.

</div>

<!--
## Remove approvers or reviewers to an approval workflow in the new document area

If your organization uses enterprise storage, you will see the new documents area when you access documents in Workfront. For more information about enterprise storage, see [Enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

To create a an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page. 

   ![Add approvers in document summary](assets/approvals-icon-new.png)


1. Click **Edit workflow**.

1. Locate the participant you want to remove, then click the **Remove** icon next to their name.

    The approval or review request is removed and the approver receives a notification that their approval is no longer needed.

1. (Optional) To change the role of an approver to a reviewer, or vice versa, click the drop-down menu next to the username, and select the new role.

1. Repeat the previous step to remove any additional approvers or reviewers.

   ![remove participants from a stage](assets/add-or-remove-participants.png)
1. Click **Save**.

-->