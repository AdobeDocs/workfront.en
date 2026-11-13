---
title: First Quarter 2027 Administrator enhancements
description: First Quarter 2027 Administrator enhancements
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
---

# First Quarter 2027 Administrator enhancements

This page describes Administrator enhancements made with the First Quarter 2027 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the First Quarter 2027 release cycle, see [First Quarter 2027 release overview](/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-release-overview.md).

## Environment Promotion available for Workfront Planning

>[!NOTE]
>
>Production and Sandboxes fast release: November 12, 2026
>Production, Preview, Sandboxes for everyone: December 17, 2026
>[!BADGE Off schedule]{type=Neutral}

>[!NOTE]
>
>Environment Promotion for Workfront Planning is available only to customers who have purchased a Workfront Planning package in addition to a Workflow package. It is not available to customers who have purchased Workfront Planning as a standalone product.

Workfront administrators can now promote Workfront Planning workspaces and their objects from one environment to another, so you no longer need to rebuild configurations manually. This saves time and reduces the errors that come with manual setup.

Records, automations, and fields that don't belong to the exported workspaces cannot be promoted.

This capability requires Prime or Ultimate Workflow and Planning packages, a Standard license, and Workfront administrator access.

For information, see [Use Environment Promotion for Workfront Planning](/help/quicksilver/planning/general/planning-environment-promotion.md).

## Permissions for removing an attached custom form

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

When sharing a custom form, you can now set permissions for users with Manage access to the form to remove the form from objects it is attached to.

For more information, see [Share a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Mark a custom field as a favorite

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: December 17, 2026
>Production for everyone: January 21, 2027

You can now mark a custom field as a favorite, either in the field list or in the custom form designer. When you work in certain lists and reports (such as project, task, and issue lists) and build filters, views, and groupings, the favorite fields appear at the top of the list of available fields in the Suggested section.

Fields marked as favorites also appear at the top of the field library in the form designer.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Values verified on custom fields when changing the format

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

The system now checks for incompatible values when you change an existing Text custom field format to Number or Currency.

If the existing values for the field are all numeric, the system simply updates the field format. However, if any of the existing values are non-numeric, the system shows a warning message that incompatible values will be cleared when you save the field.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Change History now tracks Canvas Dashboard objects

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: October 29, 2026
>Production for everyone: October 29, 2026
>[!BADGE Off schedule]{type=Neutral}

Change History now records changes to Canvas Dashboards. You can see who created, updated, or deleted a dashboard or report, when they did it, and what changed.

To start tracking Canvas Dashboard changes, you must configure the **Dashboard**, **Report**, and **Report Config** objects in Setup > Change Tracking > Configuration.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).
