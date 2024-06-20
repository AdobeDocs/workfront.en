---
user-type: administrator
product-area: system-administration;user-management
keywords: group,preferences,task,groups,issue,unlock
navigation-topic: create-and-manage-groups
title: Configure timesheet and hour preferences for a group
description: At the system level, an Adobe Workfront administrator can unlock the timesheet and hour preference sections General Preferences and Pre-Populate timesheets with. This allows group administrators to configure the options in those sections independently for their own groups.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
---
# Configure timesheet and hour preferences for a group

An Adobe Workfront administrator can unlock the following sections of timesheet and hour preferences at the system level so that group administrators can configure them independently for their own groups:

* General preferences
* Where users can log time
* Pre-Populate timesheets

If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).

The following sections on the Timesheet and Hours Preferences page are configurable only at the system level and can't be unlocked for groups:

* Deleted projects, tasks, and issues

For information about how a Workfront administrator unlocks a timesheet and hour preference, see the section [Unlock timesheet and hour preferences for groups](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) in the article [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>Group-level configuration is also possible for project preferences and for task and issue preferences. For information, see [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) and [Configure task and issue preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

+++

## Group timesheet and hour preferences

Consider the following information about configuring an unlocked timesheet or hour preference for a group:

* If you are a group administrator and you configure a timesheet or hour preference for your group, it affects people who use the group as their Home Group.
* Typically, an unlocked preference remains unlocked indefinitely. If the Workfront administrator re-locks it, the system setting takes effect again and settings for the preference made by the group administrators are lost.
* A timesheet inherits the timesheet and hour preferences configured for the timesheet owner's Home Group. 

  <!--
  Add example here?
  -->

* After a Workfront administrator unlocks a preference at the system level and you configure it for your group, you can then lock it to ensure that everyone in the groups below yours is using the same configuration. This is parallel to the ability that a Workfront administrator has to configure and lock a preference for everyone in the system. For more information, see [Lock or unlock a group timesheet and hour preference](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Configure an unlocked timesheet or hour preference for a group

>[!TIP]
>
>If you are a Workfront administrator, you can bypass steps 1-4 by going to Setup > Timesheet & Hours > Preferences, then searching for the group's name in the box at the top of the page.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **Groups** ![](assets/groups-icon.png).

1. Click the name of the group whose timesheet or hour preferences you want to configure.
1. In the left panel, click **Timesheets & Hours**.

1. On the page that displays, in the **General preferences** section, configure any of the following options:

   >[!TIP]
   >
   >If you hover over a preference and a tool tip displays to tell you that it is locked, you can ask your Workfront administrator to unlock it for all groups in the organization.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Log time for future dates</td> 
      <td> <p>Allows users to log time for future dates throughout the system in:</p> 
       <ul> 
       <li>Any projects, tasks, and issues where they have access to log time, regardless of project's group</li> 
       <li>Their timesheets as General Time</li>
       </ul> 
       <p>This is useful when users plan to be away from the office and want to log that time beforehand.</p> 
       <p><b>NOTE</b>: You cannot prevent users from logging time on tasks or issues that are closed or canceled. You can only prevent users from logging time on complete or dead projects. We recommend that you use filters in lists of tasks and issues to exclude the ones that have been completed or canceled from being visible to users.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Add expenses from a timesheet</td> 
      <td> <p>Enables users to record both time and expenses in the timesheet.</p> 
      <p>When this preference is enabled for a group and the group is set as the home group for certain users, an expense icon displays next to projects and tasks on those users' timesheets. The users can click this icon to add or edit expenses for the project or task.</p>
      </td> 
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
      <td> <p>Restrict editing to timesheet owners, regardless of project's group and Workfront administrators. When this option is disabled, timesheets can also be edited by:</p> 
       <ul> 
        <li> <p>Users with administrative access to timesheets and hours in their access level</p> </li> 
        <li> <p>Timesheet approvers if "Can edit hours" is enabled on the timesheet</p> </li> 
        <li> <p>The manager of the timesheet owner</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restrict hour editing to owners and admins</td> 
      <td>Restrict editing to the user who input the hours and Workfront administrators. This setting applies to the Hours tab in a project or in an Hours report.</td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Where users can log time** section, configure any of the following options:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Log time directly on projects</td> 
      <td>Allows users to log time on the project (both on the Updates tab and timesheet). If you want to restrict your users from recording time at the project level, leave this option unchecked.</td>
     </tr>
     <tr>
      <td role="rowheader">Log time on projects that are complete</td>
      <td>Allows users to record time on a project that has been marked complete. If this option is disabled, users cannot record time for the work they have completed on projects in the Complete status.</td>
     </tr>
     <tr>
      <td role="rowheader">Log time on projects that are dead</td> 
      <td>When this option is enabled, users can log hours on projects with a Dead status.</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >This preference is applied based on configuration of the user's Home Group preferences. If these settings are enabled in the user's Home Group preferences, they will be able to log time directly on projects, including completed or dead projects, regardless of whether the project's group preferences allow it or not.

1. In the **Pre-Populate timesheets** section, configure any of the following options: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Work that is within &lt;number of weeks&gt; of the timesheet's work range</td> 
      <td> <p>Defines the number of weeks before and after the date range of the timesheet that contains dates of tasks and issues assigned to the user. The default setting is 1 week, and you can extend this range to 4 weeks. This means that the timesheet is pre-populated with tasks and issues which have dates anywhere between four weeks before the date range of the timesheet up to four weeks after the date range of the timesheet, if you select 4 weeks for your range. </p> </td> 
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

1. Click **Save**.
