---
product-area: projects
navigation-topic: manage-issues
title: Edit issues
description: You can edit information on issues that you have created, or that other users have created if they shared the issues with you.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
---
# Edit issues

You can edit information on issues that you have created, or that other users have created if they shared the issues with you.

You can edit a single issue or you can edit issues in a list. For information about editing issues in a list, see [Edit issues in a list](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to edit issues in the Issues  section of a task or a project</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to an issue to edit the following fields in the Details area: </p>
   <ul>
   <li>Description</li>
   <li>Status</li>
   <li>Severity</li>
   </ul>
   <p>Manage permissions to an issue to edit all the fields in the Details area or in the Edit Issue box</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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

1. Go to the **Main Menu**.
1. Click **Projects**, then click the name of a project to open the project.
1. (Optional)&nbsp;Click **Tasks** , then click the name of a task to open the task. 
1. Click **Issues** in the left panel.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. (Optional) To edit limited information about an issue, click **Issue Details** in the left panel.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator or Group administrator modified your Layout Template, the fields in the Issue Details area might be rearranged or not display. For information, see [Customize the Details view using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   To edit information in the Details section, do the following:

   1. (Optional) Click the **Collapse All** icon in the upper-right corner to collapse all areas. 
   1. (Optional and conditional) When an area is collapsed, click the **right-pointing arrow** ![](assets/right-pointing-arrow.png) next to each area to expand the area you want to edit. 
   1. (Optional) To attach a custom form, start typing the name of a form in the **Add custom form** field, then select it when it displays in the list, then click&nbsp;**Save Changes**. 
   1. (Optional) Click the **Export** icon ![](assets/export.png) to export the Overview and custom forms information to a PDF file, then click **Export**. Select from the following:

      * Select all (displays only when there is at least one custom form attached)
      * Overview
      * The name of one or multiple custom forms

      The PDF file downloads to your computer.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      For more information, see [Export custom forms and object details](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

   For information about the fields visible in the Issue Details section, continue with editing the issue in the Edit issue box as described below. 

1. To edit all information about an issue, select an issue in a list, then click&nbsp;**Edit** at the top of the list

   Or

   Click the name of an issue in a list then click the **More** menu next to the issue name, then **Edit.**

   The **Edit Issue** dialog box displays.

   >[!IMPORTANT]
   >
   >You must have Manage permissions to the issue in order to see the Edit link.

   All issue fields are available in the Edit Issue box and are grouped by the areas listed in the left panel. 

1. Consider specifying information in any of the following sections:

   * [Issue Name](#issue-name)
   * [Overview](#overview)
   * [Assignments](#assignments)
   * [Custom Forms](#Custom%C2%A0F)
   * [Settings](#settings)

   >[!NOTE]
   >
   >Depending on how your Workfront administrator sets up our Layout Template, the fields in the Edit Issue box might be different in your environment. For information, see [Customize the Details view using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
   >
   >Most fields listed in the sections below are also accessible from the New Issue box, when you create an issue. The sections under which the fields are located do  not match the New Issue box. For information about creating issues, see [Create issues](../../issues/manage-issues/create-issues.md). 

### Issue Name {#issue-name}

1. Begin editing an issue as described above.
1. Click **Issue Name**.

   ![](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. Update the **Issue Name** field. 
1. Click **Save** or continue editing the following sections.

### Overview {#overview}

1. Begin editing an issue as described above.
1. Click **Overview**.

   ![](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. Update or review any of the fields in the following table: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td> <p>Add additional information about the issue.</p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader">Basic information section</td> 
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
       </ul> <p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For more information about editing priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Create and customize priorities</a>.</p> </td> 
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
       </ul> <p>Depending on the Project Preferences selected by your Workfront administrator, the names of severities might be different for you. For more information about editing severities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">Create or customize issue severities</a>.</p> </td> 
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
      <td role="rowheader">Primary Contact</td> 
      <td>By default, the Primary Contact is the creator of the issue. To modify this, start typing the name of any active user in Workfront, then select it from the list. An issue can have only one Primary Contact.<br> If you change the Primary Contact, the original primary contact still has Manage access to the issue. You must manually remove this access from the Issue Access box, when sharing an issue.
      
      <b>TIP</b>

      <p>When adding a Primary Contact user, notice the avatar, the user's Primary Role, and their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them.</p>
      <p> You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">Grant access to users</a>.</p>

      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Commit Date and time</td> 
      <td> <p>This is the date when the assignee of the issue estimates that the issue will be completed. Only assignees can edit this field.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planned Start&nbsp;Date</td> 
      <td>By default, the Planned Start Date is the date and the time when the issue was created. You can update the <strong>Planned Start Date</strong> of the issue. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planned Completion Date and time</td> 
      <td> By default, the Planned Completion Date is 24 hours from the default Planned Start Date. By default, issues have a Duration of 1 day. You can update the <strong>Planned Completion Date</strong> of the issue.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actual Start Date and time</td> 
      <td>The Actual Start Date is automatically populated when you change the status of the issue to <strong>In Progress</strong>. You can update the <strong>Actual Start Date</strong> of the issue. You can manually update the date, if needed. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actual Completion Date and time</td> 
      <td>The Actual Completion Date is automatically populated when you change the status of the issue to <strong>Closed</strong> or<strong>Resolved</strong>. You can update the <strong>Actual Completion Date</strong> for the issue. You can manually update the date, if needed.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resolved By</td> 
      <td> <p>This shows whether the issue is resolved by another object. You can select whether this issue is resolved by a task, a project, or another issue from the drop-down menu, then start typing the name of the task, project, or issue that will resolve the issue. Select it when it appears in the list.</p> 
      
      <b>NOTE</b>
          
      When you select an object to resolve an issue, the issue status is linked to the status of the resolving object and cannot be changed on the issue. For more information about resolving objects, see <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>. 
      
      <b>TIP</b>

      When your system or group administrator adds the "Resolved By" field to an issue custom header, the field changes to "Resolving Issue", "Resolving Task", or "Resolving Project" when there is a resolving object associated with the issue.

      You cannot edit this field when it displays in the issue header. For more information about customizing issue headers, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">Customize object headers using a layout template </a>
      </td> 
     </tr>

     <tr> 
      <td role="rowheader">Resolving Issue, Resolving Task, or Resolving Project</td> 
      <td>The linked name of the issue, task, or issue that resolves the issue.  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">This Resolves</td> 
      <td>The linked name of the issue which completes when the issue you are accessing is resolved.  </td> 
     </tr> 


    </tbody> 
   </table>

    
    
  

1. Click **Save** or continue editing the following sections.

#### Assignments {#assignments}

1. Begin editing the issue as described above.
1. Click **Assignments** in the left panel.

   ![](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. Click **Search people, role and teams** and start typing the name of a user, role, or team that you want to assign to the task, then click it or press Enter when it displays on the list.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)</p>
   -->

   >[!NOTE]
   >
   >If the user's name contains a special character, you must include the special character in the search field.

   >[!TIP]
   >
   >You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
   >
   >
   >If a user, job role, or team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following: 
   >
   >* Reassign the work item to active resources. 
   >* Associate the users in a deactivated team with an active team and reassign the work item to the active team. 

1. (Optional) Indicate whether an assignee is the primary assignee on the issue, by hovering over the name of the assignee and clicking **Make Primary**. A team cannot be the primary assignee of an issue. 
1. Update the following fields: 

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Planned Hours</td> 
      <td> <p>This is the amount of actual time it would take the assignees of the issue to complete it. Type the number of Planned Hours for the issue.<br></p> <p>Note:  Changing the Planned Hours of the issue will not change the issue Planned Completion Date. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Assignee's Role</td> 
      <td> <p>Select a role from the <strong>Assignee's Role</strong> drop-down menu when you selected a person as an assignee. This is the role that the assignee can fulfill on this issue. </p> <p><b>TIP</b>
      
      Only the job roles associated with each assignee in their profile appear in the drop-down menu.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save** or continue editing the following sections.

### Custom&nbsp;Forms

1. Begin editing an issue as described above.
1. Click **Custom Forms**.

   ![](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. In the **Add custom form** field, select the custom form or forms that you want to associate with the issue. You must build the custom forms before they are available to select in this field. Only active custom forms display in the list. For more information about building custom forms, see [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). You can add up to ten custom forms to an issue. 

1. (Conditional) If you attached a custom form to the issue, edit any fields on the form. You must specify all required fields before you can save the issue.

   >[!NOTE]
   >
   >Depending on how your Workfront Administrator set the permissions for the sections in your custom form, not everyone can view or edit the same fields on a given custom form. The permissions to edit fields within a section of a custom form depend on the permissions you have on the issue itself. For information about setting permissions on sections of a custom form, see [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). For information about setting issue permissions, see [Share an issue](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

1. Click **Save** or continue editing the following section.

### Settings {#settings}

1. Begin editing an issue as described above.
1. Click **Settings**.

   ![](assets/settings-section-edit-issue-box-nwe-350x240.png)

   Update the following information:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Approval Process</td> 
      <td> 
       <div> 
       <p>Select an approval process that you want to associate with the issue. Your Workfront administrator must define system-level Approval Processes before you can associate them with issues. Users with administrative access to Approval processes <span> can also create group-specific approval processes.</span>For more information about creating Approval Processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>. </p> 
       <p>Consider the following when adding approval processes: </p> 
       <ul> 
       <li>Only active approval processes display in the list. </li> 
       <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list.</p> <p>Important: If the group of the project changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
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
     <tr> 
      <td role="rowheader">Reminder Notifications</td> 
      <td> <p>Select the checkbox for which Reminder Notifications you would like to attach to this issue. All reminder notifications for issues display. Your Workfront administrator must configure Reminder Notifications before you can select them on an issue. For more information about configuring Reminder Notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save.**

## Edit an issue in the issue header (limited)

You can edit a limited amount of information in the issue header. 

Your system or group administrator can customize the fields you see in the issue header. For information, see [Customize object headers using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

![](assets/issue-header-350x19.png)

The following fields are included in the issue header, by default:

* Issue name
* Percent complete
* Assignments
* Planned Completion Date and time 
* Status
* Make approval decisions if you are set as the approver in a current approval process
