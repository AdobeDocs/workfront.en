---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Duration Types in Adobe Workfront and Microsoft Project
description: The Duration Types available in Adobe Workfront are different than their counterparts in Microsoft Project which are called Task Types. This can be sometimes confusing when exporting or importing projects between Workfront and Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
---
# Duration Types in Adobe Workfront and Microsoft Project

The Duration Types available in Adobe Workfront are different than their counterparts in Microsoft Project which are called Task Types. This can be sometimes confusing when exporting or importing projects between Workfront and Microsoft Project.

For information about importing and exporting projects between Workfront and Microsoft Project, see the following articles:

* [Export a project to Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md) 
* [Import a project from Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Duration Types in Workfront and Microsoft Project

Workfront has four task duration types:

* Simple
* Effort Driven
* Calculated Work
* Calculated Assignment

For information, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

These duration types are not recognized by Microsoft Project. Currently, Microsoft Project has three Task Types similar to Duration Types in Workfront:

* Fixed Units
* Fixed Work
* Fixed Duration

## Duration Type changes when exporting from Workfront to MS Project

When exporting projects from Workfront to Microsoft Project, Effort Driven tasks become Fixed Work. Simple, Calculated Work, and Calculated Assignment become Fixed Units.

## Duration Type changes when importing from MS Project to Workfront

When importing projects from Microsoft Project in to Workfront, Fixed Units become Effort Driven. Fixed Work and Fixed Duration receive the default duration type that your Workfront administrator selected for your system. For information, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
