---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Delete a Custom Status
description: You can delete a custom system status if it is no longer useful to your organization.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
---
# Delete a custom status

You can delete a custom system status if it is no longer useful to your organization. 

Whether the status is locked or unlocked determines if the status is deleted for all groups in the system:

* When you delete a system status that is currently locked, the status is removed for all groups in the system, regardless of whether the group has renamed it.
* Conversely, when you delete a system status that is currently unlocked, the status remains for all groups in the system.


>[!NOTE]
>
>You cannot delete the following:
>
>* A locked or unlocked system status used in a system approval process that is currently pending approval for at least one object in your system.
>
>  However, you can delete an unlocked system status used in a single-use or a group-level approval process that is currently pending approval.
>
>  You can run a report to find the objects and resolve the pending approvals, then try again to delete the status. For instructions, see [List objects with a pending approval processes using a certain status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md). 
>
>* Statuses used in approval processes that are currently pending approval for at least one object in your system.

For instructions on deleting a group status, see [Delete a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Delete a custom system status

{{step-1-to-setup}}

1. In the left panel, click **Project Preferences** > **Statuses**.

1. To delete the status across the entire system (including for individual groups), mouse over the status, click **Edit**, then ensure that **Lock for all groups** is selected. Click **Save**.

   Or

   To delete the system status but retain it for individual groups, mouse over the status, click **Edit**, then ensure that **Lock for all groups** is unselected. Click **Save**.

1. Hover over the status you want to delete, then click **Delete**.
1. In the message that appears, click **Delete Status**.
1. In the **Delete Status** box that displays, select a status in the field labeled **Set all projects currently with this status to**.

   Projects that were using the status that you are deleting are set to the status you select.  
   
   Statuses are available in the drop-down list only if they equate with the same status as the status you are deleting.  
   
   For example, if you are deleting a status that equates with Current, only statuses that also equate with Current are available to select.

1. Click **Delete Status**.
