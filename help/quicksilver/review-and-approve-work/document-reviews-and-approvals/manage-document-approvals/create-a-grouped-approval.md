---
product-area: documents
navigation-topic: approvals
title: Create a grouped approval
description: You can bundle multiple assets into a single approval workflow so they move through the same stages together.
author: Courtney
feature: Work Management, Digital Content and Documents
---

# Create a grouped approval

{{highlighted-preview-article-level}}

A grouped approval bundles multiple assets under a single approval workflow, so all the assets move through the same stages together instead of requiring a separate approval per asset. 

Grouped approvals support Basic and Advanced mode, multiple stages, and parallel paths the same way single-asset approvals do.

After you create a grouped approval, you can add or remove participants and assets without recreating the workflow. For more information, see [Manage grouped approvals](manage-grouped-approvals.md).

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

## Select the assets for the group

Grouped approvals are available only in the new Documents area, which appears when your organization uses Adobe cloud storage. For more information, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

1. Go to the project, task, or issue that contains the documents, then select **Documents** in the left panel.

1. Switch to **List** or **Card** view.

1. Click the first asset you want to include, then Shift+click the additional assets to select multiple assets.

1. With the assets selected, click the **Approvals** icon, then click **Create workflow**.

The **Request approval** dialog opens in **Basic** mode by default. Basic mode is a single stage with one set of approvers or reviewers. Switch to **Advanced** mode to configure multi-stage approvals or parallel paths.

## Create a basic grouped approval

To create a single-stage grouped approval:

1. With your assets selected, click the **Approvals** icon, then click **Create workflow**. The **Request approval** dialog opens in Basic mode.

1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Use an approval template (optional)</strong></td>
   <td>The templates field is collapsed by default. Click the field to expand it, then select a template from the drop-down menu. If the template has one path and one stage, it applies in Basic mode. If the template has more than one stage or more than one path, the dialog automatically switches to Advanced mode and any input you entered in Basic mode is replaced by the template's content.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user name or email to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
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

1. (Optional) Click the **Documents** tab to confirm the assets included in the group.

1. Click **Request approval**.

## Create an advanced grouped approval

Advanced mode supports parallel paths. Each path runs independently and contains one or more sequential stages. When all required decisions in a stage are made, the next stage in that path begins, the previous stage is locked, and the new stage's reviewers and approvers receive an email notification.

A "Needs work" decision stops the path it's on but does not affect the approval workflow on other paths. You can configure up to 30 paths and 100 stages total.

To create an advanced grouped approval:

1. With your assets selected, click the **Approvals** icon, then click **Create workflow**.

1. In the top right of the **Request approval** dialog, click **Go to advanced**. Any input you entered in Basic mode is preserved and applied to **Path 1**, **Stage 1**.

   >[!TIP]
   >
   >While you're creating the approval, you can return to Basic mode by clicking **Go to basic** in the top right. After you click **Request approval**, the **Go to basic** option is no longer available.

1. Fill in details for Stage 1 of Path 1:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Stages are named <em>Stage 1</em>, <em>Stage 2</em>, and so on by default. Rename the stage to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user name or email to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.<p>Note: A reviewer or approver can be assigned to only one open stage at a time on the same asset. If multiple parallel stages are open simultaneously, the same person can't be added to more than one.</p></td>
   </tr>
   <tr>
   <td><strong>Only one decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due on (optional)</strong></td>
   <td>The first stage of each path supports an absolute due date. Each subsequent stage in the path supports a relative due date — the number of days from when that stage opens. Users are notified by email 72 hours, then 24 hours before the due date.</td>
   </tr>
   <tr>
   <td><strong>Add Custom Message (optional)</strong></td>
   <td>Type a message in the <strong>Add Custom Message</strong> text box. The message appears in the approval email notification and in the Approvals tab in Workfront.<p>When you add a second stage, <strong>Show this message on all stages</strong> is selected by default. Leave it selected to use the same message in every stage. To use a different message for each stage, clear <strong>Show this message on all stages</strong>, then type the stage-specific message in each stage's <strong>Add Custom Message</strong> text box.</p></td>
   </tr>
   </table>

1. (Optional) Click **Add stage** to add another stage to the path. Stages within a path run sequentially in the order they're listed. You can reorder stages within a path, but you can't move a stage from one path to another. Each path can have a different number of stages.

1. (Optional) Under **Parallel paths**, click **Add path** to add another path. The new path starts with one empty stage and becomes the selected path. To rename a path, hover the path label, click the pencil icon, then type a new name.

1. (Optional) To remove a path, hover the path label and click the trash icon. **Path 1** can't be removed, and paths can't be reordered. Other paths can be removed only if no stage within the path is locked or completed.

1. (Optional) To clear all paths and stages and start over, click **Reset** in the top right.

1. (Optional) Click the **Documents** tab to confirm the assets included in the group.

1. Click **Request approval**.
