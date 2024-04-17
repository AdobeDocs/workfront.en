---
content-type: release-notes
keywords: notes,quarterly,update
navigation-topic: product-releases
title: 21.1 Project Management enhancements
description: This page describes all Project Management enhancements made with the 21.1 release to the Preview environment. These enhancements will be made available in the Production environment the week of February 15, 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
---
# 21.1 Project Management enhancements

This page describes all Project Management enhancements made with the 21.1 release to the Preview environment. These enhancements will be made available in the Production environment the week of February 15, 2021.

For a list of all changes available with the 21.1 release, see [21.1 release overview](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Export now available in Metrics section on a project

To more easily share the status and progress of a project, you can now export the entire dashboard in the Metrics section of a project to a .png file.

For more information, see [Overview of project metrics](../../../manage-work/projects/manage-projects/project-metrics.md).

This feature is now included in the [Planner Fundamentals for the new Workfront experience, Part 3: Manage a Project](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-MCG6OJL724XRBLHBXEAKGAUZOJ6U) learning path on Workfront One.

## Update issue percent complete when the project or task converted from the issue update

We have updated the way the percent complete of issues works for issues that have been converted to projects or tasks. With the new functionality, when an issue is converted to a task or a project, the percent complete of the issue updates in sync with the percent complete of the resolving task or project when the "Automatically update Resolvable Issue status when the status of the Resolving Object changes" setting is enabled from setup.

For information about converting issues, see [Overview of Resolving and Resolvable Objects](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## New Submitted Requests list

To allow you to manage your Submitted Requests in an easier, more consistent way, we have removed the Requests I've Submitted and All Requests sections in the Requests area and replaced them with a new Submitted list. The list has a familiar look and feel that matches all other lists in the system, allowing you to filter for different categories of submitted requests and quick search for a request that might be hard to find.

For information about how to locate submitted requests, see [Locate submitted requests](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

This feature is now included in the [Collaborator Fundamentals for the new Workfront Experience](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) learning path on Workfront One.

This feature is now included in the [Requests in the new Workfront experience](https://one.workfront.com/s/learningpath3/core-team-requests-in-the-new-workfront-experience-MCHWSSDWRFC5EKXFBXTQ6MJNKE7E) learning path on Workfront One.

## Fields removed from the New Request page

>[!NOTE]
>
>Removed from release.

As part of the redesign of the New Request page, we have updated the New Issue Fields that are set up in the Queue Setup section of a project.

The following New Issue Fields display only when creating an issue from the project's Issues section. They do not display when submitting an issue using a request queue in the Requests area:

* Severity
* Planned Hours
* Planned Start Date
* URL
* Assigned To
* Job Role
* Team

We have replaced the Assigned To, Job Role, and Team fields with the new Assignments field on the New Request page, to efficiently designate a user, job role, or team in a common field as you submit a new request.

For information about defining New Issue Fields for a project, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## New experience when submitting requests in the Requests area

>[!NOTE]
>
>Removed from release; will remain in Preview and release to Production with 21.2.

To bring consistency with the new Workfront experience and create efficiencies for you when submitting requests, we have redesigned the New Request box in the Requests area. The following are some of the improvements:

* A consisted user interface with the rest of the the new Workfront experience
* Eliminated the New Requests area for an easier and more intuitive experience
* A new, more efficient way of attaching documents to your requests

Ability to share a link to the request queue, topic group, or queue topic as you enter the request.

For information about submitting requests, see [Create and submit Workfront requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Share a link to a request queue when submitting a request

>[!NOTE]
>
>Removed from release; will remain in Preview and release to Production with 21.2.

We have now made it possible to share a link to a request queue, topic group, or queue topic As you create a request.

Before you submit a new request, you can copy a link to the request queue, topic group, or queue topic of the request and share it with other users, or embed it in a dashboard.

For information about sharing a link to a request queue when submitting a request, see [Share a link to a request queue](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Search for a group you want to assign to a project and view its details

It's now easier to make sure you identify the right group when you are assigning a group to a project. Hover over the name of a group you find in the Group box, then click the info icon that displays next to the name to view the Group Details tooltip.

This tooltip includes the hierarchy of groups above the group, if any, and the group's administrators.

Depending on the details configured for the group, you might also see the group's Business Leader and description.

With this information, you can be assured that you are selecting the right group to assign to the project.

For more information, see [Manage information in the project Overview area](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## New User Delegation report

Previously, information for task, issue, and project approval delegations could only be viewed by the delegate in their Home area. To allow other users to see this information, Plan users can now create the User Delegation report, which tells you:

* Who has delegated these approvals to another user
* Which user has been delegated these approvals
* The start and end date of these delegations

To learn more, see [Create a User Delegation report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
