---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: View and Manage Subgroup Members
description: When you are viewing a group that you manage, you can view and manage all of the users in the group's subgroups.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
---
# View and manage subgroup members

When you are viewing a group that you manage, you can view and manage all of the users in the group's subgroups.

If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).

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
   <td> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level. </li> 
     <li> <p><b>Users</b> setting in your access level configured to <b>Edit</b> access, with <b>Create</b> and at least one of the two <b>User Admin</b> options enabled under <b>Fine-tune your settings</b> <img src="assets/gear-icon-settings.png">. </p> <p>Of these two options, if <b>User Admin (Group Users)</b> is enabled, you must be a group administrator of a group where the user is a member.</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## View and manage members of the subgroups under a group

{{step-1-to-setup}}

1. Click **Groups**.

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Click the name of the group for which you want to view or manage subgroup members.
1. In the left panel, click **Subgroup Members**.

   This left panel item is available only if the group has subgroups.

1. Do any of the following:

   * Select a member in the list, then click Edit ![](assets/edit-icon.png) to modify that person's user profile.

     For more information, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) or [Edit user profiles in bulk](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
   
   * Select any number of members in the list, then click Update ![](assets/comment-icon.png) to add a comment to their user profiles.

     The user or users receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates area in the user's profile.
   
   * Select any number of members in the list, then click Deactivate ![](assets/deactivate-user.png) or Activate ![](assets/activate-user.png).

     For more information, see [Deactivate or reactivate a user](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
   
   * Export ![](assets/export.png) the list of members.
