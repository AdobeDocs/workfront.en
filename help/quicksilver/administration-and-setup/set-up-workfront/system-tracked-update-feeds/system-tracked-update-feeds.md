---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: System-tracked updates
description: Adobe Workfront captures the activity taking place on certain objects by logging status information in the object's Updates area.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
---
# System-tracked updates

Adobe Workfront captures the activity taking place on certain objects by logging status information in the object's Updates area.

The Updates area includes the following types of updates:

* **User updates:** Manually entered by users. Also referred to as comments, replies, and notes.

  ![](assets/updates-qs-350x125.png)

* **System updates:** Automatically made by the system. A system update includes a brief note describing what kind of change happened to the item. 

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

The following objects can have updates:

* Project
* Task
* Issue
* Portfolio
* Program
* User
* Templates
* Template tasks
* Documents
* Timesheets

Your Workfront license determines whether system updates display by default in the Updates area of objects. Workfront users with a Plan license have system updates displayed in the Updates area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other Workfront licenses filter system updates by default.

Workfront administrators can define what type of changes the system should track in the Updates area. Not all objects have configurable update status feeds. The following objects have an Updates area that captures system-tracked update feeds, but do not have configurable update status feeds:

* Templates
* Template tasks
* Documents
* Timesheets

For more information about system update feeds and how to enable them, see [Configure system updates](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md). For more information about configuring user updates, see [Configure preferences for user updates](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
