---
title: Second Quarter 2024 Administrator enhancements
description: Second Quarter 2024 Administrator enhancements
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
---
# Second Quarter 2024 Administrator enhancements

This page describes all administrator enhancements made with the Second Quarter 2024 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Second Quarter 2024 release cycle, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## Workfront native fields are available in the form designer beta

>[!NOTE]
>
>Preview release: February 29, 2024; Production for fast release: With the 24.3 release (March 14, 2024); Production for all customers: 24.4 (April 2024)

Fields native to Workfront are now available for you to add to your custom forms. This new field type allows you to organize and present data to your users in a logical way, without having to re-create existing data in custom fields.

After you select Native Field in the custom forms field list to add the field to the form designer, you can select any native field for the form's objects. For example, if the Object Types list at the top of the form designer shows Project, you will be able to select native fields for projects but not fields that are specific to tasks.

When the custom form is attached to an object, the field is populated from the object data. For example, the Description field on a custom form attached to a project will pull in the project description. (The field may show "N/A" if no data is available.)

Native fields used in custom forms become available in the field library in the designer for re-use, They are also visible in the Setup > Custom Forms > Fields area so that you can see which forms they are used in.

This feature is available only in the form designer beta, not in the legacy form builder.

The Experience League articles for this feature will be updated by March 7.

## Attribute mapping now available for organizations that have migrated to Adobe IMS

>[!NOTE]
>
>Preview release: February 22, 2024; Production for all customers: February 22, 2024

Workfront system administrators can now set up user attribute mapping for organization that have migrated to Adobe IMS. This allows user information to pass into Workfront from the organization's SSO (Single Sign-on) provider, so that the user's data does not have to be entered into both Workfront and the SSO provider.

Previously, this functionality was only available to organizations that had not yet been onboarded to Adobe IMS.

For instructions on configuring attribute mapping, see **Map user attributes in the Adobe unified experience** in the article [Map user attributes and auto-provision new users](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## Skip logic and display logic are now available in the form designer beta

>[!NOTE]
>
>Preview release: February 8, 2024; Production for fast release: With the 24.2 release (February 15, 2024); Production for all customers: TBD

You can now edit existing display and skip logic and add new logic to custom forms in the form designer beta. An easy-to-use logic builder helps you define which fields to display or skip based on selections in the form.

Icons on a field in the form designer canvas indicate that logic is configured on that field, or that the field is used in logic rules configured on other fields.

For more information, see [Add display logic and skip logic with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).