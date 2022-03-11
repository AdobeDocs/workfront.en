---
filename: set-task-issue-preferences
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configure system-wide task and issue preferences
description: As an Adobe Workfront administrator, you can configure system-wide preferences for tasks and issues. These preferences impact the way that your users create tasks and issues in Workfront.
---

# Configure system-wide task and issue preferences

As an `Adobe Workfront administrator`, you can configure system-wide preferences for tasks and issues. These preferences impact the way that your users create tasks and issues in `Workfront`.

By default, these preferences are locked and `group administrators` cannot modify them at the group level unless you unlock them for all groups throughout the system. For more information, see the section [Lock task and issue preferences for groups](#lock) in this article.

<!--
SPLIT OUT BOTTOM SECTION TO NEW ARTICLE?
-->

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure task and issues preferences for everyone in `Workfront`

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2">In the left panel, click <span class="bold">Project Preferences</span> ><span class="bold"> Tasks & Issues.</span></li> 
 <li value="3"> On the page that appears, continue with one of the 5 sections listed below to configure settings for New Task Defaults, Issues, Deletion, Actual Dates, and Access.</li> 
 <li value="4"> <p>Click <span class="bold">Save</span>.</p> </li> 
</ol>

* [New Task Defaults](#new-task-defaults) 
* [Issues](#issues) 
* [Deletion](#deletion) 
* [Actual Dates](#actual-dates)

  <!--
  Work On It
  -->

* [Access](#access)

### New Task Defaults

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Start Date on New Tasks</td> 
   <td> <p>Determines the default start date for new tasks for project managers. The start date for new tasks can either be the planned start date of the project or the day the task is created on.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Duration Type </p> </td> 
   <td> <p>Determines the relationship between the number of resources (and their allocation percent) and the duration or the total effort for the task. For more information, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Task Duration and Duration Types</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Revenue Type</td> 
   <td> <p>Calculates planned and actual revenue estimates for a task. When the <span class="bold">Revenue Type</span> is set to<span class="bold"> Not Billable</span>, the hours planned and the actual hours recorded do not generate a revenue estimate for the task, and the work on the task does not contribute to project-level revenue.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cost Type</td> 
   <td> <p>Calculates planned and actual cost estimates for a task. When set to <span class="bold">No Cost</span>, the hours planned and the actual hours recorded do not generate a planned or an actual cost estimate for the task, and the work on the task does not contribute to project-level costs.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Issues

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Automatically update Resolvable Issue status when the status of the Resolving Object changes</td> 
   <td> <p>When someone converts an issue into a project or task, both the original issue and the converted project or task become resolving objects. This setting lets you correlate the resolution of the original issue to the resolution of its resolvable object. For more information on resolving objects, see <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> <p>In order for this setting to have any effect, the option to <span class="bold">Keep the original issue and tie its resolution to the task</span> must be selected.</p> 
    <ul> 
     <li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li> 
     <li>When this setting is disabled, resolving&nbsp;object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Access the list of system issue statuses</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">When converting an issue to a task</td> 
   <td> <p>The settings in this section determine what happens during the conversion process from issue to task:</p> 
    <ul> 
     <li> <p><span class="bold">Keep the original issue and tie its resolution to the task</span>: When you are converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes. When this is deselected, the issue is deleted.</p> <p>Note:  <p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a> </p> </li> 
       </ul> </p> </li> 
     <li><span class="bold">Allow Primary Contact to have access to the task</span>: Gives the primary contact (issue creator)&nbsp;access to the task to review the task, make updates, and stay informed of its progress</li> 
     <li> <p><span class="bold">Allow these settings to be changed during conversion</span>: Allows the user who is converting the issue to change these options during the conversion of an issue to a task.</p> <!--
       Screenshot when possible
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">When converting an issue to a project</td> 
   <td> <p>The settings in this section determine what happens during the conversion process from issue to project:</p> 
    <ul> 
     <li> <p><span class="bold">Keep the original issue and tie its resolution to the project</span>: When you are converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project&nbsp;completes. When this is deselected, the issue is deleted. </p> <p>Note:  <p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a> </p> </li> 
       </ul> </p> </li> 
     <li><span class="bold">Allow Primary Contact to have access to the project</span>: Gives the primary contact (issue creator)&nbsp;access to the project to review the project, make updates, and stay informed of its progress.</li> 
     <li><span class="bold">Allow these settings to be changed during conversion</span>: Allows the user who is converting the issue to change the listed options during the conversion of an issue to a project.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Deletion

`Allow users to delete tasks & issues with logged hours`: Lets you determine whether you allow the deletion of tasks or issues where hours are logged. This option is selected by default.
Tip: This setting also applies to deleting projects that have tasks or issues with hours logged on them. This setting does not apply to deleting projects where time is logged directly for the project.

* When it is selected, you receive an informational warning when you delete a task or issue. The warning reminds you that if the task or issue has logged hours, they will either be moved to the project or deleted. You can configure whether the hours are deleted or moved to the project in the Timesheet & Hours Preferences area of the Setup. After you confirm that you have seen the warning, the task or issue is deleted. For more information about configuring Timesheet & Hours Preferences, see [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md). 
  Tip: When you delete a project with tasks and issues that have logged hours, the logged hours are either deleted or they are preserved according to the settings in the Timesheet & Hours Preferences area of Setup. The warning message does not display when deleting a project. 
* `When you deselect this option, you receive a prohibitive warning when you delete a task or issue with logged hours` , or when you delete a project with hours logged for its tasks or issues `.` The warning specifies that the administrator does not allow for tasks or issues with logged hours to be deleted. The tasks, issues, or projects that have hours logged for tasks and issues cannot be deleted.

### Actual Dates

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">When a task or issue goes from "New" to "In Progress," set the Actual Start Date to</td> 
   <td> <p>Select one of the following options for when the Actual Start Date is recorded in <span>Workfront</span> when a task or issue goes from <span class="bold">New</span> to <span class="bold">In Progress</span>:</p> 
    <ul> 
     <li><span class="bold">Now:</span> The Actual Start Date is set to the current date.</li> 
     <li><span class="bold">The Planned Start Date:</span> The Actual Start Date is set to the Planned Start Date of the task or issue.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">When a task or issue is completed, set the Actual Completion Date to</td> 
   <td> <p>Select one of the following options for when the Actual Completion Date is&nbsp;recorded in <span>Workfront</span> when a task or issue is completed:</p> 
    <ul> 
     <li><span class="bold">Now:</span> The Actual Completion Date is set to the current date.</li> 
     <li> <p><span class="bold">The Planned Completion Date:</span> The Actual Completion Date is set to&nbsp;the Planned Completion Date of the task or issue.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
Work On It You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work. Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date. To switch to the Start button: Select Change the Work On It button to a Start button to automatically update the status of an item. In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. Note: Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button. If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status. This setting is not currently available in The Workfront Mobile App Workfront for Office 365 Workfront email notifications This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level. If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
-->

### Access

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">When someone is assigned to a task</td> 
   <td> 
    <ul> 
     <li><span class="bold">Give them ... access to a task</span>: Defines the default permission a user has to the task they are assigned to. For more information about task permissions, see<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</li> 
     <li> <p><span class="bold">Also grant them ... access to the project</span>: Defines the default permission a user has to the project on which they have a task assigned to them. For more information about project permissions, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">When someone is assigned to an issue</td> 
   <td> 
    <ul> 
     <li><span class="bold">Give them ... access to a task</span>: Defines the default permission a user has to the task they are assigned to. For more information about task permissions, see<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</li> 
     <li> <p><span class="bold">Also grant them ... access to the project</span>: Defines the default permission a user has to the project on which they have a task assigned to them. For more information about project permissions, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">When someone submits a request</td> 
   <td> 
    <ul> 
     <li><span class="bold">Give them ... access to the issue</span>: Defines the default permission a user has on a request they submitted. For more information, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a>.</li> 
     <li> <p><span class="bold">People from the same company will inherit the same permissions for all requests</span>: Allows users to see requests submitted by other users from the same company as them. They have the same permissions on those requests as they have on their own submitted requests.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Lock task and issue preferences for groups

If groups in your organization need a task or issue preference configured differently for their unique workflows, you can unlock the preference for all groups throughout the organization so that they can configure it on their own. When a preference is unlocked and the `group administrator` modifies it, the tasks or issues associated with the group are affected by the group-level setting for the preference instead of the system-level setting.

For information about how a `group administrator` configures task and issue preferences for a group, see [Configure task and issue preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>After a `Workfront administrator` unlocks a preference at the system level, any `group administrator` can configure it and then lock it to ensure that everyone in their group and the subgroups below is using the same configuration. This is parallel to the ability that a `Workfront administrator` has to configure and lock a preference for everyone in the system. For more information, see [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) and [Lock or unlock a project, task, or issue preference for subgroups](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

To lock or unlock a task or issue preference so that groups can configure it

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Project Preferences</span> > <span class="bold">Tasks & Issues</span>.</li> 
 <li value="3"> <p>Do any of the following:</p> 
  <ul> 
   <li> <p>If you want administrators of groups below your group to be able to configure a preference for their groups, unlock it <img src="assets/unlock-toggle-button.png">.</p> </li> 
   <li> <p>If you want your group and all groups below it to use your configuration for a preference, make sure that it is locked (this is the default).</p> <note type="important">
     We recommend that you communicate with the administrators and users in groups throughout the system to ensure that all needs are accounted for in the way you configure a locked preference. When you lock it, your configuration for it is inherited by all groups in the system. And if the preference has been unlocked for any period of time, your configuration replaces those that 
     <span>group administrators</span> might have made.
    </note> </li> 
  </ul> </li> 
 <li value="4">Click <span class="bold">Save</span>.</li> 
</ol>

