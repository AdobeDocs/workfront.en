---
title: 22.4 Administrator enhancements
description: 22.4 Administrator enhancements
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
---
# 22.4 Administrator enhancements

This page describes all Administrator enhancements made with the 22.4 release to the Preview environment. These enhancements will be made available the week of October 3, 2022. 

For a list of all changes available with the 22.4 release, see [22.4 Release overview](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Use unlocked statuses in an approval processes

>[!NOTE]
>
>This feature was first introduced in the Preview environment during the 22.3 release time frame. It releases to Production September 15, 2022.

To give you more control over the approval processes and statuses in your system, we've made it possible to create an approval process based on an unlocked system status. Moreover, you can now unlock any status that is already used in an approval process. Previously, a system status used in an approval process had to be locked. This made it available for all groups—without the possibility of removing or renaming it—so group administrators couldn't streamline their group's list of statuses to fit their specific needs.

## Blueprints icon on the Main Menu now controlled through layout templates

System administrators can now add or remove the Blueprints icon on the Main Menu through layout template configuration. This provides greater control of who can browse the Blueprints catalog.

The Blueprints icon appears in the Main Menu when:

* The user has no layout template assigned

* The user's layout template has the Blueprints option in the Active Items list

* The user's layout template has the Blueprints option in the Available Items list, the icon does not appear in the Main Menu.

Existing layout templates automatically include the Blueprints icon, and administrators can remove the icon from layout templates to restrict visibility of the Blueprints catalog. New layout templates created after the 22.4 release will include the Blueprints icon in the Active Items list.

For more information, see [Configure access to Blueprints](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Issue header customization

As a Workfront or group administrator, you can now customize the fields that display in the header of an issue when you use a Layout Template.

This update includes the following enhancements:

* Remove or rearrange existing fields from the issue header.

* Add new, non-editable Issue Overview fields. You cannot add custom fields or fields that can be edited. You can also display editable fields that are currently on the issue header (for example, Status or Percent Complete).

* The issue header can include up to five fields.

* You can now add the "Resolved By" field to the issue header. When a resolving object is associated with the issue, the "Resolved By" field changes to "Resolving Issue," "Resolving Task," or "Resolving Project," depending on the type of object that is associated with the issue.

Prior to this release, only project and task headers could be customized.



For more information, see [Customize object headers using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Task header customization

As a Workfront or group administrator, you can now customize the fields that display in the header of a task when you use a Layout Template. 

This update includes the following enhancements: 

* Remove or rearrange existing fields from the task header.  

* Add new, non-editable Task Overview fields. You cannot add custom fields or fields that can be edited. You can also display editable fields that are currently on the task header (for example, Status or Percent Complete).    

* The task header can include up to five fields. 

Prior to this release, only project headers could be customized. 

For more information, see [Customize object headers using a Layout Template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[View a video demonstration of this feature.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Early feature opt-in for the latest features on boards

We are excited to open new boards features for early feature opt-in. This optional tool is available to all organizations.

Only a Workfront administrator can opt in to the early features. When the administrator opts in to early features, all users in the organization are opted in, and the additional features are enabled in your production Workfront environment.

For more information, see [Early feature opt-in for Adobe Workfront Boards](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[View a video demonstration of this feature.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## Custom form field calculation editor displays error information

>[!NOTE]
>
>This feature was first introduced in the Preview environment during the 22.3 release time frame. It releases to Production with the 22.4 release.

Editing calculations for custom fields is now easier with helpful error information indicated directly in the calculation. While you are creating a calculated field in a custom form, errors are highlighted in pink. When you hover over the highlighted portion, a tooltip displays to describe what the problem is.

For more information, see [Add calculated data to a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

[View a video demonstration of this feature.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migration to Adobe Unified Experience

NOTE: This migration has been postponed to Q1-Q2 of 2023. Any affected customers will be notified at that time.

If your organization has been onboarded to the Adobe Admin Console, your Workfront instance will be migrated to the Adobe Unified Experience with the 22.4 release.

The Adobe Unified Experience includes:

* A single login for all Adobe applications through Adobe Experience Cloud

* An "organization switcher" to move between Workfront organizations and environments

* Navigation with options for Workfront pages, Adobe Experience Cloud preferences, and your Workfront profile

For more information, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[View a video demonstration of this feature.](https://video.tv.adobe.com/v/3412388/){target=_blank}
