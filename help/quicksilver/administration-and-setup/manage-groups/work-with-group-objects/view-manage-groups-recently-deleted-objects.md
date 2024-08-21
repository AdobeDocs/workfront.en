---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: View and Manage a Group's Recently Deleted Items
description: When you are viewing a group that you manage in the Groups area, you can view, filter, restore, and export its recently deleted work items, documents, and templates.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
---
# View and manage a group's recently deleted items

When you are viewing a group that you manage in the Groups area, you can view and work with its recently deleted projects, tasks, issues, documents, and templates in the following ways:

* View, filter, and group a list of recently deleted items
* Restore recently deleted items that you select
* Export a list of recently deleted items

If there are any groups above your group, their administrators can also do these things for your group. The same is true for Workfront administrators (for any group).

For more information about deleted items, see [Manage deleted items](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>The deleted items must be associated with the group or any of its subgroups. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

+++

## View and manage a group's recently deleted items

{{step-1-to-setup}}

1. In the left panel, click **Groups** ![](assets/groups-icon.png).

1. Click the name of the group.
1. In the left panel, click **Recently Deleted**.
1. Open one of the following tabs where you want to view and manage the group's recently deleted items:

   * Projects
   * Tasks
   * Issues
   * Documents
   * Templates

   Each tab lists items of the corresponding object type that belong to the current group or its subgroups and that were deleted within the past 30 days.

   >[!NOTE]
   >
   >If someone deleted a project, all of its individual tasks, issues, and documents were deleted with it. These do not display individually on the Tasks, Issues, Documents, or Templates tabs. However, restoring the project also restores all of these child objects to the project.
   >
   >
   >If someone deleted a task, issue, document, or template individually, you can view and manage it on the appropriate tab.

1. Do any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Restore objects</p> </td> 
      <td> <p>Select up to 10 objects, then click <strong>Restore</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Export the entire list of objects on the tab</p> </td> 
      <td> <p>Click <strong>Export</strong>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>Change the display of information in the list</p> </td> 
      <td> <p>In the upper-right corner above the list, use <strong>Filter</strong> to define what is displayed based on criteria you provide. Use <strong>View</strong> to define which fields are displayed as columns. Use <strong>Grouping</strong> to group the items into categories.</p> </td> 
     </tr> 
    </tbody> 
   </table>
