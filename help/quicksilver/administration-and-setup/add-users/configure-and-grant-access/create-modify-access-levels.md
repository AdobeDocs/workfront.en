---
title: Create or modify custom access levels
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: As an Adobe Workfront administrator, you can create custom access levels and apply them to users.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
---
# Create and modify custom access levels

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

As an Adobe Workfront administrator, you can create custom access levels and apply them to users. As you work with access levels, it is important to understand how they work together with the object permissions that users grant when they share objects with each other. For more information about access levels, see:

* [New access levels overview](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Access levels overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>We strongly recommend that you leave the built-in access levels unchanged so that you can refer to them after you set up your users. To customize an access level, copy the default access level and modify the copy. You can do this for every access level except for System Administrator and External User.

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>New plan: Standard
   <p>or</p>
   <p>Current plan: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p></td> 
  </tr> 
 </tbody> 
</table>

## Create or edit a custom access level

{{step-1-to-setup}}

1. Click **Access Levels** in the left panel.
1. Select the access level you want to copy and customize, then click **Copy**.

   Or

   If you are editing an existing access level (that you copied previously), click its name.

1. In the box that displays, do any of the following to start configuring the custom access level:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>Type a name for your access level. </p> <p>If you just copied an access level to create a new one, the default name is Access Level Name (Copy), where Access Level Name is the access level you copied.</p> <p><strong>Tip</strong>: We recommend that you include the original name of the access level in the name of the copy. For example, at ACME company, a copy of the Standard access level might be named ACME Standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description </td> 
      <td>Type a description for the access level. It's helpful to list here what an user with this access level will be able to access.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">License Type</td> 
      <td>Make sure that the license selected here is the one that is most closely associated with the type of access level you are creating or editing. The selected license determines what settings are available for the access level. For more information, see <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">New licenses overview</a> or <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Licenses overview</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditional) If **Standard** or **Plan** is selected in the **License Type** box, scroll to the section **Allow administrative access for** and select administrative access permissions for those who will have this access level.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Approval Processes</td> 
      <td>Create and manage approval processes for use throughout the system and for specific groups.<p>Without this access, users can create only adhoc approval processes on items they have access to manage.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Companies</td> 
      <td>Add new and edit existing companies in Workfront.<br><p>Without this access, users can only view existing companies.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom forms</td> 
      <td>Create and manage all custom forms within their group. <br><p>Without this access, users can only attach existing forms to the objects they have access to contribute or manage.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exchange rates</td> 
      <td> Add new currency in Workfront. <p>Without this access, the user can add an existing currency only to a project they create.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Expenses</td> 
      <td>View all expenses on objects in Workfront.<p>Without this access, the user can only view the following:</p>
       <ul>
        <li>Expenses on projects, tasks or issues they manage</li>
        <li>Their own expenses</li>
        <li>The expenses of their subordinates</li>
       </ul><p><b>NOTE</b>: This does not allow the user to create new Expense Types.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Job roles</td> 
      <td> With this access, the user is allowed to do the following: 
       <ul> 
        <li>View and edit existing job roles</li> 
        <li>Add new job roles</li> 
        <li>Edit role billing and cost rates</li> 
       </ul> 
       <p>For important information about access to financial data that is available to a Standard or Planner user with administrative access to job roles, see <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">Standard or Planner users with administrative access to job roles</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Milestones in my group</td> 
      <td>View all the milestone paths in the system under the Milestone Paths menu in Setup. Users can also edit or delete any milestone paths belonging to any of their groups. Users cannot manage (edit or delete) milestone paths that are not assigned to their of groups.<p>Without this access, users can only view existing milestone paths and apply them to projects they have access to manage.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reminder notifications</td> 
      <td>Create and manage reminder notifications in Workfront.<p>Without this access, users are limited to receiving and viewing notifications.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timesheets &amp; hours</td> 
      <td> Group administrators can assign timesheet profiles to users in the groups and subgroups they manage. <p>Without this option enabled, group administrators cannot assign timesheet profiles to other users in the groups and subgroups they manage, although they can create them.</p> <p>All other users with a Standard or Plan license can view all hours and timesheets in Workfront.</p> <p>Without this option enabled, users can view hours only on:</p> 
       <ul> 
        <li>Projects, tasks or issues they manage</li> 
        <li>Their own timesheet</li> 
        <li>A timesheet of someone that reports to them</li> 
        <li>A timesheet they approve</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Set additional restrictions**, then set any of the following restrictions for the access level.

   >[!IMPORTANT]
   >
   >For external users such as vendors (anyone not in your organization), we recommend that you restrict access to tasks, projects, updates, announcements, other companies, teams and groups.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Never give access to the whole project when assigned to a task or issue</td> 
      <td> Prevents users assigned to tasks or issues to also gain permissions to the parent project, even if the project permissions allow that.<p>For more information about configuring the permissions on a project, see the section <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> in the article <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Never inherit document access from projects, tasks, issues, etc...</td> 
      <td>Prevents documents from inheriting the permissions set on their parent object.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">View only updates in which they have been included in the conversation</td> 
      <td> Enables users to see only comments where their name or the name of their team has been included. <p> <p><b>NOTE</b>: This prevents users from subscribing to items in Workfront. For more information about subscribing to items, see <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Subscribe to items in Adobe Workfront</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Never allow users to delete comments </td> 
      <td> Prevents users from deleting the comments they make on items.  <p><b>NOTE</b>: No one can delete the comments of other users.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">View only companies, groups &amp; teams they belong to</td> 
      <td>Allows users to view and share items only with companies, groups, and teams they belong to.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Never allow visibility of Planned Hours or Actual Hours</td> 
      <td>Prevents users from seeing the Planned and Actual Hours of work items they have access to. They can, however, see Actual Hours they log themselves, or hours that are logged by someone who reports to them.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Never allow users to delete announcements</td> 
      <td>Prevents users from deleting announcements in the Announcement Center. For more information, see <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Send announcements</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditional and optional) If your Workfront system is set up for users that belong to multiple companies, restrict the visibility to other users based on what company they belong to in the section **People in other companies should only view users from**.

   You can restrict the users to see just users from their own company or from the company you designated as the primary company. The primary company typically represents your Workfront account where most of your users work. For more information about the primary company, see [Create and edit companies](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >If two users belong to two different companies, but they can both see users from the primary company, they can see the Updates area associated with the primary company.

1. (Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in [Configure access to Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), such as [Grant access to tasks](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) and [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Click **Save**.

   After the access level is created, you can assign it to a user (unless it is a System Administrator access level). 
   
   For more information, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). 
   
   For information about how an Adobe administrator assigns a System Administrator access level to a users, see [Grant a user full administrative access](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Standard or Planner users with administrative access to job roles {#planner-users}

If you grant a Standard or Planner user administrative access to job roles, the Edit Role Billing &amp; Cost Rates setting is automatically enabled for the user automatically.

Later, if you disable administrative access to job roles for the user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled.

If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see [Grant access to financial data](grant-access-financial.md).
