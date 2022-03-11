

# Delete a custom status

You can delete a custom system status if it is no longer useful to your organization.

>[!NOTE]
>
>You cannot delete the following built-in statuses: Planning, Current, and Complete. You can update the names, edit the colors, and lock or unlock these built-in statuses, but you cannot delete them.

Whether the status is locked or unlocked determines if the status is deleted for all groups in the system:

* When you delete a system status that is currently locked, the status is removed for all groups in the system, regardless of whether the group has&nbsp;renamed it.
* When you delete a system status that is currently unlocked, the status remains for all groups in the system.

For information about deleting a status only for a specific group, see [Create or edit a status for a group](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create) in [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Access requirements

You must have the following to perform the steps in this article:

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

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Project Preferences</span> > <span class="bold">Statuses</span>.</li> 
 <li value="3"> <p>To delete the status across the entire system (including for individual groups), mouse over the status, click <span class="bold">Edit</span>, then ensure that <span class="bold">Lock for all groups</span> is selected. Click <span class="bold">Save</span>.</p> <p>Or</p> <p>To delete the system status but retain it for individual groups, mouse over the status, click <span class="bold">Edit</span>, then ensure that <span class="bold">Lock for all groups</span> is unselected. Click <span class="bold">Save</span>.</p> </li> 
 <li value="4">Hover over the status you want to delete, then click <span class="bold">Delete</span>.</li> 
 <li value="5">In the message that appears, click <span class="bold">Delete Status</span>.</li> 
 <li value="6"> <p>In the <span class="bold">Delete Status</span> box that displays, select a status in the field labeled <span class="bold">Set all projects currently with this status to</span>.</p> <p>Projects that were using the status that you are deleting are set to the status you select.<br>Statuses are available in the drop-down list only if they equate with the same status as the status you are deleting.<br>For example, if you are deleting a status that equates with Current, only statuses that also equate with Current are available to select.</p> </li> 
 <li value="7">Click <span class="bold">Delete Status</span>.</li> 
</ol>

