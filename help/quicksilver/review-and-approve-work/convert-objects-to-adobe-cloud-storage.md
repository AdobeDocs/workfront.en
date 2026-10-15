---
product-area: documents
navigation-topic: approvals
title: Convert legacy objects to Adobe cloud storage
description: Learn the three cases where you can convert a legacy Workfront storage object to Adobe cloud storage, and understand what moves and what stays during each conversion.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
---
# Convert legacy objects to Adobe cloud storage

In most scenarios, you can move, copy, and convert Workfront objects only between like storage models. For example, you can move a task from one Adobe cloud storage project to another Adobe cloud storage project. In three specific cases, you can convert a legacy Workfront storage object to Adobe cloud storage:

* Convert a legacy Workfront storage task to an Adobe cloud storage project
* Convert a legacy Workfront storage portfolio to an Adobe cloud storage portfolio
* Create an Adobe cloud storage project from a legacy Workfront storage template

For an orientation to the move and what's different on Adobe cloud storage, see [Move to Workfront on Adobe cloud storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).

>[!NOTE]
>
>In all three conversion scenarios, documents and document folders don't move from legacy Workfront storage to Adobe cloud storage. Documents that exist on the legacy object before the conversion remain on legacy storage.

## Convert a legacy task to an Adobe cloud storage project

To convert a legacy Workfront storage task to an Adobe cloud storage project, use the existing convert-to-project flow on the task. During the conversion:

* Subtasks and issues move to the new project.
* Documents attached to the task and their approval workflows remain on the original project.
* Work approvals and resolving object links are removed.
* The original task is deleted.

## Convert a legacy portfolio to an Adobe cloud storage portfolio

A Workfront administrator can convert a legacy Workfront storage portfolio to an Adobe cloud storage portfolio from the Setup area. After the conversion:

* You can no longer move legacy Workfront storage projects into the portfolio.
* All new projects created in the portfolio use Adobe cloud storage.
* Frame.io is the viewer for documents in the portfolio's Adobe cloud storage projects.
* Child projects that use legacy Workfront storage stay on legacy storage.
* Child programs stay on legacy storage.

>[!NOTE]
>
>A child legacy program converts to Adobe cloud storage automatically only when someone manually adds an Adobe cloud storage project to it.

For more information, see [Convert legacy portfolios to Adobe cloud storage](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md).

## Create an Adobe cloud storage project from a legacy template

When you create a project from a legacy Workfront storage template, the **Create this project on Adobe cloud storage** checkbox in the project creation dialog box determines the storage type of the new project. The checkbox behavior depends on where you create the project:

* **Outside a portfolio**: The checkbox is available and cleared by default. Select it to create the new project on Adobe cloud storage.
* **Inside an Adobe cloud storage portfolio**: The checkbox is selected and locked. The new project must match the portfolio's storage type.
* **Inside a legacy Workfront storage portfolio**: The checkbox isn't available. The new project uses legacy Workfront storage.

For more information, see [Create projects](/help/quicksilver/manage-work/projects/create-projects/create-project.md).
