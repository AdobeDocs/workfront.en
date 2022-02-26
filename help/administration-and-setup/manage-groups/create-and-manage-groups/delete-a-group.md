---
filename: delete-a-group
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Delete a group
description: You can delete a group that you manage. If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).
---

# Delete a group

You can delete a group that you manage. If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for *Workfront administrators* (for any group).

For information about deleting a subgroup, see [Manage a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> <p>You must be a <em>group administrator</em> of the group or a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *Workfront administrator*.

## Delete a group

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Groups</span> <img src="assets/groups-icon.png">.</li> 
 <li value="3"> <p>Select the group you want to delete, then click <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     the Delete icon 
     <img src="assets/delete.png">
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    the Delete icon 
    <img src="assets/delete.png">
   </MadCap:conditionalText>.</p> <note type="important">
   When you delete a group or subgroup, you need to preserve the users, work items, and any subgroups that are currently assigned to it. To help you make sure they are preserved, a prompt requires you to reassign the group’s objects to a different group in the step below.
  </note> </li> 
 <li value="4"> <p>In the <span class="bold">Delete Group</span> box that appears, starting typing and then select the name of the group where you want to move the members, work items, and subgroups of the group you are deleting.</p> <p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.<draft-comment>
    <MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
      Depending on the details configured for the group, you might also see its Business Leader and description.
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
     Depending on the details configured for the group, you might also see its Business Leader and description.
   </MadCap:conditionalText></p> </li> 
 <li value="5">Click <span class="bold">Delete Them</span>.</li> 
</ol>

