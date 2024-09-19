---
title: Grant Users Administrative Access to Certain Areas
description: As an Adobe Workfront administrator, you can use an access level to grant users with a Plan license administrative access to certain areas of the system.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
---
# Grant users administrative access to certain areas

<!--Linked in several places, do not rename or change URL.-->

As an Adobe Workfront administrator, you can use an access level to grant users with a Plan license administrative access to certain areas of the system.

>[!NOTE]
>
>This is different from giving a user full administrative access to Workfront, which is explained in [Grant a user full administrative access](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).​

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Grant Plan users administrative access to certain areas of Workfront

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
      <td role="rowheader">Job roles</td> 
      <td> <p>With this access, the user is allowed to do the following:</p> 
       <ul> 
        <li>View and edit existing job roles</li> 
        <li>Add new job roles</li> 
        <li>Edit role billing and cost rates</li> 
       </ul> <p><b>IMPORTANT</b>: If you grant a Planner user administrative access to job roles, the Financial Data access setting Edit Role Billing &amp; Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Planner user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </td> 
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
