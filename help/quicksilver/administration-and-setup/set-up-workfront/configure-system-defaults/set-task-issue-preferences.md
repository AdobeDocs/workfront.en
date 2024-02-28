---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configure system-wide task and issue preferences
description: You can configure system-wide preferences for tasks and issues. These preferences impact the way that your users create tasks and issues in Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
---
# Configure system-wide task and issue preferences

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

As an [!DNL Adobe Workfront] administrator, you can configure system-wide preferences for tasks and issues. These preferences impact the way that your users create tasks and issues in [!DNL Workfront].

By default, task and issue preferences are locked and group administrators cannot modify them at the group level unless you unlock them for all groups throughout the system. For more information, see the section [Lock task and issue preferences for groups](#lock-task-and-issue-preferences-for-groups) in this article.


## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   or
   <p>Current: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a [!DNL Workfront] administrator.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Configure task and issues preferences for everyone in [!DNL Workfront]

{{step-1-to-setup}}

1. In the left panel, click **[!UICONTROL Project Preferences]** >**[!UICONTROL Tasks & Issues].**

1. On the page that appears, continue with one of the 5 sections listed below to configure settings for [!UICONTROL New Task Defaults], [!UICONTROL Issues], [!UICONTROL Deletion], [!UICONTROL Actual Dates], and [!UICONTROL Access]:

    * [[!UICONTROL New Task Defaults]](#new-task-defaults)
    * [[!UICONTROL Issues]](#issues)
    * [[!UICONTROL Deletion]](#deletion)
    * [[!UICONTROL Actual Dates]](#actual-dates)
    * [[!UICONTROL Delegation]](#delegation)

   <!--
  <li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>
  -->

* [[!UICONTROL Access]](#access)

### [!UICONTROL New Task Defaults] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Start Date]</td> 
    <td> <p>Determines the default start date for new tasks for project managers. The start date for new tasks can either be the planned start date of the project or the day the task is created on.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[!UICONTROL Duration Type] </p> </td> 
    <td> <p>Determines the relationship between the number of resources (and their allocation percent) and the duration or the total effort for the task. For more information, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Task Duration and Duration Types</a></p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Revenue Type]</td> 
    <td> <p>Calculates planned and actual revenue estimates for a task. When the <strong>[!UICONTROL Revenue Type]</strong> is set to <strong>[!UICONTROL Not Billable]</strong>, the hours planned and the actual hours recorded do not generate a revenue estimate for the task, and the work on the task does not contribute to project-level revenue.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Cost Type]</td> 
    <td> <p>Calculates planned and actual cost estimates for a task. When set to <strong>[!UICONTROL No Cost]</strong>, the hours planned and the actual hours recorded do not generate a planned or an actual cost estimate for the task, and the work on the task does not contribute to project-level costs.</p> </td> 
    </tr> 
  </tbody> 
</table>

### Issues {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Automatically update Resolvable Issue status when the status of the Resolving Object changes]</td> 
    <td> <p>When someone converts an issue into a project or task, both the original issue and the converted project or task become resolving objects. This setting lets you correlate the resolution of the original issue to the resolution of its resolvable object. For more information on resolving objects, see <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> <p>In order for this setting to have any effect, the option to <strong>[!UICONTROL Keep the original issue and tie its resolution to the task]</strong> must be selected.</p> 
      <ul> 
      <li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li> 
      <li>When this setting is disabled, resolving object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Access the list of system issue statuses</a>.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"[!UICONTROL >When converting an issue to a task]</td> 
    <td> <p>The settings in this section determine what happens during the conversion process from issue to task:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Keep the original issue and tie its resolution to the task]</strong>: When you are converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to [!UICONTROL Closed] when the task completes. When this is deselected, the issue is deleted.</p> <p><b>NOTE</b>:  <p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Allow Primary Contact to have access to the task]</strong>: Gives the primary contact (issue creator) View access to the task to review the task, stay informed of its progress, and make comments on the Updates section of the task.</li> 
      <li> <p><strong>[!UICONTROL Allow these settings to be changed during conversion]</strong>: Allows the user who is converting the issue to change these options during the conversion of an issue to a task.</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When converting an issue to a project]</td> 
    <td> <p>The settings in this section determine what happens during the conversion process from issue to project:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Keep the original issue and tie its resolution to the project]</strong>: When you are converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to [!UICONTROL Closed] when the project completes. When this is deselected, the issue is deleted. </p> <p><b>NOTE</b>:  <p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Allow Primary Contact to have access to the project]</strong>: Gives the primary contact (issue creator) View access to the project to review the project, stay informed of its progress, and make comments on the Updates section of the project.</li> 
      <li><strong>[!UICONTROL Allow these settings to be changed during conversion]</strong>: Allows the user who is converting the issue to change the listed options during the conversion of an issue to a project.</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL Deletion] {#deletion}

**[!UICONTROL Allow users to delete tasks & issues with logged hours]**: Lets you determine whether you allow the deletion of tasks or issues where hours are logged. This option is selected by default.

  >[!TIP]
  >
  >This setting also applies to deleting projects that have tasks or issues with hours logged on them. This setting does not apply to deleting projects where time is logged directly for the project.

* When it is selected, you receive an informational warning when you delete a task or issue. The warning reminds you that if the task or issue has logged hours, they will either be moved to the project or deleted. You can configure whether the hours are deleted or moved to the project in the [!UICONTROL Timesheet & Hours Preferences] area of the [!UICONTROL Setup]. After you confirm that you have seen the warning, the task or issue is deleted. For more information about configuring Timesheet & Hours Preferences, see [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

    >[!TIP]
    >
    >When you delete a project with tasks and issues that have logged hours, the logged hours are either deleted or they are preserved according to the settings in the [!UICONTROL Timesheet & Hours Preferences] area of [!UICONTROL Setup]. The warning message does not display when deleting a project.

* When you deselect this option, you receive a prohibitive warning when you delete a task or issue with logged hours, or when you delete a project with hours logged for its tasks or issues. The warning specifies that the administrator does not allow for tasks or issues with logged hours to be deleted. The tasks, issues , or projects that have hours logged for tasks and issues cannot be deleted.

### [!UICONTROL Actual Dates] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL When a task or issue goes from "New" to "In Progress," set the Actual Start Date to]</td> 
    <td> <p>Select one of the following options for when the Actual Start Date is recorded in [!DNL Workfront] when a task or issue goes from <strong>[!UICONTROL New]</strong> to <strong>[!UICONTROL In Progress]</strong>:</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> The Actual Start Date is set to the current date.</li> 
      <li><strong>[!UICONTROL The Planned Start Date]:</strong> The Actual Start Date is set to the Planned Start Date of the task or issue.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When a task or issue is completed, set the Actual Completion Date to]</td> 
    <td> <p>Select one of the following options for when the Actual Completion Date is recorded in [!DNL Workfront] when a task or issue is completed:</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> The Actual Completion Date is set to the current date.</li> 
      <li> <p><strong>[!UICONTROL The Planned Completion Date]:</strong> The Actual Completion Date is set to the Planned Completion Date of the task or issue.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### Delegation

Enabling the **[!UICONTROL Allow users to delegate their tasks & issues]** setting allows all users in  to temporarily delegate their work to others.

When this setting is enabled, users can see the following:

* The [!UICONTROL Delegate] link in their [!UICONTROL Home] area. They can delegate approvals, or task and issue assignments from here.
* An indication that a task or issue is delegated to another user in the [!UICONTROL Assignments and delegations] area in the task or issue header.

  If you disable the [!UICONTROL Allow users to delegate their tasks & issues] setting, the delegations that are currently scheduled will stop and the users delegated will receive an email notification that the delegation was stopped.

For information about delegating work to others, see the following articles:

* [Delegate work overview](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Manage task and issue delegation](../../../manage-work/delegate-work/how-to-delegate-work.md)

<!--
<p><strong>Work On It</strong></p>
This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it.</p>
Here's what Jeremy Flores says on 12/1/20:</p>
I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.</p>
<p>You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.</p>
<p>Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.</p>
<p>To switch to the Start button:</p>
<ol>
<li value="1"> <p>Select <strong>Change the Work On It button to a Start button to automatically update the status of an item</strong>.</p> </li>
<li value="2"> <p>In the lists of check boxes that display below this option, select one or more statuses for each work item type.</p> <p>With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item.</p> </li>
</ol> <note type="note">
<ul class="preview">
<li>Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.</li>
<li>If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.</li>
<li>This setting is not currently available in
<ul>
<li>The Workfront Mobile App</li>
<li>Workfront for Office 365</li>
<li>Workfront email notifications</li>
</ul></li>
<li>This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.</li>
<li>If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.</li>
</ul>
</note>
-->

### [!UICONTROL Access] {#access}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone is assigned to a task]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to a task]</strong>: Defines the default permission a user has to the task they are assigned to. For more information about task permissions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</li> 
      <li> <p><strong>[!UICONTROL Also grant them ... access to the project]</strong>: Defines the default permission a user has to the project on which they have a task assigned to them. For more information about project permissions, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone is assigned to an issue]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to a task]</strong>: Defines the default permission a user has to the task they are assigned to. For more information about task permissions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</li> 
      <li> <p><strong>[!UICONTROL Also grant them ... access to the project]</strong>: Defines the default permission a user has to the project on which they have a task assigned to them. For more information about project permissions, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone submits a request]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to the issue]</strong>: Defines the default permission a user has on a request they submitted. For more information, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a>.</li> 
      <li> <p><strong>[!UICONTROL People from the same company will inherit the same permissions for all requests]</strong>: Allows users to see requests submitted by other users from the same company as them. They have the same permissions on those requests as they have on their own submitted requests.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. Click **[!UICONTROL Save]**.

