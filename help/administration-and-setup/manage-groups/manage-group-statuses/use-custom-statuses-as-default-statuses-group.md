---
filename: use-custom-statuses-as-default-statuses-group
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Use a custom status as a default status for a group
description: As a group administrator, you can configure a custom status as a default status for a group or subgroup that you manage. This is useful when the system needs to automatically assign a Workfront status to a project, task, or issue. A project, task, or issue always displays the custom status that you set as a default status instead of displaying the Workfront status that it equates to.
---

# Use a custom status as a default status for a group

As a group administrator, you can configure a custom status as a default status for a group or subgroup that you manage. This is useful when the system needs to automatically assign a Workfront status to a project, task, or issue. A project, task, or issue always displays the custom status that you set as a default status instead of displaying the Workfront status that it equates to.

The status you configure can be any custom status created for the group, inherited from a group above the group, or inherited from the system level.

If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).

` `**Example: **`` You could create a custom status called Finished and set it as a default status equated with the Workfront status Complete.

Then, for tasks set to change to the status Complete when they reach 100%, the status displays as Finished instead of Complete.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

## Set a custom status as a default status for a group

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> In the left panel, click Groups, then click the name of the group where you want to create or customize statuses. 
 <li value="3"> <p>In the left panel, click Statuses. </p> </li> 
 <li value="4">Click <span class="bold">Set Default Statuses</span> near the upper-right corner.</li> 
 <li value="5"> <p>In the drop-down area that displays, next to the status where you want to set the default status, select the default status you want to set.</p> </li> 
 <li value="6"> <p>Click <span class="bold">Save</span>.</p> <p>The status is now available as a default status for use with projects associated with the group.</p> </li> 
 <li value="7"> <p>Associate the custom status with the project where you want to use it.</p> <p>You associate the status with the project by associating the group where the status resides with the project. Users can use the custom status only if the group where the status resides is associated with the project.</p> <note type="note">
    If you assign the project to a different group, the project status will reload and could change.
  </note> 
  <ol> 
   <li value="1"> <p>Go to the project where you want to use the custom status.</p> </li> 
   <li value="2"> <p> Click the More menu , then click Edit. </p> </li> 
   <li value="3">In the <span class="bold">Edit Project</span> box that displays, in the <span class="bold">Group</span> field under <span class="bold">Project association</span>, select the group that the custom status is associated with.</li> 
   <li value="4">Click <span class="bold">Save Changes</span>.</li> 
  </ol> </li> 
</ol>

## Groups inherit default status configurations

After a Workfront administrator configures a custom status as a default status, new groups that are created inherit that configuration.

Similarly, after a group administrator sets a custom status as a default status, new subgroups created directly below the group inherit that configuration.

For more information, see [How groups inherit statuses](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## When a default status is hidden

If you hide a default status (by enabling the Hide status option for it), the system tries to set another status of the equivalent type as the default instead.

If there is no available status of the equivalent type, the status type displays as `Hidden` and is not available for work items.

![](assets/when-hide-default-status-no-equivalent-350x245.png)

