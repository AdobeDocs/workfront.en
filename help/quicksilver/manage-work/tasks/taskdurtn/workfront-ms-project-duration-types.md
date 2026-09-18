---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Duration Types in Adobe Workfront and Microsoft Project
description: The Duration Types available in Adobe Workfront are different than their counterparts in Microsoft Project which are called Task Types. This can be sometimes confusing when exporting or importing projects between Workfront and Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
TQID: https://experienceleague.adobe.com/avh0ZuYJpsf7Ed5HiWuLkxEA-0PD-1iFvzHmWvpDZiI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
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
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
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
 
(drafting this because it is misleading)
 
</note>
-->
