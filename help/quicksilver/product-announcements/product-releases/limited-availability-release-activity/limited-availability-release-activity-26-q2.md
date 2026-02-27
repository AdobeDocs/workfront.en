---
content-type: release-notes
title: Second Quarter 2026 Release Activity for Adobe Workfront Limited Availability Features
description: This is the release activity for limited availability features in Adobe Workfront for the Second Quarter 2026.
author: Lisa
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
hide: yes
hidefromtoc: yes
exl-id: 32c616b2-5bba-434e-9918-c27f6518693d
---
# Second Quarter 2026 release activity for Adobe Workfront limited availability features

This article describes the limited availability Workfront features that are releasing during the Second Quarter of 2026.

<!--keep the sentence below for all future quarterly release pages-->

For a list of all limited availability features released for Adobe Workfront, see [Adobe Workfront limited availability features release activity: article index](/help/quicksilver/product-announcements/product-releases/limited-availability-release-activity/limited-availability-release-activity-article-index.md).

## Release notes for limited availability features

This section includes the release notes for new functionality.

### Updated experience when single- or bulk-assigning tasks

>[!NOTE]
>
>Production release date: February 12, 2026

We have updated the Assignments section in the Edit Tasks box when editing single tasks or editing them in bulk.

There is a new experience for assigning resources to tasks. This is now available both when editing one task or editing several tasks in bulk. We have added the following fields to the Assignments section:

* Allocations
* Owner or Task Owner
* Assignee's Role

For information, see [Edit tasks](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).

### Preserve billing rates on staffing plans

>[!NOTE]
>
>Production release date: March 3, 2026

We have added the **Preserve Billing** field to the Finance section of the Staffing Plan Details page.

When this flag is set to False (off), the billing rates are not preserved and the rate hierarchy is used for billing rate calculations.

When this flag is set to True (on):

* The current billing rates of the assigned resources on the staffing plan are preserved, and any changes to rates in the hierarchy are not reflected on the Resources area of the staffing plan.
* If you add a new row to the Resources table, the initial billing rate that comes from the billing rates hierarchy is preserved.
* If a user has overridden the billing rate value manually before the flag was turned on, the override rate is preserved. Once the flag is turned on, manual billing rate overrides are not permitted.

Once preservation is activated, it cannot be turned off.

When you copy a staffing plan that has the flag turned on, the flag is automatically turned off on the copy. The resource manager must turn the flag on if it is needed on the new staffing plan.

<!--### Title

>[!NOTE]
>
>Production release date: MONTH DAY, 2026

text
-->

## Maintenance Updates for limited availability features

This section describes the issues fixed in the weekly Workfront updates for limited availability features.

<!--

### Maintenance Updates week of March 1-7, 2026

**Title**

text

### Maintenance Updates week of March 8-14, 2026

**Title**

text

### Maintenance Updates week of March 15-21, 2026

**Title**

text
-->
