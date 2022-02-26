---
filename: timesheet-and-hour-preferences
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Configure timesheet and hour preferences
description: As an Adobe Workfront administrator, you can specify preferences for timesheets and hours in Workfront in order to define what items the timesheets can pre-populate with and what items users can log time to.
---

# Configure timesheet and hour preferences

As an *Adobe Workfront administrator*, you can specify preferences for timesheets and hours in *Workfront* in order to define what items the timesheets can pre-populate with and what items users can log time to.

Any changes you make to timesheets impact all timesheets that are created in the future.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Set timesheet and hour preferences

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Timesheet & Hours</span> > <span class="bold">Preferences</span>.</li> 
</ol>

<ol data-mc-continue="true"> 
 <li value="3"> <p>On the page that displays, in the <span class="bold">General Preferences</span> section, configure any of the following options: </p> <p> 
   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Log time for future dates</td> 
      <td> <p>Allows users to log time for future dates throughout the system in:</p> 
       <ul> 
        <li>Any projects, tasks, and issues where they have access to log time</li> 
        <li>Their timesheets as General Time</li> 
       </ul> <p>This is useful when users plan to be away from the office and want to log that time beforehand.</p> <note type="note">
        You cannot prevent users from logging time on tasks or issues that are closed or canceled. You can only prevent users from logging time on complete or dead projects. We recommend that you use filters in lists of tasks and issues to exclude&nbsp;the ones that have been completed or canceled from being visible to users.
       </note> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Add expenses from a timesheet</td> 
      <td> <p>Enables users to record both time and expenses in the timesheet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assign Job Roles to hour entries manually</td> 
      <td> <p>Allow users to manually select any Job Role assigned in their user profile or assigned to the object.</p> <note type="important"> 
        <ul> 
         <li>If you disable this setting after assigning job roles to hour entries, users must adjust hours logged under various roles on the Hours tab of the project, task, or issue.</li> 
         <li>If the user does not have a job role assigned in their profile and there is a task assigned as the Task Owner in the Advanced Assignments dialog box, that job role appears when the user logs time on the task.</li> 
        </ul> 
       </note> </td> 
     </tr> <draft-comment>
      <tr data-mc-conditions=""> 
       <td role="rowheader">Restrict timesheet editing to owners and admins</td> 
       <td> <p>Restrict editing to timesheet owners and <em>Workfront administrators</em>. When this option is disabled, timesheets can also be edited by:</p> 
        <ul> 
         <li> <p>Users with administrative access to timesheets and hours in their access level</p> </li> 
         <li> <p>Timesheet approvers if “Can edit hours” is enabled on the timesheet</p> </li> 
         <li> <p>The manager of the timesheet owner</p> </li> 
        </ul> </td> 
      </tr>
     </draft-comment>
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restrict timesheet editing to owners and admins</td> 
      <td> <p>Restrict editing to timesheet owners and <em>Workfront administrators</em>. When this option is disabled, timesheets can also be edited by:</p> 
       <ul> 
        <li> <p>Users with administrative access to timesheets and hours in their access level</p> </li> 
        <li> <p>Timesheet approvers if “Can edit hours” is enabled on the timesheet</p> </li> 
        <li> <p>The manager of the timesheet owner</p> </li> 
       </ul> </td> 
     </tr> <draft-comment>
      <tr data-mc-conditions=""> 
       <td role="rowheader">Restrict hour editing to owners and admins</td> 
       <td>Restrict editing to the user who input the hours and <em>Workfront administrators</em>. This setting applies to the Hours tab in a project or in an Hours report.</td> 
      </tr>
     </draft-comment>
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restrict hour editing to owners and admins</td> 
      <td>Restrict editing to the user who input the hours and <em>Workfront administrators</em>. This setting applies to the Hours tab in a project or in an Hours report.</td> 
     </tr> 
    </tbody> 
   </table> </p> </li> <draft-comment>
  <li value="4" data-mc-conditions="SnippetConditions-wf-groups.system-level"> <p>In the <span class="bold">Logging Time</span> section, configure any of the following options: </p> 
   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Log time directly on projects</td> 
      <td>Allows users to log time on the project (both on the Updates tab and timesheet). If users do not record&nbsp;time at the project level, this options should remain unchecked.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Log time on projects that are complete</td> 
      <td>Allows users to record time on a project that has been marked complete. If this option is disabled, users cannot record time for the work they have completed on projects in the Complete status.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Log time on projects that are dead</span> </td> 
      <td>When this option is enabled, users can log hours on projects with a Dead status.</td> 
     </tr> 
    </tbody> 
   </table> </li>
 </draft-comment>
 <li value="4" data-mc-conditions="SnippetConditions-wf-groups.system-level"> <p>In the <span class="bold">Logging Time</span> section, configure any of the following options: </p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Log time directly on projects</td> 
     <td>Allows users to log time on the project (both on the Updates tab and timesheet). If users do not record&nbsp;time at the project level, this options should remain unchecked.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Log time on projects that are complete</td> 
     <td>Allows users to record time on a project that has been marked complete. If this option is disabled, users cannot record time for the work they have completed on projects in the Complete status.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Log time on projects that are dead</span> </td> 
     <td>When this option is enabled, users can log hours on projects with a Dead status.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5"> <p>In the <span class="bold">Pre-Populate timesheets with&nbsp;</span>section, configure any of the following options: </p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Work that is within <number of weeks> of the timesheet's work range</td> 
     <td> <p>Defines the number of weeks before and after the date range&nbsp;of the timesheet that contains dates of tasks and issues assigned to the user. The default setting is 1 week, and you can extend this range to 4 weeks. This means that the timesheet is pre-populated with tasks and issues which have dates anywhere between four weeks before the date range of the timesheet up to four weeks after the date range of the timesheet, if you select 4 weeks for your range. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Tasks & Issues that have been completed</td> 
     <td>If multiple resources are typically assigned to a single task, we recommend this setting. This means when one resource records time against the task and marks it as complete, the other resources assigned to the task can still find the task or the issue in their timesheet, to record their hours.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Tasks & Issues that have Planned Dates in timesheet's date range</td> 
     <td> <p>When selected, the timesheet includes tasks and issues that have either a Planned Start Date or Completion Date that falls within the date range of the timesheet.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"> Tasks that have Projected Dates in timesheet's date range</td> 
     <td> <p>When selected, the timesheet includes tasks that have either a Projected Start Date or Completion Date that falls within the time frame of the project, even if the planned date of the issue or task falls outside of the timesheet date range.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> <draft-comment>
  <li value="6" data-mc-conditions="SnippetConditions-wf-groups.system-level"> <p>In the <span class="bold">Project, Task or Issue Deletion Preferences</span> section, specify the following:</p> 
   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">When deleting projects</td> 
      <td> 
       <ul> 
        <li><span class="bold">Keep logged time already added to timesheets as general time</span>: If this project is restored at a later time, the time remains on the timesheet.</li> 
        <li><span class="bold">Delete any logged time</span>: If this project is later restored, time already logged is restored to the project.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">When deleting tasks or issues</td> 
      <td> 
       <ul> 
        <li><span class="bold">Move any logged time to the project where the task or issue resides</span>: If this task or issue is later restored, the time remains on the project.<br></li> 
        <li> <p><span class="bold">Delete any logged time</span>: If this task or issue is later restored, logged time is restored to the task or issue.</p> <p>For more detailed information about these options, see <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">Configure affect on hours when an object is deleted and restored</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table> </li>
 </draft-comment>
 <li value="6" data-mc-conditions="SnippetConditions-wf-groups.system-level"> <p>In the <span class="bold">Project, Task or Issue Deletion Preferences</span> section, specify the following:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">When deleting projects</td> 
     <td> 
      <ul> 
       <li><span class="bold">Keep logged time already added to timesheets as general time</span>: If this project is restored at a later time, the time remains on the timesheet.</li> 
       <li><span class="bold">Delete any logged time</span>: If this project is later restored, time already logged is restored to the project.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">When deleting tasks or issues</td> 
     <td> 
      <ul> 
       <li><span class="bold">Move any logged time to the project where the task or issue resides</span>: If this task or issue is later restored, the time remains on the project.<br></li> 
       <li> <p><span class="bold">Delete any logged time</span>: If this task or issue is later restored, logged time is restored to the task or issue.</p> <p>For more detailed information about these options, see <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">Configure affect on hours when an object is deleted and restored</a>.</p> </li> 
      </ul> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="7"> <p>Click <span class="bold">Save</span>.</p> </li> 
