---
title: 21.4 Administrator enhancements
description: 21.4 Administrator enhancements
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
---
# 21.4 Administrator enhancements

This page describes all Administrator enhancements made with the 21.4 release to the Preview environment. These enhancements will be made available in the Production environment the week of October 4, 2021.

For a list of all changes available with the 21.4 release, see [21.4 Release overview](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## For administrators: See which groups are associated with an approval process

To help you find out which groups are associated with the approval processes in your system, we've added a Group Name column to the Standard view on the Approvals page in Setup. Now you can view this information without having to create a custom view.

For information about approval processes, see [Approval process overview](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

For information about managing group approval processes, see [Group-level approval processes](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## New for administrators: Groups can configure their own timesheet and hour preferences

>[!NOTE]
>
>Initially, in Production, this functionality will be available as part of a phased rollout only for customers on Cluster 4. This note will be updated as the functionality becomes available to other clusters.

In a large organization, some groups might need to configure timesheet and hour preferences independently to fit their unique workflows, rather than inheriting the preferences configured by an administrator at the system level. Now Workfront administrators can unlock a timesheet and hour preference for all groups in the system so that they can configure it on their own.

This ability was also added recently for project preferences and for task and issue preferences.

For information about how a Workfront administrator unlocks a timesheet and hour preference, see the section [Unlock timesheet and hour preferences for groups](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) in the article [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

For information about how a group administrator configures unlocked task and issue preferences for a group, see [Configure timesheet and hour preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## New for Workfront administrators: Configure layout templates for auto-provisioned users in the new Workfront experience

Now you can configure layout templates in the new Workfront experience for auto-provisioned users. In the Workfront User Attribute drop-down menu where you map user attributes (Setup > System > Single Sign-On), a new "NWE Layout Template" menu item is now available for making this configuration. Previously, you were able to configure layout templates for auto-provisioned users only in Workfront Classic.

For instructions on mapping user attributes, see [Map user attributes and auto-provision new users](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## New field displays the groups your users belong to

Now it's easy to find out which groups your users belong to. In a report or view that lists users, you can create a column using the new Other Groups field. This field lists the groups where each user is a member.

For information about using reports and views, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) and [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Blueprints details page now displays an image

The details page for each blueprint now displays an image of the project template that is installed with the blueprint. The image provides a preview of the blueprint contents so that you know what you are about to install. You can optionally preview the full image in the browser or download the image.

For more information, see [Blueprints overview](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## Blueprints preferences for new issues

New issue preferences are now available for some blueprints. They are installed by default, but you can opt out of installing the preferences when you configure your installation details.

The preferences include queue topic groups, queue topics, and routing rules to collect the correct information when an issue or request is submitted, and send the issue or request to the correct job role or team. Using the preferences helps create consistency in the way that new issues or requests are captured on your projects.

Note that using these preferences does not make the projects created from the template into request queues.

For more information, see [Configure a blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## New for group administrators: View and manage a group's recently deleted and restored items

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

We are continuing to make it easier to manage your groups and their associated objects in one place. Now you can view and work with a group's recently deleted and restored items from the Groups area. This saves you from having to go to the Recently Deleted or Recently Restored area in Setup to manage those items. And it keeps the list of group items you're working with separate from the other deleted and restored items in the system.

For more information, see [View and manage a group's recently deleted items](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) and [View and manage a group's recently restored items](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## New for group administrators: Group preferences now affect group templates

It's now easier to make sure that your group's project templates meet your group's needs. When you assign a new project template to a group at the time when you create it, the template inherits the following settings from the group's project and task preferences:

* Performance Index Method
* Condition Type
* Schedule from
* User time off
* Update type
* Access section settings

When you create a new template task within a project template that is associated with a group, the template task inherits the following settings from the group's task preferences:

* Duration Type
* Revenue Type
* Cost Type

Previously, project templates and project template tasks inherited these settings from the project and task preferences set at the system level.

If you create a template or template task without a group—for example, from the main Templates page—the settings above are inherited from the system-level project and task preferences. However, if you later assign a group to the template or template task, the group's preferences don't affect it.

For more information, see the section How preferences apply to templates and template tasks in the article [Create and modify a group's project templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## New for administrators: Find out which custom forms are using a custom field

Now it's easier to change a custom field in a custom form. With a single click in the custom form, you can find out about any other custom forms that are also using the field. It's important to assess whether those forms will need adjustments in order to keep working properly after you make the change.

For more information, see [View all custom forms that use a particular custom field or widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## New for group administrators: Lock and unlock project, task, and issue preferences for a group

Now you can ensure that everyone in the subgroups below your group is using the same preference settings, or you can allow them to configure a preference setting for their unique workflows.

* After a Workfront administrator unlocks a preference at the system level, you can configure and then lock it for all subgroups below your group. Though you can still reconfigure the locked preference, administrators of lower subgroups can't do so for their groups.

  Conversely, you can unlock a preference for your group. This allows subgroup administrators to configure it for their users' unique project, task, or issue workflow needs.

  For more information, see [Lock or unlock a project, task, or issue preference for subgroups](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* If you are a Workfront administrator, you don't need to go to the Groups area to configure a subgroup's preferences. From the main Project Preferences, Tasks & Issues Preferences, or Timesheets and Hours Preferences area, you can use the search box at the top of the page to find the subgroup and configure its preferences.

  For more information, see [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) and [Configure task and issue preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## New for group administrators: Create and edit templates from the Groups area

>[!NOTE]
>
>This feature is available only in the new Workfront experience.

We're continuing to make it easier to manage your groups and their associated objects in one place. Now you can view and work with a group's templates from the Groups area in Setup. This saves you from having to go to the Templates area to manage a group's templates. And it keeps the list of group templates you're working on separate from the others throughout the system.

For more information, see [Create and modify a group's project templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Enter and save information in one attached custom form at a time

>[!NOTE]
>
>This feature is available only in the new Adobe Workfront experience.

It's now easier to supply information in the Details section for an object: Type and save information in a single custom field or expandable area (such as Overview and Finance), even if required fields in other custom forms on the object are not yet filled out.

Previously, when you entered information in one custom form or expandable area for an object, all custom forms attached to the object went into edit mode and all their required fields had to be completed before you could save your changes. This was a problem if you couldn't complete a required field because it was intended for another user.

If you do want to edit all custom forms and expandable areas in the Details section for an object, you can click Edit all on the new Edit menu that we added to the Edit icon. Or, on the same menu, you can click a name to scroll to the custom form or section where you want to make changes

>[!NOTE]
>
>This feature was originally released to Preview with the 21.3 release.

To make it easier for all levels of an organization to manage and control their workflows independently, we've introduced the ability to create and manage statuses for subgroups. Now, from the Groups section in Setup, you can do the following for groups you administer on any level:

* Create, edit, delete, and hide a status for a group
* Lock a status for any group so that all lower subgroups below it can use it in the same way
* Unlock a status for any group so that administrators of lower subgroups can customize it to meet their unique needs
* Set a group status as a default status
* Reorder and hide the display of group statuses on objects

Workfront administrators can also do these things (for all groups).

Previously, this functionality was available only for top-level groups.

For more information, see [Manage group statuses](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## New for Workfront administrators: Migrate layout templates from Workfront Classic to the new Workfront experience on your own

>[!NOTE]
>
>This feature was released to the Preview environment on July 1, 2021. It will release to the Production environment on July 15, 2021.

To help you manage layout templates while your users switch to using the new Workfront experience, we have created a button you can use to migrate layout templates from Workfront Classic to the new experience without relying on Workfront Customer Support.

Previously, only Workfront Customer Support could migrate your layout templates from Workfront Classic to the new Workfront experience.

## When associating a template with a group, select a group approval process in Queue Details and Queue Topics

We have added a new option to the process of associating a template with a group. Now you can select group-specific approval processes for issues in the template's Queue Details or in one of its Queue Topics.

In 21.3, when we added the ability to associate a group template with a group, you could select a group-specific approval process in the template, but you couldn't do so in the template's Queue Details or Queue Topics.

For more information, see [Associate a new or existing approval process with work](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
