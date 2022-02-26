---
filename: create-recurring-tasks
product-area: projects
navigation-topic: create-tasks
title: Create recurring tasks
description: You can create recurring tasks for tasks you have to repeat as part of a single project.
---

# Create recurring tasks

You can create recurring tasks for tasks you have to repeat as part of a single project.

For general information about recurring tasks, including the impact of editing an existing recurring task, see [Recurring tasks overview](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Work</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task in&nbsp;Adobe Workfront</a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Create a recurring task

>[!NOTE]
>
>You cannot create a recurring task by modifying an existing task. You must create a task from scratch.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<ol>
<li value="1"> <p>Go to the project where you want to create a recurring task, then click the <span class="bold">Tasks</span> section in the left panel.</p> </li>
<li value="2"> <p>Click <span class="bold">New Task</span>.</p> <p>The New Task dialog box displays.</p> <p> <img src="assets/nwe-create-task-small-screen-350x272.png" style="width: 350;height: 272;"> </p> </li>
<li value="3"> <p>Click <span class="bold">More Options</span> then enter a name for the task in the <span class="bold">Task Name</span> field.</p> </li>
<li value="4"> <p> Continue updating the task the same way you would if you added a new task. For more information about adding a new task, see <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a></p> </li>
<li value="5"> <p>Click <span class="bold">Overview</span> in the left panel.</p> </li>
<li value="6"> <p>Scroll down to the <span class="bold">Recurrence Schedule</span> section, then select the <span class="bold">Make this a recurring task</span> option.</p> <p> <img src="assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png" style="width: 350;height: 351;"> </p> </li>
<li value="7"> <p>In the <span class="bold">Frequency</span> drop-down list, select the number of time units when you want the task to occur and the type of time units.&nbsp;Select from the following options: </p>
<table cellspacing="0">
<col>
<col>
<thead>
<tr>
<th>Recurrence Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td role="rowheader"><span class="bold">Day</span> </td>
<td> <p>The task repeats every day, every 2 days, every 3 days, and so forth, depending on the cadence that you select. You can configure tasks to repeat up to every 6th day. The default setting is 1 Day. </p> </td>
</tr>
<tr>
<td role="rowheader"><span class="bold">Working Day</span> </td>
<td> <p> The task repeats every working day, every 2 working days, every 3 working days, and so forth, depending on the cadence that you select. You can configure tasks to repeat up to every 6th working day.</p> <p>This option uses the default schedule that is defined by the system administrator, as described in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> </td>
</tr>
<tr>
<td role="rowheader"><span class="bold">Week</span> </td>
<td> <p> The task repeats every week, every 2 weeks, every 3 weeks, and so forth, depending on the cadence that you select.</p> <p>In the <span class="bold">Repeats</span> field, select the day of the week when you want each task to occur. You can select multiple days. </p> </td>
</tr>
<tr>
<td role="rowheader"><span class="bold">Month</span> </td>
<td> <p>The task repeats every month, every 2 months, every 3 months, and so forth, depending on the cadence that you select. You can select between 1 and 12 months. </p> <p>In the <span class="bold">Repeats</span> field, select from the following options when you want the task to occur:</p>
<ul>
<li> <p><span class="bold">every month on day <month date></span> </p> <p>You can select days from 1 to 30 or you can select <span class="bold">last</span>. For example, you can select "every month on the 30th". </p> </li>
<li> <p><span class="bold">every month on the <number> <day of the week></span> </p> <p>In the first drop-down menu, you can select a number between 1 and 4 for the number of the week in the month, or you can select "last". </p> <p>In the second drop-down menu, you can select any day of the week. </p> <p>For example, you can select "every month on the 2nd Tuesday". </p> </li>
</ul> </td>
</tr>
</tbody>
</table> <note type="note">
If you have a Schedule Exception associated with the project's schedule, recurring tasks can't start during the exception. Recurring tasks that occur during the schedule exception are scheduled to start on the first business day that follows the exception. For more information on schedule exceptions, see the article
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li value="8"> <p>In the <span class="bold">Starts</span> field, select the date and time when you want the recurring tasks to begin. </p> </li>
<li value="9"> <p>In the <span class="bold">Ends</span> field, select the date and the time when you want the recurring tasks to complete</p> <p>Or</p> <p>Select <span class="bold">after <number>&nbsp;occurrences</span> to indicate how many times the recurring task should occur. <em>Workfront</em> creates the same number of recurrences for the tasks as the number you indicate in this field. </p> </li>
<li value="10"> <p>Click <span class="bold">Create Task.</span></p> <p>The task list displays. The recurring task is created as a parent, and all the recurrences are its children. <em>Workfront</em> auto-generated the names of the children tasks, using the name you entered for the parent followed by a number. For more information about what fields are auto-filled from the parent recurring task, see <a href="../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md" class="MCXref xref">Recurring tasks overview</a>. </p> <p> <img src="assets/recurring-tasks-in-task-list-nwe-350x87.png" style="width: 350;height: 87;"> </p> </li>
<li value="11"> <p>(Optional) Modify each recurring task as you would any other task in the project.</p> <p>For example, you can add assignments, predecessors, durations, and modify any other information about the task, including custom fields. </p> <note type="important">
Modifying the parent recurrence after the children have been modified individually may cause different information between the children or between the children and the parent.&nbsp;For more information, see
<a href="../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md" class="MCXref xref">Recurring tasks overview</a>.
</note> </li>
</ol>
</div>
-->

<ol> 
 <li value="1"> <p>Go to the project where you want to create a recurring task, then click the <span class="bold">Tasks</span> section in the left panel.</p> </li> 
 <li value="2"> <p>Click <span class="bold">New Task</span>.</p> <p>The New Task dialog box displays.</p> <p> <img src="assets/nwe-create-task-small-screen-350x272.png" style="width: 350;height: 272;"> </p> </li> 
 <li value="3"> <p>Click <span class="bold">More Options</span> then enter a name for the task in the <span class="bold">Task Name</span> field.</p> </li> 
 <li value="4"> <p> Continue updating the task the same way you would if you added a new task. For more information about adding a new task, see <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a></p> </li> 
 <li value="5"> <p>Click <span class="bold">Overview</span> in the left panel.</p> </li> 
 <li value="6"> <p>Scroll down to the <span class="bold">Recurrence Schedule</span> section, then select the <span class="bold">Make this a recurring task</span> option.</p> <p> <img src="assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png" style="width: 350;height: 351;"> </p> </li> 
 <li value="7"> <p>In the <span class="bold">Frequency</span> drop-down list, select the number of time units when you want the task to occur and the type of time units.&nbsp;Select from the following options: </p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Recurrence Type</th> 
     <th>Description</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Day</span> </td> 
     <td> <p>The task repeats every day, every 2 days, every 3 days, and so forth, depending on the cadence that you select. You can configure tasks to repeat up to every 6th day. The default setting is 1 Day. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Working Day</span> </td> 
     <td> <p> The task repeats every working day, every 2 working days, every 3 working days, and so forth, depending on the cadence that you select. You can configure tasks to repeat up to every 6th working day.</p> <p>This option uses the default schedule that is defined by the system administrator, as described in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Week</span> </td> 
     <td> <p> The task repeats every week, every 2 weeks, every 3 weeks, and so forth, depending on the cadence that you select.</p> <p>In the <span class="bold">Repeats</span> field, select the day of the week when you want each task to occur. You can select multiple days. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Month</span> </td> 
     <td> <p>The task repeats every month, every 2 months, every 3 months, and so forth, depending on the cadence that you select. You can select between 1 and 12 months. </p> <p>In the <span class="bold">Repeats</span> field, select from the following options when you want the task to occur:</p> 
      <ul> 
       <li> <p><span class="bold">every month on day <month date></span> </p> <p>You can select days from 1 to 30 or you can select <span class="bold">last</span>. For example, you can select "every month on the 30th". </p> </li> 
       <li> <p><span class="bold">every month on the <number> <day of the week></span> </p> <p>In the first drop-down menu, you can select a number between 1 and 4 for the number of the week in the month, or you can select "last". </p> <p>In the second drop-down menu, you can select any day of the week. </p> <p>For example, you can select "every month on the 2nd Tuesday". </p> </li> 
      </ul> </td> 
    </tr> 
   </tbody> 
  </table> <note type="note">
   If you have a Schedule Exception associated with the project's schedule, recurring tasks can't start during the exception. Recurring tasks that occur during the schedule exception are scheduled to start on the first business day that follows the exception. For more information on schedule exceptions, see the article 
   <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
  </note> </li> 
 <li value="8"> <p>In the <span class="bold">Starts</span> field, select the date and time when you want the recurring tasks to begin. </p> </li> 
 <li value="9"> <p>In the <span class="bold">Ends</span> field, select the date and the time when you want the recurring tasks to complete</p> <p>Or</p> <p>Select <span class="bold">after <number>&nbsp;occurrences</span> to indicate how many times the recurring task should occur. <em>Workfront</em> creates the same number of recurrences for the tasks as the number you indicate in this field. </p> </li> 
 <li value="10"> <p>Click <span class="bold">Create Task.</span></p> <p>The task list displays. The recurring task is created as a parent, and all the recurrences are its children. <em>Workfront</em> auto-generated the names of the children tasks, using the name you entered for the parent followed by a number. For more information about what fields are auto-filled from the parent recurring task, see <a href="../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md" class="MCXref xref">Recurring tasks overview</a>. </p> <p> <img src="assets/recurring-tasks-in-task-list-nwe-350x87.png" style="width: 350;height: 87;"> </p> </li> 
 <li value="11"> <p>(Optional) Modify each recurring task as you would any other task in the project.</p> <p>For example, you can add assignments, predecessors, durations, and modify any other information about the task, including custom fields. </p> <note type="important">
   Modifying the parent recurrence after the children have been modified individually may cause different information between the children or between the children and the parent.&nbsp;For more information, see 
   <a href="../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md" class="MCXref xref">Recurring tasks overview</a>. 
  </note> </li> 
</ol>

