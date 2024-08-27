---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Use Diagnostics to trigger automated processes
description: You can use Diagnostics to manually trigger automated processes, such as time-based scripts, recalculations, or email notifications.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
---
# Use Diagnostics to trigger automated processes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

You can use Diagnostics to manually trigger automated processes, such as time-based scripts, recalculations, or email notifications.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Use diagnostics to trigger automated processes

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  

1. Expand **System**, then click **Diagnostics**.
1. Select from any of the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Send Overdue Notifications</td> 
      <td> <p>Manually sends the automatic reminder notifications for overdue tasks and issues. </p> <p>For more information about setting up automatic reminders, see <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Set up automatic reminders</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Send Early Notifications</td> 
      <td> <p>Manually sends the automatic reminder notifications for tasks and issues that are approaching their due dates.</p> <p>For more information about setting up automatic reminders, see <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Set up automatic reminders</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Send Reminder Notifications</td> 
      <td> <p>Manually sends reminder notifications. </p> <p>For more information about setting up reminder notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Check All POP Accounts</td> 
      <td> <p>Checks for new emails that have been sent to POP accounts linked to Workfront. </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Recalculate Timelines</td> 
      <td> <p>Recalculates the timeline for all projects in Workfront that are in a status of Current. </p> <p>For more information about calculating the timeline of projects automatically or manually, one project at a time, see <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Restore Default Customer Reports</td> 
      <td>Restores the default reports that were originally delivered with Workfront, so that they are visible in the <strong>Reports</strong> section for all users.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Generate Timesheets</td> 
      <td>Generates timesheets for users based on their recurring timesheet profiles. This option needs to be run only if the timesheet profile has been altered significantly after it has been assigned to users, and only after any current and future timesheets have been deleted.</td> 
     </tr> 
    </tbody> 
   </table>
