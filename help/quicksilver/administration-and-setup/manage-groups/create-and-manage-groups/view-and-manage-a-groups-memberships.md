---
user-type: administrator
product-area: system-administration;user-management
keywords: add,users,group,add,another,assign,administrator,remove,user,view,roles,members,export,membership,data
navigation-topic: create-and-manage-groups
title: View and Manage a Group's Memberships
description: As an Adobe Workfront administrator, you can view, add, remove, export, activate, and deactivate members of any group that you manage. You can also edit their profiles, add Updates to their profiles, and assign them as additional group administrators for the group.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
---
# View and manage a group's memberships

As an Adobe Workfront administrator, you can view, add, remove, export, activate, and deactivate members of any group that you manage. You can also edit their profiles, add Updates to their profiles, and assign them as additional group administrators for the group.

If there are any groups above your group, their administrators can also do these things for your group. The same is true for Workfront administrators (for any group).

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

## View and manage a group's memberships

{{step-1-to-setup}}

1. In the left panel, click **Groups**.

   In the list that displays, Workfront administrators can see all groups and subgroups. Group administrators can see only the groups and subgroups they administer.

1. Click the name of the group that you want to edit.
1. On the page that appears, with **Group Members** selected in the left menu, do any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Add a user to the group</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Click <strong>Add Members</strong> <img src="assets/add-icon-plus-in-circle.png">, start typing the user's name, then select it when it appears.</li> 
        <li value="2"> <p>Repeat this for any other users you want to add.</p> <p>You can click the X to the right of a name if you decide not to add that user.</p> </li> 
        <li value="3">Click <strong>Done</strong> when you are finished.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Remove a user from the group</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Select one or more user name, then click <strong>Remove member</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>Click <strong>Remove</strong> in the warning message that displays.</p> <p>You can find a user you want to remove from the list by clicking <strong>Search people and groups in the list</strong>, typing their name in the box, then clicking the name when it appears.</p> <p><b>NOTE</b>:  
          <ul> 
           <li>If this group is the Home Group for a user you want to remove, you must first assign another Home Group in the user's profile. For more information, see <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">Home Groups overview</a> and <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</li> 
           <li>If the group has only one group administrator and you need to remove him or her from the group, you need to assign another group administrator to the group first.</li> 
           <li>A user can belong individually to a subgroup as well as to the parent group. When you remove someone from a subgroup, they remain part of the parent group. Similarly, when you remove them from the parent group, they will remain part of the subgroup. If you do not want a user to have the access allowed for the parent group, you must remove the user both from the subgroups as well as the parent group, if they are listed in both places individually.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Edit a user's profile information</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Select one or more user name, then click <strong>Edit</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>Change the user's profile information.</p> <p>For information about the changes you can make, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Export user membership data</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Select one or more user name, then click <strong>Export</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>Export the data as a PDF, Excel, or tab delimited file.</p> <p>For more information about exporting data, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Export data</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">View and edit members' group roles</td> 
      <td> <p>The <strong>Group Role</strong> column lists each member's role. As a group administrator, you can double-click a member's role to change it.</p> <p>For members of the group who are not group administrators, this column is not editable.</p> <p>Group administrators are always at the top of the list.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Send a comment to group members</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Select one or more user name, then click <strong>Update</strong> <img src="assets/comment-icon.png">.</li> 
        <li value="2">Type the comment.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activate a user in Workfront</td> 
      <td>Select one or more inactive users, then click <strong>Activate user</strong> to activate them in Workfront. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deactivate a user in Workfront</td> 
      <td>Select one or more active users, then click <strong>Deactivate user</strong><img src="assets/deactivate-user.png"> to deactivate them in Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sort by column</td> 
      <td>Click the heading of a column to sort the list by the contents in that column.</td> 
     </tr> 
    </tbody> 
   </table>
