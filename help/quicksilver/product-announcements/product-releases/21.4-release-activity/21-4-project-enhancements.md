---
title: 21.4 Project enhancements
description: 21.4 Project enhancements
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
---
# 21.4 Project enhancements

This page describes all Project enhancements made with the 21.4 release to the Preview environment. These enhancements will be made available in the Production environment the week of October 4, 2021.

For a list of all changes available with the 21.4 release, see [21.4 Release overview](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Include images in updates

On the Updates tab of an object, you can now add images by clicking the Image icon on the toolbar. You can also drag and drop an image into the update area. Note that your Workfront administrator must enable adding images before you can see the Image icon.

You can add images in both updates and replies. An image thumbnail in the update indicates that recipients can preview the image in the browser or download it, and email and in-app notifications show that images are attached to the update.

Previously, the only way to share an image in Workfront was to attach it to an object as a document. Images added on the Updates tab are only available on that tab and not on the Documents tab.

For more information, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Before Workfront users can include images in updates, this feature must first be enabled by the Adobe Workfront administrator, as described in [Configure preferences for user updates](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## Updated algorithm for smart assignments

We have improved the algorithm used when making smart assignments. With the new improvement, Workfront looks at the 30 most recent assignments made by the logged-in user to make suggestions when they assign tasks and issues. The list of suggestions can contain up to 50 users.

Prior to this enhancement, Workfront was considering the assignments on the parent tasks and other user attributes related to those assignments when suggesting users.

For information about smart assignments, see [Smart assignments overview](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## New experience when creating a project from a template

To make your use of Workfront consistent with the new Workfront experience, we have redesigned the interface for creating a project from template. The functionality for creating a project using a template has not changed. However, some of the improvements of this newly redesigned interface include the following:

* Preview template information before attaching it
* Add templates to a list of favorites during the project creation process

We have updated the interface for creating the project both when you create it from the Projects as well as from the Templates area.

For information, [Create a project using a template](../../../manage-work/projects/create-projects/create-project-from-template.md).

## New experience when attaching templates to projects

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

To make your use of Workfront consistent with the new Workfront experience, we have redesigned the interface for attaching a template to a project. The functionality for attaching a template has not changed. However, there are some of the improvements of this newly redesigned interface that include the following:

* Preview template information before attaching it
* Add templates to a list of favorites during the attachment process
* View all options for managing template and project settings in one continuous page

For information, see [Attach a template to a project](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Unified duration and duration unit values for tasks

For a cleaner and more streamlined user experience, we have merged the value of the Duration field with the duration unit of time. Prior to this enhancement, the unit of time displayed in a separate drop-down field after the Duration field.

In addition to the Duration fields in the Task Details, Edit Tasks and New Task boxes, we are also updating the following fields to match this experience:

* Duration field when making advanced assignments
* Leveling Delay field when creating or editing a task
* Frequency field when creating a recurring task (available soon)
* Lag field when adding a predecessor (available soon)

For information, see [Edit tasks](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## Disable adding issues inline on projects

To ensure that users provide accurate information when adding issues to projects by completing an issue form, we have introduced a new setting that allows you to manage whether they can add issues to a project or its tasks inline. This setting is enabled by default in the new Issue Settings area of the Edit Project box. Disabling it dims the Add More Issues option in the Issues section of a project so users cannot add any more issues in the list. Users can still add issues to the projects by using the New Issue option in the Issues section or using a request queue if one is configured for the project.

>[!NOTE]
>
>This setting is available only in the new Workfront experience. Users who work in Workfront classic can still add issues inline to a project or its tasks even if this setting has been disabled for the project by a user working in the new Workfront experience.

For more information, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

## Custom field display improvement for checkboxes and radio buttons

Viewing and selecting checkbox and radio button options in custom forms just became easier—a custom field with many checkbox or radio button options now displays in multiple columns across the page. Previously, they displayed in a single column, which required extra scrolling for users filling out the form.

This does depend on how you position the fields in the custom form—if you place another field in the same row with the checkbox or radio button field, the options might have only enough horizontal space to display in a single column.

For information about filling out a custom form, see [Edit information in custom form fields](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

For information about creating a checkbox or radio button field in a custom form, see the sections [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) and [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#configur) in the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

