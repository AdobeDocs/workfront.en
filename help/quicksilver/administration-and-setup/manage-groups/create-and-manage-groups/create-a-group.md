---
user-type: administrator
product-area: system-administration;user-management
keywords: create,group,subgroup,new
navigation-topic: create-and-manage-groups
title: Create a Group
description: As an Adobe Workfront administrator, you can create groups to organize users and projects and to assign access rights within Workfront.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
---
# Create a group

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

As an Adobe Workfront administrator, you can create groups to organize users and projects and to assign access rights within Workfront. For more information, see [Groups overview](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Every subgroup needs at least one group administrator. Group administrators can use the Groups page to manage their groups in one place.

If you are a group administrator or a Workfront administrator, you can also create subgroups under a group. For instructions, see [Create a subgroup](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

+++

## Create a top-level group from scratch

These steps explain how to create a new group from scratch. For information about creating a group or subgroup by copying an existing one, see [Create a top-level group by copying an existing group or subgroup](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) in this article.

You must be a Workfront administrator to create a top-level group.

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![](assets/groups-icon.png).

1. Above the list of groups, click **New Group**.

   >[!TIP]
   >
   >At the bottom of the list of groups, you can also click **Add More Groups** to add a group in-line, then click **Enter** when you are finished adding the group information.

1. In the **New Group** box that displays, type a name for the group.
1. Specify the following information:

   <table style="table-layout:auto"> 
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
      <td role="rowheader">Is Active</td> 
      <td> <p>(Enabled by default) Makes the group active in your Workfront instance.</p> <p>In type-ahead fields like the one shown below, when regular users search for a group to attach it to an object or to share an object with it, only active groups display in the list.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>To streamline this for your users, you can disable the Is Active option for groups that are not currently in use.</p> <p>You can easily view, filter and group the Groups list based on active or inactive status using this field. For information about using views, filters, and groupings in lists, see <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Reporting elements: filters, views, and groupings</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Make this group and its subgroups public</td> 
      <td> <p>(Available only if you are viewing Details for a top-level group, not a subgroup.) Enable this option to allow users in the group with edit-user access (who are not administrators of the group) to add this group and its subgroups to the user profile of other users.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> <p><b>NOTE</b>:  
        <ul> 
         <li>You can't make a subgroup public by itself, but you can make its top-level parent group public, which also makes all of the parent's subgroups public.</li> 
         <li>A subgroup that belongs to a public group is public by default, so any user with edit-user access can add the subgroup to other users, as well.</li> 
        </ul> </p> <p>If you need information about the access needed to edit users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>. For information about editing users, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>You can assign one user as a Business Leader for a group that you manage. A Business Leader is someone who makes business decisions for the group. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Business Leader overview</a><span>.</span></p> <p>If the person is not already a member of the group, adding their name to this field also adds them to the group.</p> <p><b>NOTE</b>:  
        <ul> 
         <li>Before you can remove the Business Leader from a group, you must remove their name from the Business Leader field.</li> 
         <li>If you remove the name from the Business Leader field, that user remains a member of the group unless you remove them from it. For instructions on removing someone from a group, see the section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Manage a group's memberships</a> in the article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Manage a group</a>.</li> 
        </ul> </p> <p>For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Business Leader overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Group Members and Group Administrators</td> 
      <td>
        <p>To add group members, start typing the name of an existing user or group you want to add, then select the name when it appears.</p> 
        <p>Users and groups that you add have access to all objects shared with the group.</p>
        <p>A top-level group must have at least one group administrator. </p>
     </tr> 
     <tr> 
      <td role="rowheader">Search people and groups in the list</td> 
      <td> If you need to find a user or group already assigned to this group, you can type their name here and select it when it appears.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Create Group**.

## Create a top-level group by copying an existing group or subgroup {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

As a Workfront administrator, you can create a new top-level group by copying an existing group or subgroup.

Keep the following in mind when you want to do this:

* All of the members and any subgroups belonging to the existing group are copied to the new top-level group.
* The members of the copied group retain the assignments they had in the original group. Therefore, the group administrators of the original group are also designated as the group administrators in the copied group.

To create a new top-level group by copying a group or subgroup:

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![](assets/groups-icon.png).

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Select the group you want to copy, then click the Copy icon ![](assets/copy-icon.png).
1. In the **Copy Group** box that appears, type a **Group Name** for the copied group.  

1. Specify the following information:

   <table style="table-layout:auto"> 
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
      <td role="rowheader">Is Active</td> 
      <td> <p>(Enabled by default) Makes the group active in your Workfront instance.</p> <p>In type-ahead fields like the one shown below, when regular users search for a group to attach it to an object or to share an object with it, only active groups display in the list.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>To streamline this for your users, you can disable the Is Active option for groups that are not currently in use.</p> <p>You can easily view, filter and group the Groups list based on active or inactive status using this field. For information about using views, filters, and groupings in lists, see <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Reporting elements: filters, views, and groupings</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Make this group and its subgroups public</td> 
      <td> <p>(Available only if you are viewing Details for a top-level group, not a subgroup.) Enable this option to allow users in the group with edit-user access (who are not administrators of the group) to add this group and its subgroups to the user profile of other users.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> <p><b>NOTE</b>:  
        <ul> 
         <li>You can't make a subgroup public by itself, but you can make it's top-level parent group public, which also makes all of the parent's subgroups public.</li> 
         <li>A subgroup that belongs to a public group is public by default, so any user with edit-user access can add the subgroup to other users, as well.</li> 
        </ul> </p> <p>If you need information about the access needed to edit users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Grant access to users</a>. For information about editing users, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Edit a user's profile</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>You can assign one user as a Business Leader for a group that you manage. A Business Leader is someone who makes business decisions for the group. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader overview</a><span>.</span></p> <p>If the person is not already a member of the group, adding their name to this field also adds them to the group.</p> <p><b>NOTE</b>:  
        <ul> 
         <li>Before you can remove the Business Leader from a group, you must remove their name from the Business Leader field.</li> 
         <li>If you remove the name from the Business Leader field, that user remains a member of the group unless you remove them from it. For instructions on removing someone from a group, see the section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Manage a group's memberships</a> in the article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Manage a group</a>.</li> 
        </ul> </p> <p>For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Group Members and Group Administrators</td> 
      <td> 
       <ul> 
        <li> <p>Group members: To add users and groups to the group, start typing the name of an existing user or group you want to add, then select the name when it appears.</p> <p>The users and groups that you add have access to all objects shared with the group.</p> </li> 
        <li> <p>Group administrators: Any group administrators of the original group are also designated as the group administrators in the copied group. You can assign a group member as an administrator for the group using the drop-down menu to the right of the user's name.</p> <p>A top-level group must have at least one group administrator.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Search people and groups in the list</td> 
      <td> If you need to find a user or group already assigned to this group, you can type their name here and select it when it appears.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* If the original group has subgroups, the subgroups are added to the new group, and their names are, by default, "The original subgroup name (Copy)."
   >* You can eliminate any user or subgroup from the original group by clicking the X to the right of the user's or subgroup's name.

1. Click **Create Group**.
