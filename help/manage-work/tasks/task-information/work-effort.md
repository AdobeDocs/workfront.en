---
filename: work-effort
content-type: overview
product-area: projects
navigation-topic: task-information
title: Work Effort overview
description: As a project manager, you can decide how you want to estimate the amount of work needed for tasks to complete in a project. Estimate the amount of work needed to complete tasks using one of the following indicators:
---

# `Work Effort` overview

As a project manager, you can decide how you want to estimate the amount of work needed for tasks to complete in a project. Estimate the amount of work needed to complete tasks using one of the following indicators: 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Planned Hours</td> 
   <td> <p> A manual numeric entry or a <span>Adobe Workfront</span> calculation that displays the number of hours that it would take for the resources assigned to a task to complete it. </p> <p>Consider the following about Planned Hours: </p> 
    <ul> 
     <li>This is the default method. </li> 
     <li>You can manually update Planned Hours only for tasks with a Duration&nbsp;Type of Calculated Assignment or Simple. </li> 
    </ul> <p>For information about Planned Hours, see <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Planned Hours overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Work Effort</span> </td> 
   <td> <p>A manual label that defines whether it takes a user a small, medium, or large amount of daily effort to complete a task. <!--
      The level of effort is estimated to be a percentage of the daily amount of working time.
     --> </p> <p>Consider the following about <span>Work Effort</span>:</p> 
    <ul> 
     <li>This field is available only for tasks with a Simple Duration Type. </li> 
     <li>You can enable the use of this label and define the percentage of working time associated with it at the project level. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

This article describes what `Work Effort` is and how you should use it when estimating the amount of work for your tasks.

>[!NOTE]
>
>Planned Hours and `Work Effort` influence each other. Updating the Planned Hours can update the `Work Effort` and updating the `Work Effort` can update the Planned Hours of the task.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project and its tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Considerations for using `Work Effort`

