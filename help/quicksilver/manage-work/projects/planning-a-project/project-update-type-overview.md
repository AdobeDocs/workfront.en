---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Project Update Type Overview
description: The Update Type of a project indicates how Adobe Workfront calculates the timeline of a project. Changes in the project plan might trigger changes in the timeline of the project. The timeline of the project must be automatically or manually recalculated to ensure it is up to date with these changes.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
---
# Project Update Type overview

The Update Type of a project indicates how Adobe Workfront calculates the timeline of a project. Changes in the project plan might trigger changes in the timeline of the project. The timeline of the project must be automatically or manually recalculated to ensure it is up to date with these changes.

For information about recalculating the project timeline, see [Recalculate project timelines](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Project Update Types

There are four Update Types for a project, depending on when you want Workfront to recalculate the project timeline. Choose an Update Type from the list below.

For information about how to update the project's Update Type, see [Select the project Update Type](../../../manage-work/projects/manage-projects/select-project-update-type.md).

>[!IMPORTANT]
>
>If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.

* **Automatic and On Change:**&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp;   
  This is the recommended setting as it ensures that the project timeline is always up to date.

  When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.

  ![](assets/dates-dimmed-when-insline-editing-350x146.png)

  This indicates that the recalculation is not yet finished, and the dates are subject to change. 

* **Change Only:**&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.   
  You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.

* **Automatic Only:**&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.  
  You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.

  >[!NOTE]
  >
  >A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.

* **Manual Only:**&nbsp;The project timeline is updated only&nbsp;when you select the option to **Recalculate Timelines**, as described in the section "Manual Recalculation" in&nbsp;the article [Recalculate project timelines](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).  
  You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).
