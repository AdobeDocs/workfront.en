---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Task Constraint overview
description: Task constraints determine when a task should start and end on a project.
feature: Work Management
---

# Task Constraint overview

Task constraints determine when a task should start and end on a project.

## Overview of Task Constraints

As you build your project plan, you make decisions on the sequence and time frame of your tasks on the project. Tasks can function independently of any task sequence but they might impact the project timeline. Task Constraints allow a project manager to plan when certain tasks can start or complete on a project.

Depending on the constraint you use, you might have to specify a Planned Start Date, a Planned Completion Date, or both for the task.

Constraint types that require defined dates impact predecessor relationships.

>[!TIP]
>
>Consider using a constraint type that does not require specific dates if using predecessor relationships between tasks.

The following table displays each constraint and its abbreviation. Abbreviations are used on task lists and when creating Kick-Start import files. Click the linked title of each task constraint for more information about that type of constraint.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Constraint Name</strong> </p> </th> 
   <th> <p><strong>Abbreviation</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Task Constraint overview: As Soon As Possible</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Task&nbsp;Constraint overview: As Late As Possible </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Task Constraint overview: Earliest Available Time</a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Task Constraint overview: Latest Available Time</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Task Constraint overview: Start No Earlier Than</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Task Constraint overview: Start No Later Than</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Task Constraint overview: Finish No Earlier Than</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Task Constraint overview: Finish No Later Than</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Task Constraint overview: Must Start On</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Task Constraint overview: Must Finish On</a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Task Constraint overview: Fixed Dates</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
  </tr> 
 </tbody> 
</table>

## Overview of default Constraints

When you create new tasks, a Task Constraint is automatically selected by Workfront.

Workfront uses two variables to decide what Task Constraint is selected by default for a new task:

* The **Project Schedule From** field on the project.

  For information about the Project Schedule From field, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

* The **Start Date** preference configured by your Workfront or group administrator in the **Tasks & Issues** area of **Setup**.

  For information about Tasks & Issues Preferences, see the "New Task Defaults" section in [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

The following table shows the default Task Constraint when choosing different variables for your project and your new tasks:

| Project Schedule From |Task Start Date |Task Constraint Default |
|---|---|---|
| Start Date |Based on the Project Planned Date |As Soon As Possible |
| Start Date |Today |Start No Earlier Than |
| Completion Date |Based on the Project Planned Date |As Late as Possible |
| Completion Date |Today |Start No Later Than |

