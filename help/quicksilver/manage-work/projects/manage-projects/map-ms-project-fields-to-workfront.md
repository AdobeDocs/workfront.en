---
product-area: projects
navigation-topic: manage-projects
title: Map Microsoft Project Fields to Adobe Workfront Projects
description: Projects in Adobe Workfront and Microsoft Project are mostly compatible. This article describes how the most common project fields from the two applications map to one another.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
---
# Map Microsoft Project fields to Adobe Workfront projects

Projects in Adobe Workfront and Microsoft Project are mostly compatible. Using the two applications, you can do the following:

* Export projects from Microsoft Project and import them into Workfront
* Export projects from Workfront and import them to Microsoft Project.&nbsp;

For more information about importing projects from Microsoft Project in to Workfront, see [Import a project from Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

For more information about exporting a project from Workfront to import it into Microsoft Project, see [Export a project to Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

When performing such imports of data, it is important to understand how information translates from one application to the other. Most times, you will have to make some manual modifications to the project, after you complete the import.&nbsp;

## Overview of field mapping

>[!NOTE]
>
>Planned dates do not always correspond&nbsp;between both systems. Discrepancies can be accounted for through schedule and differences in system preferences between Workfront and Microsoft Project. These date discrepancies can&nbsp;also result in differences in effort, duration, and percent complete.

| **Microsoft Project Field** |**Workfront Field** |
|---|---|
| Project Title |Project Name |
| Start and Finish Dates |Planned Start and Completion Dates |
| Task Name |Task Name |
| Task Duration |Task Planned Duration |
| Task Work | Task Planned Hours  |
| Task %&nbsp;Complete |Task % Complete (based on the Duration of the task) |
| Task&nbsp;Work %&nbsp;Complete |Task % Complete (based on the Planned Hours of the task) |
| Scheduled Start and Finish  |Planned Start and Completion Dates |
| Actual&nbsp;Start and Finish |Actual&nbsp;Start&nbsp;and Completion Dates |
| Resource Name |Task Assignment |
| Assignment Units |Assignment Allocation Percentage |
| Task Note |Task Description |
| Predecessor |Predecessor |

## Overview of data that is not included

There are a number of project fields that are&nbsp;not imported to or exported from Workfront.

These fields include but are not limited to the following:

* Document attachments
* Custom fields (at the project or task levels)
* Workfront notes
* Issues
* Negative lag in tasks with a Start/ Finish predecessor relationship (tasks are imported without the lag)
* Assignments
* Task Constraints

  >[!NOTE]
  >
  >Because Constraints do not map between Microsoft Project and Workfront, ensure that there are predecessor relationships between the tasks. Otherwise, the Planned Start and Planned Completion Dates of the tasks might not accurate in the imported project.&nbsp;
