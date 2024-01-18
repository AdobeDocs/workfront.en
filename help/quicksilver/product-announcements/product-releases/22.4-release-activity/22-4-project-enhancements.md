---
title: 22.4 Project enhancements
description: 22.4 Project enhancements
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
---
# 22.4 Project enhancements

This page describes all Project enhancements made with the 22.4 release to the Preview environment. These enhancements will be made available the week of October 3, 2022. 

For a list of all changes available with the 22.4 release, see [22.4 Release overview](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Predecessor details now available

To view the details of a task's predecessors, you can now hover over the predecessor number in the Predecessors column. The details box displays the predecessor task and project being referenced, planned start and end dates for the predecessor task, and the predecessor task's number of predecessors and successors. You can expand the project details to see more information about the project. Additional information is included for cross-project predecessors.

For more information, see [Create a predecessor relationship on the task list](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Assign multiple teams to a task or issue

To give you much more flexibility in the way you manage tasks and issues, we have made it possible to assign multiple teams to a task or issue. Previously, only one team could be assigned to a task or issue.

>[!NOTE]
>
>This functionality is not currently available in the Workload Balancer in the Teams area.

For more information, see [Assign tasks](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) and [Assign issues](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Smart user selection for project roles in the Edit and Details areas 

We have improved the way users display when you add them to the following project fields from the Edit box and the Details section of the project:  

* Project Owner 

* Project Sponsor 

* Resource Manager 

Now, when you add a user to any of these fields in the Edit or Details areas, in addition to their name and avatar, their Primary Role and their email also display. This helps distinguish between multiple users with similar or identical names.    

For more information, see [Edit Projects](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

NOTE: Additional user fields for projects, tasks, and issues will be updated with this functionality in future releases.

[View a video demonstration of this feature.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## Calculated date fields are always saved based on Coordinated Universal Time (UTC)

Now, you can be sure that all date functions in calculated fields work consistently and produce the same result for everyone, regardless of how a custom data expression is updated, or where users are collaborating on the object across the world. 

All calculations are now calculated and saved by one standard— Coordinated Universal Time (UTC)—not by the time zone configurations set for your organization's instance and your individual user profile. However, calculations are displayed in a custom form based on each users' individual time zones set in their browser.

Previously, time settings in calculations caused confusion when they varied in these situations:

* If someone recalculated a calculated field expression using "Update previous calculations" on the form builder, date function results were determined by UTC time zone of your organization.

* If someone edited the object and that caused the calculated field expression to recalculate, date function results were determined by the user's local time zone. Calculated date field results in this scenario will also be calculated based on the UTC.

For more information, see [Working across time zones](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Custom form enhancements: Adobe XD and the Quick Filter

Based on your feedback, we've introduced the following enhancements to improve your experience when managing custom forms:

* Add an Adobe XD file to make a custom form more visual and informative. When the form is attached to an object, users who work with the object can view and interact with the XD file from within the form.

    For more information, see [Add or edit an image or other asset widget in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Use the Quick Filter to easily locate items in the modernized custom forms and fields list. Also enjoy an improved look and feel while managing your forms and fields.

    For more information about the Quick Filter, see [Apply the quick filter to a list](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[View a video demonstration of this feature.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Public Beta - New filter experience for projects, tasks, and issues

Filtering in project, task, and issue lists has been redesigned to help you create and share filters quickly. Features include:

*   An intuitive "beta builder" interface for creating a new filter
    
*   The ability to mark a filter as a favorite
    
*   Filter stacking (applying more than one saved filter)
    
*   Duplicating filters
    
*   Sharing filters
    
*   Removing filters shared with you
    

The new filter experience is also available in timesheet lists and the Scenario Planner.

Text mode remains available for advanced filter editing, and system administrators can still assign default filters for all users through the layout templates.

### Where will this be available?

*   Project/Tasks/Issues Lists
    
*   Scenario Planner
    
*   Timesheets
    

### We want your Feedback!

With this Public Beta Users are given the opportunity to submit feedback directly to the team working on the filters experience by clicking on the feedback button. We look forward to hearing from you and your users on the new filter experience in public beta. If your team would like to meet with product directly to provide additional feedback, feel free to schedule a meeting here: https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&date=2022-08-25

### What is next?

*   New Groupings and Views (also known as Columns) Experience
    
    We will begin to work on the new experience for groupings and views (also known as columns) so it will be consistent with the new filters experience and have some of the same great features as the new filters experience.
    
*   Implement new filters in other areas of Adobe Workfront
    
    We will work with teams across the product to implement the new filters experience in other areas throughout in Workfront.
    

We want to deliver value to you iteratively so we will continue to deliver as the new experiences and other areas are ready. Stay tuned for more exciting updates.

For more information, see [Filters overview](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) and [Create or edit filters in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[View a video demonstration of this feature.](https://video.tv.adobe.com/v/3412391/)
