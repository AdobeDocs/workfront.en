---
content-type: o
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Work On It and Done button overview
description: When you are assigned to a task or issue, you can use a contextual button that changes names and function depending on your involvement with the work item.
author: Lisa and Alina
feature: Get Started with Workfront
role: User
exl-id: cfda6702-1a9a-4645-b031-8b2f201ac0af
---
# Work On It and Done button overview

When you are assigned to a task or issue, you can use a contextual button that changes names and function depending on your involvement with the work item.

Using the contextual button to accept or complete work items, you can let Adobe Workfront update several fields on the items without having to manually update them yourself.

## Work on it and Done button names

Depending what area of Workfront you access your task or issue from, the Work On&nbsp;It or Done button can change names, as described in the following scenarios:&nbsp;

* When the task or issue is first assigned to you and the status is New, the button displays as Work on it.

  ![](assets/nwe-work-on-it-button.png)

  >[!TIP]
  >
  >You can replace the Work On It button with a Start button. For information about replacing the Work On It button with a Start button, see  [Replace the Work On It button with a Start button](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md) .

* After you have clicked Work On It accept, the button changes to Mark as done or Done , depending on where in&nbsp;Workfront you access the task or the issue from. For information about where you can access the Work On It button, see the section [Locate the Work On It and Done button](#locate-the-work-on-it-and-done-button) in this article.

  ![](assets/nwe-mark-as-done-button-350x122.png)

* If you are not the only one assigned to the task or issue and you are accessing your work item from the Work List in the Home area, the button changes to Done with my part.

  ![](assets/home-left-done-with-my-part-button-350x184.png)

## Locate the Work On&nbsp;It and&nbsp;Done button {#locate-the-work-on-it-and-done-button}

You can locate the Work On&nbsp;it and Done button in the following areas of Workfront:

* The Home area, both in the Work List or the details panel

  For information about marking an item as Done in the Home area, see [Mark an item as Done in the Home area](../../workfront-basics/using-home/using-the-home-area/mark-item-done-in-home.md). 

* In the header of the task or issue

  For information about the object headers, see [New object headers](../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

* In the task or issue Summary panel in a list or in the Workload Balancer

  For information about using the Summary panel, see [Summary overview](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

## Overview of fields that automatically update when you click the Work On It and Done button

The benefit of using the Work On It and Done buttons is that you can allow Workfront to automatically update information on the work item assigned to you.

* [Work On It button](#work-on-it-button) 
* [Start button](#start-button) 
* [The Done button](#the-done-button)

### Work On It button {#work-on-it-button}

When you click Work On It, the following items also update:

* Assignment Status updates from Requested to Working

  >[!TIP]
  >
  >The Assignment Status field is visible only in reports and lists. For information about the Assignment Status field, see the [Glossary of Adobe Workfront terminology](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Commit date

  For information about the commit date, see [Commit Date overview](../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

### Start button {#start-button}

If you have access to edit teams, you can replace the Work On&nbsp;It button with a Start button for a team. When users with that team as their Home Team click the Start button on items they are assigned to, additional fields on their work items update automatically. For information about replacing the Work On It button with a Start button, see [Replace the Work On It button with a Start button](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

In addition to the fields that update when you click the Work On&nbsp;It button, the following fields automatically update on a task or issue when you click the Start button:

* Status
* Actual&nbsp;Start Date

  For information about the Actual Start Date, see [Overview of the project Actual Start Date](../../manage-work/projects/planning-a-project/project-actual-start-date.md).

* Actual Completion Date if the Start button is associated with a status that equates with Complete or Closed.

  For information about the Actual Completion Date, see [Overview of the project Actual Completion Date](../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

>[!NOTE]
>
>Clicking the Undo button returns the work item to the original status and deletes the Actual Start Date. 
>
>The Undo  button is not available in the following areas:
>
>* Team requests
>* Task header
>

### The Done button {#the-done-button}

If you have access to edit teams, you can configure the&nbsp;Done button for a team to update the task or issue statuses when you mark an item as completed. When users with that team as their Home Team click the Done button on their items the following fields automatically update on a task or issue:

* Status
* Assignment Status updates from&nbsp;Working to&nbsp;Done
* Actual&nbsp;Completion&nbsp;Date

For information about configuring the Done button for a team, see the following articles:

* [Configure the Done button for tasks](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) 
* [Configure the Done button for issues](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)
