---
filename: delete-job-roles
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Delete job roles
description: You can delete job roles that your organization no longer uses. We recommend that you do not delete job roles if they have been associated with work items in the past. To keep all your historical information about work assignments, we recommend that you deactivate roles, rather than delete them when they become obsolete. For information about deactivating roles, see Deactivate job roles.
---

# Delete job roles

You can delete job roles that your organization no longer uses. We recommend that you do not delete job roles if they have been associated with work items in the past. ```To keep all your historical information about work assignments, we recommend that you deactivate roles, rather than delete them when they become obsolete. For information about deactivating roles, see [Deactivate job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).```

## Access requirements

You must have the following:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to Job roles</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Delete a job role

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click**Job Roles.**
1. Select the job role that you want to delete, then click **Delete.**
1. If there are any objects (users, tasks, issues) that&nbsp;are assigned to the job role, do one of the following:

   * **Replace the job role with a different job role:** Select the new job role from the drop-down list.

     Any current and past resource allocations that are&nbsp;associated with the deleted job role are transferred to the job role that you select.

     Users who have only one job role assigned to&nbsp;them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.
   
   * **Delete the job role and its resource allocation:** Select**None**&nbsp;from the drop-down list.

     >[!IMPORTANT]
     >
     >Deleting a job role deletes all current and past resource allocation related to that job role for all projects.

     ​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.

1. Click  **Yes, Delete It**.

