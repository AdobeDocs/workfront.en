---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Custom Statuses on a Task or Issue that Is Moved or Copied
description: When you move or copy a task or issue to a different project, some statuses on the task or issue might update to match statuses used by the destination project's group.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
TQID: https://experienceleague.adobe.com/GzG3KBfUw05edjA0DVRtODyGprG2mKVjOuUV2L5eWto
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Custom statuses on a task or issue that is moved or copied

When you move or copy a task or issue to a different project, some statuses on the task or issue might update to match statuses used by the destination project's group. This depends on whether statuses with the same key exist in that group:

* If a status on the task or issue has the same key as a status used by the destination project's group, the status on the task or issue remains the same.

  If the label of these two statuses don't match, the status on the task or issue inherits the label of the status used by the destination project's group.

* If a status in the task or issue does not have the same key as the equivalent status in the destination project's group, the status in the task or issue changes to the equivalent default status in the destination project's group.

For information about status keys, see [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
