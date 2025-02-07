---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Delete a Group
description: You can delete a group that you manage. If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f92eb1f5-fe98-4c7e-8ef7-8ed7134db8d4
---
# Delete a group

You can delete a group that you manage. If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).

For information about deleting a subgroup, see [Manage a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md).

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

## Delete a group

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![Groups](assets/groups-icon.png).

1. Select the group you want to delete, then click the Delete icon ![Delete](assets/delete.png).

   >[!IMPORTANT]
   >
   >When you delete a group or subgroup, you need to preserve the users, work items, and any subgroups that are currently assigned to it. To help you make sure they are preserved, a prompt requires you to reassign the group's objects to a different group in the step below.

1. In the **Delete Group** box that appears, starting typing and then select the name of the group where you want to move the members, work items, and subgroups of the group you are deleting.

   You can make sure you are selecting the right group by hovering over it and clicking the information icon ![Info icon](assets/info-icon.png) that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.

1. Click **Delete Them**.
