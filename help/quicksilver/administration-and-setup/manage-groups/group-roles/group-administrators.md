---
title: Group administrators
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Adobe Workfront administrators in a large organization with many departments might not want to manage all the organization's departments and groups within those departments. Instead, they can create a group for each department and subgroups within that group, each managed by a group administrator.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
---
# Group administrators

<!-- Audited: 12/2023 -->

Adobe Workfront administrators in a large organization with many departments might not want to manage all the organization's departments and groups within those departments. Instead, they can create a group for each department and subgroups within that group, each managed by a group administrator.

A group administrator can manage the needs of a group, such as user membership, layout templates, custom data, statuses, and preferences.

Up to 14 levels of subgroups can exist under one group.

>[!NOTE]
>
>All group administrators in the hierarchy above a subgroup have administrative rights to manage that subgroup.

For information about creating and managing groups, see [Create a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) and [Manage a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Also, see [Subgroups overview](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Designating group administrators

Every top-level group must have at least one group administrator. A Workfront administrator or administrator of a group can assign group administrators to the group's subgroups, but this is not required. For more information, see [Create a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

If you are a Workfront administrator, we recommend that you do the following before designating users as group administrators:

* Make note of the current number of Workfront administrators in your system.
* Make note of the number of groups you have in your system.
* Determine whether you can change the access level of some of the Workfront administrators and designate them as group administrators instead.

  For more information about the capabilities of group administrators, see [Tasks done by group administrators](#tasks-done-by-group-administrators) in this article.

* Determine whether you want group administrators to be able to log in as other users, or to reset passwords for users in the groups you administer. Additional access is needed to perform these tasks, as explained below in [Access needed for group administrators](#access-needed-for-group-administrators).
* For better user management, consider assigning groups or subgroups instead of users to the following objects:

   * Layout Templates
   * Schedules
   * Timesheet Profiles

## Access needed for group administrators {#access-needed-for-group-administrators}

Every group administrator is required to have

* A Plan license in the current pricing and packaging model
* A Standard license in the new pricing and packaging model

We recommend that group administrators have Edit access to users so that they can perform the following tasks:

* Log in as other users in the groups and subgroups they manage.
* Reset the password of another user in the groups they manage.

>[!IMPORTANT]
>
>Group admins must have higher access than those they manage; otherwise, they will not be able to view or modify lower access levels.
>For instructions on granting this access, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

For a group administrator who needs to assign timesheet profiles to users in their groups and subgroups, we also recommend Administrative access to timesheets and hours. For instructions on granting this access, see [Grant users administrative access to certain areas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Tasks done by group administrators {#tasks-done-by-group-administrators}

As a group administrator, you can carry out the tasks outlined below to manage the groups that you oversee. Some of these are the same as abilities afforded to a Workfront administrator.

>[!NOTE]
>
>In the new pricing and packaging model, you must have a Prime plan or higher to perform the following:
>
> * Create group event notifications
> * Configure group project preferences
> * Configure group task and issue preferences
> * Unlock configuration of subgroup preferences
> * Group timesheet and hour preferences
> * Unlock timesheet and hour preference

### Manage group members {#manage-group-members}

* Create, edit and delete subgroups within the groups and subgroups you manage. For instructions, see [Create a subgroup](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Add any users for whom you have Edit access to your groups and subgroups. Or add users to groups and subgroups by editing their profiles.

  You can also update the fields in a group member's profile if you have the User Admin (Group Users) permission enabled in your access level.

  For more information, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Workfront administrators can override changes to group memberships made by a group administrator.

* Reset passwords for users that are members of the groups you manage. For more information, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Log in as users that are members of the groups you manage. For more information, see [Log in as another user](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* View the number of available licenses available for your group and the subgroups below it. For more information, see [Manage available licenses in your system](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Manage group objects {#manage-group-objects}

* Create group-level Layout Templates and associate them with the groups and subgroups you manage. For more information, see [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Create group-level timesheet profiles, associate them with users and groups you manage, and manually generate timesheets. For more information, see [Create, edit, and assign timesheet profiles](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Without administrative access to approval processes, create and edit approval processes for the groups and subgroups you manage. For more information, see [Create an approval process for work items](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  For information about administrative access to approval processes, see [Grant users administrative access to certain areas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Create schedules and associate them with a group you manage. For more information, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Manage a team that is assigned to a group you manage, without being a member of the team. Also, create a team report based on the Group field to identify which group a certain team is assigned to. For more information, see [Create a team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Restore a project that is associated with a group you manage, along with any tasks, issues, or documents associated with the project. For more information, see [Restore deleted items](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Manage group preferences and tools {#manage-group-preferences-and-tools}

* When a project preference, task or issue preference, or timesheets and hours preference is unlocked for groups throughout the system, edit that preference for groups you manage. These preferences impact project, task, and issue behavior. For more information, see the following:

   * [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 
   * [Configure task and issue preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Create and edit group statuses for groups you manage. For more information, see [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Configure an event notification for groups you manage. You can do this only after a Workfront administrator unlocks the ability to configure event notifications for groups through out the system. For more information, see [View and configure event notifications for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
