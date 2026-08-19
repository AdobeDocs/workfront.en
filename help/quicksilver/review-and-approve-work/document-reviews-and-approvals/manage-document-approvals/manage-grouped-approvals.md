---
product-area: documents
navigation-topic: approvals
title: Manage grouped approvals
description: You can add or remove participants and assets in a grouped approval without disrupting the workflow for the rest of the group.
author: Courtney
feature: Work Management, Digital Content and Documents
---

# Manage grouped approvals

{{highlighted-preview-article-level}}

A grouped approval bundles multiple assets under a single approval workflow, so all the assets move through the same stages together instead of requiring a separate approval per asset. You can add or remove participants and assets in an active grouped approval without recreating the workflow.

Grouped approvals support Basic and Advanced mode, multiple stages, and parallel paths the same way as single-asset approvals. For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

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

1. Click **Edit workflow**.

1. Locate the participant you want to remove from the active stage, then click the **Remove** icon next to their name.

1. Click **Save**.

   The remaining participants' approval status is re-evaluated to account for the change.

## Add assets to a grouped approval

You can add assets to a grouped approval until its first stage is locked. Once the first stage locks, you can no longer add assets, because the participants in that stage wouldn't have had the chance to review them.

To add an asset to a grouped approval:

1. Go to the project, task, or issue that contains the grouped approval, then select **Documents** in the left panel.

1. Click any document in the group, then click the **Approvals** icon on the right side of the page.

1. Click **Edit workflow**, then click the **Documents** tab.

1. Select the asset or assets you want to add to the group.

1. Click **Save**.

   All participants in the group are notified that an additional asset was added for them to review.

## Remove assets from a grouped approval

You can remove an asset from a grouped approval at any point in the workflow. The removed asset becomes its own standalone approval and keeps all of its existing decisions, comments, and history without restarting. Because the asset already carries an approval decision, you can't add it back to a grouped approval afterward.

To remove an asset from a grouped approval:

1. Go to the project, task, or issue that contains the grouped approval, then select **Documents** in the left panel.

1. Click the document you want to remove, then click the **Approvals** icon on the right side of the page.

1. Click **Edit workflow**, then click the **Documents** tab. The document you selected is pinned at the top of the list and already checked.

1. Clear the selection for the document you want to remove from the group.

1. Click **Save**.

   The asset's approval status stays visible and unchanged from the moment it was removed. The grouped approval view updates to reflect the remaining assets in the group.
