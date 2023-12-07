---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Task Constraint overview
description: Task constraints determine when a task should start and end on a project.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
---
# Task Constraint overview

Task constraints determine when a task should start and end on a project.

## Overview of Task Constraints

As you build your project plan, you make decisions on the sequence and time frame of your tasks on the project. Tasks can function independently of any task sequence but they might impact the project timeline. Task Constraints allow a project manager to plan when certain tasks can start or complete on a project.

Depending on the constraint you use, you might have to specify a Planned Start Date, a Planned Completion Date, or both for the task.

Constraint types that require defined dates impact predecessor relationships.

>[!TIP]
>
>Consider using a constraint type that does not require specific dates if you are using predecessor relationships between tasks.

The following table displays each constraint and its abbreviation. Abbreviations are used on task lists and when creating Kick-Start import files. Click the linked title of each task constraint for more information about that type of constraint.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>Constraint Name</strong> </p> </th> 
   <th> <p><strong>Abbreviation</strong> </p> </th> 
   <th> <p><strong>Description</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Task Constraint overview: As Soon As Possible</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td>
   <td scope="col"> <p>Places the start time of the task as close to the beginning of the project as possible.</p> 
   <p>It is the default constraint if the project uses a Schedule Mode from Start Date and if the system default start date for a new task is set to Based on the Project Planned Date. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Task Constraint overview: As Late As Possible </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
   <td scope="col"> <p>Places the completion time of the task as close to the end of the project as possible.</p> 
   <p>This is the default constraint when the project Schedule Mode is from Completion Date and the system or group default for the Start Date of a task is set to Based on the Project Planned Date. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Task Constraint overview: Earliest Available Time</a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
 <td scope="col"> <p>Schedules a task to begin at the earliest available time after considering any predecessor relationships.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Task Constraint overview: Latest Available Time</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
   <td scope="col"> <p>Schedules a task to begin at the latest available time after considering predecessor-successor relationships in the project.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Task Constraint overview: Start No Earlier Than</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
   <td scope="col"> <p>Schedules a task to start after the date you specify.</p> 
   <p>This is the default constraint if the project Schedule Mode is from Start Date and if the system or group default Start Date for a new task is set to Today.   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Task Constraint overview: Start No Later Than</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
   <td scope="col"> <p>Schedules a task to start prior to the date you specify.</p> 
   <p>This is the default constraint if the project Schedule Mode is from Completion Date and if the system or group default for the Start Date of a task is set to Today. 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Task Constraint overview: Finish No Earlier Than</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td>
   <td scope="col"> <p>Schedules a task to complete after the date you specify.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Task Constraint overview: Finish No Later Than</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
   <td scope="col"> <p>Schedules a task to complete before the date you specify.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Task Constraint overview: Must Start On</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
   <td scope="col"> <p>Schedules a task to start exactly on a specific date.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Task Constraint overview: Must Finish On</a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
   <td scope="col"> <p>Schedules a task to end on a specific date.</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Task Constraint overview: Fixed Dates</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
   <td> <p>Schedules a task to start and end on specific dates.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Overview of default constraints

When you create new tasks, a Task Constraint is automatically selected by Workfront.

Workfront uses two variables to decide which Task Constraint is selected by default for a new task:

* The **Project Schedule From** field on the project.

  For information about the Project Schedule From field, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

* The **Start Date** preference configured by your Workfront or group administrator in the **Tasks & Issues** area of **Setup**.

  For information about Tasks & Issues Preferences, see the [New Task Defaults](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#new-task-defaults) section in [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

The following table shows the default Task Constraint when choosing different variables for your project and your new tasks:

| Project Schedule From |Task Start Date |Task Constraint Default |
|---|---|---|
| Start Date |Based on the Project Planned Date |As Soon As Possible |
| Start Date |Today |Start No Earlier Than |
| Completion Date |Based on the Project Planned Date |As Late as Possible |
| Completion Date |Today |Start No Later Than |
