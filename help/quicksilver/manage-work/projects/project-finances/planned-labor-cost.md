---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculate Planned Labor Cost
description: As you plan the work on your projects, Adobe Workfront calculates the Planned Labor Cost for the roles and users assigned to this work based on their Cost Per Hour values.
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
---
# Calculate Planned Labor Cost

As you plan the work on your projects, Adobe Workfront calculates the Planned Labor Cost for the roles and users assigned to this work based on their Cost Per Hour values.

The Planned Labor Cost of a project is a calculation between the cost associated with the job roles or the users assigned to complete the work on the project and the amount of hours planned (Planned Hours) that might take each role or user to complete that work.

## Overview of the Planned Labor Cost

The **Planned Labor Cost** of a project is calculated by adding all the Planned Labor Costs of all the tasks on the project.

>[!TIP]
>
>There is no Planned Labor Cost associated with issues or with the project itself.

Workfront calculates the Planned Labor Cost of a project using the following formula:

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

The Task Planned Labor Cost is calculated based on the following:

* The number of resources on the task and their individual allocation to the task
* The Cost Type of task.

The Task Planned Labor Cost is calculated using the following formula:

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

For more information about how Workfront calculates Planned Labor Cost for tasks, depending on task assignments and Cost Type, see the "Modify Cost Types for individual tasks" section in the article [Track costs](../../../manage-work/projects/project-finances/track-costs.md).

## Locate the Planned Labor Cost

You can locate the Planned Labor Cost of a project in the following areas of Workfront:

* A Project report
* A list of projects
* A Baseline report where you can track it over time
* Through the API

For information about creating reports and using the Workfront API, see the following articles:

* [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) 
* [API basics](../../../wf-api/general/api-basics.md)
