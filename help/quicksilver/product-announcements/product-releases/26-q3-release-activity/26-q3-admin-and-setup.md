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

<!--

## Change tracking for unified review and approval

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The Change History page in Workfront now captures activity across unified review and approval workflows, giving administrators a complete governance trail for review and document lifecycle events.

Approval, stage, and participant actions are now tracked. These actions may include:

* Making an approval decision in the Frame.io viewer
* Creating or deleting an approval
* Updating a document such as renaming, moving, or deleting it

Each entry includes the standard tracked fields: date and time, operation, user name (or "system generated"), and object name. Frame.io viewer comments are not included.

This phase of change tracking does not include MCP events. Those will be part of a future release.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

-->

## Internal lookup field replacing Typeahead field type

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The new **Internal lookup** field type in custom forms provides dynamic filtering. It is similar to the Typeahead field type and allows users to search and select existing Workfront objects by typing part of the name. The filter on the internal lookup can reference the value in another field on the form, which is not possible with Typeaheads.

Multi-select is supported on internal lookups, and this field type also provides improved performance for large datasets. The following native Workfront objects are supported in internal lookups: Project, Company, Group, Job Role, Portfolio, Program, Team, Template, User, Task, Issue, Document, and Location.

The Internal lookup field type is replacing the Typeahead field type. You can quickly convert existing Typeahead fields to Internal lookups by clicking the button in the field options on the right. When you convert, historical data remains on the field and it is used the same way in reports.

>[!IMPORTANT]
>
>External integrations such as Workfront Fusion scenarios or API-based automations may reference legacy field structures and require updates after the conversion. You should verify any integrations before converting Typeahead fields to Internal lookup fields.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Default value logic supported on native reference fields

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026
>
>This feature is only available for organizations on the Workflow Prime or Ultimate packages.

In custom forms, native reference fields now allow you to add default value logic.

This logic type on native reference fields is available only in the user interface and not in the Workfront API.

For information, see [Add default value logic to a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) in the article [Add logic rules to custom forms and fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

## Updates to native field filtering in custom forms

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

System filters that exist on native fields are now applied to the fields in custom forms and are visible to administrators.

When you add a native reference field that has a system filter applied, you can apply the same filter to the field in the custom form and modify the filter if needed in the Text Mode box.

Adding your own custom filter to the field overrides the system filter for the field. If you do not enter a custom filter, the system filter is applied by default.

Also, dynamic filtering is now available on native reference fields. A dynamic filter allows you to narrow the list of items based on the value of another field.

For example, when you use `?portfolioID={portfolio}.{ID}` in a Project field filter and a Portfolio native field is on the custom form, the Project field shows only projects that are in the selected portfolio. If the Portfolio field is left blank, then all projects are available in the Project field.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Protect field names from accidental renaming

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

To protect integrations and data integrity, we've updated how field names can be edited in the field settings panel of a custom form.

Field names in the field settings panel are now read-only by default. You can still edit the field name, but renaming requires an explicit confirmation step. The field previously called **Name** has also been updated to **API Name** to better reflect its technical significance. The **Label** field remains editable.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

## View change history for Workfront objects

>[!NOTE]
>
>Preview: June 11, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026

To make it easier for you to see the changes that have occurred in one central list, we've create the Change History List. This list displays information such as the object, the operation, and the source of the change (such as a user or the Workfront system).

Previously, Audit logs were available but did not cover objects.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

## New system preference to convert legacy storage portfolios to Adobe cloud storage

>[!NOTE]
>
>Preview: June 11, 2026
>Production for everyone: June 11, 2026
>[!BADGE Off schedule]{type=Neutral}

Workfront administrators can now convert legacy storage portfolios to Adobe cloud storage directly from System Preferences. To convert portfolios, select them in the new Select portfolios to convert to enterprise storage field and save the page.

When a portfolio is converted to Adobe cloud storage:

* You can no longer move projects that use legacy Workfront storage to this portfolio
* All new projects created in this portfolio use Adobe cloud storage
* Frame.io is the viewer for documents using Adobe cloud storage
* Child objects using legacy Workfront storage stay on legacy storage

Previously, adding an Adobe cloud storage project to a Legacy storage portfolio automatically converted the portfolio to Adobe cloud storage.

For more information, see [Configure system preferences](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

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

For more information, see [Configure system preferences](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).
