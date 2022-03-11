---
filename: project-planned-completion-date
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Set the project Planned Completion Date
description: The Planned Completion Date of a project is the date by which the project is set to complete.
---

# Set the project Planned Completion Date

The Planned Completion Date of a project is the date by which the project is set to complete.

The Planned Start and the Planned Completion Dates of a project rely on the dates of the tasks on the project.&nbsp;This article describes how you can manually or automatically set the Planned Completion Date of a project.&nbsp;For more information about the Planned Completion Date of a task, see [Overview of the task Planned Completion Date](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

The Planned Completion Date of a project can be set manually or automatically, depending on whether you schedule the project from the Start or from the Completion Date.&nbsp;

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Manually set the Planned Completion Date of a project

You must manually set the Planned Completion Date of a project when you schedule the project from Completion Date.&nbsp;

To schedule a project from Completion Date:

1. Click the Main Menu icon in the upper-right corner, then click Projects.
1. Click New Project then New Project.

   For more information about creating projects, see the article [Create a project](../../../manage-work/projects/create-projects/create-project.md).

1. Select Project Details in the left panel, then click the Edit Project icon in the upper-right corner.
1. In the `Schedule From` field, select `Completion Date`.

1. Specify the `Planned Completion Date` of the project.
1. Click `Save Changes`.

   As you start adding tasks to your project, the `Planned Start Date` of the project calculates based on the total Duration of all of the tasks.&nbsp;

## Automatically set the Planned Completion Date of a project

The Planned Completion Date of a project is automatically calculated by Adobe Workfront when you schedule the project from Start Date.&nbsp;

To schedule a project from Start Date:

1. Click the Main Menu icon in the upper-right corner, then click Projects.
1. Click New Project then New Project.

   For more information about creating projects, see the article [Create a project](../../../manage-work/projects/create-projects/create-project.md).

1. Select Project Details in the left panel, then click the Edit Project icon in the upper-right corner.
1. In the `Schedule From` field, select `Start Date`.

1. Specify the `Planned Start Date` of the project.
1. Click `Save Changes`.

   As you start adding tasks to your project, the `Planned Completion Date` of the project calculates based on the total Duration of all of the tasks.&nbsp;

   For more information about Task Duration, see the article [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   The Planned Completion Date of the project coincides, in this case, with the Planned Completion Date of the last task on the project.

<!--
The Planned Completion Date of a task You can either specify the Planned Completion Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria. Manually set the Planned Completion Date of a task How the Planned Completion Date is calculated for a task Manually set the Planned Completion Date of a task Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task. You can manually set the Planned Completion Date when creating a task, as described in the article Create tasks in a project. You can manually specify the Planned Completion Date when you select any of the following Task Constraints: Task Constraint Type Effect of Manually Changing the Planned Completion Date Must Finish On Finish No Later Than Finish No Earlier Than The Planned Start Date is adjusted in order to keep the Duration the same. Fixed Dates The Duration is adjusted in order to keep the Planned Start Date the same. How the Planned Completion Date is calculated for a task When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task: Task Constraint For more information about Task Constraints, see the article Task Constraint overview. Task predecessor relationship For more information about task predecessors, see the article Overview of task predecessors. Project Completion Date, when the project is scheduled from Completion Date. The time off schedule of the Primary Assignee of the task. When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the Consider user time off in task durations setting is selected for the User Time Off field. New projects inherit this setting from the Project Preferences area, but you can edit the setting at the project level. For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. For information about the User Time Off preference, see the articles Configure system-wide project preferences or Edit projects. When set automatically, the Planned Completion Date is determined based on the following calculation: Planned Completion Date = Planned Start Date + Duration For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26. Note: The Update Type for the project must also be set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically adjusted. For more information about the Update Type, see the article Select the project Update Type .
-->

