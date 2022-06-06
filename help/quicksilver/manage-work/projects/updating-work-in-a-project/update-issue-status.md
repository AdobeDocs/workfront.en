---
filename: update-issue-status
product-area: projects
navigation-topic: update-work-in-a-project
title: Update issue status
description: You can update the status of an issue to inform others about where the issue is and how it is progressing.
---

# Update issue status

You can update the status of an issue to inform others about where the issue is and how it is progressing.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Issue statuses

The following are the default statuses for issues in Workfront:

* New
* In Progress
* Awaiting Feedback
* On Hold
* Won't Resolve
* Reopened
* Closed
* Resolved

Your Adobe Workfront administrator can add custom statuses for issues for your organization. They can also make statuses available depending on the issue type.

For more information about custom statuses and issue types, see the following articles:

* [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) 
* [Create issues](../../../manage-work/issues/manage-issues/create-issues.md)

You can manually update issue statuses or you can let Workfront automatically update them when certain actions take place.

## Manually update issue status

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Optional) Do any of the following to provide additional information about the update, then click **Update** or, if the issue has a status that equates with Complete, click **Done:**

   * To add a note about the update, go to the **Updates** section and click **Start a new update**, then type your note.

     ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * To notify certain users about the update, type their names in the **Notify** box that appears when you type a note about the update.
   * To update the condition of the issue, click **Condition**, then select the condition that best reflects the current condition of the issue. Select from the following options:

      * Going Smoothly
      * Some Concerns
      * Major Roadblocks

   * To update the Commit Date of the issue, expand the **Commit Date** drop-down calendar, and select a new date.

## Automatically update issue status

Workfront automatically updates the existing status of an issue to a different status when the actions listed in the table below occur.

>[!NOTE]
>
>The statuses in the following table are default system statuses. Your Workfront administrator or a group administrator can rename the statuses in your instance of Workfront. For information about creating and managing statuses in Workfront, see [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Action</td> 
   <td>Original Status</td> 
   <td>New Status</td> 
  </tr> 
  <tr> 
   <td>Update the issue percent complete to 100%</td> 
   <td>New or In Progress</td> 
   <td>Closed</td> 
  </tr> 
  <tr> 
   <td>Update the issue percent complete from 100% to a lower number</td> 
   <td>Closed </td> 
   <td>In Progress</td> 
  </tr> 
  <tr> 
   <td>Update the status of a resolving object attached to the issue</td> 
   <td>Various statuses</td> 
   <td> <p>Various statuses</p> <p>For information about resolving objects and how they affect the status of issues, see the section "Synchronize the Status of the Resolvable Object with that of the Resolving Object" in the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Click the Start Issue button to accept working on an issue assigned to you</span> </td> 
   <td><span>New</span> </td> 
   <td> <p>Any status associated with the Start Issue button in your Home Team settings. </p> <p>For information about replacing the Work On It button with a Start Issue button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span><span>.</span> </p> <p>Tip: Clicking <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">the Undo button</span> after clicking Start Issue reverts the status to New. </p> </td> 
  </tr> 
 </tbody> 
</table>

