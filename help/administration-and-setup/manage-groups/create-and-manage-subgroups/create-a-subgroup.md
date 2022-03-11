---
filename: create-a-subgroup
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Create a subgroup
description: The highlighted information on this page refers to functionality available only in the new Workfront experience beta.
---

# Create a subgroup

The highlighted information on this page refers to functionality available only in the new Workfront experience beta.

You can create a subgroup under a group you manage to organize users and projects and to assign access rights within `Adobe Workfront`.

If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for `Workfront administrators` (for any group).

Typically, however, `group administrators` manage groups and subgroups. They can use the Groups page to manage their groups and subgroups in one place. For information about how groups and subgroups work within `Workfront`, see [Groups overview](../../../administration-and-setup/manage-groups/groups-overview/groups.md) and [Subgroups overview](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> <p>You must be a <span>group administrator</span> of the group or a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your `Workfront administrator`.

## Add a subgroup

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>Click <span class="bold">Groups</span>.</p> <p>In the list of groups that displays, <span>group administrators</span> can see the groups they manage, as well as any subgroups of those groups. <span>Adobe Workfront administrators</span> can see all groups.</p> </li> 
 <li value="3"> <p>Select the existing group or subgroup where you want to add a new subgroup.</p> </li> 
 <li value="4"> <p>Click <span class="bold">New Subgroup</span>.</p> </li> 
 <li value="5"> <p>In the <span class="bold">New Subgroup</span> box that appears, type a <span class="bold">Group Name</span> for the subgroup.</p> </li> 
 <li value="6"> <p>(Optional) specify any of the following information:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Group Name</td> 
     <td>Change the name of the group.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Description</td> 
     <td>Type a description for the <span>subgroup</span>. You can type up to 512 characters.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Make this group and its subgroups public</td> 
     <td> <p>(Available only if you are viewing Details for a top-level group, not a subgroup.) Enable this option to allow users in the <span>subgroup</span> with edit-user access (who are not administrators of the group) to add this group and its subgroups to the user profile of other users.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> <note type="note"> 
       <ul> 
        <li>You can’t make a subgroup public by itself, but you can make it’s top-level parent group public, which also makes all of the parent’s subgroups public.</li> 
        <li>A subgroup that belongs to a public group is public by default, so any user with edit-user access can add the subgroup to other users, as well.</li> 
       </ul> 
      </note> <p>If you need information about the access needed to edit users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Grant access to users</a>. For information about editing users, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Edit a user's profile</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Business Leader </td> 
     <td> <p>You can assign one user as a Business Leader for a <span>subgroup</span> that you manage. A Business Leader is someone who makes business decisions for the <span>subgroup</span>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader overview</a><span>.</span></p> <p>If the person is not already a member of the <span>subgroup</span>, adding their name to this field also adds them to the group.</p> <note type="note"> 
       <ul> 
        <li>Before you can remove the Business Leader from a <span>subgroup</span>, you must remove their name from the Business Leader field.</li> 
        <li>If you remove the name from the Business Leader field, that user remains a member of the <span>subgroup</span> unless you remove them from it. For instructions on removing someone from a group, see the section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Manage a group’s memberships</a> in the article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Manage a group</a>.</li> 
       </ul> 
      </note> <p>For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader overview</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Group Members and Group Administrators</td> 
     <td> 
      <ul> 
       <li> <p>Group members: To add users and groups to the <span>subgroup</span>, start typing the name of an existing user or group you want to add, then select the name when it appears.</p> <p>The users and groups that you add have access to all objects shared with the group.</p> </li> 
       <li> <p><span>Group administrators</span>:A subgroup inherits the group administrators of the group above it, so specifying a user as a group administrator for a subgroup is optional. You can assign a group member as an administrator for the group using the drop-down menu to the right of the user’s name.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Search people and groups in the list</td> 
     <td> If you need to find a user or group already assigned to this <span>subgroup</span>, you can type their name here and select it when it appears.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="7">Click <span class="bold">Save.</span></li> 
</ol>

