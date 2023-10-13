---
title: Fourth Quarter 2023 Administrator enhancements
description: Fourth Quarter 2023 Administrator enhancements
author: Lisa
feature: Product Announcements
---
# Fourth Quarter 2023 Administrator enhancements

This page describes all administrator enhancements made with the Fourth Quarter 2023 release to the Preview environment. These enhancements will be made available in the Production environment with the 23.10 release.

For a list of all changes available at this point in the Fourth Quarter 2023 release cycle, see [Fourth Quarter 2023 release overview](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Calculated fields on custom forms can now use the $$USER wildcard

The `$$USER` wildcard is now available in calculated custom fields and external lookup fields on the new form designer. Referencing `$$USER` in a calculation adds the current user's ID. You can also use the wildcard with another field. For example, `$$USER.{name}` would add the current user's name.

For more information on calculated fields, see [Add calculated fields with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Add value options from an external API to a custom form

A new field type, **External lookup**, is now available on the custom form designer. When you have data stored on an external system, this field type allows you to load options from an external API and filter based on other field values in the custom form.

When the form is added to an object, the values returned from the API appear in a dropdown field and the user can select one.

>[!NOTE]
>
>The new **External lookup** field type is not available on the legacy form builder.

For more information, see [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
