---
product-area: templates
navigation-topic: templates-navigation-topic
title: Overview of Start and Completion Days in a template
description: You can use project templates to capture most of the repeatable processes, information, and settings associated with the projects in your organization. While projects have specific start and completion dates, templates have generic start and completion days as an indication for where these dates will fall on the project, based on the overall timeline of the project.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
---
# Overview of Start and Completion Days in a template

You can use project templates to capture most of the repeatable processes, information, and settings associated with the projects in your organization. While projects have specific start and completion dates, templates have generic start and completion days as an indication for where these dates will fall on the project, based on the overall timeline of the project.

**Example:** If a project's Start Date is April 1 and you want a task to start on April 3rd (two days after the start of the project), the corresponding task on the template that creates the project should start on Day 2 of the template, where the first day of the template is considered Day 0.

## Start Day

Consider the following when working with templates and template tasks:

* By default, templates have a Start Day of 0 and the template tasks and the template show a Start Day of 0. The Start Day of the template tasks can change but this does not change the Start Day of the template.
* The start day of a template task represents the number of business days that Workfront adds to the task's Planned Start Date when a project is created from the template. For example, you can have a template with only one task and the Start Day of the template task is 4. The Start Day of the template is still 0. When you create a project from this template where the project's Schedule Mode is Start Date, and the Planned Start Date of the project is November 1, 2019, the newly-created task adds 4 days to this date and sets its Planned Start Date value to November 5, 2019.

The following are some actions that might change the Start Day of the template tasks:

* Update the Duration of predecessor template tasks
* Update the Task Constraints

  When using date-based Task Constraints, you can manually update the Start Day of the template tasks. Some examples of date-based Task Constraints are Fixed Dates, Start No Earlier Than, Start No Later Than, Must Start On. 

* Update the template task predecessors

## Completion Day

The Completion Day of the template is the day when the last template task completes. By default, all template tasks and the template show a Completion Day of 1, because Workfront assumes that any template task has a Duration of 1 Day. The Completion Day of the template tasks can change and this also changes the Completion Day of the template. The Completion Day of the template becomes the Planned Completion Date of the future project and the Completion Days of the template tasks become the Planned Completion Dates of the future project tasks.

The following are some actions that might change the Completion Day of the template tasks:

* Update the Duration of the template tasks
* Update the Task Constraints

  When using date-based Task Constraints, you can manually update the Completion Day of the template tasks. Some examples of date-based Task Constraints are Fixed Dates, Finish No Earlier Than, Finish No Later Than, Must Finish On. 

* Update the template task predecessors

## Work with templates scheduled from Completion

You can schedule a template from Completion Day. For more information, see [Edit project templates](../../../manage-work/projects/create-and-manage-templates/edit-templates.md). 

Consider the following when working with templates scheduled from Completion Date:

* Changing the Start Day sets the Task Constraint to Must Start On.
* Changing the Completion Day sets the Task Constraint to Must Finish On.
* When the template is scheduled from Completion Day, the Task Constraint Day is calculated from the Completion Day.

  **Example:** Your template's duration is 285 days, and you have a template task with duration 60 days. If you set the Task Constraint to Must Start On and Constraint Day to 120, you will have a Start Day of 165 (285 - 120) and Completion Day of 225 (165 + 60). So when you edit the Start Day, it is actually being interpreted as Constraint Day.
