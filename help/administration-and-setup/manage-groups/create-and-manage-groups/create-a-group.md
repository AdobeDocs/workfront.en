---
filename: create-a-group
user-type: administrator
product-area: system-administration;user-management
keywords: create,group,subgroup,new
navigation-topic: create-and-manage-groups
title: Create a group
description: The highlighted information on this page refers to functionality available only in the new Workfront experience beta.
---

# Create a group

The highlighted information on this page refers to functionality available only in the new Workfront experience beta.

As an `Adobe Workfront administrator`, you can create groups to organize users and projects and to assign access rights within `Workfront`. For more information, see [Groups overview](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Every subgroup needs at least one `group administrator`. `Group administrators` can use the Groups page to manage their groups in one place.

If you are a `group administrator` or a `Workfront administrator`, you can also create subgroups under a group. For instructions, see [Create a subgroup](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

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

## Create a top-level group from scratch

These steps explain how to create a new group from scratch. For information about creating a group or subgroup by copying an existing one, see [Create a top-level group by copying an existing group or subgroup](#copying-an-existing-group-and-sub-group) in this article.

You must be a `Workfront administrator` to create a top-level group.

<ol data-mc-continue="false"> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Groups</span> <img src="assets/groups-icon.png">.</li> 
 <li value="3"> <p>Above the list of groups, click <span class="bold">New Group</span>.</p> <note type="tip">
   At the bottom of the list of groups, you can also click 
   <span class="bold">Add More Groups</span> to add a group in-line, then click 
   <span class="bold">Enter</span> when you are finished adding the group information.
  </note> </li> 
 <li value="4"> <p>In the <span class="bold">New Group</span> box that displays, type a name for the group.</p> </li> 
 <li value="5"> <p>Specify the following information:</p> 
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
     <td>Type a description for the <span>group</span>. You can type up to 512 characters.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Make this group and its subgroups public</td> 
     <td> <p>(Available only if you are viewing Details for a top-level group, not a subgroup.) Enable this option to allow users in the <span>group</span> with edit-user access (who are not administrators of the group) to add this group and its subgroups to the user profile of other users.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> <note type="note"> 
       <ul> 
        <li>You can’t make a subgroup public by itself, but you can make it’s top-level parent group public, which also makes all of the parent’s subgroups public.</li> 
        <li>A subgroup that belongs to a public group is public by default, so any user with edit-user access can add the subgroup to other users, as well.</li> 
       </ul> 
      </note> <p>If you need information about the access needed to edit users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>. For information about editing users, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Business Leader </td> 
     <td> <p>You can assign one user as a Business Leader for a <span>group</span> that you manage. A Business Leader is someone who makes business decisions for the <span>group</span>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Business Leader overview</a><span>.</span></p> <p>If the person is not already a member of the <span>group</span>, adding their name to this field also adds them to the group.</p> <note type="note"> 
       <ul> 
        <li>Before you can remove the Business Leader from a <span>group</span>, you must remove their name from the Business Leader field.</li> 
        <li>If you remove the name from the Business Leader field, that user remains a member of the <span>group</span> unless you remove them from it. For instructions on removing someone from a group, see the section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Manage a group’s memberships</a> in the article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Manage a group</a>.</li> 
       </ul> 
      </note> <p>For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Business Leader overview</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Group Members and Group Administrators</td> 
     <td> 
      <ul> 
       <li> <p>Group members: To add users and groups to the <span>group</span>, start typing the name of an existing user or group you want to add, then select the name when it appears.</p> <p>The users and groups that you add have access to all objects shared with the group.</p> </li> 
       <li> <p><span>Group administrators</span>: You can assign a group member as an administrator for the group using the drop-down menu to the right of the user’s name.</p> A top-level group must have at least 1 group administrator. </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Search people and groups in the list</td> 
     <td> If you need to find a user or group already assigned to this <span>group</span>, you can type their name here and select it when it appears.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6"> <p>Click <span class="bold">Create Group</span>.</p> </li> 
</ol>

## Create a top-level group by copying an existing group or subgroup

As a `Workfront administrator`, you can create a new top-level group by copying an existing group or subgroup.

Keep the following in mind when you want to do this:

* All of the members and any subgroups belonging to the existing group are copied to the new top-level group.
* The members of the copied group retain the assignments they had in the original group. Therefore, the `group administrators` of the original group are also designated as the `group administrators` in the copied group.

To create a new top-level group by copying a group or subgroup:

<ol data-mc-continue="false"> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>In the left panel, click <span class="bold">Groups</span> <img src="assets/groups-icon.png">.</p> <p>In the list of groups that displays, <span>group administrators</span> can see the groups they manage, as well as any subgroups of those groups. <span>Adobe Workfront administrators</span> can see all groups.<br></p> </li> 
 <li value="3">Select the group you want to copy, then click the Copy icon.</li> 
 <li value="4">In the <span class="bold">Copy Group</span> box that appears, type a <span class="bold">Group Name</span> for the copied group.<br></li> 
 <li value="5"> <p>Specify the following information:</p> 
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
     <td>Type a description for the <span>group</span>. You can type up to 512 characters.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Make this group and its subgroups public</td> 
     <td> <p>(Available only if you are viewing Details for a top-level group, not a subgroup.) Enable this option to allow users in the <span>group</span> with edit-user access (who are not administrators of the group) to add this group and its subgroups to the user profile of other users.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> <note type="note"> 
       <ul> 
        <li>You can’t make a subgroup public by itself, but you can make it’s top-level parent group public, which also makes all of the parent’s subgroups public.</li> 
        <li>A subgroup that belongs to a public group is public by default, so any user with edit-user access can add the subgroup to other users, as well.</li> 
       </ul> 
      </note> <p>If you need information about the access needed to edit users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Grant access to users</a>. For information about editing users, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Edit a user's profile</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Business Leader </td> 
     <td> <p>You can assign one user as a Business Leader for a <span>group</span> that you manage. A Business Leader is someone who makes business decisions for the <span>group</span>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader overview</a><span>.</span></p> <p>If the person is not already a member of the <span>group</span>, adding their name to this field also adds them to the group.</p> <note type="note"> 
       <ul> 
        <li>Before you can remove the Business Leader from a <span>group</span>, you must remove their name from the Business Leader field.</li> 
        <li>If you remove the name from the Business Leader field, that user remains a member of the <span>group</span> unless you remove them from it. For instructions on removing someone from a group, see the section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Manage a group’s memberships</a> in the article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Manage a group</a>.</li> 
       </ul> 
      </note> <p>For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader overview</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Group Members and Group Administrators</td> 
     <td> 
      <ul> 
       <li> <p>Group members: To add users and groups to the <span>group</span>, start typing the name of an existing user or group you want to add, then select the name when it appears.</p> <p>The users and groups that you add have access to all objects shared with the group.</p> </li> 
       <li> <p><span>Group administrators</span>:Any group administrators of the original group are also designated as the group administrators in the copied group. You can assign a group member as an administrator for the group using the drop-down menu to the right of the user’s name.</p> A top-level group must have at least 1 group administrator. </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Search people and groups in the list</td> 
     <td> If you need to find a user or group already assigned to this <span>group</span>, you can type their name here and select it when it appears.</td> 
    </tr> 
   </tbody> 
  </table> <note type="note"> 
   <ul> 
    <li>If the original group has subgroups, the subgroups are added to the new group, and their names are, by default, "The original subgroup name (Copy)".</li> 
    <li>You can eliminate any user or subgroup from the original group by clicking the X to the right of the user’s or subgroup’s name.</li> 
   </ul> 
  </note> </li> 
 <li value="6"> <p>Click <span class="bold">Create Group</span>.</p> </li> 
</ol>

##  

