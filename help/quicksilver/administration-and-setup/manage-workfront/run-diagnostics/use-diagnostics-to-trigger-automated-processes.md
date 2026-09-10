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
TQID: https://experienceleague.adobe.com/MPnQTGB88j8sZHuA6p6SVWI-1tDn7wi77GMsq0vX05c
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Use Diagnostics to trigger automated processes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

You can use Diagnostics to manually trigger automated processes, such as time-based scripts, recalculations, or email notifications.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>System Administrator</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Use diagnostics to trigger automated processes

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  

1. Expand **System**, then click **Diagnostics**.
1. Select from any of the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Send overdue notifications</td> 
      <td> <p>Manually sends the automatic reminder notifications for overdue tasks and issues. </p> <p>For more information about setting up automatic reminders, see <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Set up automatic reminders</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Send early notifications</td> 
      <td> <p>Manually sends the automatic reminder notifications for tasks and issues that are approaching their due dates.</p> <p>For more information about setting up automatic reminders, see <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Set up automatic reminders</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Send reminder notifications</td> 
      <td> <p>Manually sends reminder notifications. </p> <p>For more information about setting up reminder notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Check all POP accounts</td> 
      <td>Checks for new emails that have been sent to POP accounts linked to Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Recalculate timelines</td> 
      <td> <p>Recalculates the timeline for all projects in Workfront that are in a status of Current. </p> <p>For more information about calculating the timeline of projects automatically or manually, one project at a time, see <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Restore default customer reports</td> 
      <td>Restores the default reports that were originally delivered with Workfront, so that they are visible in the <strong>Reports</strong> section for all users.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Generate timesheets</td> 
      <td>Generates timesheets for users based on their recurring timesheet profiles. This option needs to be run only if the timesheet profile has been altered significantly after it has been assigned to users, and only after any current and future timesheets have been deleted.</td> 
     </tr> 
    </tbody> 
   </table>
