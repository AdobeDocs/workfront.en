---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Updates section overview
description: The Updates section of an object displays comments that users make on the object or system updates that track changes to the object.
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
---

# Updates section overview

<!-- Audited: 1/2024 -->


<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>
-->

The Updates section of an object displays comments that users make on the object or system updates that track changes to the object.

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process.
--> 

## Overview of the Updates section

The Updates section of an object shows system updates, and up to 200 of the most recent updates users made within the past 90 days.

![Updates section](assets/updates-tab-with-unified-experience-for-issues-all-tab.png)

<!--Info for April 11: Add the following right under the screen shot above:-->

The following objects have an Updates section where you can add comments or review system updates: 

* Projects
* Tasks
* Issues
* Programs
* Portfolios
* Templates
* Template tasks
* Users
* Timesheets
* Teams
* Goals
* Cards in the Boards area
* Iterations

<!--info for April 11: remove all the information below, all the way down to the following section: -->

<!--
Depending on what objects you access the commenting experience for, you might find the following experience for the Updates section:

* Both the new and legacy commenting experience for the following objects: 

  * Project
  * Task (this includes Stories)
  * Issue
  * Document

    >[!TIP]
    >
    >Use the New commenting option to display the new commenting experience (when you enable it) or the legacy commenting experience (when you disable it). The new commenting experience is the default. For more information, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 

* Only the new commenting experience for the objects listed below. There is no option to enable the legacy commenting experience for these objects:   

  * Goal

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 

  * Card on a board
  * Team
  * Template
  * Template Task
  * Timesheet
  * Program
  * Portfolio
  * User

* Only the legacy commenting experience for the following objects:

  * Iterations

    There is no option to enable the new commenting experience for iterations. For more information, see [Manage iteration comments](/help/quicksilver/agile/use-scrum-in-an-agile-team/iterations/manage-iteration-updates.md). 
-->

<!--Info for April 11: reword the section title below to: Overview of the Updates section; and remove the preview tags-->

### Overview of the Updates section 

![Updates section](assets/updates-tab-after-unified-experience-for-tasks-all-tab.png)

* The Updates section displays information in the following tabs:

  * **Comments**: Displays comments made by users and replies to those comments. Use the Comments tab to add new comments or reply to existing ones. For information about updating objects, see [Update work](../updating-work-items-and-viewing-updates/update-work.md).
  * **System Activity**: Displays system updates which are informational messages that Workfront creates to record certain events on an objects. For example, changes in status, name, or custom fields are captured with system updates. Your Workfront or group administrator can enable system updates for your objects. Any replies that were made to system activity records in the legacy commenting experience are populated on the System Activity tab as read-only. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).
  * **All (read-only)**: Displays both user comments and system activity comments in one place. This is a view-only tab. You cannot reply to comments or tag other users in existing comments in the All tab. To reply to a specific comment, use the link from the All tab to the Comments tab. For information about updating objects, see [Update work](../updating-work-items-and-viewing-updates/update-work.md).

* The following objects have similar experiences in all three tabs in the Updates section:

  * Projects
  * Tasks
  * Issues
  * Programs
  * Portfolios
  * Users
  * Timesheets

* The following objects don't have a System Activity tab or an All tab, and the experience in the Comments tab matches that of all other objects:

  * Team
  * Template
  * Template Task

* The following objects don't have a System Activity tab or an All tab, and the experience in the Comments tab differs from that of all other objects:
  * Iterations
  * Ad-hoc Card

    For more information about updates on cards, see [Add an ad hoc card to a board](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

* The following objects don't have an All tab, and the experience in the Comments tab matches that of most objects:

  * Goals

    For more information about updates on goals, see [Manage goal comments](/help/quicksilver/workfront-goals/goal-management/manage-goal-comments.md).

<!-- info for April 11: hide the entire section below: -->

<!--
### Overview of the legacy Updates section 

![](assets/updates-tab-before-unified-experience-for-tasks.png)

The legacy Updates section shows the following information:

* **User updates**: Comments made by users and replies to those comments. 
* **System updates**: Informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your objects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

The following objects don't record system updates:

* Team
* Template
* Template Task
* Iterations
-->

## Updates that also appear on higher-ranking objects

Comments, replies, or system updates of certain objects also appear on the Updates section of higher-ranking objects.

For example, when you add an update to a task, the update appears on the Updates section for the task and on the Updates section for the project containing the task.

The following table shows the objects whose comments also display on their higher-ranking objects: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Object where the original update was added</strong> </th> 
   <th> <p><strong>Higher-ranking objects where the original update also appears</strong> </p> </th> 
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
   <td><p>User, Team</p>
   <p><b>NOTE</b></p>
   <p>Timesheet comments display in the Updates section of the user who makes the comment and the Updates section of their Home Team.</p>
   </td> 
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

<tr> 
   <td>Result</td> 
   <td>Goal</td> 
  </tr> 
  <tr> 
   <td>Activity</td> 
   <td>Goal</td> 
  </tr> 
 </tbody> 
</table>
 
<!--info for April 11: hide the note below-->

<!--
>[!NOTE]
>
>Replies added to system updates do not roll up to the parent object. Only direct replies on a child object and replies added to existing updates roll up to parent objects.
>
>For information about the object hierarchy in Adobe Workfront, see [Understand objects in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
>
> It is not possible to reply to system updates in the new commenting experience. For more information, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
-->


## Limitations of the Updates section

There are some limitations in the Updates section of a team and when entering updates on behalf of other users. 

### Limitations for users and teams

Consider the following when viewing updates for users and teams: 

* You cannot add new comments in the Updates section of a team. 

* The Updates section for teams is populated by updates entered on the following objects:

  * Users
  * Stories
  * Timesheets
  * Iterations

* You can add a reply to an update you view on a team. The reply displays in the team's Updates section as well as the Updates section of the object it belongs to.

* On the Updates section for users and teams, you can view the updates that have been entered in the past 90 days.

  If you want to see all the updates made on a user or a team, beyond the 90-day limit, you can build a report for notes. The report should not have a time filter that displays all updates made for users or teams. For more information, see [Create a custom report](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Limitations when entering comments on behalf of another user

Adobe Workfront administrators and group administrators can log in as other users and perform actions in Workfront such as entering comments. 

For information, see [Log in as another user](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

Consider the following when logging in as another user and adding comments:

* Any comments made on behalf of another user are indicated on the comment.

* A group administrator can comment on behalf of another person but cannot delete that comment. Only an Adobe Workfront administrator can delete a comment that they made on behalf of another user.

* A Workfront or group administrator can only edit a comment they added on behalf of another user only when they log out as the user and log back in as themselves. They cannot delete a comment on behalf of another user. 

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
