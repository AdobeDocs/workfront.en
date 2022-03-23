---
filename: autocompleted-task-still-shows-up-on-my-work-list
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Autocomplete tasks still show up on My Work screen
description: I have a task set to autocomplete, but when the due date arrives and the task autocompletes, the task is not removed from the Working On list in My Work.
---

# Autocomplete tasks still show up on My Work screen

## Problem

I have a task set to autocomplete, but when the due date arrives and the task autocompletes, the task is not removed from the Working On list in My Work.

## Solution

You still have to mark the task as **Done** in the Working On list.

The My Work "Done" and the Task Status "Complete" are two separate code paths in Adobe Workfront. When an item is marked Done, it can also automatically be set to complete the task.

However, when a task status is set to Complete, it will not automatically mark the task as Done for the assigned user, leaving it in My Work. The task must be marked as Done to be removed from the work queue.

This is useful when follow-up items like hours and billing are needed after tasks are complete, and is how the product is designed. Setting a task Status to Complete will not automatically mark the task as Done.
