---
filename: edit-issues
product-area: projects
navigation-topic: manage-issues
title: Edit issues
description: You can edit information on issues that you have created, or that other users have created if they shared the issues with you.
---

# Edit issues

You can edit information on issues that you have created, or that other users have created if they shared the issues with you.

You can edit a single issue or you can edit issues in a list. For information about editing issues in a list, see [Edit issues in a list](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to edit issues in the Issues tab of a task or a project</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to an issue to edit it in the Issue Details area </p> <p>Manage permissions to an issue to edit it in the Edit Issue box</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Limitations when editing issues

There are some limitations that might prevent you from editing issues.

* You cannot edit issues that are in an Approval Process. You can only log time or update the status on an issue that is in Pending Approval. 
* You can edit and add documents to issues on a project that has a status of Complete, Dead, or is Pending Approval only when your Workfront administrator or a group administrator enabled this functionality in the Project Preferences area. For information about setting project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Edit a single issue

You can edit an issue using the Edit Issue or Issue Details areas. The following steps describe editing an issue in the Edit issue box.

1. Go to the **Projects** area in the Global Navigation Bar. 
1. Select the **Projects** tab, then  click the name of a project to open the project.
1. (Optional)&nbsp;Click **Tasks** , then click the name of a task to open the task. 
1. Click the **Issues** tab. 
1. Do one of the following:

   * To edit a limited number of fields for the issue, click the name of an issue, then select the **Issue Details** tab and edit the fields under the **Overview** and **Custom Forms** sub-tabs.

     >[!IMPORTANT]
     >
     >You must have Manage permissions on the issue to edit information in the Issue Details tab.

   * To edit all the fields of an issue, click the name of an issue in a list, then click **Edit Issue.**

     The **Edit Issue** dialog box displays.

     >[!IMPORTANT]
     >
     >You must have Manage permissions to the issue in order to see the Edit Issue option.

     All issue fields are available in the Edit Issue box and are grouped by the areas listed in the left panel

     ![edit_issue_box.png](assets/edit-issue-box-350x361.png)

1. Consider specifying information in any of the following sections:

   * [Overview](#overview)
   * [Settings](#settings)
   * [Custom Forms](#custom-forms)
   * [Assignments](#assignments)
   * [Comment](#comment)

### Overview {#overview}

1. Begin editing an issue as described above.
1. Click **Overview**.

   ![overview_section_edit_issue.png](assets/overview-section-edit-issue-350x443.png)

1. Update or review any of the fields in the following table: 

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>Type a name for the issue.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td> <p>Add additional information about the issue.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>Type a web link that relates to the information about the issue.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type</td> 
      <td> <p>According to the Queue Properties selected by your project manager in the Queue Details area of the project, you might be able to specify the type of the issue. Select from the following options in the <b>Type</b> drop-down menu: </p> 
       <ul> 
        <li> <p><strong>Bug Report</strong> </p> </li> 
        <li> <p><strong>Change Order</strong> </p> </li> 
        <li> <p><strong>Issue</strong> </p> </li> 
        <li> <p><strong>Request</strong> </p> </li> 
       </ul> <p>Depending on the Project Preferences selected by your Workfront administrator, the names of the types of the issues might be different for you.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td> <p>Select the status of the issue. For more information about issue statuses, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Access the list of system issue statuses</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priority</td> 
      <td> <p>This is a visual flag for you which allows you to prioritize issues.</p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>None</strong> </p> </li> 
        <li> <p><strong>Low</strong> </p> </li> 
        <li> <p><strong>Normal</strong> </p> </li> 
        <li> <p><strong>High</strong> </p> </li> 
        <li> <p><strong>Urgent</strong> </p> </li> 
       </ul> <p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For more information about editing priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities-.md" class="MCXref xref">Create and customize priorities</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Severity</td> 
      <td> <p>This is a visual flag for you which indicates how severe the problem described in the issue is. Severities are specific to issues. Select from the following options:</p> 
       <ul> 
        <li> <p style="font-weight: bold;">Cosmetic</p> </li> 
        <li> <p style="font-weight: bold;">Causes Confusion</p> </li> 
        <li> <p style="font-weight: bold;">Bug with workaround</p> </li> 
        <li> <p style="font-weight: bold;">Bug with no workaround</p> </li> 
        <li> <p style="font-weight: bold;">Fatal error</p> </li> 
       </ul> <p>Depending on the Project Preferences selected by your Workfront administrator, the names of severities might be different for you. For more information about editing severities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">Create and customize issue severities</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Primary Contact</td> 
      <td> <p>By default, the Primary Contact is the creator of the issue. To modify this, start typing the name of any active user in Workfront, then select it from the list. An issue can have only one Primary Contact.<br></p> <p>Note:  If you change the Primary Contact, the user who was the primary contact still has Manage access to the issue. You must manually remove this access under <strong>Project Actions</strong> &gt; <strong>Sharing</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planned Hours</td> 
      <td> <p>This is the amount of actual time it would take the assignees of the issue to complete it. Type the number of Planned Hours for the issue.<br></p> <p>Note:  Changing the Planned Hours of the issue will not change the issue Planned Completion Date. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actual Hours</td> 
      <td> <p>This is the number of hours that users logged on the issues. You cannot edit this field from this box. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planned Start&nbsp;Date and time </td> 
      <td> <p>By default, the Planned Start Date is the date and the time when the issue was created. You can update the <strong>Planned Start Date</strong> of the issue. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actual Start Date and time </td> 
      <td> <p>The Actual Start Date is automatically populated when you change the status of the issue to <strong>In Progress</strong>. You can update the <strong>Actual Start Date</strong> of the issue. You can manually update the date, if needed. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planned Completion Date and time </td> 
      <td> <p> By default, the Planned Completion Date is 24 hours from the default Planned Start Date. By default, issues have a Duration of 1 day. You can update the <strong>Planned Completion Date</strong> of the issue.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actual&nbsp;Completion Date and time </td> 
      <td> <p>The Actual Completion Date is automatically populated when you change the status of the issue to <strong>Closed</strong> or<strong>Resolved</strong>. You can update the <strong>Actual Completion Date</strong> for the issue. You can manually update the date, if needed.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resolved By</td> 
      <td> <p>This shows whether the issue is resolved by another object. You can select whether this issue is resolved by a task, a project, or another issue from the drop-down menu, then start typing the name of the task, project, or issue that will resolve the issue. Select it when it appears in the list.<br></p> <p>Note:  When you select an object to resolve an issue, the issue status is linked to the status of the resolving object and cannot be changed on the issue. For more information about resolving objects, see <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save Changes** or continue editing the following sections.

### Settings {#settings}

1. Begin editing an issue as described above.
1. Click **Settings**.

   ![settings_area_edit_issue.png](assets/settings-area-edit-issue-350x255.png)

   Update the following information:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Reminder Notifications</td> 
      <td> <p>Select the checkbox for which Reminder Notifications you would like to attach to this issue. All reminder notifications for issues display. Your Workfront administrator must configure Reminder Notifications before you can select them on an issue. For more information about configuring Reminder Notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approval Process</td> 
      <td> 
       <div> 
        <p>Select an approval process that you want to associate with the issue. Your Workfront administrator must define system-level Approval Processes before you can associate them with issues. Users with administrative access to Approval processes <span> can also create group-specific approval processes.</span>For more information about creating Approval Processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>. </p> 
        <p>Consider the following when adding approval processes: </p> 
        <ul> 
         <li>Only active approval processes display in the list. </li> 
         <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list.</p> <p>Important: If the group of the project changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
         <li> <p data-mc-conditions="QuicksilverOrClassic.Classic"> If you added a single-use approval process, it displays as "&lt;Custom&gt;" in this field. </p> </li> 
         <li> <p>You can define default approval processes to be automatically attached to issues when creating request queues or Queue Topics. For information about updating Queue Details, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. For information about creating Queue Topics, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Create Queue Topics</a>. </p> </li> 
         <li>When bulk-editing issues, the following scenarios exist:
          <ul>
           <li><p>When you select multiple issues from the same group, both system-level and group-specific approval processes display in this field.</p></li>
           <li><p>When you select multiple issues from different groups, only system-level approval processes display in this field.</p></li>
           <li><p>When any of the issues have a single-use approval process attached, it is replaced by the system-level or group-level approval process you select. </p></li>
          </ul></li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save Changes** or continue editing the following sections.

### Custom Forms {#custom-forms}

1. Begin editing an issue as described above.
1. Click **Custom Forms**.

   ![custom_forms_area_edit_issue.png](assets/custom-forms-area-edit-issue-350x153.png)

1. Select the custom form or forms that you want to associate with the issue. You must build the custom forms before they are available to select in this field. Only active custom forms display in the list. For more information about building custom forms, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). You can add up to ten custom forms to an issue. 
1. (Conditional) If you attached a custom form to the issue, edit any fields on the form. You must specify all required fields before you can save the issue.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator set the permissions for the sections in your custom form, not everyone can view or edit the same fields on a given custom form. The permissions to edit fields within a section of a custom form depend on the permissions you have on the issue itself. For information about setting permissions on sections of a custom form, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). For information about setting issue permissions, see [Share an issue in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

1. Click **Save Changes** or continue editing the following sections.

### Assignments {#assignments}

1. Begin editing an issue as described above.
1. Click **Assignments**.

   ![assignments_ara_edit_issue.png](assets/assignments-ara-edit-issue-350x94.png)

1. Click **Add Assignee** to add a new assignee to the issue. You can assign users, roles, or teams to an issue. You can have multiple assignees on an issue. 

   ``` ```**Tip: **`````` You can assign multiple users or job roles, and you can assign only one team. ```You can assign only active users, ```job roles```, and teams.```

   ```If a user, ```job role```, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:```

   * ```Reassign the work item to active resources.``` 
   * ```Associate the users in a deactivated team with an active team and reassign the work item to the active team.```

1. (Optional) Indicate whether an assignee is the primary assignee on the issue, by selecting the **Issue Owner** radio button. 
1. (Optional) Select a role from the **Assignee's Role** drop-down menu.  
   This is the role that the assignee can fulfill on this issue. Only the job roles associated with each assignee in their profile appear in the drop-down menu.  

1. Click **Save Changes** or continue editing the following section.

### Comment {#comment}

1. Begin editing an issue as described above.
1. Click **Comment**.

   ![comment_area_edit_issue.png](assets/comment-area-edit-issue-350x189.png)

1. Specify a comment that you want to display in the updates stream of the issue in the available field. This comment is visible for everyone with View access to the issue and with access to view Notes.
1. Click **Save Changes**.  
   Your changes will be submitted for this issue. Any notifications that are triggered by making edits to the issue and meet the conditions to be sent at this time, will now be sent to the users associated with this issue.

