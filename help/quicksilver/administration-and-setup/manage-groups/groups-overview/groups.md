---
title: Groups overview
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: A Workfront administrator can create groups of users that coincide with your departmental structure. Groups are similar to but distinct from teams and companies.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
---
# Groups overview

<!-- Audited: 01/2024 -->

A Workfront administrator can create groups of users that coincide with your departmental structure. Groups are similar to but distinct from teams and companies.

The Workfront administrator grants groups the access to the Workfront areas where they need to work and communicate. Each group can then keep their Workfront information such as users, templates, and custom forms, and projects separate from those of other departments.

At least one group administrator is required for every group. Group administrators can use the Groups page to manage their groups in one place. For more information, see [Group administrators](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

You can create up to 14 levels of subgroups under one group. For more information, see [Subgroups overview](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) and [Create a subgroup](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Using groups to organize users

As a Workfront administrator or group administrator, you can associate users with groups and subgroups. If you make a group public, users with a Standard (new) or Plan (current) license can associate users with it. For more information about group administrators and public groups, see [Create a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

When you create a user, we recommend that you add that user to the appropriate Home Group and other groups that the user should work in. A user can have only one Home Group, but can be in multiple other groups.

Being part of a group gives the user access to objects that are shared with the group and the subgroups. For example, if you share a project with a group, users in the group and the group's subgroups have access to it.

>[!TIP]
>
>If departments in your organization often work together to manage projects and the resources on those projects, it might not be necessary to divide departments into many smaller groups. A few high level groups might work best.

A group can have an unlimited number of users.

For more information about creating new users, see [Add users](../../../administration-and-setup/add-users/add-users.md).

## Granting a group access to objects

When you share an object with a group, all members of that group (including members of any subgroups) have access to the object. For more information about sharing in Workfront, see [Overview of sharing permissions on objects](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Associating a group with an object

When you are creating or editing one of the following Workfront objects, you can associate it with a group:

* **Project**: You can associate a single group with a project in order to indicate ownership of the project.

  This does not implicitly grant each member of the group rights to the project. In order to have rights to the project users must have the project shared with them.

  While users can be members of multiple groups, a project can have a single group associated with it. Users from other groups can still work on the same project, if the project has been shared with them or their groups. The group associated with the project is usually either the group responsible for completing the project, or the group for whom the project is delivered.

  For instructions on associating a project with a group, see [Manage information in the project Overview area](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, program, or company**: When you are creating or editing a portfolio, program, or company, you can assign a single group to it to indicate that the group owns or has responsibility for it. With this association made, administrators and users can easily identify which portfolios, programs, and companies their groups are working on.

  For example, a group administrator can list all of the portfolios in the organization using a list or report and note in the Group column which portfolios are assigned his or her group.

  >[!NOTE]
  >
  >Assigning a group to a portfolio, program, or company with a group does not automatically mean that information in that the group has access to its data. You need to manually share access to the data with the group before they can see it.

  For instructions, see [Create a portfolio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Create a program](../../../manage-work/portfolios/create-and-manage-programs/create-program.md), and [Create and edit companies](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Approval Process**: You can make an approval process available for projects, tasks, and issues belonging to a certain group. For more information, see [Create an approval process for work items](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Milestone Path**: You can allow users in certain groups to use a milestone path with their projects. For more information, see [Create a milestone path](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Layout Template**: You can give a group's administrators permission to modify a Layout Template. For instructions, see [Grant administrative access for a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Timesheet Profile**: You can give a group's administrators permission to modify a timesheet profile. For more information, see [Create, edit, and assign timesheet profiles](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Schedules**: You can give a group's administrators permission to modify a schedule. For more information, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Teams**: You can associate a group with a team so that the administrators of the groups and its subgroups can view and work with those teams from the Groups area. For more information, see [Create a team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) or [Edit team settings](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Template**: You can assign a group to a project template. This can help you streamline the project creation process and to help you more easily identify and report on which groups own which project templates. For more information, see the section [Overview](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) in the article [Edit project templates](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Recently deleted and restored items**: You can view and manage the groups recently deleted items. For more information, see [View and manage a group's recently deleted items](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) and [View and manage a group's recently restored items](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
