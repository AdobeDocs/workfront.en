---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configure timeline recalculations for projects
description: Recalculating timelines allows managers to see how forces outside of the project are impacting the project's timeline. A project's timeline refers to the planned and projected dates for the project.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
---
# Configure timeline recalculations for projects

Recalculating timelines allows managers to see how forces outside of the project are impacting the project's timeline. A project's timeline refers to the planned and projected dates for the project.

As an Adobe Workfront administrator, you can manually recalculate timelines for all projects in the system. Project owners can also manually recalculate timelines for individual projects. For more information, see [Recalculate project timelines](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

This article describes how you, as a Workfront administrator, can determine how and when Workfront automatically calculates project timelines by configuring project preferences in the Setup area.

## Access requirements

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator access level</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure automatic recalculations

As an Adobe Workfront administrator, you can configure when Workfront automatically recalculates project timelines. Workfront can recalculate project timelines either every night or when the project scope changes, or both.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Setup** ![](assets/gear-icon-settings.png). 

1. Click **Project Preferences** > **Projects.**

1. In the **Timelines** section, enable or disable one or both of the settings below. By default, both settings are enabled.

   * **Every night:** Workfront​​​ recalculates timelines at night only for projects that have a status of Current and were updated in the past three months.

     In this case, Workfront recalculates the timeline for all projects that have an Update Type of Automatic or Automatic and On Change. 
   
   * **When a project's scope changes**: For information about what constitutes a project scope change, see [Recalculate project timelines](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     In this case, Workfront recalculates the timeline for all projects that have an Update Type of Automatic and On Change or On Change Only.

   For information about project Update Types, see [Project Update Type overview](../../../manage-work/projects/planning-a-project/project-update-type-overview.md). 

1. Click **Save**.

   The timeline of all projects in the system recalculates automatically based on the Update Type of each project.

## Recalculate timelines for the entire Workfront instance

You can run the Recalculate Timeline diagnostic to manually recalculate all timelines in the Workfront system. This allows all Project Managers to see the influence of external changes immediately on both planned and projected dates. For more information, see [Use Diagnostics to trigger automated processes](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
