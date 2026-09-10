---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Project Status Will not Change from Complete to Current
description: This article describes a scenario where you cannot update the Project Status from Complete to Current.
author: Alina
feature: Work Management
exl-id: 774c103f-8785-4d8b-83e9-a074e6518293
TQID: https://experienceleague.adobe.com/xyEO0R-Rpodl3YX8QrNk4-xF-i0-s1WRJ-QCy8Cb8kk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
---
# Project status will not change from Complete to Current

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Although this can be added as an FAQ, I have left this as its own article for search-ability reasons)</p>
-->

## Problem

The project Status does not change from Complete back to Current.

The cause of this problem is the Completion Mode setting on your project. If a project's Completion Mode is set to Automatic, then the project will automatically change the status from Current to Complete after all tasks and issues are completed and the project's percent complete bar is 100%. In this case, manually changing the status of the project from Complete back to Current is not possible.

## Solution

If a project's Completion Mode is set to Manual, then the project status can be changed from Complete back to Current anytime.

To update a project's completion mode to Manual:

1. Go to the project you want to update.
1. Click the **More** icon ![More icon](assets/more-icon.png) to the right of the project name, then click **Edit**.
1. Click **Project** **Settings**.

1. Locate the **Completion Mode** drop-down menu, and select **Manual**.

1. Click **Save** .
