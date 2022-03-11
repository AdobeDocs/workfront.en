---
filename: project-planned-start-date
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overview of the project Planned Start Date
description: The Planned Start and the Planned Completion Dates of a project rely on the dates of the tasks on the project. This article describes the Planned Start Date of a project. For information about the task Planned Start Date, see Overview of the task Planned Start Date.
---

# Overview of the project Planned Start Date

The Planned Start and the Planned Completion Dates of a project rely on the dates of the tasks on the project.&nbsp;This article describes the Planned Start Date of a project. For information about the task Planned Start Date, see [Overview of the task Planned Start Date](../../../manage-work/tasks/task-information/task-planned-start-date.md).

The Planned Start Date of a project can be set manually or automatically, depending on whether you schedule the project from the Start or from the Completion Date.&nbsp;

## Manually set the Planned Start Date of a project

You must manually set the Planned Start Date of a project when you schedule the project from Start Date.&nbsp;

For information about setting the project's Planned Start Date, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

<!--
Click the Main Menu icon in the upper-right corner, then click Projects. Click New Project then New Project. For more information about creating projects, see Create a project. Click the Edit Project icon in the upper-right corner. In the Schedule From field, select Start Date. Specify the Planned Start Date of the project. Click Save Changes. As you start adding tasks to your project, the Planned Completion Date of the project calculates based on the total Duration of all of the tasks.
-->

## Automatically set the Planned Start Date of a project

The Planned Start Date of a project is automatically set when you create the project in the following ways:

* from scratch and when you schedule the project from Completion Date.&nbsp;

  The Planned Start Date is automatically calculated by Adobe Workfront, based on the date you select for the Completion Date and the durations of all the tasks on the project.

  For information about creating a project from scratch, see [Create a project](../../../manage-work/projects/create-projects/create-project.md). 

* import it from&nbsp;Microsoft Project.

  The Planned Start&nbsp;Date is the Start&nbsp;Date of the project in Microsoft Project.

  For information about importing a project from&nbsp;Microsoft Project, see [Import a project from Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* import it using Workfront Kick-Starts, when you are a Workfront administrator.

  The Planned Start&nbsp;Date always matches your computer's time and date, unless you specify otherwise in the setPlannedStartDate field on the Project sheet of the kick-start file.

  For information about importing data using kick-starts, see [Import data into Adobe Workfront via a Kick-Start template](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  For information about importing projects using kick-starts, see [Kick-Starts scenario: simple project and task import preparation](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

<!--
To schedule a project from Completion Date: Click the Main Menu icon in the upper-right corner, then click Projects. Click New Project then New Project. For more information about creating projects, see Create a project. Click the Edit Project icon in the upper-right corner. In the Schedule From field, select Completion Date. Specify the Planned Completion Date of the project. Click Save Changes. As you start adding tasks to your project, the Planned Start Date of the project calculates based on the total Duration of all of the tasks, counting backwards from the Planned Completion Date. For more information about Task Duration, see the article Overview of Task Duration and Duration Type. The Planned Start Date of the project coincides, in this case, with the Planned Start Date of the first task on the project.
-->

## The Planned Start Date of a task

You can either specify the Planned Start Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria.&nbsp;

For information about the Planned Start&nbsp;Date of a task, see [Overview of the task Planned Start Date](../../../manage-work/tasks/task-information/task-planned-start-date.md).

<!--
The Planned Start Date of a task You can either specify the Planned Start Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria. Manually set the Planned Start Date of a task How the Planned Start Date is calculated for a task Manually set the Planned Start Date of a task Setting the Planned Start Date of a task depends on the type of Task Constraint you assign to the task. You can manually set the Planned Start Date when creating a task, as described in the article Create tasks in a project. You can manually specify the Planned Start Date when you select any of the following Task Constraints: Task Constraint Type Effect of Manually Changing the Planned Completion Date Must Start On Start No Earlier Than Start No Later Than The Planned Completion Date is adjusted in order to keep the Duration the same. Fixed Dates The Duration is adjusted in order to keep the Planned Completion Date the same. How the Planned Start Date is calculated for a task When it is calculated automatically by the system, the following can influence the Planned Start Date of a task: The Start Date preference setting in the Tasks & Issues area in Setup Your Workfront or group administrator can determine whether a new task starts on the same date as the project's Planned Start Date or on the day you create the task. For information about Tasks & Issues preferences, see Configure system-wide task and issue preferences. Task Constraint For more information about Task Constraints, see the article Task Constraint overview Task predecessor relationship For more information about task predecessors, see the article Overview of task predecessors. Project Start Date, when the project is scheduled from Start Date. The time off schedule of the Primary Assignee of the task. When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the Consider user time off in task durations setting is selected for the User Time Off field. New projects inherit this setting from the Project Preferences area, but you can edit the setting at the project level. For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 1 marked for Time-off, the task Planned Start Date becomes June 2. For information about the User Time Off preference, see the articles Configure system-wide project preferences and Edit projects. When set automatically, the Planned Start Date is determined based on the following calculation: Planned Start Date = Planned Completion Date - Task Duration For example, if your task has a Completion Date of September 16 and a duration of 10 days, the Planned Start Date is September 6. Note: The Update Type for the project must also be set to 'Automatic and On Change' or 'Automatically' in order for the Planned Hours and Duration to be automatically adjusted. For more information about the Update Type, see the article Select the project Update Type .
-->

