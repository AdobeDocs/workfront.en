---
title: Third Quarter 2026 Administrator enhancements
description: Third Quarter 2026 Administrator enhancements
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
---
# Third Quarter 2026 Administrator enhancements

This page describes Administrator enhancements made with the Third Quarter 2026 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Third Quarter 2026 release cycle, see [Third Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Rich Text replacing Text with Formatting field type

>[!NOTE]
>
>Preview: May 28, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026

The new **Rich text** field type in custom forms is a robust text editor, with formatting options such as superscript and subscript, headings, and tables, in addition to the traditional options of bold, italics, underline, bullets, numbering, hyperlinks, and block quotes. The character limit remains 15,000.

The Rich text field type is replacing the Text with formatting field type. You can quickly convert existing Text with formatting fields to Rich text, by clicking the button in the field options on the right. When you convert, historical data remains on the field and it is used the same way in reports.

>[!IMPORTANT]
>
>External integrations such as Workfront Fusion scenarios or API-based automations may reference legacy field structures and require updates after the conversion. You should verify any integrations before converting fields to Rich text.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Native financial fields supported in custom forms

>[!NOTE]
>
>Preview: May 28, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026

You can now include Workfront native financial fields in custom forms. Previously, the financial fields were not supported.

The available financial fields that you can reference depend on the type of form.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields).

## Custom forms can be shared system-wide with access to attach

>[!NOTE]
>
>Preview: May 28, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026

A new sharing option, "Everyone in the system can view and attach," has been added to custom forms. When you select this option, all users system-wide can attach the form to other objects.

Sharing system-wide eliminates the need to manually share forms and update permissions across groups or agencies when new groups are added.

For more information, see [Share a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## New system preference to enforce required fields in bulk edit

>[!NOTE]
>
>Preview: May 28, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026

Currently, when bulk editing objects, required fields are only enforced when a user modifies the field. If a field is not modified, it is treated as optional and not validated.

A new system preference now allows you to enforce required fields in bulk edit. To not allow bulk edited objects to be saved unless all required fields have values, select the option **Always enforce required fields in bulk edit** on the Setup > System > Preferences page.

