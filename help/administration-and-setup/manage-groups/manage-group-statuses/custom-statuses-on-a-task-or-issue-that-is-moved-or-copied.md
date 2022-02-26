---
filename: custom-statuses-on-a-task-or-issue-that-is-moved-or-copied
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Custom statuses on a task or issue that is moved or copied
description: When you move or copy a task or issue to a different project, some statuses on the task or issue might update to match statuses used by the destination project's group. This depends on whether statuses with the same key exist in that group:
---

# Custom statuses on a task or issue that is moved or copied

When you move or copy a task or issue to a different project, some statuses on the task or issue might update to match statuses used by the destination project's group. This depends on whether statuses with the same key exist in that group:

* If a status on the task or issue has the same key as a status used by the destination project's group, the status on the task or issue remains the same.

  If the label of these two statuses don't match, the status on the task or issue inherits the label of the status used by the destination project's group.

* If a status in the task or issue does not have the same key as the equivalent status in the destination project's group, the status in the task or issue changes to the equivalent default status in the destination project's group.

For information about status keys, see [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
