---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overview of Project Duration
description: Adobe Workfront calculates the Duration of a project by taking into account the Start Date of the earliest task and the Completion Date of the latest task and counts the number of days between the two dates.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
TQID: https://experienceleague.adobe.com/1j0nj2W5f7FtgIk46G3ePFA-zwt7VAyV9fQWKm2kZJ4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Overview of project Duration

Adobe Workfront calculates the Duration of a project by taking into account the Start Date of the earliest task and the Completion Date of the latest task and counts the number of days between the two dates. 

## Project Duration

The Duration of the project is calculated by the following formula:

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>The Duration of issues on the project does not affect the Duration of the Project.

The duration of the project counts the number of days between the two task dates based on the Schedule associated with the project or the users assigned to the tasks. For information about which schedule Workfront uses to calculate duration, see [Schedules overview](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## Types of project Duration

There are two types of Project Duration and the formulas by which Workfront calculates them:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **Planned Duration**: 

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```

* **Actual Duration**: 

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```

## Locate the project Duration

You can locate the Project Planned and Actual Durations in the following areas of Workfront:

* . In the Project Details area, in the Overview section.

  For more information about the Overview sub-tab of a project, see the article [Manage information in the project Overview area](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* In a Project report, by including the Duration or the Actual Duration fields in the report.

  For more information about creating reports, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
