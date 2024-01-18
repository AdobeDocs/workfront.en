---
title: 22.1 Administrator enhancements
description: 22.1 Administrator enhancements
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
---
# 22.1 Administrator enhancements

This page describes all Administrator enhancements made with the 22.1 release to the Preview environment. These enhancements will be made available in the Production environment 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

the week of January 17, 2022.

For a list of all changes available with the 22.1 release, see [22.1 Release overview](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Document downloads logged in the Updates area

To help your users track downloads of documents they store in Workfront, the system now logs an entry in the Updates area for a document when someone downloads it.

>[!NOTE]
>
>We recommend testing this feature in Preview on a newly uploaded document.

For information about how Workfront logs automatic updates on objects, see [System-tracked updates](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Grant access to teams using access levels

A new section in the Access Levels area gives you more granular controls for managing your users' access to teams. Now you can determine who can create, edit, and view teams.

This does not change your users' existing access to teams.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## Group mapping now available in blueprints

Some blueprints now include groups, which you can customize before installing the blueprint. You can map a group in the blueprint to an existing group in your Workfront instance, or create a new group if needed.

For more information, see [Configure a blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Styling updates in the Custom Forms area

The Custom Forms area has a new look and feel that brings it up to date with many other areas in the new Workfront experience.

For information about creating a custom form, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Many enhancements for creating calculated custom fields

Creating calculated custom fields is now much easier with these additions in the new Calculation Editor:

* You can hover over any expression in your calculation to display information about it, including a description, an example of how it can be used, and a link to more information in a help article.
* Each expression you add is color-coded, depending on its type. This makes it easier to spot your expressions and immediately recognize their type.
* Line numbers help you identify and reference functions in a long calculation.
* When you start typing an expression or field name, a list of available items displays so that you can choose the one you want. And, when you type an open parenthesis, the closing parenthesis is added automatically.
* You can preview the result of your calculation using an existing object without leaving the calculation editor.

Also, in the customizable "Instructions" hover text for a calculated custom field, you can display or hide the field's formula. This is useful if you think that the users who will fill out the custom form won't need that information.

For more information about creating a calculated custom field, see [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## View audit log information about statuses and companies

Now you can more easily troubleshoot incidents involving statuses and companies by viewing information about them in the Audit Logs area in Setup.

For example:

* You can find out who renamed, locked, or hid a status, and when they did so.
* You can find out who removed some members or job roles from a company, and when they did so.

For information about viewing audit log information, see [View and export audit logs](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Blueprints company mapping and other enhancements

The following Blueprints enhancements are now available:

* Some blueprints now include companies, which you can customize before installing the blueprint. You can map a company in the blueprint to an existing company in your Workfront instance, or create a new company if needed.
* A new blueprint type, Organizational Structure, is now available. Some blueprints include elements from multiple types (for example, Project Template and Organizational Structure). You can filter by blueprint type on the catalog page.
* The "Install Preferences" and "Template Ownership" sections on the configuration page have been combined into "Template Preferences" for simplicity.

For more information, see [Configure a blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Manage company memberships more easily

In the Companies area, an updated toolbar makes it easy to add existing Workfront users to a company and to remove company members.

Previously, these actions were available only in the Edit Company box.

The updated toolbar also contains all of the actions that were available in the previous toolbar, such as editing members' user profile information and deactivating them in the system.

For more information, see [Manage company memberships](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Select expressions and fields in the new calculated field window

We're continuing to make it easier to create a calculated field in a custom form. Now, when you click Maximize to open the new Calculation Editor, you can find and select the expressions and fields you need.

For more information, see [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Groups can configure their own timesheet and hour preferences

>[!NOTE]
>
>This feature was initially available as part of a phased rollout only for customers on Cluster 4 as part of the 21.4 release. This feature will be available for all remaining clusters in Production on November 8, 2021.

In a large organization, some groups might need to configure timesheet and hour preferences independently to fit their unique workflows, rather than inheriting the preferences configured by an administrator at the system level. Now Workfront administrators can unlock a timesheet and hour preference for all groups in the system so that they can configure it on their own.

This ability was also added recently for project preferences and for task and issue preferences.

For information about how a Workfront administrator unlocks a timesheet and hour preference, see the section [Unlock timesheet and hour preferences for groups](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) in the article [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

For information about how a group administrator configures unlocked task and issue preferences for a group, see [Configure timesheet and hour preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Select multiple notifications that you want to unlock or re-lock for groups

It's now faster and easier to unlock or re-lock email notifications for groups. Now you can select multiple notifications, check your selections to make sure they're correct, then click the new Unlock or Lock button that displays in the toolbar.

Previously, you had to unlock and re-lock notifications one at a time. Workfront currently has 95 notifications, so this took a while if you had to do it for all or many of them.

For more information, see [Unlock or lock configuration of event notifications for all groups](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## For group administrators: Easier to select a replacement group when you delete a group

When you are deleting a group, two improvements in the Delete Group box make it easier to select the replacement group that you want to preserve the deleted group's users, work items, and subgroups:

* You can start typing the name of the group to find it quickly. Previously, there was only a drop-down list that you couldn't type in. This was problematic for organizations with many groups because you had to scroll through the list to find the group you wanted. Also, the drop-down list had an item limit, so it was possible that the group you wanted wasn't displayed.
* You can use the new info icon to make sure you are selecting the replacement group you want. Hovering over the icon displays a tooltip listing information about the group, such as the hierarchy of groups above it and the names of its administrators.

For more information, see [Delete a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Larger area for creating calculated fields

Now it's easier to build complex calculated fields in a custom form. Click the new Maximize button to open a large editing window for building your calculation. When you are finished, click Minimize to continue working on your custom form.

For more information, see [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Add custom forms to groups

Custom forms are now supported for the Group object. This makes it easier for groups in your organization to capture and share information that meets their specific needs and workflows. Users can do the following for a group, just like they can for other Workfront objects:

* Create a custom form
* Attach a custom form
* Save custom form data
* Remove a custom form
* Edit custom data from lists and, in the new Workfront experience, from the Group page

For information about custom forms, see [Custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Create OAuth2 apps to integrate applications with Workfront

Now you can integrate Workfront with other applications that Workfront doesn't offer a built-in integration for. By creating an OAuth2 app for the application you want to integrate with, you can allow that application to access Workfront, while knowing that your data is protected by the secure, industry-standard OAuth2 authentication protocol.

Previously, you could only integrate with other applications through built-in integrations, Workfront Fusion, or the Workfront API.

For more information, see [Create OAuth2 applications for Workfront integrations](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Interface text improvements in Companies area

In the Companies area in Setup, new confirmation messages and slight wording changes make it easier to manage company memberships. For example, the section name "People" in the left panel is now "Company Members."

For information about managing company memberships, see [Manage company memberships](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