## Lock task and issue preferences for groups {#lock-task-and-issue-preferences-for-groups}

If groups in your organization need a task or issue preference configured differently for their unique workflows, you can unlock the preference for all groups throughout the organization so that they can configure it on their own. When a preference is unlocked and the group administrator modifies it, the tasks or issues associated with the group are affected by the group-level setting for the preference instead of the system-level setting.

For information about how a group administrator configures task and issue preferences for a group, see [Configure task and issue preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>After a [!DNL Workfront] administrator unlocks a preference at the system level, any group administrator can configure it and then lock it to ensure that everyone in their group and the subgroups below is using the same configuration. This is parallel to the ability that a [!DNL Workfront] administrator has to configure and lock a preference for everyone in the system. For more information, see [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) and [Lock or unlock a project, task, or issue preference for subgroups](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

To lock or unlock a task or issue preference so that groups can configure it:

{{step-1-to-setup}}

1. Click **[!UICONTROL Project Preferences]** > **[!UICONTROL Tasks & Issues]**.

1. Do any of the following:

   * If you want administrators of groups below your group to be able to configure a preference for their groups, unlock it ![](assets/unlock-toggle-button.png).
   * If you want your group and all groups below it to use your configuration for a preference, make sure that it is locked (this is the default).

      >[!IMPORTANT]
      >
      >We recommend that you communicate with the administrators and users in groups throughout the system to ensure that all needs are accounted for in the way you configure a locked preference. When you lock it, your configuration for it is inherited by all groups in the system. And if the preference has been unlocked for any period of time, your configuration replaces those that group administrators might have made.

1. Click **[!UICONTROL Save]**.
