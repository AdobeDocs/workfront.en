---
filename: manage-subgroups
user-type: administrator
product-area: system-administration;user-management
keywords: manage,subgroup,edit
navigation-topic: create-and-manage-subgroups
title: Manage a subgroup
description: As an group administrator of a subgroup, you can create, move, view, edit, copy, rename, export, and delete the subgroup.
---

# Manage a subgroup

As an group administrator of a subgroup, you can create, move,view, edit, copy, rename, export, and delete the subgroup.

If there are any groups above your group, their administrators can also do these things for your group. The same is true for Workfront administrators (for any group).

For more information about subgroups, see [Subgroups overview](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## Create, move,view, edit, copy, rename, export, or delete a subgroup

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Groups` ![](assets/groups-icon.png).

   In the list of groups that displays, group administrators can see the groups they manage, as well as any subgroups of those groups. Adobe Workfront administrators can see all groups.

1. Do any of the following:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Create a new subgroup</td> 
      <td> If you want to create the new subgroup one level down from the group you are viewing, click Add subgroup. Or, if you want to create the new subgroup beneath another subgroup in the list, select that subgroup, then click Add subgroup. <p>For information about the options you can use to configure the subgroup, see the table in <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Create a subgroup</a>.</p> <p>A group hierarchy cannot exceed 15 levels, but a single level can have an unlimited number of parallel groups.</p> </td> 
     </tr> Move a subgroup You can move existing subgroups under another group you administer. A group hierarchy cannot exceed 15 levels, but a single level can have an unlimited number of parallel groups. (Optional) Select a subgroup to make it the destination group. If you skip this step, the group you selected in step 3 is the destination group. Click Add Subgroup &gt; Existing Group. In the Existing Group box that appears, start typing the name of a subgroup you want to move. The results that display do not contain groups above the destination group. You can make sure you are selecting the right group by hovering over it and clicking the information icon that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators. Depending on the details configured for the group, you might also see its Business Leader and description. Click the name of the subgroup you want to move when you see it display in the list. Repeat Steps c-d for any other subgroups you want to move to the destination group Click Save. 
     <tr> 
      <td role="rowheader">Edit a subgroup</td> 
      <td> <p>Select the subgroup you want to edit, then click the Edit icon.</p> <p>For information about the options you can use to configure the subgroup, see the table in <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> </td> 
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
      <td> <p>(Available only for Workfront administrators.) When you copy a subgroup, it becomes a parent group. All group members and subgroups are copied with it. The groups members retain any assignments they had in the original group.</p> <p>For more information about copying a subgroup, see <a href="#copying" class="MCXref xref">Copying a subgroup</a> in this article.</p> 
       <ol> 
        <li value="1">Select a subgroup, then click the Copy icon to create a new top-level group based on the selected group.</li> 
        <li value="2"> <p>Configure the new group’s settings.</p> <p>For help with these settings, see the table in the section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Create a top-level group by copying an existing group or subgroup</a> in the article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Create a top-level group by copying an existing group or subgroup</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Delete a subgroup</td> 
      <td> <p>Important: When you delete a group or subgroup, you need to preserve the users, work items, and any subgroups that are currently assigned to it. To help you make sure they are preserved, a prompt requires you to reassign the group’s objects to a different group in the step below.</p> 
       <ol> 
        <li value="1">Select the subgroup, then click the Delete icon.</li> 
        <li value="2">In the <span class="bold">Delete Group</span> box that appears, starting typing and then select the name of the group where you want to move the members, work items, and subgroups of the group you are deleting.</li> 
        <li value="3">Click <span class="bold">Delete Them</span>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

` `**Tip: **`` When you are managing a group that contains subgroups, it’s helpful to be able to identify and filter data about the entire group and all of its subgroups. You can do this by using the Top Parent ID field in a report or list.

For example, imagine that you manage a large Marketing department and you want a list of all of the projects that the entire department is working on.

In Workfront, this Marketing department is represented by a group called Marketing, with 3 subgroups called Field Marketing, Product Marketing, and Digital Marketing. To list the projects that belong to the entire Marketing department (all 4 groups), you could create a Filter for the Projects area with the following Filter Rule:

```
Group: Top Parent ID > Equal > Marketing
```

You can also use the Top Parent Name field to identify data associated with a top-level group, but only in Views, not in Filters or Groupings.
View and manage a group’s subgroup members When you are viewing the main page of a group you administer, you can view and manage all of the users in the group’s subgroups. For instructions, see View and manage subgroup members. 

## Copying a subgroup

Consider the following when you copy a subgroup.

* If a subgroup you copy has its own subgroups, they are included in the copy and their names are formatted as follows:

  *Original subgroup name* (Copy)

* Any subgroup that belongs to a public group is also public, so any user with edit-user access, in or out of the group, can add users to the subgroup.

