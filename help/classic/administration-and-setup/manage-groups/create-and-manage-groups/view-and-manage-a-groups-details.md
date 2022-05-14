---
title: View and manage a group’s details
description: View and manage a group’s details
draft: Probably
---
# View and manage a group’s details

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can view and manage the main details for a group you administer. These include the group’s name, description, Business Leader, and group administrators. You can also make the group and all of its subgroups public or private.

For information about other ways you can manage a group, see [Create a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Access requirements

You must have the following to perform the steps in this article:

<table> 
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

## View and manage a group’s details

1. Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.
1. Click **Groups**.

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Click the name of the top-level group that you want to edit.
1. If you want to deactivate or reactivate the group, 
1. In the box that displays, make any of the following changes:

   <table> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Group Name</td> 
      <td>Change the name of the group.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Type a description for the group. You can type up to 512 characters.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Make this group and its subgroups public</td> 
      <td> <p>(Available only if you are viewing Details for a top-level group, not a subgroup.) Enable this option to allow users in the group with edit-user access (who are not administrators of the group) to add this group and its subgroups to the user profile of other users.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> <p>Note:  
        <ul> 
         <li>You can’t make a subgroup public by itself, but you can make it’s top-level parent group public, which also makes all of the parent’s subgroups public.</li> 
         <li>A subgroup that belongs to a public group is public by default, so any user with edit-user access can add the subgroup to other users, as well.</li> 
        </ul> </p> <p>If you need information about the access needed to edit users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>. For information about editing users, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>You can assign one user as a Business Leader for a group that you manage. A Business Leader is someone who makes business decisions for the group. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Business Leader overview</a><span>.</span></p> <p>If the person is not already a member of the group, adding their name to this field also adds them to the group.</p> <p>Note:  
        <ul> 
         <li>Before you can remove the Business Leader from a group, you must remove their name from the Business Leader field.</li> 
         <li>If you remove the name from the Business Leader field, that user remains a member of the group unless you remove them from it. For instructions on removing someone from a group, see the section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Manage a group’s memberships</a> in the article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Manage a group</a>.</li> 
        </ul> </p> <p>For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Business Leader overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Group Members and Group Administrators</td> 
      <td> 
       <ul> 
        <li> <p>Group members: To add users and groups to the group, start typing the name of an existing user or group you want to add, then select the name when it appears.</p> <p>The users and groups that you add have access to all objects shared with the group.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.groups">A top-level group must have at least 1 group administrator.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Search people and groups in the list</td> 
      <td> If you need to find a user or group already assigned to this group, you can type their name here and select it when it appears.</td> 
     </tr> 
    </tbody> 
   </table>

