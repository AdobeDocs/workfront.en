---
filename: system-task-statuses
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: System task statuses
description: There are 3 built-in system task statuses in Workfront. All 3 are required, which means that you can unlock, rename, and reorder them, but you cannot hide or delete them.
---

# System task statuses

There are 3 built-in system task statuses in `Workfront`. All 3 are required, which means that you can unlock, rename, and reorder them, but you cannot hide or delete them.

You can also add new system task statuses to match the needs in your organization.

Changing the status of a task is typically a manual process. However, there are times outlined in the following list when the status of a task is changed automatically, depending on other factors that are happening in the system.

The following task statuses are provided with your `Workfront` instance:

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>System Task Status</th> 
   <th>When this Task Status`Actions that Happen when the Task Is in This Status Occurs</th> 
   <th>Actions that Happen when the Task&nbsp;Is in This Status</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>New (required status)</td> 
   <td>This is the default status for every newly created task.</td> 
   <td>If the task is on a project in a status of Current, the task displays in the Work Requests tab of the users who are assigned to the tasks. Users can now start working on the task.</td> 
  </tr> 
  <tr> 
   <td>In Progress (required status)</td> 
   <td>You may place a task in this status to indicate that work on that task has started.</td> 
   <td> <p>When you mark&nbsp;a task as&nbsp;In Progress, the task shows a value for the&nbsp;Actual Start Date.</p> <p>Progress on the task is not recorded until you manually update the percent complete of the task.</p> </td> 
  </tr> 
  <tr> 
   <td>Complete (required status)</td> 
   <td> <p>You can manually mark a task complete when the work on it is completed.</p> <p>When the Tracking Mode of a task is set to Autocomplete, the task is automatically marked Complete when it reaches the Planned Completion Date.</p> </td> 
   <td> <p>When a task is completed, the percent complete of the task is marked as 100%. The task is removed from the assignee's Work List in the Home area when it is completed.</p> <p>When you mark a task as Complete, the task shows a value for the Actual Completion&nbsp;Date.</p> <p>Note: If the task has incomplete issues and you change the task status to Complete, the status automatically changes to Complete - Pending Issues.</p> </td> 
  </tr> 
 </tbody> 
</table>

