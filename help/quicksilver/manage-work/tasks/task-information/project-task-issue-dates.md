---
filename: project-task-issue-dates
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overview of project, task, and issue dates
description: Introduction about dates in WF
---

# Overview of project, task, and issue dates

Introduction about dates in WF

Tasks are associated with Start and Completion Dates to illustrate their timeline in the life of a project.&nbsp;

There are several sets of dates associated with tasks. Some of them can be manually edited, and some of them are automatic calculations that Adobe Workfront performs after certain actions or events occur on the task.&nbsp;

The following table contains information about dates associated with projects, tasks, and issues: 

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Date Name</span> </th> 
   <th><span class="bold">Definition</span> </th> 
   <th><span class="bold">Object</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Actual Completion Date</td> 
   <td>The date when the task actually completes. A task can receive an Actual Completion Date when its status changes from In Progress to Complete.</td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks&nbsp;</li> 
     <li>Issues</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Actual Start Date</td> 
   <td>The date when the task actually starts. A task can automatically receive an Actual Start Date when its status changes from New to In Progress.&nbsp;</td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Approval Path Completion Date</td> 
   <td>The date when the task in a Pending Approval status is either approved or rejected. This date is not populated for tasks without Approval Processes or with Approval Processes which have not been granted yet.&nbsp;&nbsp;<br><p>Note:  If you grant an approval on a task more than once, or if you attach multiple Approval Processes to the task and you grant several approvals for the multiple statuses, only the last time when you approve or reject the task is recorded as the Approval Path Completion Date.</p></td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Project</li> 
     <li>Task&nbsp;</li> 
     <li>Issue</li> 
    </ul> &nbsp; </td> 
  </tr> 
  <tr> 
   <td>&nbsp;Approval Path Start Date</td> 
   <td> <p>The date when the task is placed in a Pending Approval status. This date is not populated for tasks without Approval Processes or Approval Processes which have not started yet.</p> <p>Note:  If you place the task in the Pending Approval status more than once, or if you attach multiple Approval Processes to the task and you place the task in a Pending Approval status for multiple statuses, only the last time when you placed the task in a Pending Approval status is recorded as the Approval Path Start Date.&nbsp;</p> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks&nbsp;</li> 
     <li>Issues</li> 
    </ul> &nbsp; </td> 
  </tr> 
  <tr> 
   <td>Auto Closure Date</td> 
   <td>&nbsp;</td> 
   <td> <p> This date applies to </p> 
    <ul> 
     <li> Issues </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Budgeted Completion Date</td> 
   <td>&nbsp;</td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Budgeted Start Date</td> 
   <td>&nbsp;</td> 
   <td> <p> This date applies to </p> 
    <ul> 
     <li> Projects </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Commit Date</td> 
   <td> <p> When the Project Owner creates a task, the Commit Date and the Planned Completion Date of the task are identical.</p> <p>An assignee of a task can suggest a new Commit Date to indicate that they would not be able to complete the task by the date suggested by the Project Owner. This does not change the Planned Completion Date automatically, and from this on, the two dates are different.<br></p> <p>Note:  Only an assignee of a task can modify the Commit Date. The Project Owner, a system administrator or any other user with Contribute permissions to the task cannot modify the Commit Date.</p> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Tasks</li> 
     <li>Issues</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Completion Pending Date</td> 
   <td><span class="wysiwyg-color-pink">&nbsp;</span> </td> 
   <td> <p>This date applies to&nbsp;</p> 
    <ul> 
     <li>Tasks</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Constraint Date</td> 
   <td> <p>If a task has a forced constraint around the Planned Start or Planned Completion Dates, the date of the constrained date is the Constraint Date.&nbsp;</p> <p>The following are possible forced Task Constraints:</p> 
    <ul> 
     <li>Must Start On</li> 
     <li>Must Finish On</li> 
     <li>Start No Later Than</li> 
     <li>Start No Earlier Than</li> 
     <li>Finish No Later Than</li> 
     <li>Finish No Earlier Than</li> 
    </ul> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Tasks</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Date 1</td> 
   <td>&nbsp;</td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Delivery Date</td> 
   <td>&nbsp;</td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Due Date</td> 
   <td>It is the same as the Planned Completion Date.</td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Tasks</li> 
     <li>Issues</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Entry Date</td> 
   <td>The date when the task was created.&nbsp;</td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Estimated Due Date</td> 
   <td> <p> &nbsp;It is similar to the Projected Completion Date, and they are closest to the reality of when a task can complete, based on its progress, predecessor relationship, and work left to be completed.</p> <p>For more information about the Estimated Dates and how they are different than the Projected Dates, see <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Differentiate between Projected and Estimated Dates </a>.</p> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Estimated Start Date</td> 
   <td> <p> The Estimated Start Date is similar to the Projected Start Date, and they are closest to the reality of when a task can start, based on its progress, predecessor relationship, and work left to be completed.</p> <p>For more information about the Estimated Dates and how they are different than the Projected Dates, see <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Differentiate between Projected and Estimated Dates </a>.</p> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Fixed End Date</td> 
   <td>&nbsp;</td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Fixed Start Date</td> 
   <td>&nbsp;</td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Handoff Date</td> 
   <td> <p>The Handoff Date is the date a task becomes available for work. This typically means that its predecessors have resolved and the assignee of the task can start working on it.&nbsp;</p> <p>For more information about the Handoff Date and how it is calculated, see <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">Task Handoff Date overview</a>.</p> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Tasks</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Last Calc Date</td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Last Finance Update Date</td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Last Update Date</td> 
   <td> <p>The date when the task was last updated. The following are examples of what constitutes an update on a task:</p> 
    <ul> 
     <li>A user edits any information on the task in the Edit Task dialog box, or the Task Details tab</li> 
     <li>A comment is added to the task in the Updates tab</li> 
     <li>An Approval Process is added to the task</li> 
     <li>An approval decision is granted</li> 
     <li>An Expense is added to the task.</li> 
     <li>The predecessor relationship is updated.&nbsp;</li> 
    </ul> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Planned Completion Date</td> 
   <td> <p>This is the original Completion Date of the task, as planned by the Project Owner or the creator of the task.</p> <p>The Planned Completion Date can be automatically updated when any of the following actions occur:</p> 
    <ul> 
     <li>The Project Owner accepts a new Commit Date from an assignee.</li> 
     <li>The Duration of the task changes and the Planned Start Date does not.</li> 
     <li>The Duration Type of the task changes.</li> 
     <li>The number of assignees on the task changes, along with the Duration Type.&nbsp;</li> 
    </ul> <p>&nbsp;</p> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Planned Start Date</td> 
   <td> <p>This is the original Start Date of the task, as planned by the Project Owner or the creator of the task.</p> <p>The Planned Start Date can be automatically updated when any of the following actions occur:</p> 
    <ul> 
     <li>The Duration of the task changes and the Planned Completion Date does not.</li> 
     <li>The task is assigned a predecessor or the predecessor of the task changes dates.</li> 
    </ul> </td> 
   <td>Manually updated by the user or automatically updated by Workfront.&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Planned Date Alignment</td> 
   <td>&nbsp;</td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues&nbsp;</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Planned Start Date</td> 
   <td>Start On = Planned Start Date - this is a date set by a user (e.g. Project/Task/Issue owner) or Workfront&nbsp;indicating when a Project/Task/Issue is planned to be started:&nbsp;</td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Projected Completion Date</td> 
   <td> <p>It is similar to the Estimated Completion Date, and they are closest to the reality of when a task can complete, based on its progress, predecessor relationship, and work left to be completed.</p> <p>For more information about the Projected Dates and how they are different than the Estimated Dates, see <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Differentiate between Projected and Estimated Dates </a>.&nbsp;&nbsp;</p> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues&nbsp;</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Projected Start Date</td> 
   <td> <p> It is similar to the Estimated Start Date, and they are closest to the reality of when a task can start, based on its progress, predecessor relationship, and work left to be completed.</p> <p>For more information about the Projected Dates and how they are different than the Estimated Dates, see <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Differentiate between Projected and Estimated Dates </a>.</p> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Slack Date</td> 
   <td> <p>The Slack Date displays the exact date when a task could definitely impact the Completion Date of the project.</p> <p>For more information about Slack Dates, see "Understanding&nbsp;</p> </td> 
   <td> <p>This date applies to</p> 
    <ul> 
     <li>Tasks</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

