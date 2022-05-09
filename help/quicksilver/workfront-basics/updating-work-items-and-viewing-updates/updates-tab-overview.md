---
filename: updates-tab-overview
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Updates tab overview
description: The Updates tab shows up to 200 of the most recent updates made within the past 90 days. You can reply to updates on the following objects - EDIT ME.
---

# Updates tab overview

The Updates tab shows up to 200 of the most recent updates made within the past 90 days.&nbsp;You can reply to updates on the following objects:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Projects</li> 
     <li>Portfolios</li> 
     <li>Programs</li> 
     <li>Templates</li> 
     <li>Template Tasks</li> 
     <li>Tasks</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Issues</li> 
     <li>Iterations</li> 
     <li>Stories</li> 
     <li>Users</li> 
     <li>Documents</li> 
     <li>Timesheets</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Updates that also appear on higher-rank objects

As shown in the following table, replies made to updates on certain objects also appear on the Updates tab of higher-ranked objects.

For example, when you add an update to a task, the update appears on the Updates tab for the task and on the Updates tab for the project containing the task.

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Object where the original update was added</strong> </th> 
   <th> <p><strong>Higher-ranked object where the original update also appears</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Issue</td> 
   <td>Project</td> 
  </tr> 
  <tr> 
   <td>Task</td> 
   <td>Project</td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Program, Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Document </td> 
   <td>Object where document is attached, Project </td> 
  </tr> 
  <tr> 
   <td>Program</td> 
   <td>Portfolio</td> 
  </tr> 
  <tr> 
   <td>User</td> 
   <td>Team</td> 
  </tr> 
  <tr> 
   <td>Timesheet</td> 
   <td>User, Team</td> 
  </tr> 
  <tr> 
   <td>Template Task</td> 
   <td>Template</td> 
  </tr> 
  <tr> 
   <td>Story</td> 
   <td>Iteration, Team</td> 
  </tr> 
  <tr> 
   <td>Iteration</td> 
   <td>Team</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Replies added to system updates do not roll up to the parent object. Only direct replies on a child object and replies added to existing updates roll up to parent objects.

For informatics about the object hierarchy in Adobe Workfront, see [Understand objects in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Limitations of the Updates tab

### Limitations for users and teams

You cannot make updates on teams. The Updates tab for teams is&nbsp;populated by updates entered on the following objects:

* Users
* Timesheets
* Stories
* Iterations

On the Updates tab for&nbsp;users and teams, you can view the updates that have been entered in the past 90 days.

If you want to see all the updates made on a user or a team, beyond the 90-day limit, you can build a report for notes. The report should not have a time filter that displays all updates made for users or teams. For more information, see [Create a custom report](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Limitations when entering comments on behalf of another user

Adobe Workfront administrators and group administrators can log in as other users and perform actions in Workfront such as entering comments. (For information, see [Log in as another user](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).) Any comments made on behalf of another user are indicated on the comment.

A group administrator can comment on behalf of another person but cannot delete that comment. Only an Adobe Workfront administrator can delete a comment that they made on behalf of another user.

## View system updates on work items with the Journal Entry report

The Journal Entry report surfaces system updates from the Updates area of projects, tasks, and issues.

The report allows you to see:

* How many status changes occurred
* When a task or issue was deleted
* How values in important custom fields changed over the course of a project
* What important dates changed over the course of a project
* If priority changed over the course of a project
* If the owner of a project changed

For more information, see [Report on the Updates area](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
