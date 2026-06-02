---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-groups
title: Move a Group
description: You can move a group under another group that you manage.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f5227454-457d-40d3-865c-c2551471d83e
TQID: https://experienceleague.adobe.com/r3oRazPj4LJxhrSJZxtH6ADtOVjLg3UT2pbRlXbLHmA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Move a group

You can move a group under another group that you manage.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Access level configurations</td> 
   <td>You must be a group administrator of the group or a system administrator.</td>
  </tr>
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Move a group under another group

>[!NOTE]
>
>If the statuses of the moved group are locked, it inherits the statuses of its new parent group.
>
>If the statuses of the moved group are unlocked, it does not inherit the statuses of its new parent group, nor does the new parent group take on its statuses.
>
>For more information about group statuses, see [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) and [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![Groups](assets/groups-icon.png).

1. Select the destination group where you want to move the group, then click the Edit icon ![Edit icon](assets/edit-icon.png). 
1. In the **Edit Group** box that appears, under **Group Members and Group Administrators**, start typing the name of the group you want to move, then click it when it appears.
1. Click **Save**.

>[!TIP]
>
>You can also make a subgroup a top-level group. For instructions, see the section [Remove a subgroup from its parent group and make it a top-level group](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) in the article [Manage a subgroup](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
