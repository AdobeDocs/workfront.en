---
title: Second Quarter 2024 Administrator enhancements
description: Second Quarter 2024 Administrator enhancements
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
---
# Second Quarter 2024 Administrator enhancements

This page describes all administrator enhancements made with the Second Quarter 2024 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Second Quarter 2024 release cycle, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## Display logic and skip logic are now available in the form designer preview mode

>[!NOTE]
>
>Preview release: March 28, 2024; Production for all customers: 24.4 (April 11, 2024)

The beta custom form designer now allows you to test your display logic and skip logic in preview mode. Previously, all fields were displayed in the preview even when logic was applied.

For more information on previewing a custom form in the form designer, see [Organize and preview a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Companies and users now support advanced custom form fields

>[!NOTE]
>
>Preview release: March 14, 2024; Production for all customers: 24.4 (April 11, 2024)

Advanced custom form features such as External Lookup fields and Workfront native fields are now available when you attach a custom form to a company or a user. The advanced features are available on the Company Details and User Details pages, not on the Edit Company and Edit User dialogs. The custom form must be created in the new form designer to take advantage of these field types.

For more information about custom form fields, see [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## JumpSeat integration now available for new package types

>[!NOTE]
>
>Preview release: February 26, 2024; Production for fast release: With the 24.3 release (March 14, 2024); Production for all customers: 24.4 (April 11, 2024)

The existing JumpSeat integration is now available to accounts using one of the new package types (i.e., Select, Prime, or Ultimate). You must still have an active JumpSeat subscription to enable the integration.

For more information on the JumpSeat integration, see [Configure the JumpSeat integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Workfront native fields are available in the form designer beta

>[!NOTE]
>
>Preview release: February 29, 2024; Production for fast release: With the 24.3 release (March 14, 2024); Production for all customers: 24.4 (April 11, 2024)

Fields native to Workfront are now available for you to add to your custom forms. This new field type allows you to organize and present data to your users in a logical way, without having to re-create existing data in custom fields.

After you select Native Field in the custom forms field list to add the field to the form designer, you can select any native field for the form's objects. For example, if the Object Types list at the top of the form designer shows Project, you will be able to select native fields for projects but not fields that are specific to tasks.

When the custom form is attached to an object, the field is populated from the object data. For example, the Description field on a custom form attached to a project will pull in the project description. (The field may show "N/A" if no data is available.)

Native fields used in custom forms become available in the field library in the designer for re-use, They are also visible in the Setup > Custom Forms > Fields area so that you can see which forms they are used in.

This feature is available only in the form designer beta, not in the legacy form builder.

For more information, see [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[View a video demonstration of this feature.](https://video.tv.adobe.com/v/3427702/){target=_blank}

## Attribute mapping now available for organizations that have migrated to Adobe IMS

>[!NOTE]
>
>Preview release: February 22, 2024; Production for all customers: February 22, 2024

Workfront system administrators can now set up user attribute mapping for organization that have migrated to Adobe IMS. This allows user information to pass into Workfront from the organization's SSO (Single Sign-on) provider, so that the user's data does not have to be entered into both Workfront and the SSO provider.

Previously, this functionality was only available to organizations that had not yet been onboarded to Adobe IMS.

For instructions on configuring attribute mapping, see [Map user attributes in the Adobe unified experience](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) in the article **Map user attributes and auto-provision new users**.

## Skip logic and display logic are now available in the form designer beta

>[!NOTE]
>
>Preview release: February 8, 2024; Production for fast release: With the 24.2 release (February 15, 2024); Production for all customers: TBD

You can now edit existing display and skip logic and add new logic to custom forms in the form designer beta. An easy-to-use logic builder helps you define which fields to display or skip based on selections in the form.

Icons on a field in the form designer canvas indicate that logic is configured on that field, or that the field is used in logic rules configured on other fields.

For more information, see [Add display logic and skip logic with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
