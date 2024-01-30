---
title: Configure task and issue preferences for a group
user-type: administrator
product-area: system-administration;user-management;setup
keywords: group,preferences,task,issue,unlock
navigation-topic: create-and-manage-groups
description: If groups in your organization need to configure a task or issue preference independently from the way it is configured at the system level, an Adobe Workfront administrator can unlock the preference. Then, as a group administrator, you can configure the preference for your group and it will affect all tasks or issues associated with your group.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
---
# Configure task and issue preferences for a group

If groups in your organization need to configure a task or issue preference independently from the way it is configured at the system level, an Adobe Workfront administrator can unlock the preference. Then, as a group administrator, you can configure the preference for your group and it will affect all tasks or issues associated with your group.

If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for Workfront administrators (for any group).

For information about how the Workfront administrator unlocks preferences, see [Lock or unlock project preferences for all groups in the system](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>Group-level configuration is also possible for project preferences. For information, see [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* Typically, an unlocked preference remains unlocked indefinitely. If the Workfront administrator re-locks it, the system setting takes effect again and settings for the preference made by the group administrators are lost.
>* The preferences set for the group that is associated with a project take precedence over the preferences set for the Home Group of the user who creates the project.
>* Some group-level preferences affect project templates that you create for the group. For more information, see the section [View, work with, and create templates for your group from the Groups area](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) in the article [Create and modify a group's project templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* After a Workfront administrator unlocks a preference at the system level, you can configure it and then lock it to ensure that everyone in your group and in its subgroups is using the same configuration. This is parallel to the ability that a Workfront administrator has to configure and lock a preference for everyone in the system. For more information, see [Lock or unlock a project, task, or issue preference for subgroups](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

## Access requirements

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

## Configure unlocked task and issue preferences for a top-level group

>[!TIP]
>
>If you are a Workfront administrator, you can bypass steps 1-4 by going to Setup > Project Preferences > Tasks & Issues, then searching for the group's name in the box at the top of the page.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **Groups** ![](assets/groups-icon.png).

1. Click the name of the group for which you want to configure unlocked task and issue preferences.
1. On the page that displays for the group, in the left panel, click **Task & Issue Preferences**.
1. On the page that appears, continue with one of the 5 sections listed below these steps to configure settings for the areas New Task Defaults, Issues, Deletion, Actual Dates, and Access, then click **Save**.

   If you hover over the lock icon ![](assets/lock-toggle-button-dimmed.png) for a preference that you need to configure and a tool tip displays to tell you that is locked, you can ask your Workfront administrator to unlock it for all groups in the organization.

   When it is unlocked, you and other group administrators can configure it separately for your own groups. Also, you can lock it for your group and any subgroups below your group.

   * [New Task Defaults](#new-task-defaults) 
   * [Issues](#issues) 
   * [Deletion](#deletion) 
   * [Actual Dates](#actual-dates)

     <!--   
     <li><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>   
     -->   
   
   * [Access](#access)

### New Task Defaults {#new-task-defaults}

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Start Date on New Tasks</td> 
      <td> <p>Determines the default start date for new tasks for project managers. The start date for new tasks can either be the planned start date of the project or the day the task is created on.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Duration Type </p> </td> 
      <td> <p>Determines the relationship between the number of resources (and their allocation percent) and the duration or the total effort for the task. For more information, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Task Duration and Duration Types: article index</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenue Type</td> 
      <td> <p>Calculates planned and actual revenue estimates for a task. When the <strong>Revenue Type</strong> is set to<strong>Not Billable</strong>, the hours planned and the actual hours recorded do not generate a revenue estimate for the task, and the work on the task does not contribute to project-level revenue.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cost Type</td> 
      <td> <p>Calculates planned and actual cost estimates for a task. When set to <strong>No Cost</strong>, the hours planned and the actual hours recorded do not generate a planned or an actual cost estimate for the task, and the work on the task does not contribute to project-level costs.</p> </td> 
     </tr> 
    </tbody> 
   </table>

### Issues {#issues}

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Automatically update Resolvable Issue status when the status of the Resolving Object changes</td> 
      <td> <p>When someone converts an issue into a project or task, both the original issue and the converted project or task become resolving objects. This setting lets you correlate the resolution of the original issue to the resolution of its resolvable object. For more information on resolving objects, see <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> <p>In order for this setting to have any effect, the option to <strong>Keep the original issue and tie its resolution to the task</strong> must be selected.</p> 
       <ul> 
        <li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li> 
        <li>When this setting is disabled, resolving object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Access the list of system issue statuses</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">When converting an issue to a task</td> 
      <td> <p>The settings in this section determine what happens during the conversion process from issue to task:</p> 
       <ul> 
        <li><strong>Keep the original issue and tie its resolution to the task</strong>: When you are converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes.</li> 
        <li><strong>Allow Primary Contact to have access to the task</strong>: Gives the primary contact (issue creator) access to the task to review the task, make updates, and stay informed of its progress</li> 
        <li> <p><strong>Allow these settings to be changed during conversion</strong>: Allows the user who is converting the issue to change these options during the conversion of an issue to a task.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">When converting an issue to a project</td> 
      <td> <p>The settings in this section determine what happens during the conversion process from issue to project:</p> 
       <ul> 
        <li><strong>Keep the original issue and tie its resolution to the project</strong>: When you are converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project completes.</li> 
        <li><strong>Allow Primary Contact to have access to the project</strong>: Gives the primary contact (issue creator) access to the project to review the project, make updates, and stay informed of its progress.</li> 
        <li><strong>Allow these settings to be changed during conversion</strong>: Allows the user who is converting the issue to change the listed options during the conversion of an issue to a project.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Deletion {#deletion}

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Allow users to delete tasks &amp; issues with logged hours</td> 
      <td> <p> Lets you determine whether you allow the deletion of tasks or issues where hours are logged. This option is selected by default.</p> 
       <div> 
        <p><b>Tip</b>: This setting also applies to deleting projects that have tasks or issues with hours logged on them. This setting does not apply to deleting projects where time is logged directly for the project. </p> 
        <p>Consider the following:</p> 
        <ul> 
         <li> <p>When it is selected, you receive an informational warning when you delete a task or issue. The warning reminds you that if the task or issue has logged hours, they will either be moved to the project or deleted. You can configure whether the hours are deleted or moved to the project in the Timesheet &amp; Hours Preferences area of the Setup. After you confirm that you have seen the warning, the task or issue is deleted. For more information about configuring Timesheet &amp; Hours Preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>. </p> <p>Tip: <span>When you delete a project with tasks and issues that have logged hours, the logged hours are either deleted or they are preserved according to the settings in the Timesheet &amp; Hours Preferences area of Setup</span>. </p> </li> 
         <li><span>When you deselect this option, you receive a prohibitive warning when you delete a task or issue with logged hours, or when you delete a project with hours logged for its tasks or issues</span> <span>.</span> The warning specifies that the administrator does not allow for tasks or issues with logged hours to be deleted. The tasks, issues<span>, or projects that have hours logged for tasks and issues</span> cannot be deleted. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

### Actual Dates {#actual-dates}

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">When a task or issue goes from "New" to "In Progress," set the Actual Start Date to</td> 
      <td> <p>Select one of the following options for when the Actual Start Date is recorded in Workfront when a task or issue goes from <strong>New</strong> to <strong>In Progress</strong>:</p> 
       <ul> 
        <li><strong>Now:</strong> The Actual Start Date is set to the current date.</li> 
        <li><strong>The Planned Start Date:</strong> The Actual Start Date is set to the Planned Start Date of the task or issue.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">When a task or issue is completed, set the Actual Completion Date to</td> 
      <td> <p>Select one of the following options for when the Actual Completion Date is recorded in Workfront when a task or issue is completed:</p> 
       <ul> 
        <li><strong>Now:</strong> The Actual Completion Date is set to the current date.</li> 
        <li> <p><strong>The Planned Completion Date:</strong> The Actual Completion Date is set to the Planned Completion Date of the task or issue.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   <!--
   This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it. Here's what Jeremy Flores says on 12/1/20:
   
   I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.
   You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.
   Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.

   To switch to the Start button:
   
   Select Change the Work On It button to a Start button to automatically update the status of an item. 
   In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. 
     
   Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.
   If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.
   This setting is not currently available in
   
   The Workfront Mobile App
   Workfront for Office 365
   Workfront email notifications
   
   This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.
   If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
   -->

### Access {#access}

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">When someone is assigned to a task</td> 
      <td> 
       <ul> 
        <li><strong>Give them ... access to a task</strong>: Defines the default permission a user has to the task they are assigned to. For more information about task permissions, see<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Grant access to users</a>.</li> 
        <li> <p><strong>Also grant them ... access to the project</strong>: Defines the default permission a user has to the project on which they have a task assigned to them. For more information about project permissions, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">When someone is assigned to an issue</td> 
      <td> 
       <ul> 
        <li><strong>Give them ... access to a task</strong>: Defines the default permission a user has to the task they are assigned to. For more information about task permissions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</li> 
        <li> <p><strong>Also grant them ... access to the project</strong>: Defines the default permission a user has to the project on which they have a task assigned to them. For more information about project permissions, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">When someone submits a request</td> 
      <td> 
       <ul> 
        <li><strong>Give them ... access to the issue</strong>: Defines the default permission a user has on a request they submitted. For more information, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue</a>.</li> 
        <li> <p><strong>People from the same company will inherit the same permissions for all requests</strong>: Allows users to see requests submitted by other users from the same company as them. They have the same permissions on those requests as they have on their own submitted requests.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
