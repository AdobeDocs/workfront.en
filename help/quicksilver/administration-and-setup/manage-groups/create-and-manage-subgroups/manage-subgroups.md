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

As a group administrator of a subgroup, you can create, move, view, edit, copy, rename, export, and delete the subgroup.

You can also make a subgroup a top-level group by removing it from its parent group.

If there are any groups above your group, their administrators can also do these things for your group. The same is true for Workfront administrators (for any group).

For more information about subgroups, see [Subgroups overview](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

>[!TIP]
>
>When you are managing a group that contains subgroups, it's helpful to be able to identify and filter data about the entire group and all of its subgroups. You can do this by using the Top Parent ID field in a report or list.
>
>For example, imagine that you manage a large Marketing department and you want a list of all of the projects that the entire department is working on.
>
>In Workfront, this Marketing department is represented by a group called Marketing, with 3 subgroups called Field Marketing, Product Marketing, and Digital Marketing. To list the projects that belong to the entire Marketing department (all 4 groups), you could create a filter for the Projects area with the following filter rule:
>
>`Group: Top Parent ID > Equal > Marketing`
>
>You can also use the Top Parent Name field to identify data associated with a top-level group, but only in views, not in filters or groupings.

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
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p>
       <p>Or</p>
       <p>Current: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>You must be a group administrator of the group or a system administrator.</td>
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create a subgroup

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![Groups](assets/groups-icon.png).

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Click the name of the group where you want to add a subgroup.
1. In the left menu, click **Subgroups**.
1. To create the a new subgroup one level down from the group you are viewing, click **Add subgroup**.

   Or, if you want to create the new subgroup beneath another subgroup in the list, select that subgroup, then click Add subgroup.
   
   For information about the options you can use to configure the subgroup, see [Create a subgroup](help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
   
   A group hierarchy cannot exceed 15 levels, but a single level can have an unlimited number of parallel groups.

## Move a subgroup

You can move existing subgroups under another group you administer.

A group hierarchy cannot exceed 15 levels, but a single level can have an unlimited number of parallel groups.

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![Groups](assets/groups-icon.png).

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Click the name of the destination group (you will specify which subgroups you want to move in a later step).
1. In the left menu, click **Subgroups**.
1. (Optional) Select a subgroup to make it the destination group.
   
   If you skip this step, the group you selected in step 3 is the destination group.

1. Click **Add Subgroup > Existing Group**.
1. In the **Existing Group** box that appears, start typing the name of a subgroup you want to move.

   The results that display do not contain groups above the destination group.
   
   You can make sure you are selecting the right group by hovering over it and clicking the information icon ![information icon](assets/info-icon.png) that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.

1. Select the name of the subgroup you want to move when you locate it in the list.
1. Repeat Steps 7-8 for any other subgroups you want to move to the destination group
1. Click **Save**.

## Edit a subgroup

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![Groups](assets/groups-icon.png).

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Click the name of the group that contains the subgroup you want to edit.
1. In the left menu, click **Subgroups**.
1. Select the subgroup you want to edit, then click the **Edit** icon ![Edit icon](assets/edit-icon.png).

   For information about the options you can use to configure the subgroup, see [Create a subgroup](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Copy a subgroup

>[!NOTE]
>
>Only a system administrator can copy a subgroup.

When you copy a subgroup, it becomes a parent group. All group members and subgroups are copied with it. The group's members retain any assignments they had in the original group.

Consider the following when you copy a subgroup:

* If a subgroup you copy has its own subgroups, they are included in the copy and their names are formatted as follows:

  `Original subgroup name (Copy)`

* Any subgroup that belongs to a public group is also public, so any user with access to edit users, in or out of the group, can add users to the subgroup.

To copy a subgroup:

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![Groups](assets/groups-icon.png).

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Click the name of the group that contains the subgroup you want to copy.
1. In the left menu, click **Subgroups**.
1. Select a subgroup, then click the **Copy** icon ![Copy icon](assets/copy-icon.png) to create a new top-level group based on the selected group.
1. Configure the new group's settings.

   For help with these settings, see the table the section [Create a top-level group by copying an existing group or subgroup](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) in the article [Create a group](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

1. Click **Create group**.

## Remove a subgroup from its parent group and make it a top-level group

You can make a subgroup a top-level group by removing it from its parent group.

>[!TIP]
>
>When you deactivate a group that has subgroups below it, those subgroups also become inactive. If you want one of them to be active, you can use these instructions to remove it from its parent group, then reactivate it.
>For instructions on deactivating and reactivating groups, see [Deactivate or reactivate a group](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![Groups](assets/groups-icon.png).
1. Select the parent group of the group you want to make a top-level group, then click the **Edit** icon ![Edit icon](assets/edit-icon.png).
1. In the **Edit Group** box that appears, under **Group members and Group administrators**, start typing the name of the subgroup that you want to make a top-level group, then click the X to the right of its name it when it appears.
1. Click **Save**.

## Delete a subgroup

>[!IMPORTANT]
>
>When you delete a group or subgroup, you need to preserve the users, work items, and any subgroups that are currently assigned to it. To help you make sure they are preserved, a prompt requires you to reassign the group's objects to a different group.

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![Groups](assets/groups-icon.png).

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Click the name of the group that contains the subgroup you want to delete.
1. In the left menu, click **Subgroups**.
1. Select the subgroup, then click the **Delete** icon ![Delete icon](assets/delete.png).

   In the **Delete Group** box that appears, start typing and then select the name of the group where you want to move the members, work items, and subgroups of the group you are deleting.

1. Click **Delete It**.

## View and manage a group's subgroup members

When you are viewing the main page of a group you administer, you can view and manage all of the users in the group's subgroups. For instructions, see [View and manage subgroup members](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

