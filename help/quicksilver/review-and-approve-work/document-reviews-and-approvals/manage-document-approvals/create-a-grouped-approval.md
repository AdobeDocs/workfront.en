---
product-area: documents
navigation-topic: approvals
title: Create a grouped approval
description: You can bundle multiple documents into a single approval workflow so they move through the same stages together.
author: Courtney
feature: Work Management, Digital Content and Documents
---

# Create a grouped approval

<span class="preview">The information on this page is not available in the Preview Sandbox environment because the Frame.io integration is unavailable there. This functionality will be available in Production environments on October 14 and 15, 2026.</span>

A grouped approval bundles multiple documents under a single approval workflow. You can use Basic and Advanced mode, multiple stages, and parallel paths with grouped approvals, just as you can with single-document approvals.

Grouped approvals are available only in the new Documents area, which appears when your organization uses Adobe cloud storage. For more information, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

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
   <p>For objects using Adobe cloud storage, you must have a Standard license to create approval workflows.</p>
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

## Create a basic grouped approval

To create a single-stage grouped approval:

1. Go to the project, task, or issue that contains the documents, then select **Documents** in the left panel.

1. Click the first document you want to include, then Shift+click the additional documents to select multiple documents.

1. With the documents selected, click **Request Approval** in the bottom menu. The **Request approval** dialog opens in Basic mode.

   ![create a grouped approval](assets/requeset-grouped-approval.png)

1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Use an approval template (optional)</strong></td>
   <td>The templates field is collapsed by default. Click the field to expand it, then select a template from the drop-down menu. If the template has one path and one stage, it applies in Basic mode. If the template has more than one stage or more than one path, the dialog automatically switches to Advanced mode and any input you entered in Basic mode is replaced by the template's content.</td>
   </tr>
   <tr>
   <td><strong>Add people or teams in preview</strong></td>
   <td><p>Begin typing a user name, team, or email address, then choose if they are an <strong>Approver</strong> or <strong>Reviewer</strong>. Workfront adds each active member of a team individually.</p>
   <p>Note: If a user is already added, or belongs to more than one team you add, they're included once.</p></td>
   </tr>
   <tr>
   <td><strong>Only one decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due on (optional)</strong></td>
   <td>Set a due date for the approval. Users are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   <tr>
   <td><strong>Add Custom Message (optional)</strong></td>
   <td>Type a message in the <strong>Add Custom Message</strong> text box. The message appears in the approval email notification and in the Approvals tab in Workfront.</td>
   </tr>
   </table>

1. (Optional) Click the **Documents** tab to review the documents included in this approval.

1. Click **Request approval**.

   ![basic grouped approval](assets/basic-group-approval.png)

## Create an advanced grouped approval

Advanced mode supports parallel paths. Each path runs independently and contains one or more sequential stages. When all required decisions in a stage are made, the next stage in that path begins, the previous stage is locked, and the new stage's reviewers and approvers receive an email notification.

A "Needs work" decision stops the path it's on but does not affect the approval workflow on other paths.

<!--
You can configure up to 30 paths and 100 stages total.
-->

To create an advanced grouped approval:

1. Go to the project, task, or issue that contains the documents, then select **Documents** in the left panel.

1. Click the first document you want to include, then Shift+click the additional documents to select multiple documents.

1. With the documents selected, click **Request Approval** in the bottom menu.

   ![create a grouped approval](assets/requeset-grouped-approval.png)

1. In the top right of the **Request approval** dialog, click **Go to advanced**. Any input you entered in Basic mode is preserved and applied to **Path 1**, **Stage 1**.

   >[!TIP]
   >
   >While you're creating the approval, you can return to Basic mode by clicking **Go to basic** in the top right. Once you submit the approval request, the **Go to basic** option is no longer available.

1. Fill in details for Stage 1 of Path 1:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Stages are named <em>Stage 1</em>, <em>Stage 2</em>, and so on by default. Rename the stage to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add people or teams in preview</strong></td>
   <td><p>Begin typing a user name, team, or email address, then choose if they are an <strong>Approver</strong> or <strong>Reviewer</strong>. Workfront adds each active member of a team individually.</p>
   <p>Note: If a user is already added, or belongs to more than one team you add, they're included once.</p></td>
   </tr>
   <tr>
   <td><strong>Only one decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due on (optional)</strong></td>
   <td>The first stage of each path supports an absolute due date. Each subsequent stage in the path supports a relative due date (the number of days from when that stage opens). Users are notified by email 72 hours, then 24 hours before the due date.</td>
   </tr>
   <tr>
   <td><strong>Add Custom Message (optional)</strong></td>
   <td>Type a message in the <strong>Add Custom Message</strong> text box. The message appears in the approval email notification and in the Approvals tab in Workfront.<p>When you add a second stage, <strong>Show this message on all stages</strong> is selected by default. Leave it selected to use the same message in every stage. To use a different message for each stage, clear <strong>Show this message on all stages</strong>, then type the stage-specific message in each stage's <strong>Add Custom Message</strong> text box.</p></td>
   </tr>
   </table>

1. (Optional) Add additional stages to Path 1:
   1. Click **Add stage** to add another stage to the current path. Stages within a path run sequentially in the order they're listed. 
   1. Fill in details for the new stage, then repeat this step to add more stages as needed.

      >[!NOTE]
      >
      >You can reorder stages within a path, but you can't move a stage from one path to another. Each path can have a different number of stages.


1. (Optional) Add a parallel path:
   1. Under **Parallel paths** on the left side of the screen, click **Add path** to add another path. 
   1. Follow the same steps to add stages and participants to the new path. Each path runs independently, so you can have different numbers of stages and different participants in each path.

1. (Optional) To remove a path, hover the path label and click the trash icon. **Path 1** can't be removed, and paths can't be reordered. Other paths can be removed only if no stage within the path is locked or completed.

1. (Optional) To clear all paths and stages and start over, click **Reset** in the top-right corner.

1. (Optional) Click the **Documents** tab to review the documents included in this approval.

1. Click **Request approval**.

   ![advanced grouped approval](assets/advanced-group-approval.png)


<!--

## Add additional documents to a grouped approval

You can add additional documents to a grouped approval after the approval has been created as long as the first stage has not been completed. 

To add an additional document to a grouped approval:

1. Click any document in the grouped approval, then click **Manage Approval** in the bottom menu.
1. Click **Documents on this approval**, then click **Add**.

   ![add document grouped approval](assets/add-document-to-grouped-approval.png)
1. Choose the documents you want to add, then click **Add to approval**. 
1. Once you add all of the documents, click **Edit approval**. The new documents are added to the grouped approval and all participants are notified of the change.

-->

## Known limitations

* Currently, you can't add or remove documents from a grouped approval workflow once it's created. This functionality is planned for a future release.
* Grouped approvals are temporarily limited to 3 paths and 25 documents per group.