</ol>

## Unlock timesheet and hour preferences for groups

Groups in your organization might need a timesheet or hour preference configured differently for their unique workflows. You can unlock the preference for all groups throughout the organization so that they can configure it on their own.

When a preference is unlocked and a *group administrator* modifies it, it affects timesheet owners if the group is their Home Group.

For information about how a *group administrator* configures timesheet and hour preferences for a group, see [Configure timesheet and hour preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>After a *Workfront administrator* unlocks a preference at the system level, any *group administrator* can configure it and then lock it to ensure that everyone in their group and the subgroups below is using the same configuration. This is parallel to the ability that a *Workfront administrator* has to configure and lock a preference for everyone in the system. For more information, see [Lock or unlock a group timesheet and hour preference](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

To unlock a project preference so that groups can configure it:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Timesheets & Hours</span>, then click <span class="bold">Preferences</span>.</li> 
 <li value="3"> <p>Do any of the following:</p> 
  <ul> 
   <li>If you want <em>group administrators</em> to be able to configure a preference for their groups, unlock it <img src="assets/unlock-toggle-button.png">.</li> 
   <li>If you want all groups to use your configuration for a preference, make sure that it is locked (this is the default).<note type="important">
     We recommend that you communicate with the administrators and users in groups throughout the system to ensure that all needs are accounted for in the way you configure a locked preference. When you lock it, your configuration for it is inherited by all groups in the system. And if the preference has been unlocked for any period of time, your configuration replaces those that 
     <em>group administrators</em> might have made.
    </note></li> 
  </ul> </li> 
 <li value="4">Click <span class="bold">Save</span>.</li> 
</ol>

