---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overview of the project Projected Start Date
description: The Projected Start Date is a real-time date of when the project is going to start based on the Projected Start Date of the first task on the project.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
TQID: https://experienceleague.adobe.com/2rcx201EGt4cqRpqfXws6P-NbRnXyVlFoTbJrQJBipg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
---
# Overview of the project Projected Start Date

## Overview of the Projected Start Date for projects and tasks

The Projected Start Date is a real-time date of when the project is going to start based on the Projected Start Date of the first task on the project.  

When you first plan a project, the Planned Start Date and the Projected Start Date of the tasks and of the project are identical. As delays may happen or tasks might be completed earlier, the Projected Start Date can become different than the Planned Start Date.  

Changes in the Projected Start Date of the first task on the project trigger changes in the Projected Start Date of the project.  

## Modify the Projected Start Date of a task

The Projected Start Date for a project or a task is a calculation done by Adobe Workfront, and it cannot be manually modified.  

The following events can trigger a modification in the Projected Start Date of a task:

* When you start working on a task, the Actual Start Date of the task becomes its Projected Start Date.
* If the Planned Start Date of a task passes, the Projected Start Date moves into the future, indicating the soonest date available for the task to start.  
  Workfront takes into account the amount of Planned Hours on the task, as well as the schedule of the project or of the user assigned to the task when calculating the earliest available date for the task to start.  
* Predecessor tasks that are running behind have an impact on the Projected Start Date of their dependent tasks. The Projected Start Date of the dependent tasks moves according to the Dependency Type of the predecessor relationship and according to the Projected Dates of the predecessors.  

If any of these tasks is the first task on a project, the Projected Start Date of the project changes to match the Projected Start Date of this task.  

## Locate the Projected Start Date of a project or task

You can locate the Projected Start Date of a project or a task in the following areas of Workfront:

* You can add it to a project or a task report or view.

  For more information about creating a report, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* In the Project  Details section of a project or the Task  Details section of a task.
