---
title: 23.2 Resource management enhancements
description: 23.2 Resource management enhancements
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
---
# 23.2 Resource management enhancements

This page describes all resource management enhancements enhancements made with the 23.2 release to the Preview environment. These enhancements will be made available in the Production environment with the 23.2 release. 

For a list of all changes available at this point in the 23.2 release cycle, see [23.2 Release overview](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Introducing the Work Time field to accurately calculate user capacity 

>[!NOTE]
>
>Preview release: February 16, 2023; Planned Production release: March 2, 2023

To allow resource managers to accurately calculate the availability of their users and account for the time users devote to actual, project-related work, we are introducing the Work Time concept to Adobe Workfront.

You can define the value of the Work Time field for every user, when you create or edit their profile. For more information, see [Edit a user's profile](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

The Work Time field represents the percentage of Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number with a value between 0 and 1. For example, a 20% availability for actual work would be 0.2.

The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work.

As a result of this update, Workfront calculates the user's availability using the formulas below, depending on your selection in the Resource Management preferences area:

* Default Schedule:
* User Capacity = [(Schedule Hours – Schedule Exceptions) * FTE – Time off] * Work Time
* User's Schedule:
* User Capacity = (Schedule Hours – Schedule Exceptions - Time off) * Work Time.

For more information, see [Configure [!UICONTROL Resource Management] preferences](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3415608/){target=_blank}
