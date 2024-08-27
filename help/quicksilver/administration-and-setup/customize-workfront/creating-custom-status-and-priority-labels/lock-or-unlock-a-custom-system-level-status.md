---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Locked and Unlocked System-Level Statuses
description: Locking custom statuses is a way to ensure that people throughout your organization are using the same processes in their flow of work. When a status is locked, it's available to all users in the system. Though you can edit or delete it, group administrators can't do so for their groups. Conversely, unlocking custom statuses allows group administrators more flexibility to manage the unique workflows used in their groups. They can change the attributes of an unlocked status or delete it for their groups.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
---
# Locked and unlocked system-level statuses

Locking custom statuses is a way to ensure that people throughout your organization are using the same processes in their flow of work. When a status is locked, it's available to all users in the system. Though you can edit or delete a status that you lock, group administrators can't do so for their groups; they can change only its display order in the Status list.

Conversely, unlocking custom statuses allows group administrators more flexibility to manage the unique workflows used in their groups. When a status is unlocked, group administrators can change its attributes or delete it for their groups.

>[!IMPORTANT]
>
>If you lock a custom status after it has been unlocked for any period of time, your system-wide settings for the status replace those made by group administrators. While the status is locked, group administrators cannot modify or delete the status for their groups.

For instructions on locking or unlocking a system-level status, see [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Unlocked statuses in approval processes

You can use both locked and unlocked statuses in a system approval process. If you create a system approval process with an unlocked system status, users throughout the system can attach the approval process to any project, task, or issue in the system. 

 Warning messages display in the following scenarios to help you and your users make sure you understand outcomes of the following scenarios:

* An administrator unlocks a system-level status that is used in an approval process. A message warns that  might delete the unlocked status for their groups, which would prevent group members from using that approval process properly for objects assigned to their group. 

 * A user starts to edit an approval process that uses an unlocked status. A message alerts the user about the unlocked status so they can evaluate whether it would be a good idea to re-lock or replace it. 

* A system-level approval process with an unlocked status is attached on an object, and the status was deleted for the group assigned to the object. When a group member goes to the Approvals section for the object, a message explains that the approval process can't be initiated for the object.

You can use both locked and unlocked statuses in a group approval process. If you create a group approval process with an unlocked group status, users can attach the approval process to any project, task, or issue that is associated with the group.