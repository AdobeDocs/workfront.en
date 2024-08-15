---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configure Timeline Recalculations for Projects
description: Recalculating timelines allows managers to see how forces outside of the project are impacting the project's timeline. A project's timeline refers to the planned and projected dates for the project.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
---
# Configure timeline recalculations for projects

Recalculating timelines allows managers to see how forces outside of the project are impacting the project's timeline. A project's timeline refers to the planned and projected dates for the project.

As an [!DNL Adobe Workfront] administrator, you can manually recalculate timelines for all projects in the system. Project owners can also manually recalculate timelines for individual projects. For more information, see [Recalculate project timelines](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

This article describes how you, as a [!DNL Workfront] administrator, can determine how and when [!DNL Workfront] automatically calculates project timelines by configuring project preferences in the [!UICONTROL Setup] area.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator access level</p> <p><b>NOTE</b>: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configure automatic recalculations

As an [!DNL Adobe Workfront] administrator, you can configure when [!DNL Workfront] automatically recalculates project timelines. [!DNL Workfront] can recalculate project timelines either every night or when the project scope changes, or both.

{{step-1-to-setup}}

1. Click **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects].**

1. In the **[!UICONTROL Timelines]** section, enable or disable one or both of the settings below. By default, both settings are enabled.

   * **Every night:** [!DNL Workfront​​​] recalculates timelines once every 24 hours, at night, only for projects that have a status of [!UICONTROL Current] and that were updated in the past three months. Depending on the system load and other factors, the recalculation time might be delayed by more than 24 hours.

      In this case, [!DNL Workfront] recalculates the timeline for all projects that have an [!UICONTROL Update Type] of [!UICONTROL Automatic] or [!UICONTROL Automatic and On Change].

   * **When a project's scope changes**: For information about what constitutes a project scope change, see [Recalculate project timelines](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

      In this case, [!DNL Workfront] recalculates the timeline for all projects that have an Update Type of [!UICONTROL Automatic and On Change] or [!UICONTROL On Change Only].
   For information about project Update Types, see [Project Update Type overview](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Click **[!UICONTROL Save]**.

   The timeline of all projects in the system recalculates automatically based on the Update Type of each project.

## Recalculate timelines for the entire [!DNL Workfront] instance

You can run the [!UICONTROL Recalculate Timeline] diagnostic to manually recalculate all timelines in the [!DNL Workfront] system. This allows all Project Managers to see the influence of external changes immediately on both planned and projected dates. For more information, see [Use Diagnostics to trigger automated processes](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
