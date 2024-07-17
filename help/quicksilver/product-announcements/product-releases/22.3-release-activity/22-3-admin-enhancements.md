---
title: 22.3 Administrator enhancements
description: 22.3 Administrator enhancements
author: Luke
draft: No
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
---
# 22.3 Administrator enhancements

This page describes all Administrator enhancements made with the 22.3 release to the Preview environment. These enhancements were made available the week of July 11, 2022. For a list of all changes available with the 22.3 release, see [22.3 Release overview](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Integrate Adobe Workfront with JumpSeat

You now can integrate JumpSeat with Workfront to create custom, in-product guidance for your users. You must have an Adobe Workfront enterprise license and an active JumpSeat subscription to enable the integration.

For more information, see [Configure the JumpSeat integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Proof default settings moved to Workfront

You can now edit the following proof settings inside the Workfront Setup Area:

*   Proof default settings
    
*   Proof decision settings

For more information, see [Configure default proof settings](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Use unlocked statuses in an approval processes

**Note:** Removed from the 22.3 Production release. This feature is planned to release to Production on September 15, 2022.

To give you more control over the approval processes and statuses in your system, we've made it possible to create an approval process based on an unlocked system status. Moreover, you can now unlock any status that is already used in an approval process.

Previously, a system status used in an approval process had to be locked. This made it available for all groups—without the possibility of removing or renaming it—so group administrators couldn't streamline their group's list of statuses to fit their specific needs.

For more information, see the following articles:

*   [Create an approval process for work items](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
    
*   [Create or edit a status](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
    
*   [Locked and unlocked system-level statuses](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)
    

## Add a PDF file to a custom form

We are continuing to help you make custom forms more visual and informative with new asset widgets you can add, such as images and videos. Now you can add a link to a PDF file to a custom form. When the form is attached to an object, users who work with the object can view and interact with the PDF from within the form.

## Custom form field calculation editor displays error information

>[!NOTE]
>
>This feature is temporarily unavailable. This page will be updated when the feature is available.

Editing calculations for custom fields is now easier with helpful error information indicated directly in the calculation. While you are creating a calculated field in a custom form, errors are highlighted in pink. When you hover over the highlighted portion, a tooltip displays to describe what the problem is.

## Project header customization

As a Workfront or group administrator, you can now customize the fields that display in the header of a project when you use a Layout Template.

This update includes the following enhancements:

*   Remove existing fields from the project header.
    
*   Add new, non-editable Project Overview fields. You cannot add custom fields or fields that can be edited. Editable fields that are currently on the project header can remain on the header.
    
*   The object header can include up to five fields.
    

Prior to this release, fields in the object headers could not be customized.

For more information, see [Customize object headers using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Control creating a blank project

As a system or a group administrator, you can now control whether users can create blank projects, without using a template. We have introduced a new setting in the Project Preferences area of Setup that allows you to disable creating blank projects in the following areas:

*   From the New Project option in a list of projects
    
*   When converting an issue to a project from the issue page
    

The new setting is "Allow users to create projects without using a template" and it is enabled by default.

**Note:** Users can still convert a task to a blank project.

For more information, see [Configure system-wide project preferences](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Deactivate a group from the Groups page

Recently, we added the ability to deactivate and reactivate groups. To make that action quicker and easier, we have added it to a group's page. Now, after you click a group's name to go to its page, you can select the More menu ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) next to the group's name, then select Deactivate or Reactivate.

Previously, you could deactivate or reactivate a group only by using the Is active check box on its Details page.

For more information, see [Deactivate or reactivate a group](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Add videos to custom forms

Now you can provide a new mode of information, visual interest, and creativity to a custom form by adding a video. When the form is attached to an object, users who work with the object can play the video any time.

Previously, you could add only text-based fields and images to a custom form.

