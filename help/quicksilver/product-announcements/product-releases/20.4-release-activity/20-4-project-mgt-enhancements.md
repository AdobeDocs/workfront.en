---
title: 20.4 Project management enhancements
description: 20.4 Project management enhancements
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
---
# 20.4 Project management enhancements

This page describes all project management enhancements made with the 20.4 release to the Preview environment. These enhancements will be made available in the Production environment the week of November 9, 2020.

For a list of all changes available with the 20.4 release, see [20.4 release overview](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## New for administrators: Control how a custom field is shared

To give you greater control over who can edit, delete, and use custom fields you create, we have added the ability to configure exactly how you want them shared.

Up until now, when you created a custom field, it was editable by everyone in the system. This is still the default state of a custom field, but now you can limit the sharing of a custom field to certain users, roles, teams, groups, and companies. And you can determine whether your recipients can manage or only view the custom field.

Also, to make this experience familiar for you, we've designed the user interface for this capability to be similar to other object areas sharing throughout Workfront.

For more information, see [Configure sharing for custom fields and widgets](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md).

## New for administrators: Standardized Custom Form sharing

We have standardized sharing for Custom Forms so you can use the same Workfront object sharing process you already know. And the new sharing experience gives you greater control over who can edit, delete, and use Custom Forms you create. You can limit sharing for a Custom Form to certain users, roles, teams, groups, and companies. And you can determine whether those recipients can view or manage the Custom Form.

For more information, see [Share a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Export custom forms and overview information from the Details section of a project, task, or issue

You can now export the custom form information to a .pdf file. You can export custom forms from projects, tasks, or issues when you access the form in the Details section of the objects.

In addition to exporting the custom forms of projects, tasks, and issues, you can now also include the Overview area to your exported pdf.

For information about exporting custom forms from an object, see [Export custom forms and object details](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Quickly add an iteration

>[!NOTE]
>
>This feature has been temporarily removed from the Production environment. This page will be updated when the feature becomes available.

To simplify the experience of creating an iteration, we've added a new button that allows you to add an iteration from the iterations tab. Here, you can create an iteration, then add tasks and issues later.

You can still create an iteration on the backlog tag as before.

For more information, see [Create an iteration](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## New Metrics section available in projects

To save time and increase understanding of the overall health of a project, there is now a Metrics section available in a project that includes information around the following:

* Work that is complete, incomplete, overdue, and upcoming
* Task and issue amounts grouped by status or priority
* Work effort assigned to each user

You can make selections on the charts to see different aspects of the tasks and issues in a project and click certain elements to display task information.

This feature is now included in the [Planner Fundamentals, Part 3 learning path](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA) on Workfront One.

## New for administrators: Assign a business leader to a group

To help you better organize and define your groups, we've added the ability to assign a user as a Business Leader for a group (or subgroup). A Business Leader is a Workfront user who makes business decisions for a group.

The new Business Leader field can be used in report filters, views, and groupings. For example, you can filter by a certain Business Leader to list only the groups for whom that person is assigned in that role.

For more information, see [Business Leader overview](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One.

## New for administrators: Associate portfolios, programs, and companies with groups

When Workfront administrators create or edit a portfolio, program, or company, they can assign it to a group. With groups assigned to these objects, it's easy to identify your group's responsibilities for them.

For example, you can list all of your organization's portfolios in a report and look at the Group column to see which ones your group is working on.

For more information, see the section "About associating a group with an object" in the article [Groups overview](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One.

## New for administrators: Administrators for a group assigned to a company can manage the company

We have made it easy for a Group Administrator to manage a company that is associated with their group in Workfront. Access to manage the company is automatically available when the association is made. This is especially important when the Group Administrator does not have administrative access to companies.

For more information, see [Create and edit companies](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

For information about administrative access to companies, see [Grant users administrative access to certain areas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One.

## Replace the Work On It button with a Start button

To help capture the date and time work actually starts on a work item, users can replace the Work On It button with a Start button that automatically updates the status and the Actual Start Date of the work item.

Updated on September 24th: After clicking Start task or Start issue, you now have the option to revert your choice and indicate that you might not be ready to start working on a work item by clicking Undo. The work item returns to a status of New and the Commit Date and Actual Start Date are deleted. The Undo option displays for a very short time and is cleared after you navigate away from or refresh the page.

For more information on configuring this option, see [Replace the Work On It button with a Start button](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

This feature is now included in the [Worker Fundamentals learning path](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA) and the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One.

## Allow multiple drafts for a queue topic

To give you more freedom when working with requests, there is no longer a limit for how many drafts you can save for one queue topic. When creating a new request, you can select an existing draft from a list of drafts for the same queue topic, overwrite it and submit it as a new request or you can create a new request from scratch.

Prior to this enhancement, Workfront saved only one draft for each queue topic in your request queue.

For information about submitting requests, see " [Create and submit Workfront requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Assign a group to a team

To make it easier to manage and report on the teams that are associated with a group, you can now assign any group to a team that you have access to edit.

When you assign a team to a group, its Group Administrators can manage the team without being a member of it. On the Team Details page, they can see the teams assigned to groups they manage. And they can run a report to list all teams associated with a certain group.

For more information, see [Create a team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One.

## New fields allow you to report on data for a top-level group and all its subgroups

To help you identify data associated with a top-level group and its subgroups, we have added a new Top Parent ID field that you can use in Filters, Views, and Groupings when you create reports about Group objects.

This field should be especially useful for Group Administrators who manage groups that contain several subgroups.

For example, imagine that you manage a group called Marketing that has the subgroups Field Marketing and Digital Marketing. You could list the projects that belong to all 3 groups by creating a Projects area filter that has the following Filter Rule:
<pre>Group: Top Parent Name > Equal > Marketing</pre>We have also added a new Top Parent Name field that you can use to identify data associated with top-level groups in Views (not in Filters or Groupings).

For information about using fields in lists and reports, see [Glossary of Adobe Workfront terminology](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## New option to cancel your action when discarding a request draft

When discarding a saved draft, you can now click Cancel on the confirmation message that informs you that your draft will be deleted. This way, you don't lose the draft in case you change your mind about discarding it.

This feature is available only in the new Workfront experience. For information, see [Create and Submit Workfront requests](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html).

