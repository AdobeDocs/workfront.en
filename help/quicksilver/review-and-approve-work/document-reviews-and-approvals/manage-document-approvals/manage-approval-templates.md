---
product-area: documents
navigation-topic: approvals
title: Manage approval templates
description: You can edit, share, and delete approval templates after they're created.
author: Courtney
feature: Work Management, Digital Content and Documents
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
# Manage approval templates

After you create an approval template, you can edit, share, or delete it. System Administrators can also edit, delete, and bulk-delete any template in the account, regardless of who created or shared it.

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
   <td><p>Any Workfront package to manage approvals using legacy Workfront storage</p>
<p>Any Workflow package to manage approvals using Adobe cloud storage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p> 
   <p>Plan</p>
   </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Edit a template

To edit a template:

1. In the left panel, click **Review and Approval** > **Approval Templates**.
1. Select the checkbox next to the template you want to edit. A bar appears at the bottom of the page.
1. In the bar, click **Edit**.
1. Update the template as needed.
1. Click **Save**.

You can edit templates you created. System Administrators can edit any template in the account, regardless of who created it.

## Share a template

By default, a template is visible only to you, the creator. You can share it with specific users, or with everyone in your organization, so they can view and use it when requesting an approval.

To share a template:

1. In the left panel, click **Review and Approval** > **Approval Templates**.
1. Select the checkbox next to the template you want to share. A bar appears at the bottom of the page.
1. In the bar, click **Share**. The **Share approval template** dialog opens.
1. Click the sharing drop-down, then select one of the following:

   <table>
   <tr>
   <td><strong>Shared with everyone</strong></td>
   <td>All users in your organization can view and use the template.</td>
   </tr>
   <tr>
   <td><strong>Only invited people can access</strong></td>
   <td>Only you and the users you add can view and use the template. This is the default for new templates.</td>
   </tr>
   </table>

1. If you selected **Only invited people can access**, under **Give approval template access to**, use the **Search for people** field to add the users you want to give access to.
1. Click **Share**.

The **Shared with** column in the Approval Templates list shows who has access to each template. You are always listed as the template's creator and can't be removed.

## Delete a template

You can delete a template you created. System Administrators can delete or bulk-delete any template in the account, including templates created by other System Administrators, regardless of sharing settings.

To delete one or more templates:

1. In the left panel, click **Review and Approval** > **Approval Templates**.
1. Select the checkbox next to one or more templates.
1. In the bar at the bottom of the page, click **Delete**, then confirm the deletion.

>[!WARNING]
>
>Deleting a template is permanent. If you're a System Administrator, your selection can include templates you don't own. Review the list carefully before confirming, especially when deleting multiple templates at once.
