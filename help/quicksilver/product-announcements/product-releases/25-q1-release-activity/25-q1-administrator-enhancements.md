---
title: First Quarter 2025 Administrator enhancements
description: First Quarter 2025 Administrator enhancements
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: fa24040d-0403-4799-b690-c3d172797115
---
# First Quarter 2025 Administrator enhancements

This page describes all administrator enhancements made with the First Quarter 2025 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the First Quarter 2025 release cycle, see [First Quarter 2025 release overview](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

## Compare objects between environments for environment promotion

>[!NOTE]
>
>Preview release: January 6, 2024; Production release for all customers: With the 25.1 release (January 2025)

To make it easier to determine which object should be included in an environment promotion package, we've added the ability to compare objects across environments. Now, you can select object types and environments. Workfront generates a list of objects of that type, whether they are present in the target environment, and whether that object has differences between the source environment and the target environment. You can then add objects to a package directly from this list.

Previously, if a user wanted to compare objects between environments, they must check those objects manually.

For more information, see [Compare objects between environments](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md).

## More objects available for environment promotion

>[!NOTE]
>
>Preview release: January 6, 2024; Production release for all customers: With the 25.1 release (January 2025)

To expand the capabilities of environment promotion functionality, we've added more objects. Now, you can add the following objects to an environment promotion package:

* Locations
* Rate cards
* Assignments

Previously, these objects were not available for environment promotion.

For more information on objects available for environment promotion, see [Supported objects for environment promotion](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) in the article Environment promotion overview.

## Prevent Moving tasks when there are Hours logged

>[!NOTE]
>
>Preview release: December 19, 2024; Production release for all customers: With the 25.1 release (January 2025)

Because moving tasks or issues that have logged hours can sometimes cause compliance or audit problems, we have added a preference in the Task & Issues Preferences area of Setup that allows you to prevent users from moving tasks and issues if there are hours logged on them. Prior to this enhancement, users could move tasks and issues to other projects, even if there were hours logged on them. 

For information, see [Configure system-wide task and issue preferences](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Preference to use project or user schedule for single-assignment tasks

>[!NOTE]
>
>Preview release: November 21, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025)

As a system or group administrator, you now have a new preference to indicate whether Workfront should use the project's or the user's schedule to calculate the timeline of the project when you assign one user to a task and both the project and the user are associated with a schedule. Prior to this enhancement, this setting existed for multiple-user assignments. The setting is now available for single-user assignments to tasks.  

For more information, see [Configure system-wide project preferences](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Business rules now support hyperlinks

>[!NOTE]
>
>Preview release: November 21, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025)

You can now include hyperlinks in the custom error message of a business rule, to guide the user on how to modify their action within the constraint of the rule. The static URL could link to documentation or other pages that would be helpful to the user.

For information, see [Create and edit business rules](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

## Filtering on native typeahead fields is now available

>[!NOTE]
>
>Preview release: November 21, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025)

When you add a native field reference to a custom form and it references a typeahead field (such as Portfolio, Company, or Owner), a filter option is now available. The filter allows you to limit the objects users can choose when they are using the field. This custom filter works the same as a filter on a custom typeahead field, using Text Mode to define the filter.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## "Move to" icon added to custom fields

>[!NOTE]
>
>Preview release: October 29, 2024; Production for fast release: With the 24.11 release (November 14, 2024); Production for quarterly release: With the 25.1 release (January 2025)

When a custom form contains multiple sections with many fields, it can be difficult to move a field from one section to another by dragging and dropping. A "move to" icon has been added to each field, allowing you to select the section that the field is placed in.

For more information, see [Organize and preview a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
