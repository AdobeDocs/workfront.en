---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Delete Job Roles
description: You can delete job roles that your organization no longer uses. We recommend that you do not delete job roles if they have been associated with work items in the past. To keep all your historical information about work assignments, we recommend that you deactivate roles, rather than delete them when they become obsolete. For information about deactivating roles, see Deactivate job roles.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
---
# Delete job roles

You can delete job roles that your organization no longer uses. We recommend that you do not delete job roles if they have been associated with work items in the past.

To keep all your historical information about work assignments, we recommend that you deactivate roles, rather than delete them when they become obsolete. For information about deactivating roles, see [Deactivate job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>New: [!UICONTROL Standard]</p>
   <p>Or</p>
   <p>Current: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>Administrative access to Job Roles</td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Delete a job role

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

{{step-1-to-setup}}

1. Click **[!UICONTROL Job Roles].**
1. Select the job role that you want to delete, then click **[!UICONTROL Delete].**
1. If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:

   * **Replace the job role with a different job role:** Select the new job role from the drop-down list.

      Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.

      Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.

   * **Delete the job role and its resource allocation:** Select **[!UICONTROL None]** from the drop-down list.

      >[!IMPORTANT]
      >
      >Deleting a job role deletes all current and past resource allocation related to that job role for all projects.

      &#x200B;For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.

1. Click  **[!UICONTROL Yes, Delete It]**.
