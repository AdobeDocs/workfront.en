---
product-area: documents
navigation-topic: approvals
title: Remove approvers or reviewers from an asset or document
description: You can remove individual approvers or reviewers from a document.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
---
# Remove approvers or reviewers from an asset or document

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

## Remove approvers or reviewers to an approval<!--in the legacy document area-->

<!--If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Workfront Storage vs. Adobe enterprise storage](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).-->

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document opens.

1. Scroll down to the **Approvals** section in the Document Summary panel. 

1. Click **Edit workflow**.

1. Locate the participant you want to remove, then click the **Remove** icon next to their name.

    The approval or review request is removed and the approver receives a notification that their approval is no longer needed. Their approval-related share access is also removed.

    ![edit approval workflow](assets/edit-approval-in-legacy.png)

1. (Optional) To change the role of an approver to a reviewer, or vice versa, click the drop-down menu next to the username, and select the new role.

1. Repeat the previous step to remove any additional approvers or reviewers.

<!--Need to see this in the new docs area to finish 
## Remove approvers or reviewers to an approval workflow in the new document area

If your organization uses enterprise storage, you will see the new documents area when you access documents in Workfront. For more information about enterprise storage, see [Enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

To create a an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the Approvals icon on the right side of the page. 

   ![Add approvers in document summary](assets/approvals-icon-new.png)

1. Click **Create workflow**, then fill in the following details:

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

   ![Document details](assets/new-stage.png)

-->