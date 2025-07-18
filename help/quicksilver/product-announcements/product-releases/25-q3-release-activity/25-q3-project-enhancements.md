---
title: Third Quarter 2025 Project enhancements
description: Third Quarter 2025 Project enhancements
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
hide: yes
hidefromtoc: yes
exl-id: 33fa5a61-5300-402c-9f80-f2701f7999a8
---
# Third Quarter 2025 Project enhancements

This page describes Project enhancements made with the Third Quarter 2025 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Third Quarter 2025 release cycle, see [Third Quarter 2025 release overview](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Updates to experience when making a request

>[!NOTE]
>
>* Preview: July 9, 2025
>* Production fast release: July 17, 2025
>* Production for all customers: July 17, 2025

We've updated the experience when making a request in the new requesting experience. 

* The available request forms and paths appear in a list, instead of on cards. The most recent appear in a section near the top.
* All request forms, including Workfront and Workfront Planning request forms, appear in the list. Previously, only the first 50 appeared.
* Request paths and Request forms are listed in separate sections, both in the Recent area and in the larger list below.
* When you search for a request queue, the list filters to display only forms and paths that include the search term. The search term is highlighted in each displayed request form or path.

For information on making a request, see [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Existing Actual Hours field replaced with Legacy Actual Hours and new Actual Hours field created 

>[!NOTE]
>
> Preview and Production: June 24, 2025 

We added a new Actual Hours field that stores the time logged for projects, tasks, and issues in hours, with decimal precision. The field is stored in the Workfront database as `actualWorkRequiredDouble`. 

The existing field of Actual Hours has been renamed to Legacy Actual Hours. The field stores the time logged for projects, tasks, and issues in minutes and is stored in the Workfront database as `actualWorkRequired`.  

Both the Actual Hours and the Legacy Actual Hours fields are visible in project, task  and issues views and reports.

The Actual Hours field visible in the project, tasks, and issues Details section represents the new Actual Hours.

>[!IMPORTANT]
>
>Depending on when the hours were logged, there might be a discrepancy between Actual Hours and Legacy Actual Hours for a project, task, or issue.<br>
>The following scenarios exist:
>
>* Actual Hours represent hours logged for projects, tasks and issues since May 2021.
>* Legacy Actual Hours represent hours logged for projects, tasks and issues for the life of the project, task, or issue. This includes hours logged before May 2021 until the current time. 
><br>You might need to update your reports to reflect the new field and its values.
><br>Workfront uses Legacy Actual Hours to calculate Actual Labor Costs.

For information, see [View Actual Hours](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).


## Change in the way Actual Hours are stored in the database for API calls

>[!NOTE]
>
>* Preview: With the next API version, scheduled for later in 2025
>* Production fast release: With the next API version, scheduled for later in 2025 
>* Production for all customers:  With the next API version, scheduled for later in 2025

This update introduces a change in the way the Actual Hours for projects, tasks, and issues are stored in the database. Starting with this update, the Actual Hours will be using a valuefield of `actualWorkRequiredDouble` (with a value in hours).

Prior to this update, the Actual Hours were stored with a valuefield of `actualWorkRequired` (with a value in minutes). This update will ensure a more accurate count for the Actual Hours when calculating them using an API call.

Because of this change, you might need to update any API calls that refer to the original valuefield. You should make no changes if you are using a valuefield of `actualWorkRequiredExpression` in the API calls.

This update does not change the calculations for Actual Hours for projects, tasks, and issues, in calculated custom fields columns.

## Update in using the Percent Complete slider in a task or issue header

>[!NOTE]
>
>* Preview: May 27, 2025
>* Production fast release: May 27, 2025 
>* Production for all customers:  May 27, 2025

We have updated the way the percent complete slider works for tasks and issues.

The following functionality is now available:

* When you slide the Percent Complete blue bubble in a task or issue's header, the Percent Complete of the task or the issue will now update in five point increments. Prior to this update, sliding the blue Percent Complete bubble updated the tasks or issues in one point increments.

* You can double-click the blue bubble and manually update it with any desired number without using the slider. This functionality has not changed.

There are no other changes introduced to updating the Percent Complete of tasks and issues in other areas of Workfront.

For information, see [View and update Percent Complete for tasks](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

## More transparency when using AI Assistant on projects, tasks, and issues

>[!NOTE]
>
>* Preview: May 19, 2025
>* Production fast release: May 19, 2025 
>* Production for all customers:  May 19, 2025

To make it more clear how AI Assistant is locating answers to questions about Workfront projects, tasks, and issues, we've added this information to the question response. Now, AI Assistant includes its search information in the output. You can use this information as a way to check that AI Assistant correctly identified the question you were asking and to understand the context of the answer. 

Previously, this information was not available in the AI Assistant's response. 

For information about using AI Assistant to get information about Workfront items, see [Use AI Assistant to work with projects, tasks, and issues](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).


