---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Custom Statuses in a Group that Is Moved or Deleted
description: This article explains what happens to group custom statuses when you move or delete a group.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
---
# Custom statuses in a group that is moved or deleted

This article explains what happens to group custom statuses when you move or delete a group.

## Customized statuses in a group that is moved

Consider the following scenarios describing what happens to group custom statuses when you move one group to a new location under another group.

For information about moving a group, see [Move a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">When you move a group under another group </td> 
   <td> <p>All of the moved group's statuses remain with it. They are not added to the statuses of the group's new parent group.</p> <p>But the moved group inherits any locked statuses in the group or groups that are now higher in its hierarchy. And, from now on, if an administrator locks a status higher in the hierarchy, the moved group inherits that status.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">When a status in both groups has the same key but different attributes</td> 
   <td> <p>Suppose that two different subgroups inherit the same unlocked status from a parent group. The group administrators of the 2 groups then customize the status for their groups in different ways.</p> <p>Later, one of the two groups is moved under the other one. Now they both have a status with the same key, but it has different attributes in the two groups.</p> <p>In this case, one of the following is true:</p> 
    <ul> 
     <li>If the status in the new parent group is unlocked, the status in the moved group retains its attributes, unaffected by the move.</li> 
     <li>If the status in the new parent group is locked, the attributes of the status in the parent group override those of the status in the moved group.</li> 
    </ul> <p>For information about status keys, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>When a moved group has statuses inherited from its previous parent group </td> 
   <td> <p>All custom statuses inherited from the previous parent group come with the moved group and become its own custom statuses. They are no longer connected with the previous parent group.</p> 
    <ul> 
     <li>If the previous parent group edits a locked custom status after the move, the changes do not affect the moved subgroup's status.</li> 
     <li>If the previous parent group locks a custom status that was unlocked when the group moved, the moved subgroup's status is not locked.</li> 
     <li>The moved group can now unlock statuses that were locked when it inherited them from the previous parent group.</li> 
    </ul> 
     <p><b>EXAMPLE:</b><p> 
     <p>Olivia, the group administrator for the Marketing group, creates two statuses for the group. She names one First Review, with the key ABC, and locks it. She names the other Final Review, with the key XYZ, and doesn't lock it.</p> 
     <p>She also creates a subgroup under the Marketing group called Product Marketing. At the moment when it's created, it automatically inherits both First Review and Final Review from the Marketing group.</p> 
     <p>Later, Olivia moves the Product Marketing subgroup under the Product group. Both First Review and Final Review go with the Product Marketing group to its new location under the Product group.</p> 
     <p>Though First Review was locked before the move, the Product Marketing group administrator can edit it now because it's no longer an inherited status controlled by the parent group it came from.</p> 
     <p>Final Review is unlocked and editable as it always was.</p> 
     <p>For the Marketing group, Olivia changes the colors of First Review and Final Review and renames them First Review-Edited and Final Review-Edited. She also locks Final Review-Edited. Meanwhile, in the Product Marketing group, the colors and names of the statuses First Review and Final Review don't change.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Customized statuses in a group that is deleted

When you delete a group or subgroup, you reassign the information associated with it, including its customized statuses, to another group or subgroup. The deleted group's statuses are added to those of the destination group.

If one of the deleted group's statuses was also being used by the destination group (the status in both groups has the same key), and the destination group customized the status in different ways, the settings of the destination group's version override the settings of the moved group's version.

>[!INFO]
>
>**EXAMPLE:** 
>
>The group administrator of Group A renames an unlocked system-level status for her group. The group administrator of a Group B also renames that status for his group. Though the status has different names in the two groups, it has the same key.
>
>Later, Group A is deleted and all of its information is reassigned to Group B.
>
>* The name of Group B version of the status overrides the name of the Group A version.
>* If the status was applied to an object by someone in Group A before that group was deleted, the status name on the object updates to the name for the status used by Group B.
>
>For information about the key for a status, see the table in this article under [Create or edit a custom status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [Create or edit a status for a group](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>For information about deleting a group, see [Delete a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
