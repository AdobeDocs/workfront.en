---
user-type: administrator
product-area: system-administration;user-management
keywords: manage,group,edit,
navigation-topic: create-and-manage-groups
title: Manage a group
description: As a group administrator, you can manage a group that you administer from the Groups area in Setup. If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
---
# Manage a group

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

As a group administrator, you can manage a group that you administer from the Groups area in Setup. If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).

>[!NOTE]
>
>When you are assigned as the administrator for a group, you inherit the group administrator role for any subgroups that are below it. The only users who can manage a subgroup are the group administrators for the top group above it and any group administrators who are assigned to the subgroup.

## Access requirements

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

## Manage a group's memberships

You can add to and remove users and other groups from a group you administer. You can also assign group members as administrators for the group and manage the user profile information of group members.

For instructions, see [View and manage a group's memberships](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## Manage a group's details

You can view and edit the Group Details page for a group or subgroup that you manage. This page includes a description of the group, the names of the Business Leader and group administrators, and an option that allows you to make the group and all of its subgroups public or private. And, if your access level allows you to manage custom forms, you can attach a custom form to a group.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

For instructions, see [View and manage a group's details](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Edit, copy, or delete a group

Without leaving the main page of a group you are viewing, you can quickly edit, copy, or delete the group.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Groups**.

   In the list that displays, you can see the groups you manage, along with any subgroups they have. Adobe Workfront administrators can see all groups.

1. Select the group, then click the Edit ![](assets/edit-icon.png), Copy ![](assets/copy-icon.png), or Delete ![](assets/delete.png) icon.

   If you need information about using the box that displays, see one of the following:

   * **Edit**: [View and manage a group's details](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)
   
   * **Copy**: [Create a top-level group by copying an existing group or subgroup](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) in the article [Create a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)
   
   * **Delete**: [Delete a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## Configure project, task, and issue preferences for a group

If you are a group administrator and your group needs different project, task, and issue preference settings from those that are set on the system level, you can ask the Workfront administrator to unlock a preference for all groups throughout the organization. After it is unlocked, you (and group administrators for all other groups) can configure it for the groups you manage.

For instructions, see [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) and  [Configure task and issue preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## List, add, and configure subgroups

You can create, view, edit, copy, rename, export, and delete subgroups beneath a group you administer.

## Configure event notifications for a group

If a Workfront administrator unlocks the ability to configure event notifications for the groups in your organization, you can configure them for a group you administer. For instructions, see [View and configure event notifications for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Create and customize statuses for a group

As a group administrator, you can create custom statuses for a top-level group that you manage. This gives your group autonomy and helps to eliminate the need for dozens of company-wide custom statuses. (A Workfront administrator can also do this, for any group.)

You can also customize system statuses for a top-level group if a Workfront administrator has configured them to allow customization.

For instructions, see [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Work with a group's projects

In the Groups area in Setup, when you are viewing the main page of a group you administer, you can do the following with projects:

* List and work with (edit, copy, delete, and export) the projects that are associated with the group and its subgroups and that have been shared with you
* Create a new project for the group

For instructions, see [Create and modify a group's projects](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## View and manage a group's approval processes

When you are viewing a group that you manage in the Groups area, you can view and work with the approval processes for which the administrators of the group, or one of its subgroups, have administrative access.

For instructions, see [Group-level approval processes](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## View and manage a group's layout templates

When you are viewing a group that you manage in the Groups area, you can view and work with the Layout Template for which the administrators of the group, or one of its subgroups, have administrative access.

For instructions, see [Create and modify a group's layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## View and manage group members' schedules

A group administrator creating a schedule for a group has to specify the group whose administrators will manage the schedule. Typically, this is the group for which the schedule is being created, but it could be a different group if the group administrator manages multiple groups and specifies one of the others instead.

When you are viewing the main page of a group you manage, if the group is designated as the one whose administrators can edit a schedule, you can view and manage the schedule from the group's page.

For instructions, see [Create and modify a group's schedules](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## View and manage group members' timesheet profiles

When you are viewing the main page of a group you administer, you can manage the timesheet profiles that you and the other administers of the group—or one of its subgroups—have permission to edit. For instructions, see [Create and manage a group's timesheet profiles](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## View and manage a group's subgroup members

When you are viewing the main page of a group you administer, you can view and manage all of the users in the group's subgroups. For instructions, see [View and manage subgroup members](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## View and manage a group's teams

When you are viewing a group that you manage in the Groups area, you can view and work with teams associated with the group or any of its subgroups.

For instructions, see [Create and modify a group's teams](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## View and manage a group's companies

When you are viewing a group that you manage in the Groups area, you can view and work with companies associated with the group or any of its subgroups. For instructions, see [Create and modify a group's companies](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## View and manage a group's portfolios and programs

When you are viewing a group that you manage in the Groups area, you can view and work with portfolios and programs when both of the following are true:

* They are associated with the group you are viewing or any of its subgroups
* You have permissions to view them because you created them or they were shared with you

For instructions, see [Create and modify a group's projects](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) and [Create, modify, and view a group's programs](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Deactivate or reactivate a group

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

You can keep a group in its default active state or deactivate it.

Deactivating a group can be useful when it is not currently in use because users no longer see it in type-ahead fields when they are searching for a group that they want to associate with another object.

For instructions on making a group inactive or active, see [Deactivate or reactivate a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
