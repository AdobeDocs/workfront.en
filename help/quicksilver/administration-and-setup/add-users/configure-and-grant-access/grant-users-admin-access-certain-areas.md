---
title: Grant Users Administrative Access to Certain Areas
description: As an Adobe Workfront administrator, you can use an access level to grant users with a Plan license administrative access to certain areas of the system.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
TQID: https://experienceleague.adobe.com/1nXA0NxLQW3tiIrhCKAd5EMfqBjQW68GHNN42dQmptQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Grant users administrative access to certain areas

{{preview-fast-release-general}}

<!--Linked in several places, do not rename or change URL.-->

As an Adobe Workfront administrator, you can use an access level to grant users with a Standard or Plan license administrative access to certain areas of the system.

>[!NOTE]
>
>This is different from giving a user full administrative access to Workfront, which is explained in [Grant a user full administrative access](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).​

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Grant Standard or Plan users administrative access to certain areas of Workfront

>[!IMPORTANT]
>
>We strongly recommend that you leave the built-in access levels unchanged so that you can refer to them after you set up your users. To customize an access level, copy the default access level and modify the copy. (You can do this for every access level except for System Administrator and External User.)

{{step-1-to-setup}}

1. In the left panel, click **Access Levels**.
1. Click the name of the access level you want to use to grant users administrative access to certain areas of Workfront.
1. In the **Allow administrative access for** section, check boxes to grant the necessary administrative access.

   These options allow you to grant the following capabilities:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Approval Processes</td> 
      <td><p>Create and manage approval processes for use throughout the system and for specific groups.</p><p>Without this access, users can create only ad-hoc approval processes on items they have access to manage.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="preview">Change history</span></td> 
      <td><p><span class="preview">View the Workfront change history logs in Setup > Change Tracking > Change History List.</span></p>
      <p><span class="preview">Without this access, users do not have this option in the Setup area.</span></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Companies</td> 
      <td><p>Add new and edit existing companies in Workfront</p>
      <p>Without this access, users can only view existing companies.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom forms</td> 
      <td><p>Create and edit (add, edit, and delete the fields) custom forms within their group.</p><p>Without this access, users can only attach existing forms to objects where they have access to contribute or manage.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exchange rates</td> 
      <td> <p>Add new currency in Workfront.</p> <p>Without this access, the user can only add an existing currency to a project they create.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Expenses</td> 
      <td><p>View all expenses on objects in Workfront.</p><p>This does not allow the user to create new Expense Types.</p><p>Without this access, the user can only view the following:</p>
       <ul>
        <li>Expenses on projects, tasks or issues they manage</li>
        <li>Their own expenses</li>
        <li>The expenses of their subordinates</li>
       </ul></td> 
     </tr>
     <tr> 
      <td role="rowheader">Milestones in my group</td> 
      <td>View all the milestone paths in the system under the Milestone Paths menu in Setup. Users can also edit or delete any milestone paths belonging to any of their groups. Users cannot manage (edit or delete) the milestone paths that are not assigned to any of their of groups.<br><p>Without this access, users can only view existing milestone paths and apply them to projects they have access to manage.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reminder notifications</td> 
      <td>Create and manage reminder notifications in Workfront.<br>Without this access, users are limited to receiving and viewing notifications.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timesheets &amp; hours</td> 
      <td> <p>Allows users to view to all hours and timesheets in Workfront.</p> <p>When this option is disabled, users can view only hours on:</p> 
       <ul> 
        <li>Projects, tasks, or issues they manage</li> 
        <li>Their own timesheet</li> 
        <li>A timesheet of someone that reports to them</li> 
        <li>A timesheet that they approve</li> 
       </ul> <p><b>NOTE</b>:  <p>Whether this option is enabled or disabled, group administrators can create timesheet profiles for the groups and subgroups they manage and assign them to group members whose user profiles they have access to edit.</p> <p>Enabling this option might provide too much access for some group administrators because they can view the timesheets generated by timesheet profiles (and the hours) for all users in the system, not only for those in the groups they administer. You can disable this option for group administrators who don't need this much access.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. When you are finished, click **Save**.
