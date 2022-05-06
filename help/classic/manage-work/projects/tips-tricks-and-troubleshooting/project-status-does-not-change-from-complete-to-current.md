---
filename: project-status-does-not-change-from-complete-to-current
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Project status will not change from Complete to Current
description: (Although this can be added as an FAQ, I have left this as its own article for search-ability reasons)
---

# Project status will not change from Complete to Current

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Although this can be added as an FAQ, I have left this as its own article for search-ability reasons)</p>
-->

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

## Problem

The project Status does not change from Complete back to Current.

The cause of this problem is the Completion Mode setting on your project. If a project's Completion Mode is set to Automatic, then the project will automatically change the status from Current to Complete after all tasks and issues are completed and the project's percent complete bar is 100%. In this case, manually changing the status of the project from Complete back to Current is not possible.

## Solution

If a project's Completion Mode is set to Manual, then the project status can be changed from Complete back to Current anytime.

To update a project's completion mode to Manual:

1. Go to the project you want to update.
1. Click **Edit Project** on the upper-right side of the screen.
1. Click **Settings**.
1. Locate the **Completion Mode** drop-down menu, and select **Manual**.

1. Click **Save** **Changes**.

