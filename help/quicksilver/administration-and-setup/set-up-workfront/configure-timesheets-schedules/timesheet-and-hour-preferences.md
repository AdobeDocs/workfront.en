---
filename: timesheet-and-hour-preferences
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Configure timesheet and hour preferences
description: Configure timesheet and hour preferences
---

# Configure timesheet and hour preferences

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

As an Adobe Workfront administrator, you can specify preferences for timesheets and hours in Workfront in order to define what items the timesheets can pre-populate with and what items users can log time to.

Any changes you make to timesheets impact all timesheets that are created in the future.

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Set timesheet and hour preferences

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Timesheet & Hours** > **Preferences**.

1. On the page that displays, in the **General Preferences** section, configure any of the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Log time for future dates</td> 
      <td> <p>Allows users to log time for future dates throughout the system in:</p> 
       <ul> 
        <li>Any projects, tasks, and issues where they have access to log time</li> 
        <li>Their timesheets as General Time</li> 
       </ul> <p>This is useful when users plan to be away from the office and want to log that time beforehand.</p> <p><b>NOTE</b>: You cannot prevent users from logging time on tasks or issues that are closed or canceled. You can only prevent users from logging time on complete or dead projects. We recommend that you use filters in lists of tasks and issues to exclude&nbsp;the ones that have been completed or canceled from being visible to users.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Add expenses from a timesheet</td> 
      <td> <p>Enables users to record both time and expenses in the timesheet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assign Job Roles to hour entries manually</td> 
      <td> <p>Allow users to manually select any Job Role assigned in their user profile or assigned to the object.</p> <p><b>IMPORTANT</b>:  
        <ul> 
         <li>If you disable this setting after assigning job roles to hour entries, users must adjust hours logged under various roles on the Hours tab of the project, task, or issue.</li> 
         <li>If the user does not have a job role assigned in their profile and there is a task assigned as the Task Owner in the Advanced Assignments dialog box, that job role appears when the user logs time on the task.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restrict timesheet editing to owners and admins</td> 
      <td> <p>Restrict editing to timesheet owners and Workfront administrators. When this option is disabled, timesheets can also be edited by:</p> 
       <ul> 
        <li> <p>Users with administrative access to timesheets and hours in their access level</p> </li> 
        <li> <p>Timesheet approvers if “Can edit hours” is enabled on the timesheet</p> </li> 
        <li> <p>The manager of the timesheet owner</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restrict hour editing to owners and admins</td> 
      <td>Restrict editing to the user who input the hours and Workfront administrators. This setting applies to the Hours tab in a project or in an Hours report.</td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Logging Time** section, configure any of the following options: 

   <table>
    <tr>
        <td>Log time directly on projects</td>
        <td>Allows users to log time on the project (both on the Updates tab and timesheet). If users do not record time at the project level, this options should remain unchecked.</td>
    </tr>
    <tr>
        <td>Log time on projects that are complete</td>
        <td>Allows users to record time on a project that has been marked complete. If this option is disabled, users cannot record time for the work they have completed on projects in the Complete status.</td>
    </tr>
    <tr>
        <td>Log time on projects that are dead</td>
        <td>When this option is enabled, users can log hours on projects with a Dead status.</td>
    </tr>
   </table>

1. In the **Pre-Populate timesheets with**section, configure any of the following options: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Work that is within &lt;number of weeks&gt; of the timesheet's work range</td> 
      <td> <p>Defines the number of weeks before and after the date range&nbsp;of the timesheet that contains dates of tasks and issues assigned to the user. The default setting is 1 week, and you can extend this range to 4 weeks. This means that the timesheet is pre-populated with tasks and issues which have dates anywhere between four weeks before the date range of the timesheet up to four weeks after the date range of the timesheet, if you select 4 weeks for your range. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tasks &amp; Issues that have been completed</td> 
      <td>If multiple resources are typically assigned to a single task, we recommend this setting. This means when one resource records time against the task and marks it as complete, the other resources assigned to the task can still find the task or the issue in their timesheet, to record their hours.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tasks &amp; Issues that have Planned Dates in timesheet's date range</td> 
      <td> <p>When selected, the timesheet includes tasks and issues that have either a Planned Start Date or Completion Date that falls within the date range of the timesheet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Tasks that have Projected Dates in timesheet's date range</td> 
      <td> <p>When selected, the timesheet includes tasks that have either a Projected Start Date or Completion Date that falls within the time frame of the project, even if the planned date of the issue or task falls outside of the timesheet date range.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Project, Task or Issue Deletion Preferences** section, specify the following:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Better title would be Deleting projects, tasks, and issues</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">When deleting projects</td> 
      <td> 
       <ul> 
        <li><strong>Keep logged time already added to timesheets as general time</strong>: If this project is restored at a later time, the time remains on the timesheet.</li> 
        <li><strong>Delete any logged time</strong>: If this project is later restored, time already logged is restored to the project.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">When deleting tasks or issues</td> 
      <td> 
       <ul> 
        <li><strong>Move any logged time to the project where the task or issue resides</strong>: If this task or issue is later restored, the time remains on the project.<br></li> 
        <li> <p><strong>Delete any logged time</strong>: If this task or issue is later restored, logged time is restored to the task or issue.</p> <p>For more detailed information about these options, see <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">Configure affect on hours when an object is deleted and restored</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.

## Unlock timesheet and hour preferences for groups

Groups in your organization might need a timesheet or hour preference configured differently for their unique workflows. You can unlock the preference for all groups throughout the organization so that they can configure it on their own.

When a preference is unlocked and a group administrator modifies it, it affects timesheet owners if the group is their Home Group.

For information about how a group administrator configures timesheet and hour preferences for a group, see [Configure timesheet and hour preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>After a Workfront administrator unlocks a preference at the system level, any group administrator can configure it and then lock it to ensure that everyone in their group and the subgroups below is using the same configuration. This is parallel to the ability that a Workfront administrator has to configure and lock a preference for everyone in the system. For more information, see [Lock or unlock a group timesheet and hour preference](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

To unlock a project preference so that groups can configure it:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **Timesheets & Hours**, then click **Preferences**.

1. Do any of the following:

   * If you want group administrators to be able to configure a preference for their groups, unlock it ![](assets/unlock-toggle-button.png).
   * If you want all groups to use your configuration for a preference, make sure that it is locked (this is the default).   
   
     >[!IMPORTANT]
     >
     >We recommend that you communicate with the administrators and users in groups throughout the system to ensure that all needs are accounted for in the way you configure a locked preference. When you lock it, your configuration for it is inherited by all groups in the system. And if the preference has been unlocked for any period of time, your configuration replaces those that group administrators might have made.

1. Click **Save**.

