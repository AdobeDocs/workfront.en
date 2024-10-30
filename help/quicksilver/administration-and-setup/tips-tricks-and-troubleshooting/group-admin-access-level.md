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
---
# Group admins must have higher access than those they manage

If a group administrator has permissions in their access level lower than those they manage, they will not be able to view, modify, or assign lower access levels.  

## Problem

If a group administrator is assigned a modified Planner access level with View permissions for Teams, but certain users are assigned a Worker access level with Edit permissions for Teams, the group administrator will not be able to interact with the modified Worker access level.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>This logic also applies to the Fine-tune your settings drop-down menu. Both access levels can have Edit access, but settings in the Fine-tune your settings drop-down menu must be higher for the group admin.
> ![](assets/fine-tune-your-settings.png)

## Solution

Group admins must have higher permissions in all areas in the access level than those they manage.