1. Assign the new access level to a user, as described in [Add users](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >You can allow users to have administrative access to users. For more information about giving users administrative access to users so they can manage user accounts, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


<!--     
     <tr> 
      <td role="rowheader">Job roles</td> 
      <td> <p><b>NOTE</b>: In the Preview environment, access to job roles is controlled as an object type in the access level. See <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-job-roles.md">Grant access to job roles</a>.</p>
      <p>With this access, the user is allowed to do the following:</p> 
       <ul> 
        <li>View and edit existing job roles</li> 
        <li>Add new job roles</li> 
        <li>Edit role billing and cost rates</li> 
       </ul> <p><b>IMPORTANT</b>: If you grant a Standard or Plan user administrative access to job roles, the Financial Data access setting Edit Role Billing &amp; Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Standard or Plan user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </td> 
     </tr>
-->

<!--
## Access of a Workfront administrator vs. access of a Standard or Plan user with administrative rights  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

The two tables below show the difference between the access rights of a user with a Workfront System Administrator access level versus those of a user with a Standard or Plan license with some administrative rights.

Workfront administrators can view all the objects in the system (regardless of who created them), create new ones, and modify or delete existing ones. They have full access to all objects in the system.

Users with a Standard or Plan license who can edit functionality in one area have full access to the functionality in that area.

>[!NOTE]
>
>Users with a Standard or Plan license who are designated as group administrators can perform some of the actions allowed for Workfront administrators. They are allowed to perform these actions only for the groups they administer, their subgroups, and the users in these groups and subgroups. For more information, see [Group administrators](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Access to the Setup area](#access-to-the-setup-area)
* [Access to objects](#access-to-objects)

### Access to the Setup area {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/object</th> 
   <th>Workfront administrator </th> 
   <th>User with a Standard or Plan license and some administrative rights</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Project Preferences: Projects</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Tasks &amp; Issues</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Statuses</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Priorities</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Severities</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Exchange Rates</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Processes: Approvals</td> 
   <td> <p>Full access</p> </td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Processes: Milestone Paths</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Custom Forms</td> 
   <td>Full access</td> 
   <td> <p>Manage custom forms they created or custom forms shared with them.</p> <p>Attach custom forms they created or custom forms shared with them to objects they have manage or contribute permissions to.</p> </td> 
  </tr> 
  <tr> 
   <td>Recycle Bin: Recently Deleted</td> 
   <td>Full access</td> 
   <td> <p>Users who are group administrators can restore projects assigned to Groups they manage, and tasks, issues, or documents associated with those projects.</p> </td> 
  </tr> 
  <tr> 
   <td>Recycle Bin: Recently Restored</td> 
   <td>Full access</td> 
   <td>Users who are group administrators can see the items they have recently restored.</td> 
  </tr> 
  <tr> 
   <td>Job Roles</td> 
   <td>Full access</td> 
   <td> <p>Modify but not delete existing job roles.</p> <p>Add new job roles.</p> </td> 
  </tr> 
  <tr> 
   <td>Teams</td> 
   <td>Full access</td> 
   <td> <p>No access to create Teams.</p> <p>Add existing teams to users when creating or editing users.</p> </td> 
  </tr> 
  <tr> 
   <td>Groups</td> 
   <td>Full access</td> 
   <td> <p>No access to create Groups.</p> <p>Only group administrators can manage group membership, subgroups, and group-level statuses for the groups they manage. </p> </td> 
  </tr> 
  <tr> 
   <td>Companies</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Log in As</td> 
   <td>Full access </td> 
   <td> <p>If their group administrative access is enabled on their access level and they are designated as a group administrator, they can log in as the users in the group they administer and their subgroups. They cannot log in as a System Administrator.<br>For more information about enabling group administrative access for users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Schedules</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Schedules.</p> <p>Access to add existing schedules to other users, at the user level. </p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Timesheet Profiles</td> 
   <td>Full access</td> 
   <td> <p>Access to assign existing Timesheet Profiles to users, at the user level.</p> <p>Users who are group administrators can create Timesheet Profiles for the groups they administer and their subgroups. </p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Hour Types</td> 
   <td>Full access</td> 
   <td> <p>Access to assign Hour Types to users, at the user level.</p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Preferences</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Event Notifications</td> 
   <td>Activate/ Deactivate all</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Reminder Notifications</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Email Templates</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Email Templates.</p> <p>Access to add existing Email Templates to Reminder Notifications.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Automatic Reminders</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Invitations</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Email Invitations.</p> <p>Access to resend email invitations to unregistered users only from the People tab.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Setup</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Scorecards</td> 
   <td>Full access</td> 
   <td> <p>Full access</p> </td> 
  </tr> 
  <tr> 
   <td>Expense Types</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Risk Types</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Access Levels</td> 
   <td> <p>Full access to modify all access levels.</p> <p>The System Administrator and External User access levels cannot be modified, by default.</p> </td> 
   <td> <p>No access to edit Access Levels.</p> <p>Assign an access level to other users which is lower or equal to theirs at the user level.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Layout Templates</td> 
   <td>Full access</td> 
   <td> <p>Access to assign existing Layout Templates to other users, at the user level. </p> <p>Users designated as group administrators can create Layout Templates for groups and subgroups they manage.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Update Feeds</td> 
   <td>Full access</td> 
   <td> <p>No access to modify Update Feeds.</p> <p>Access to add fields to be tracked in the Update Feeds when editing Custom Forms.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Filters</td> 
   <td>Full access</td> 
   <td> <p>No access to create Filters in the Setup area.</p> <p>Access to create new filters in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Views</td> 
   <td>Full access</td> 
   <td> <p>No access to create Views in the Setup area.</p> <p>Access to create new views in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Groupings</td> 
   <td>Full access</td> 
   <td> <p>No access to create Groupings in the Setup area.</p> <p>Access to create new groupings in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: List Controls</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Cloud Providers</td> 
   <td>Full access</td> 
   <td> <p>No access to configure Cloud Providers.</p> <p>Access to link documents to and from Cloud Providers from the Documents tab, after the Cloud Providers have been integrated with Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Metadata Mapping</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Documents: SharePoint Integration</td> 
   <td>Full access</td> 
   <td> <p>No access to configure a SharePoint integration.</p> <p>Access to link documents to and from SharePoint from the Documents tab, after the SharePoint integration with Workfront has been configured.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Custom Integration</td> 
   <td>Full access</td> 
   <td> <p>No access to configure a Custom Integration.</p> <p>Access to link documents to and from third-party providers from the Documents tab, after the third-party providers have been integrated with Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>System: Branding</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Customer Info</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Single Sign-On (SSO)</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Update Users for SSO</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Kick-Starts</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Diagnostics</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Preferences</td> 
   <td>Full access</td> 
   <td>No access</td> 
  <tr> 
   <td>Change Tracking: Configuration</td> 
   <td>Full access</td> 
   <td>No access</td> 
  <tr> 
   <td>Change Tracking: Change History List</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
 </tbody> 
</table>

### Access to objects {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/object</th> 
   <th>Workfront administrator </th> 
   <th>User with a Standard or Plan license and some administrative rights</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendars</td> 
   <td>Full access</td> 
   <td>Manage calendars they create and calendars shared with them.</td> 
  </tr> 
  <tr> 
   <td>Dashboards</td> 
   <td>Full access</td> 
   <td>Manage dashboards they create and dashboards shared with them.</td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>Full access</td> 
   <td>Manage documents they upload or documents shared with them.</td> 
  </tr> 
  <tr> 
   <td>Issues</td> 
   <td>Full access</td> 
   <td>Manage issues they create or issues shared with them.</td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td>Full access</td> 
   <td>Manage portfolios they create or portfolios shared with them. </td> 
  </tr> 
  <tr> 
   <td>Programs</td> 
   <td>Full access</td> 
   <td>Manage programs they create or programs shared with them.</td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Full access</td> 
   <td>Manage projects they create or projects shared with them.</td> 
  </tr> 
  <tr> 
   <td>Reports</td> 
   <td>Full access</td> 
   <td>Manage reports they create or reports shared with them. View, copy and edit system reports.</td> 
  </tr> 
  <tr> 
   <td>Tasks</td> 
   <td>Full access</td> 
   <td>Manage tasks they create or tasks shared with the</td> 
  </tr> 
  <tr> 
   <td>Templates</td> 
   <td>Full access</td> 
   <td>Manage templates they create or templates shared with them</td> 
  </tr> 
  <tr> 
   <td>Timesheets</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Users</td> 
   <td>Full access</td> 
   <td> <p>Limited access</p> <p>They cannot assign groups to users for which they are not a group administrator or groups that are not public.</p> <p>They cannot assign an access level to users which is higher then their own access level.</p> <p>If their group administrative access is enabled on their access level and they are designated as a group administrator on a group, they can reset the password of and log in as the users in the group they administer and their subgroups. They cannot reset the password of or log in as a System Administrator.<br>For more information about enabling group administrative access for users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

