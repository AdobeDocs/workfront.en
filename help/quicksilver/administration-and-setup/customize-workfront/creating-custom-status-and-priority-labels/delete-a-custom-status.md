

# Delete a custom status

You can delete a custom system status if it is no longer useful to your organization.

Whether the status is locked or unlocked determines if the status is deleted for all groups in the system:

* When you delete a system status that is currently locked, the status is removed for all groups in the system, regardless of whether the group has&nbsp;renamed it.
* When you delete a system status that is currently unlocked, the status remains for all groups in the system.


>[!NOTE]
>
>You cannot delete the following:
>
>* The built-in statuses Planning, Current, and Complete. You can update their names, edit their colors, and lock or unlock them, but they can't be deleted.
>* Statuses that are in a pending state of approval for at least one object in your system.

For instructions on deleting a group status, see [Delete a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

## Access requirements

You must have the following access to perform the steps in this article: 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Delete a custom system status

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

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

