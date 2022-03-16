---
filename: tasks-on-my-work-list-when-project-on-hold
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Tasks still display in My Work list when project in On Hold
description: Tasks still show in My Work, after a project has been placed On Hold.
---

# Tasks still display in My Work list when project in On Hold

## Problem

Tasks still show in My Work, after a project has been placed On Hold.&nbsp;

## Cause

The default On Hold status serves as a visual communication of where the project is, but it does not inhibit or prevent items from being associated with or worked on the project.&nbsp;

## Solution

Creating a custom status is a simple work around that will allow users to&nbsp;remove tasks associated with a project that is On Hold from their My Work lists. The custom status will have a status &nbsp;"Equates With" Planning, but will show a status&nbsp;that the project is On Hold.

Steps to Create a Custom On Hold Status:

1. Click `Setup`.
1. From the Setup screen, open `Project Preferences` from the left-side menu, then click `Statuses`.

1. At the bottom of the list of Statuses, select  `Add a New Status`. A new row appears for your new custom status.
1. Give you new status a descriptive name. For example, "On Hold - Update My Work."
1. Set the `Equates With` field on your new status to  `Planning`.

1. Click `Save` to save your new status.
1. Return to the project and click `Edit Project`.
1. Update the project  `Status` to the new custom status.

Steps to Remove Tasks From My Work: Once the custom status is created, go to the user's "My Work" page. The tasks associated with the project you just set to "'On Hold' Update My Work" will display a message: "This project has been set to Planning status, so you don't need to work on this anymore." They will also have a button to "Remove" the task. Click "Remove" to remove the task from the user's My Work page. When the project becomes active again, simply update the project status to "Current". The tasks associated with that project will reappear in the user's My Work > Work Requests page where they can select "Work on It" to pull the tasks back into their Working On list.  