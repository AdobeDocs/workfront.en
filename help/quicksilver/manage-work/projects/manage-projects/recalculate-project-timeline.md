---
filename: recalculate-project-timeline
product-area: projects
navigation-topic: manage-projects
title: Recalculate project timelines
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Recalculate project timelines

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

Recalculating Timelines allows managers to see how different factors related to the project are impacting the project's timeline. A project's timeline refers to planned and projected dates.

Making changes to schedules, personnel time off, and other items outside the scope of a project do not impact the project timeline immediately. The project timeline is impacted when the timeline is recalculated. External influences do not take effect on your project until the recalculation occurs.

This article describes the ways in which timeline recalculation happens.

## Access requirements

Automatic timeline recalculation happens without special access for any of the users involved in working on the project.

However, you must have the following access to manually recalculate the timeline of a project: 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Automatic recalculation

By default, project timelines are automatically recalculated daily when the project scope changes or every night. The Workfront administrator determines whether to automatically calculate timelines every night or with every scope change by managing the Timelines settings in the Project&nbsp;Preferences area of Setup. For more information, see [Configure timeline recalculations for projects](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!NOTE]
>
>If the timeline of a project is longer than 15 years, the automatic recalculation is disabled for that project. You can only select an Update Type of Manual for a project longer than 15 years. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically.

* [Automatic recalculation of project timelines](#understanding-automatic-recalculation) 
* [Actions that trigger an automatic recalculation of project timelines](#actions-that-trigger-automatic-timeline-recalculation)

### Automatic recalculation of project timelines

Adobe Workfront recalculates timelines daily only for projects where all of the following conditions are met:

* Have a status of Current
* Update Type of the project is set to Automatic or Automatic and On&nbsp;Change

  For information about the type of project Update Type, see [Project Update Type overview](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* Have a Last&nbsp;Update Date within the past three months  
  Workfront administrator can change this default functionality, as described in [Configure timeline recalculations for projects](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* Last calculation date of the project timeline is not within the current calendar day. This means that the last calculation date of the project timeline is before 00:00 of the current day.

You can configure how frequently the timeline for your project is updated. When the project timeline is updated, it is recalculated based on changes made to the project 

<!--
or changes made to another project that the timeline is dependent on
-->

.

For information, see [Select the project Update Type](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
You can configure how the timeline for your project is updated: Go to the project for which you want to configure how the timeline is updated. Click the More icon to the right of the project name, then click Edit. The Edit Project dialog box is displayed. Click Settings. In the Update Type drop-down list, select from the following options: - Automatic and On Change: (Default setting) The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. This is the recommended setting for this field because it ensures that the project timeline is always up to date. When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. This indicates that the recalculation is not yet finished, and the dates are subject to change. - Change Only: The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on. - Automatic Only: The project timeline is updated each night; it is not updated immediately after changes are made. You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on. Note: A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change. - Manual Only: The project timeline is updated only when you select the option to Recalculate Timelines, as described in Manual recalculation. You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change). For more information about the project Update Type, see Select the project Update Type Note: If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically. Click Save Changes.
-->

### Actions that trigger an automatic recalculation of project timelines

Various scope changes in the life of a project automatically recalculate the project timeline, including the following actions:

* Updating task status.
* Moving a task to a different project.
* Updating the Planned Date or Planned Completion Dates of the tasks. 
* Updating the Duration Type, Task Constraint, or the number of assignees on the tasks. 
* Updating task predecessor relationships. 
* Adding an approval to a task that also adds time to the Planned Completion Date of the task.   
  For more information about approval settings, see [Configure global approval settings](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## Manual recalculation

As a project owner, you can manually recalculate the timelines for individual projects. The Workfront administrator can manually recalculate all timelines in Workfront.

* [Recalculate timelines for individual projects](#recalculating-timelines-for-individual-projects) 
* [Manually recalculate timelines in bulk in the Edit Projects box](#recalculate-finances-in-bulk) 
* [Recalculate timelines for all projects in the system (Workfront administrators only)](#recalculating-timelines-for-the-entire-workfront-site)

### Recalculate timelines for individual projects

You can recalculate the timeline of a project in Workfront from the project page or from a project list or report.

1. Go to the project for which you want to recalculate the timeline.
   Or Go to a project list or report and select one or several projects. 
1. Click the More icon , then click Recalculate Timeline.

   After the timeline is recalculated, you see a message indicating that the recalculation was successful.  
   Before the timeline recalculation is finished, some planned or projected dates might display as dimmed. This means that the recalculation is not yet finished, and the dates are subject to change.

### Manually recalculate timelines in bulk in the Edit Projects box

You can manually recalculate the timelines of several projects by editing them in bulk.

1. Go to a list of projects.
1. Select several projects in the list, then click `Edit`.
1. Click `Settings`, then select `Recalculate Timelines`.

1. Click `Save Changes`.

### Recalculate timelines for all projects in the system (Workfront administrators only)

Workfront administrators can run the Recalculate Timeline diagnostic to immediately recalculate all timelines in the Workfront system. This allows all Project Managers to see the influence of external changes immediately on both planned and projected dates.

For more information about recalculating timelines for the entire Workfront site, see the section "Recalculate timelines for the entire Workfront instance" in [Configure timeline recalculations for projects](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

<!--
Project Update Types For information about how to update the project's Update Type, see Select the project Update Type . Important: If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual. You can select how each project calculates its timeline by choosing between the following Update Types: Important: If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual. Automatic and On Change: This is the default setting. The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. This is the recommended setting as it ensures that the project timeline is always up to date. When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. This indicates that the recalculation is not yet finished, and the dates are subject to change. Change Only: The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. You might want to select this option if you are concerned about system performance and if changes rarely occur in the project or in other projects that the timeline is dependent on. Automatic Only: The project timeline is updated each night; it is not updated immediately after changes are made. You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on. Note: A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change. Manual Only: The project timeline is updated only when you select the option to Recalculate Timelines, as described in the section "Manual Recalculation" in the article Recalculate project timelines. You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).
-->

