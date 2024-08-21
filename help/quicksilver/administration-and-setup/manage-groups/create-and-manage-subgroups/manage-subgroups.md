---
user-type: administrator
product-area: system-administration;user-management
keywords: manage,subgroup,edit
navigation-topic: create-and-manage-subgroups
title: Manage a Subgroup
description: As an group administrator of a subgroup, you can create, move, view, edit, copy, rename, export, and delete the subgroup. You can also make a subgroup a top-level group by removing it from its parent group.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
---
# Manage a subgroup

As an group administrator of a subgroup, you can create, move, view, edit, copy, rename, export, and delete the subgroup.

You can also make a subgroup a top-level group by removing it from its parent group.

If there are any groups above your group, their administrators can also do these things for your group. The same is true for Workfront administrators (for any group).

For more information about subgroups, see [Subgroups overview](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## Create, move, view, edit, copy, rename, export, or delete a subgroup

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![](assets/groups-icon.png).

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Click the name of the group that contains the subgroup you want to work on.

   Or

   If you are moving one or more subgroups, click the name of the destination group (you will specify which subgroups you want to move in a later step).

1. In the left menu, click **Subgroups**.

1. Do any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Create a new subgroup</td> 
      <td> <p>If you want to create the new subgroup one level down from the group you are viewing, click <strong>Add subgroup</strong>.</p> <p>Or, if you want to create the new subgroup beneath another subgroup in the list, select that subgroup, then click <strong>Add s</strong><strong>ubgroup</strong>.</p> <p>For information about the options you can use to configure the subgroup, see the table in <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Create a subgroup</a>.</p> <p>A group hierarchy cannot exceed 15 levels, but a single level can have an unlimited number of parallel groups.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Move a subgroup </td> 
      <td> <p>You can move existing subgroups under another group you administer.</p> <p>A group hierarchy cannot exceed 15 levels, but a single level can have an unlimited number of parallel groups.</p> 
       <ol> 
        <li value="1"> <p>(Optional) Select a subgroup to make it the destination group.</p> <p>If you skip this step, the group you selected in step 3 is the destination group.</p> </li> 
        <li value="2">Click <strong>Add Subgroup</strong> &gt; <strong>Existing Group</strong>.</li> 
        <li value="3"> <p>In the <strong>Existing Group</strong> box that appears, start typing the name of a subgroup you want to move.</p> <p>The results that display do not contain groups above the destination group.</p> <p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> </li> 
        <li value="4"> <p>Click the name of the subgroup you want to move when you see it display in the list.</p> </li> 
        <li value="5"> <p>Repeat Steps c-d for any other subgroups you want to move to the destination group</p> </li> 
        <li value="6">Click <strong>Save</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Edit a subgroup</td> 
      <td> <p>Select the subgroup you want to edit, then click the Edit icon <img src="assets/edit-icon.png">.</p> <p>For information about the options you can use to configure the subgroup, see the table in <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Export one or more subgroups</td> 
      <td> 
       <ol> 
        <li value="1">Select the subgroup or subgroups you want to export.</li> 
        <li value="2">Click the Export icon <img src="assets/export.png">, then select the file format you want.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copy a subgroup to create a new top-level group</td> 
      <td> <p>(Available only for Workfront administrators.) When you copy a subgroup, it becomes a parent group. All group members and subgroups are copied with it. The groups members retain any assignments they had in the original group.</p> <p>For more information about copying a subgroup, see <a href="#about-copying-a-subgroup" class="MCXref xref">About copying a subgroup</a> in this article.</p> 
       <ol> 
        <li value="1">Select a subgroup, then click the Copy icon <img src="assets/copy-icon.png"> to create a new top-level group based on the selected group.</li> 
        <li value="2"> <p>Configure the new group's settings.</p> <p>For help with these settings, see the table in the section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Create a top-level group by copying an existing group or subgroup</a> in the article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Create a top-level group by copying an existing group or subgroup</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Delete a subgroup</td> 
      <td> <p><b>IMPORTANT</b>: When you delete a group or subgroup, you need to preserve the users, work items, and any subgroups that are currently assigned to it. To help you make sure they are preserved, a prompt requires you to reassign the group's objects to a different group in the step below.</p> 
       <ol> 
        <li value="1">Select the subgroup, then click the Delete icon <img src="assets/delete.png">.</li> 
        <li value="2">In the <strong>Delete Group</strong> box that appears, starting typing and then select the name of the group where you want to move the members, work items, and subgroups of the group you are deleting.</li> 
        <li value="3">Click <strong>Delete Them</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>When you are managing a group that contains subgroups, it's helpful to be able to identify and filter data about the entire group and all of its subgroups. You can do this by using the Top Parent ID field in a report or list.
>
>For example, imagine that you manage a large Marketing department and you want a list of all of the projects that the entire department is working on.
>
>In Workfront, this Marketing department is represented by a group called Marketing, with 3 subgroups called Field Marketing, Product Marketing, and Digital Marketing. To list the projects that belong to the entire Marketing department (all 4 groups), you could create a Filter for the Projects area with the following Filter Rule:
>
>`Group: Top Parent ID > Equal > Marketing`
>
>You can also use the Top Parent Name field to identify data associated with a top-level group, but only in Views, not in Filters or Groupings.

## Remove a subgroup from its parent group and make it a top-level group

You can make a subgroup a top-level group by removing it from its parent group.

>[!TIP]
>
>When you deactivate a group that has subgroups below it, those subgroups also become inactive. If you want one of them to be active, you can use these instructions to remove it from its parent group, then reactivate it.
>
>For instructions on deactivating and reactivating groups, see the sections [View and manage a group's details](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) and [View and manage a group's details](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) in the article [View and manage a group's details](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![](assets/groups-icon.png).

1. Select the parent group of the group you want to make a top-level group, then click the Edit icon ![](assets/edit-icon.png). 
1. In the **Edit Group** box that appears, under **Group Members and Group Administrators**, start typing the name of the subgroup that you want to make a top-level group, then click the X to the right of its name it when it appears.
1. Click **Save**.

## View and manage a group's subgroup members

When you are viewing the main page of a group you administer, you can view and manage all of the users in the group's subgroups. For instructions, see [View and manage subgroup members](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## About copying a subgroup {#about-copying-a-subgroup}

Consider the following when you copy a subgroup.

* If a subgroup you copy has its own subgroups, they are included in the copy and their names are formatted as follows:

  `Original subgroup name (Copy)`

* Any subgroup that belongs to a public group is also public, so any user with edit-user access, in or out of the group, can add users to the subgroup.
