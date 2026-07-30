---
title: Fourth Quarter 2026 Administrator enhancements
description: Fourth Quarter 2026 Administrator enhancements
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
---
# Fourth Quarter 2026 Administrator enhancements

This page describes Administrator enhancements made with the Fourth Quarter 2026 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Fourth Quarter 2026 release cycle, see [Fourth Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Group administrators can manage business profiles

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

Group administrators can now create, edit, and delete business profiles for the groups they administer, without requiring System Administrator access. This gives organizations more flexibility to delegate business profile management at the group level.

For more information, see [View and manage business profiles](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-business-profiles.md).

## Layout template support for views on enhanced lists

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

Views for enhanced lists are now supported at the system level via a layout template. You can hide existing system views, assign a specific view as a default view, and add a custom view to the list of system views.

Examples of enhanced lists in the layout template are **All Requests** and **Advanced Assignments**. An enhanced list has a "New Experience" label next to the views.

For information, see [Customize Filters, Views, and Groupings using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Bulk edit of external lookup fields

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

Bulk edit dialogs now allow the editing of external lookup fields. This was not previously possible.

In situations where a lookup field is dependent on another lookup field, the field with the dependency cannot be bulk edited unless the first field is the same for all objects being edited.

For example, a list of countries depends on the selection made for a region. If the region for one project is Asia and the region for another project is Europe, and you bulk edit both projects, the country field will not be available because the regions do not match. If you edit the region to be the same for both projects, then you can also select a country to use on both projects.

For information on external lookup fields, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-external-lookup-fields).

## Advanced logic supported in custom form designer preview

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

The custom form designer preview mode now supports advanced logic options including advanced display logic, default value logic, validation logic, formatting logic, and editability logic. You can test the logic formulas in the form preview and adjust them as needed in the logic builder. You can also select a test object (project, task, issue, etc.) to preview the form with real contextual data.

Previously, only the basic display and skip logic options were supported in preview mode.

Note that these logic types are only available for organizations on the Workflow Prime or Ultimate packages: advanced display, default value, conditional formatting, and editability.

For more information, see [Add logic rules to custom forms and fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md) and [Organize and preview a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Change tracking for unified review and approval

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

The Change History page in Workfront now captures activity across unified review and approval workflows, giving administrators a complete governance trail for review and document lifecycle events.

Approval, stage, and participant actions are now tracked. These actions may include:

* Making an approval decision in the Frame.io viewer
* Creating or deleting an approval
* Updating a document such as renaming, moving, or deleting it

Each entry includes the standard tracked fields: date and time, operation, user name (or "system generated"), and object name. MCP activities are captured, including which LLM (such as Claude) made the update. Frame.io viewer comments are not included.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

## Define a custom application as a landing page in the layout template

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

You can now set a custom application as the landing page in a layout template. Custom applications that have already been added to the Main Menu are available to use as a landing page.

Custom applications must be created separately before they become available as Main Menu or landing page options. 

For more information, see [Customize the landing page using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md) and [Create custom applications for Workfront with Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Configure tracked fields in change history

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

You can add fields you want to track for a particular type of object throughout Workfront. When users change information in that field, the system records information about the change as an entry in the change history.

Previously, the Configuration screen for defining the tracked fields was view-only.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

## Administrative access to change history added to access levels

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

On the Standard access level, you can now define whether users with that level should have access to the Change History List. The **Change history** option is available in the **Allow administrative access for** section on the access level.

For more information, see [Grant users administrative access to certain areas](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md) and [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).


