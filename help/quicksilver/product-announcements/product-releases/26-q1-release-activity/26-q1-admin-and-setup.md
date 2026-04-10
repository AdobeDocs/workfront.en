---
title: First Quarter 2026 Administrator enhancements
description: First Quarter 2026 Administrator enhancements
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a74d036b-e4fa-49e0-bb10-4baf379e1b1c
---
# First Quarter 2026 Administrator enhancements

This page describes Administrator enhancements made with the First Quarter 2026 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the First Quarter 2026 release cycle, see [First Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Manage Priorities in the Layout Template

>[!NOTE]
>
>This feature is temporarily unavailable in the Preview environment
>Preview: December 2, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 


You can now enable or disable Priorities for specific users in the Layout Template. If you previously had Priorities disabled for your organization, it will remain disabled in the layout template with this change.

Priorities will be automatically included for license types that have default access to Requests. For example, a Contributor license will see Requests, Boards, and Priorities by default in the Main Menu, while an External license will only see Documents and Boards because it does not have access to view or submit requests.


For more information, see [Customize the Main Menu using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Check for multi-form conflicts for calculated custom fields

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 

The same calculated field can have different formulas when attached to different custom forms. If two or more forms containing the same calculated field are attached to an object, then the formulas must be identical on all of the forms. Editing the formula is not allowed if the change could cause a conflict.

To provide visibility into which objects may be affected when editing an expression on custom fields, we have added an option to check for conflicts. This dialog shows all objects that might be affected by changing the formula, grouped by object type. You can navigate to each object's details and review the fields to decide whether the field should be removed from any of the forms or the expression should remain unchanged.

For more information, see [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).


## Entry date and Entered by ID stored on custom objects

>[!NOTE]
>
>Preview: November 13, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  November 13, 2025

The entry date and entered by ID are now stored on custom forms, fields, and sections. You can use these data options in reports as filters, views, or groupings. To display them in the list of custom forms, fields, or sections in Setup, add Entry Date and Entered By: Name as columns in a new or existing view.

>[!NOTE]
>
>The entry date and entered by ID are available only on custom forms, fields, and sections created on or after November 13, 2025.

## Updates to button names when editing a layout template

>[!NOTE]
>
>Preview: October 30, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  January 15, 2026 

To provide more consistency with other areas of Setup such as the custom form designer, the buttons you see when editing a layout template have changed to **Apply**, **Save and Close**, and **Cancel**. The new option, **Apply**, allows you to save your changes to the layout template and continue editing. Previously, the available options were **Save** and **Cancel**.

For more information, see [Create and manage layout templates](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Improved field management with Active flag on custom fields

>[!NOTE]
>
>Preview: October 30, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  January 15, 2026 

When you have large numbers of custom fields in the system, management of those fields in custom forms and reports can be difficult. You can now mark custom fields inactive with the new **Active** flag. This flag is available when working with a field on a custom form or when adding or editing a field from the Fields list.

If you mark a field inactive:

* It is excluded from reports, filters, views, or other places in Workfront where you can add a custom field
* It is not available in the field library to add to other custom forms

>[!NOTE]
>
>Marking an existing field inactive makes it unavailable to use in reporting elements and custom forms from that point forward. If the inactive field is currently used in a report or a form, the field and its historical data remain in place.

For more information, see [Add or edit a custom field, section break, or widget](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/edit-a-custom-field.md).
