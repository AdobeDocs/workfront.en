---
content-type: release-notes
keywords: notes,quarterly,update
navigation-topic: product-releases
title: 21.1 Administrator enhancements
description: This page describes all Administrator enhancements made with the 21.1 release to the Preview environment. These enhancements will be made available in the Production environment the week of February 15, 2021.
author: Luke
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
---
# 21.1 Administrator enhancements

This page describes all Administrator enhancements made with the 21.1 release to the Preview environment. These enhancements will be made available in the Production environment the week of February 15, 2021.

For a list of all changes available with the 21.1 release, see [21.1 release overview](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Introduce new Access Level setting for copying projects

To give you more control, as a system administrator, to what Planners can do with a project, we have made the Edit access to projects in the access level more granular, by introducing a new setting that allows you to enable or disable their ability to copy projects. Prior to this change, when you enabled users' access to Edit projects, they automatically had access to copy them. With the new feature, you can give someone access to edit projects without necessarily having access to copy them by disabling the new Copy setting.

If your users had access to Edit projects in their access level prior to this change, they will automatically have this setting enabled when this feature is released.

For information about the Plan access level, see [Grant access to projects](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

For information about copying a project, see [Copy a project](../../../manage-work/projects/manage-projects/copy-project.md).

This feature is now included in the [Administrator Fundamentals in the new Workfront experience, Part 1: User Organization](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) learning path on Workfront One.

## In a Custom Form on an object, select all items in a multi-select drop-down field

>[!NOTE]
>
>This functionality isn't currently available when you are submitting a new Request.

On the Details page for an object, when you are filling in a multi-select drop-down field on a Custom Form, you can click Select All if you need to select all of the available options.

For information about editing data on a Custom Form, see [Edit information in custom form fields](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Recalculate all Custom Form fields for an object

Now it's easier to ensure that all data in calculated custom fields is current for an object. A new Recalculate Expressions menu option lets you quickly recalculate all data in these fields.

This is especially useful after someone edits data in another object that is referenced by a calculated custom field in your object.

Previously, users had to use workarounds to ensure that all data in calculated custom fields was current. For example, they edited the object along with other objects to use the recalculation option that is available for bulk editing.

For more information, see [Edit information in custom form fields](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Unlock task and issue preferences for Group Administrators

>[!NOTE]
>
>Until June 24, 2021, this was available as part of a phased rollout only for customers who have the ability to unlock project preferences for groups. Now it is available for all customers.

Adobe Workfront administrators can now give Group Administrators more autonomy by unlocking individual task and issue preferences. When a preference is unlocked, Group Administrators can configure it for their groups to serve each group's unique needs and internal processes.

For more information, see [Configure task and issue preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

This feature is now included in the [Administrator Fundamentals in the new Workfront experience, Part 2: Project Setup](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY) learning path on Workfront One.

## Configure access level settings for portfolios and programs separately

Now it's easier to manage user access to portfolios and programs because you can configure their access level settings separately.

Previously, the access level settings for portfolios and programs were combined. This meant that you couldn't configure access settings for programs without configuring them the same way for portfolios, and the same was true in reverse.

For information about configuring an access level, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

For information about access settings that you can configure for programs and portfolios, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

This feature is now included in the [Administrator Fundamentals in the new Workfront experience, Part 1: User Organization](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) learning path on Workfront One.

## Select all checkboxes in a series when editing information in a Custom Form

>[!NOTE]
>
>This functionality isn't currently available when you are submitting a new Request.

On the Details page for an object, when you are filling in a Custom Form field containing checkboxes, you can click Select All if you need to select all of the checkboxes available.

This option displays only if the field contains more than 2 checkboxes.

For more information, see [Edit information in custom form fields](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Configure your Workfront email allowlist

To better secure your data, you can now use an email domain allowlist to:

* Control where Workfront emails can go if they contain reports or documents stored in Workfront
* Control email domains can be in the email address that users can specify in their user profile

For example, if you want to protect sensitive data, such as a report listing your at-risk customers, you can include only your internal email domain or domains in the email allowlist. That way, users cannot send that report (or any other Workfront report) to an external email address.

For more information, see the section [Configure your firewall's allowlist](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) in the article [Configure your firewall's allowlist](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Assign a Group Administrator for a subgroup

To make it easier for the levels of your organization to operate independently, we have added the ability to assign a Group Administrator to a subgroup. Now you can make sure you are delegating subgroup management to the right people.

Previously, only a top-level group could have Group Administrators, and those administrators managed all of the subgroups beneath the top-level group.

For more information, see the section [Group administrators for subgroups](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) in the article [Subgroups overview](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

This feature is now included in the [Administrator Fundamentals in the new Workfront experience, Part 1: User Organization](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) learning path on Workfront One.

## Configure event notifications for groups

>[!NOTE]
>
>Available as part of a phased rollout only for customers who have the ability to unlock project preferences for groups. This includes all customers on Cluster 4 and 6 and a small number of customers on other clusters. This note will be updated as the functionality becomes available to more clusters.

Workfront administrators can now give Group Administrators more autonomy by allowing them to configure event notifications for their top-level groups. Subgroups inherit event notification configurations from their top parent group.

Previously, event notifications were configurable only by a Workfront administrator at the system level, which means that all groups had to use the same set of event notifications.

For more information, see the following articles:

* [Unlock or lock configuration of event notifications for all groups](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) 
* [View and configure event notifications for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

This feature is now included in the [Administrator Fundamentals in the new Workfront experience, Part 1: User Organization](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) learning path on Workfront One.

This feature is now included in the [Email and In-App Notifications in the new Workfront experience](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) learning path on Workfront One.

## Work with group projects and approval processes in the Groups area

If you are a Group Administrator, it's easy to view and work with your group's projects and approval processes now that they are listed in the Groups area. From a group's main page, you can:

* Click Projects in the left menu to see the group's projects and create new ones for the group. If a selected project has been shared with you, you can use the buttons in the toolbar to edit, export, copy, or delete it.

  For more information, see [Create and modify a group's projects](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* Click Approvals in the left menu to see and manage all of the approval processes associated with the group.

  For more information, see [Group-level approval processes](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

This functionality is also available for Workfront administrators.

## View the number of licenses used and allocated in a group

To determine how well your licenses are distributed, you can now view the number of licenses that are used in a group and any subgroups below it.

If you manage a top-level group, you can view both the number of licenses that are used in a group (and its subgroups) and the maximum number of licenses allocated for the group.

For more information, see [View the number of licenses allocated and used in a group in the new Adobe Workfront experience](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

