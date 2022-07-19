---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Locked and unlocked group statuses
description: Locking a group's custom statuses is a way to ensure that people in the group and its subgroups are using the same processes in their flow of work. When a group status is locked, it's available to all users in the group and in lower groups. Though you (or a Workfront administrator) can edit or delete a status that you lock, administrators of subgroups below can't do so for those groups. Conversely, unlocking a group's custom statuses allows administrators of lower subgroups more flexibility to manage their workflows. They can change the attributes of an unlocked status or delete it for their groups.
author: Caroline
feature: "System Setup and Administration, People Teams and Groups"
role: Admin
---

# Locked and unlocked group statuses

Locking a group's custom statuses is a way to ensure that people in the group and its subgroups are using the same processes in their flow of work. When a group status is locked, it's available to all users in the group and in lower groups. Though you (or a Workfront administrator) can edit or delete a status that you lock, administrators of subgroups below can't do so for those groups; they can change only its display order in the Status list.

Conversely, unlocking a group's custom statuses allows the administrators of lower subgroups more flexibility to manage the unique workflows used in their groups. When a group status is unlocked, administrators of lower subgroups can change its attributes or delete it for those subgroups.

>[!IMPORTANT]
>
>If you lock a custom status after it has been unlocked for any period of time, your settings for the status replace those made by group administrators in lower subgroups. While the status is locked, those administrators cannot modify or delete the status for their groups.

For instructions on locking or unlocking a group status, see [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

**Unlocked statuses in approval processes**

You can use both locked and unlocked statuses in a group approval process. If you create a group approval process with an unlocked group status, users can attach the approval process to any project, task, or issue that is associated with the group.

