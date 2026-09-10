---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Group Admins Must Have Higher Access than Those They Manage
description: If a group administrator has permissions in their access level lower than those they manage, they will not be able to view, modify, or assign lower access levels.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
TQID: https://experienceleague.adobe.com/uxZXjgW85JgdyPJA5UEEfIvwU41hLWE-B3XLDh6D89w
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
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Group admins must have higher access than those they manage

If a group administrator has permissions in their access level lower than those they manage, they will not be able to view, modify, or assign lower access levels.  

## Problem

If a group administrator is assigned a modified Planner access level with View permissions for Teams, but certain users are assigned a Worker access level with Edit permissions for Teams, the group administrator will not be able to interact with the modified Worker access level.

![Group admin modified access](assets/group-admin-modified-access.png)


>[!NOTE]
>
>This logic also applies to the Fine-tune your settings drop-down menu. Both access levels can have Edit access, but settings in the Fine-tune your settings drop-down menu must be higher for the group admin.
> ![Fine tune your settings](assets/fine-tune-your-settings.png)

## Solution

Group admins must have higher permissions in all areas in the access level than those they manage.
