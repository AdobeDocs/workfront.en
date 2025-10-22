---
product-area: projects
navigation-topic: create-tasks
title: Create Tasks Overview
description: You can create tasks in a project only after you created the project.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
---
# Create tasks overview

You can create tasks in a project only after you created the project.

For example, after creating a project, you might want to add tasks and modify them to organize the project plan. For more information about creating a project, see [Create a project](../../../manage-work/projects/create-projects/create-project.md). For information about creating tasks, see [Create tasks in a project](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

This article describes considerations, limitations, as well as defaults that apply when creating tasks.

## Ways to create tasks on a project

You can create tasks on a project in the following ways:

* From scratch, as described in [Create tasks in a project](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* Copy tasks to the same project or to a new project or duplicate tasks on the same project, as described in [Copy and duplicate tasks](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Move tasks from a project to another, as described in [Move tasks](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Limitations in creating tasks

When you have the correct access and permissions you can create tasks on a project. However, the following are cases when you might not be able to create tasks:

* Your Adobe Workfront administrator or a group administrator must enable adding tasks to a project that is in a Complete or Dead status in your Project Preferences area. For information about setting project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* You cannot add tasks to a project that is in Pending Approval.

## The maximum number of tasks allowed on a project

A project can contain up to 5,000 tasks. A warning message displays on the project when you are approaching the limit, when you have met the limit, and if you attempt to exceed the limit.

Depending on the number of tasks in your projects when this limitation was imposed, your Workfront instance might allow for more than 5,000 tasks in a single project.

If you are able to include more than 5,000 tasks in a single project, be aware of the following:

* The task limit for your Workfront environment is set to the current number of tasks in your largest project, plus an additional 10%.

  For example, if a project in your Workfront instance contains 10,000 tasks, your limit for each project throughout your Workfront instance is 11,000 tasks.

* Smaller projects improve performance and minimize management challenges that accompany large projects.

## Task defaults when adding tasks to a project

There are two types of default information that Workfront automatically updates for tasks when you create them:

* System-level default information

  Your Workfront administrator or a group administrator establishes the system-level defaults for tasks in the Tasks &&nbsp;Issues area of Project Preferences. For information about task and issue preferences, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) or [Configure task and issue preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* Project-level default information

  The rest of this section describes the project-level defaults you, as the project manager, can define for all new tasks that are added to a project

When you add a task to a project, depending on how the project is set up, Workfront might automatically attach an approval process or custom forms to the task.

For information about configuring a project to add these by default, see the "Tasks" section in the [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md) article.

When defining default information to be associated with tasks added to a project at the project level, consider the following:

* You must have Manage permissions on the project to define the default settings for the task approval process and custom forms.
* All new tasks are created with the approval process and the custom forms defined when editing the project.
* You can modify these default settings when you add tasks using the Edit Task box, but not when you add tasks in inline edit.
* You can define the approval process and the custom forms for tasks in a template.

   * When a project is created from this template, the approval process and custom forms are automatically applied to the project.
   * When a template is attached to an existing project, the project preserves the original task approval process and custom forms settings if they are defined. If they are not defined, the settings from the template become the settings for the project.
   * When a template is attached to an existing project, the tasks added to the project from the template preserve the approval process and custom forms settings they had on the template, regardless of the task settings on the project.

  For information about attaching a template to a project, see [Attach a template to a project](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* When you copy the project, the task default settings transfer to the new project.

  For information about copying a project, see [Copy a project](../../../manage-work/projects/manage-projects/copy-project.md).

* When you copy tasks from one project to another and the destination project has different default settings for tasks, the copied tasks preserve the default settings from the original project, unless they are cleared in the copying process.
* When you duplicate a task on the same project, the custom forms and approval process are transferred to the duplicate task.

  For information about copying and duplicating tasks, see [Copy and duplicate tasks](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* When you move the task to another project, the default task settings are saved on the tasks from the original project, regardless of the task default settings on the new project.

  For information about moving tasks, see [Move tasks](../../../manage-work/tasks/manage-tasks/move-tasks.md).
