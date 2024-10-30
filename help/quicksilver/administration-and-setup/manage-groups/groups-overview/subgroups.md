---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: Subgroups Overview
description: You can create up to 14 levels of subgroups under one group. On any one of these levels, you can create an unlimited number of parallel subgroups.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
---
# Subgroups overview

You can create up to 14 levels of subgroups under one group. On any one of these levels, you can create an unlimited number of parallel subgroups. For instructions, see [Create a subgroup](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

For information about groups, see [Groups overview](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## What do subgroups inherit?

Subgroups inherit the membership of their parent group. So, users and groups in a subgroup have the same visibility, permissions, and access to all objects as users and groups that belong to the parent group they share.

Also, a subgroup automatically inherits the group administrators of its top-level group, but you can also assign members of a subgroup to act as its group administrators.

>[!TIP]
>
>Sometimes, you might want to use subgroups to add multiple users to an existing group in order to give them access to an object they need.
>
>For example, suppose that you have a group of help desk technicians and a separate group of IT directors. The help desk group has permissions to a certain Request Queue. You want to add the IT directors to the help desk group so that they also have permissions to the Request Queue. Without the subgroup functionality, you would have to add the IT directors to the help desk group manually, which could be inefficient and hard to manage. If you add the IT directors group to the help desk group as a subgroup, you accomplish this task faster with just one change.

>[!NOTE]
>
>If a user was added to both a subgroup and to its parent group separately, removing the user from one doesn't remove the user from the other. If you don't want the user to have the access allowed for the parent group, you must remove the user both from the subgroup and from the parent group.

## Public and private subgroups

For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.

You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.

If you create a subgroup under a group that is public, the subgroup is also public, by default. For more information about creating a group and making it public, see [Create a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). For more information about the access needed to edit users, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Any group you add to an existing group automatically becomes a subgroup and is no longer a main group. However, the subgroup retains its existing users, as well as any associations with projects, issues, and tasks, in addition to all project, task, and issue statuses that belong to the new parent group.

## Group administrators for subgroups

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

You can assign subgroup members as group administrators to the subgroup when you create it or edit it. For instructions, see [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) in the article [Create a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Alternately, you can leave administration of the subgroup to the group administrators who are assigned to the groups above it. When you create a subgroup, group administrators over the groups above it have automatic access to manage the subgroup.

>[!NOTE]
>
>If you add a user to a subgroup and that user is a group administrator for a group anywhere above the subgroup, that user has administrative rights to manage the subgroup, even without being assigned as a group administrator for it.

To learn which actions available for an Adobe Workfront administrator managing the Workfront system, a group administrator managing a top-level group, and a group administrator managing a subgroup, see [Actions allowed for different types of administrators](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
