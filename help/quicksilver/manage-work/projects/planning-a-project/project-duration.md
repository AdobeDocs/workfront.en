---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overview of Project Duration
description: Adobe Workfront calculates the Duration of a project by taking into account the Start Date of the earliest task and the Completion Date of the latest task and counts the number of days between the two dates.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
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

* **Planned Duration**:&nbsp;

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```

* **Actual Duration**:&nbsp;

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```

## Locate the project Duration

You can locate the Project Planned and Actual Durations in the following areas of Workfront:

* . In the Project Details area, in the Overview section.

  For more information about the Overview sub-tab of a project, see the article [Manage information in the project Overview area](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* In a Project report, by including the Duration or the Actual Duration fields in the report.

  For more information about creating reports, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
