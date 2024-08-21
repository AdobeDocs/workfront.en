---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Create and Manage a Group's Timesheet Profiles
description: When you are viewing a group that you manage in the Groups area, you can view and work with the timesheet profiles for which the administrators of the group, or one of its subgroups, have administrative access.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
---
# Create and manage a group's timesheet profiles

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

When you are viewing a group that you manage in the Groups area, you can view and work with the timesheet profiles for which the administrators of the group, or one of its subgroups, have administrative access.

If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a group administrator of the group.</p>  <p>You must also have administrative access to Timesheets. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Grant users administrative access to certain areas</a>.</p>  <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

+++

## Create and edit group-level timesheet profiles

You can create and edit timesheet profiles for use in a group you manage. For instructions, see [Create, edit, and assign timesheet profiles](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Delete group-level timesheet profiles

You can delete timesheet profiles in use by a group you manage. For instructions, see [Delete timesheet profiles](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## Manually generate group timesheets

To enable changes that you made to group timesheet profiles to reflect in current group timesheets, you have to first delete the existing timesheets and then manually generate new ones. For instructions, see [Manually generate timesheets from the Timesheets & Hours area](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) in [Manually generate timesheets](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

For information about on deleting group timesheets, see [Delete timesheets in Adobe Workfront](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Export group-level timesheet profiles

{{step-1-to-setup}}

1. Click **Groups**.

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Click the name of the group with the timesheet profiles you want to export.
1. Click **Timesheet Profiles**.
1. Click **Export** to export the list of timesheet profiles for the group.
