---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 other enhancements
description: This page describes all other enhancements made with the 2020.2 release to the Production environment. These enhancements were made available in the Production environment the week of May 11, 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
---
# 2020.2 other enhancements

This page describes all other enhancements made with the 2020.2 release to the Production environment. These enhancements were made available in the Production environment the week of May 11, 2020.

For a list of all changes available with the 2020.2 release, see [2020.2 release overview](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## For Workfront administrators: Newer Layout Templates created in Workfront Classic now available in the new Workfront experience

Layout Templates created in Workfront Classic after Fall 2019 are now available in the new Workfront experience. It's a good idea to update these Layout Templates in the new Workfront experience to take advantage of new functionality and make them as useful as possible to users in that environment.

For more information, see [Layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

**Available in these environments:**

* The new Adobe Workfront experience

## Group-specific Approval Processes are available for all objects

To fully utilize group-specific approval processes, you can now add them to tasks, issues, and projects when you edit these objects.

You can also automatically attach a group-specific approval process to a task in the Tasks area of the Edit Project box, as well as to issues, when configuring request queues or Queue Topics on a project.

For information about adding approval processes to projects, tasks and issues, see the following articles:

* [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md) 
* [Edit tasks](../../../manage-work/tasks/manage-tasks/edit-tasks.md) 
* [Edit issues](../../../manage-work/issues/manage-issues/edit-issues.md) 
* [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) 
* [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## Create approval processes for groups using custom statuses

To make it easier for groups to manage their own unique workflows, you can now use group-specific custom statuses in approval processes.

Previously, a group could not use its own custom statuses with its group-specific approval processes. Only system-wide statuses were available and these didn't always fit group approval processes.

Custom statuses can be used now in both single-use and system-wide approval processes:

* Create a single-use approval process for an object (project, task, or issue) and base it on statuses that are associated with the group working on that object. This includes any custom statuses associated with the group.
* Create a global approval process and make it available only for the group or for everyone in the system.

For users with administrative access to approval processes, information about configuring approval processes is available in [Create an approval process for work items](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (or if you are using Adobe Workfront Classic, see [Creating Approval Processes](https://one.workfront.com/s/article/Creating-Approval-Processes-1001577410)).

For users, information about associating approval processes with work items is available in [Associate a new or existing approval process with work](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (or if you are using Adobe Workfront Classic, see [Associating a New or Existing Approval Process with Work](https://one.workfront.com/s/article/Associating-a-New-or-Existing-Approval-Process-with-Work-708455630)).

**Available in these environments:**

* Adobe Workfront Classic 
* The new Adobe Workfront experience

## New overlay pages for Search

To allow users to more easily navigate back and forth between search pages and previous pages in the new Workfront experience, we've added a search overlay page that partially covers the screen.

Now, when you click Advanced Search in the Search menu or perform a basic search, a page slides open from the right side of the screen.

For more information, see [Search Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

**Available in these environments:**

* The new Adobe Workfront experience

## Updates to Event Subscriptions

To better enable users to triage, troubleshoot, and resolve issues, we've modified behavior and added more data to the Event Subscriptions API. We've also made the following changes:

* Migrated underlying messaging technologies 
* Rebuilt the service to have less complex dependencies and thus scale more efficiently 
* Made improvements to monitoring and alerting

To learn more, see [FAQs - Event Subscriptions](../../../wf-api/general/event-subs-faq.md) and [Event subscription best practices](../../../wf-api/general/event-sub-best-practice.md).
