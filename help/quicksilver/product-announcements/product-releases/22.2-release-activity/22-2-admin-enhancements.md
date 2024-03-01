---
title: 22.2 Administrator enhancements
description: 22.2 Administrator enhancements
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
---
# 22.2 Administrator enhancements

This page describes all Administrator enhancements made with the 22.2 release to the Preview environment. These enhancements will be made available in the Production environment 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

the week of April 4, 2022. For a list of all changes available with the 22.2 release, see [22.2 Release overview](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Configure a custom form to work with multiple object types

Now you can configure a new or existing custom form to work with multiple object types, making the form much more widely useful. Users will be able to attach and fill out the form on objects of all types that you configure it for.

Previously you could configure a custom form to work with only one object type.

This functionality works with all custom forms created previously in your Workfront system. For example, if you already have a custom form that was created for the Task object type, you can now configure the form to work with other object types as well, such as Project and Issue.

For more information, see the section [Start creating a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start) in the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>* At the time of our initial Preview release of this functionality, we temporarily disabled the ability to copy a multi-object custom form. That ability was enabled on March 24. For information about copying a custom form, see [Copy a custom form to create a new one](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).
>* In a calculated custom field, some fields that you reference might not be compatible with object types that are configured for the form. Our solution is a wild card that will allow the calculation to output different values, depending on the object that the form is attached to. We added the wild card on March 24. For information on how to use it, see the section [Calculated custom fields in multi-object custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat) in the article [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
>* For section breaks in custom forms, we've created a set of common viewing and editing permissions that work for all object types that you can configure for a form. In one scenario, we found that one of these permissions, Limited Edit, might cause errors on a form. This was fixed on March 24. For more information about section breaks, see [Add a section break to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).
>

## Blueprints catalog is available to all users, and administrators can allow requests

All Adobe Workfront users can now browse the catalog of available blueprints. For more information, see [Browse the blueprints catalog and request installation of blueprints](../../../administration-and-setup/blueprints/browse-catalog.md).

Additionally, the system administrator can enable access for users to request installation of blueprints. Assigning a request queue to store the requests allows users to make requests from the blueprints catalog. For more information, see [Configure access to blueprints](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## Add an image to a custom form

In a custom form that you create or edit, you can now add an image and include an informational or instructive tooltip that users can read when they hover over it.

This could be helpful, for example, to show branding for a new product, or to provide visual information that people need when they are filling out the form.

Previously, custom forms were completely text based.

>[!NOTE]
>
>In the new Adobe Workfront experience areas that haven't been modernized yet, such as the box that displays when you bulk-edit items, custom form images do not display. They will display as we continue to update those areas.

For more information, see [Add or edit an asset widget in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## New default access level configurations

To better suit the needs of most administrators who create new access levels, we have changed the default configuration for the "Fine-tune your settings" options listed below. These display when you click the gear icon ![](assets/gear-icon-in-access-levels.png) on an Edit button.

All of these changes disable an option that was previously enabled by default. If this doesn't suit the needs of your organization, you can enable them when you are setting up a new access level, or any time later.

>[!IMPORTANT]
>
>This default configuration change affects only access levels that you create from now on, not any that you created previously.

* In a new access level with a Plan license type:

   * Share System-wide is now disabled for projects, tasks, issues, portfolios, programs, reports, filters, documents, and templates.
   * View Built-In Reports and Share Reports Publicly are also disabled for reports.
   * Share Documents Publicly is also disabled for documents.

* In a new access level with a Work license type:

   * Share System-wide is now disabled for filters and documents.
   * Share Documents Publicly is also disabled for documents.

* In a new access level with a Request or Review license type:

   * Share System-wide is now disabled for filters.

## Deactivate a group

As your internal organizations change, you might need to stop using certain groups in Workfront and create new ones. To help with this, we have added the ability to deactivate a group without losing its historical data. For regular users who don't need to see them, inactive groups are cleared from group type-ahead fields.

You can still find and configure options, preferences, and object associations for inactive groups that you manage. And deactivating a group doesn't change anything about the objects that the group is attached to.

Previously, it wasn't possible to deactivate a group.

For more information, see [Deactivate or reactivate a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Blueprints installation history enhancements

When you install a blueprint, a message now displays the specific objects (such as roles, teams, or groups) that were successfully installed with the blueprint and any objects that failed to install. You can also view the list of installed objects on the Blueprint Details page by clicking View Details next to a specific installation in the installation history table.

For more information, see [Install a blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).

![](assets/blueprints-installation-history-350x95.png)

## A warning now displays when installing a Preview-only blueprint in Production

Certain blueprints are only available to install in the Preview environment for testing purposes.

If you access Preview-only content in your Production environment, Sandbox 1, or Sandbox 2, the install button is not active, and you might see a warning message.

For more information, see [Install a blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).