* When the project tasks have 0 Planned Hours and you enable the Use `Work Effort` to automatically calculate task Planned Hours setting on the project, the default level of `Work Effort` associated with them will be Medium. The Planned Hours automatically update for Simple Duration&nbsp;Type tasks. For more information, see the section&nbsp; [Levels of Work Effort](#levels) in this article. 

* When the project tasks have Planned Hours that are more than 0 and you enable the Use `Work Effort` to automatically calculate task Planned Hours setting on the project, the level of `Work Effort` updates according to the amount of Planned Hours without changing the amount of the Planned Hours for Simple Duration Type tasks.&nbsp;For more information, see the section [How Workfront calculates Work Effort based on Planned Hours](#how) in this article. 

* When the project tasks have 0 Planned Hours and you enable the Use `Work Effort` to automatically calculate task Planned Hours setting on the project, then update the level of `Work Effort` from Medium to Small or Large, the Planned Hours also update. For more information, see the section [How Workfront calculates Planned Hours based on Work Effort](#how2) in this article.

* When you inline edit tasks and modify both the Planned Hours and `Work Effort` field for task at the same time, the Planned Hours will be updated with the value you specify, whereas the `Work Effort` value is calculated based on your updated Planned Hours.

* When you update the `Work Effort` value of a task, the Duration no longer auto-calculates based on the Planned Hours. For more information about how Duration calculates for Simple Duration tasks, see [Duration Type overview: Simple](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* When you change the Duration Type of a task from Simple to any other type, the `Work Effort` field is hidden on the task. The Planned Hours remain unchanged. 
* You cannot update the `Work Effort` level on a parent task. The `Work Effort` level for a parent task is automatically calculated based on the number of Planned Hours for the tasks which is a rollup of all the children tasks. For information about parent tasks, see [Create subtasks](../../../manage-work/tasks/create-tasks/create-subtasks.md).

## Enable using `Work Effort` instead of Planned Hours

<ol> 
 <li value="1"> <p> Go to a project and click the More menu , then click Edit. </p> </li> 
 <li value="2"> <p>Click Task Settings, then select the option<span class="bold"> Use <span>Work Effort</span> to automatically calculate task Planned hours</span>. This is deselected by default. </p>  <p>For more information about enabling the use of <span>Work Effort</span> on a project, see the "Tasks Settings" section in the <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a> article. </p> </li> 
 <li value="3"> Click Tasks on the left panel , then click the name of a task to access it. </li> 
 <li value="4"> <p> Click the More menu , then click Edit.Ensure the task has a Simple Duration Type. </p> Tip: You can update the Work Effort for a task in the Task Details section as well. </li> 
 <li value="5"> <p>In the <span class="bold">Overview</span> area, click the <span>Work Effort</span> drop-down menu to correct the amount of effort needed to complete the task. </p> <p> <img src="assets/work-effort-on-edit-task-page-350x239.png" style="width: 350;height: 239;"> </p> <p>For more information about updating the <span>Work Effort</span> field on a task, see the following articles:</p> 
  <ul> 
   <li> The "Overview" section in the <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a> article</li> 
   <li><a href="../../../manage-work/tasks/manage-tasks/task-information-in-overview.md" class="MCXref xref">Manage task information in the Task Details Overview area</a> </li> 
  </ul> </li> 
</ol>

## Levels of `Work Effort`

As a project manager, you can identify three levels of `Work Effort` for your projects. Each level of effort equates with a percentage of daily time that users need to complete the task.

When setting up the level of `Work Effort` you have to ask yourself the question: "How much time should a user assigned to this task spend on it daily to get it done in time?"&nbsp;

The following table illustrates the possible levels of `Work Effort` and their default corresponding percentages. As a project manager, you can update the percentages to suit the needs of your organization. You do this as you edit a project.&nbsp;For information about editing projects, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

As a `Workfront administrator`, you define the Typical hours per work day in the Project Preferences area of Setup. This is the daily amount of time considered as working time. For information about configuring Project Preferences for your instance of `Workfront`, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

>[!NOTE]
>
>In the examples below, we assume that the `Workfront administrator` has set the Typical hours per work day amount to 8 hours.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Level of <span>Work Effort</span></td> 
   <td>Percentage values</td> 
  </tr> 
  <tr> 
   <td>Small </td> 
   <td>A Small level of effort for completing a task is set to 25% of the Typical hours per work day. This means that a task assigned this level of <span>Work Effort</span> should take up to 2 hours a day to complete in one day. <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>Medium</td> 
   <td> <p>A Medium level of effort for completing a task is set to 50% of the Typical hours per work day.&nbsp;This means that a task assigned this level of&nbsp;<span>Work Effort</span> should take more than 2 and less than 6 hours to complete in one day. <code>(0.50*80=4)</code> </p> <p>Note: When the Use <span>Work Effort</span> to automatically calculate task Planned Hours setting is enabled on the project this is the default setting for a task, if the task had 0 Planned Hours before this setting was enabled. This causes the task Planned Hours to update to 4 hours. </p> </td> 
  </tr> 
  <tr> 
   <td>Large</td> 
   <td>A Large level of effort for completing a task is set to 75% of the Typical hours per work day. This means that a task assigned this level of&nbsp;<span>Work Effort</span> should take 6 hours or more to complete in one day. <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## How `Workfront` calculates Planned Hours based on `Work Effort`

When you enable the Use `Work Effort` to automatically calculate task Planned Hours setting on a project, `Workfront` calculates the number of Planned Hours for a task with a Simple Duration&nbsp;Type using the following formula:

```
Task Planned Hours = Number of days in task Duration * <span>Work Effort</span> percentage * Typical hours per work day
```

For example, a task with a Duration of 3 days and a `Work Effort` of Medium has 12 Planned Hours:

```
Planned Hours = 3*4=12
```

where the&nbsp;Typical hours per work day value is 8 hours.

>[!TIP]
>
>When a task is assigned to multiple resources, the Planned Hours are evenly distributed to each resource for each day of the task's duration.

## How `Workfront` calculates `Work Effort` based on Planned Hours

When you enable the Use `Work Effort` to automatically calculate task Planned Hours setting on a project and you already have Planned Hours on the task or you edit the number of Planned Hours on the task, `Workfront` updates the `Work Effort` value.

`Workfront` uses the following formula to update the level of `Work Effort` according to the Planned Hours:

```
<span>Work Effort</span> level = Task Planned Hours / Duration / Typical hours per work day
```

For example, if you have a task with a Duration of 2 days and you update the Planned Hours from 8 to 20 hours, the `Work Effort` for the task updates from Medium to Large:

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## Locate `Work Effort` for tasks and projects

* [Work Effort for projects](#for) 
* [Work Effort for tasks](#for2)

### `Work Effort` for projects

You can locate the `Work Effort` section on a project in the following area:

* The Task&nbsp;Settings area in the Edit Project box

### `Work Effort` for tasks

You can locate the `Work Effort` field for a task in the following areas:

* The Overview area in the Edit Task box
* The Overview area of the Task Details section, in the Working time area 
* A task list or report

