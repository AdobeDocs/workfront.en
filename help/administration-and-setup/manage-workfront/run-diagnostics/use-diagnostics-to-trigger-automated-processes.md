---
filename: use-diagnostics-to-trigger-automated-processes
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Use Diagnostics to trigger automated processes
description: You can use Diagnostics to manually trigger automated processes, such as time-based scripts, recalculations, or email notifications.
---

# Use Diagnostics to trigger automated processes

You can use Diagnostics to manually trigger automated processes, such as time-based scripts, recalculations, or email notifications.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span>Adobe Workfront</span> plan</a> </td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a> </td> 
   <td> <p><span>Plan</span> </p>You must be a <span>Workfront administrator</span>. For information on <span>Workfront administrators</span>, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</td> 
  </tr> 
 </tbody> 
</table>

## Use diagnostics to trigger automated processes

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2"> <p>Expand <span class="bold">System</span>, then click <span class="bold">Diagnostics</span>.</p> </li> 
 <li value="3"> <p>Select from any of the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Send Overdue Notifications</td> 
     <td> <p>Manually sends the automatic reminder notifications for overdue tasks and issues. </p> <p>For more information about setting up automatic reminders, see <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Set up automatic reminders</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Send Early Notifications</td> 
     <td> <p>Manually sends the automatic reminder notifications for&nbsp;tasks and issues that are approaching their due dates.</p> <p>For more information about setting up automatic reminders, see <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Set up automatic reminders</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Send Reminder Notifications</td> 
     <td> <p>Manually sends reminder notifications. </p> <p>For more information about setting up reminder notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Check All POP Accounts</td> 
     <td> <p>Checks for new emails that have been sent to POP accounts linked to <span>Workfront</span>. </p> <!--
       For more information about Workfront and POP account integrations, see and Overview of the Queue Details tab in a project.
      --> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Recalculate Timelines</td> 
     <td> <p>Recalculates the timeline for all projects in <span>Workfront</span> that are in a status of Current. </p> <p>For more information about calculating the timeline of projects automatically or manually, one project at a time, see<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Restore Default Customer Reports</td> 
     <td>Restores the default reports that were originally delivered with <span>Workfront</span>, so that they are visible in the <span class="bold">Reports</span> section for all&nbsp;users.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Generate Timesheets</td> 
     <td>Generates timesheets for users based on their recurring&nbsp;timesheet profiles. This option needs to be run only if the timesheet profile has been altered significantly after it has been assigned to users, and only after any current and future timesheets have been deleted.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

