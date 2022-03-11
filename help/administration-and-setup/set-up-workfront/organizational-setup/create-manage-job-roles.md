---
filename: create-manage-job-roles
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Create and manage job roles
description: As an Adobe Workfront administrator or a user with administrative access to Job Roles, you can create job roles which can be assigned to users and delete default job roles that are not relevant to your organization. For information about administrative access in Workfront, see Grant users administrative access to certain areas.
---

# Create and manage job roles

As an Adobe Workfront administrator or a user with administrative access to Job&nbsp;Roles, you can create job roles which can be assigned to users and delete default job roles that are not relevant to your organization. For information about administrative access in Workfront, see [Grant users administrative access to certain areas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Access requirements

You must have the following:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to Job roles</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Create a job role

<ol data-mc-continue="false"> Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Setup . 
 <li value="2">In the left panel, click<span class="bold"> Job Roles.</span></li> 
 <li value="3"> <p>Click <span class="bold">New Job Role.</span></p>   </li> 
 <li value="4"> <p>Update the following fields: </p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Name</td> 
     <td> <p>Indicate a name for the job role.&nbsp;This is the name that displays everywhere in&nbsp;Workfront where the Job&nbsp;Role field displays. </p> <note type="tip">
       The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of Workfront. 
      </note> </td> 
    </tr> Is Active Select Yes if you want the role to be active and available everywhere in Workfront to be associated with users, work items, etc. Select No, if you want the role to be deactivated and not available to assign to users, work items, etc. For information about deactivating job roles, see Deactivate job roles. 
    <tr> 
     <td role="rowheader">Description</td> 
     <td>Enter a description for the role that indicates what is unique about it. </td> 
    </tr> Base Currency This is the Base Currency, as set in the Setup area by your Workfront administrator. For information, see Set up exchange rates . Tip: You cannot edit the Base Currency at the job role level. This field is dimmed and serves as a reminder for what the base currency is for your system. 
    <tr> 
     <td role="rowheader">Cost/ Hr.</td> 
     <td>This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. <span>Enter the rate using the Base Currency.</span> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Bill/ Hr. </td> 
     <td>This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the Base Currency. </td> 
    </tr> Override Currency Select a currency associated with this job role. This is the currency that Workfront uses for calculating costs and revenue associated with this job role. This is a different than the Base Currency set up by your Workfront administrator in the Setup area, and can be different than the currency associated with a project. Tip: Only currencies available in the Exchange Rates area in your system are available in this field. For information about setting up the Base Currency in Workfront, see Set up exchange rates. For information about changing the currency of a project, see Change the project currency. Override Currency Cost/ Hour This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. Enter the rate in the Override Currency specified above. This also updates the Cost/ Hour rate for this job role when using the Base Currency. For information about how Workfront calculates cost, see Track costs. Tip: When updating an existing job role that already has a Cost/ Hour rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost/ Hour, the Cost/ Hour of the job role also updates automatically. Override Currency Billing/ Hour This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. Enter the rate in the Override Currency specified above. This also updates the Billing/ Hour rate for this job role when using the Base Currency. For information about how Workfront calculates revenue, see Overview of Billing and Revenue. Tip: When updating an existing job role that already has a Billing/ Hour rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing/ Hour, the Billing/ Hour of the job role also updates automatically. 
   </tbody> 
  </table> <note type="tip">
   Job roles are an integral&nbsp;part of managing resources. To use the resource planning tools, job roles need a cost and billing rate associated with them. For information, see 
   <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md" class="MCXref xref">Get started with Resource Management </a>. 
  </note> </li> 
 <li value="5"> <p>Click <span class="bold">Create Job Role</span>. The job role is now available to be assigned to tasks, issues, approvals, or you can share layout templates or other objects with it. For information about all uses of job roles in&nbsp;Workfront, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md" class="MCXref xref">Job role overview</a>. For information about deleting a job role, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md" class="MCXref xref">Delete job roles</a>. </p> </li> 
</ol>

<!--
Delete a job role Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Setup . Click Job Roles. Select the job role that you want to delete, then click Delete. If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following: Replace the job role with a different job role: Select the new job role from the drop-down list. Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select. Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select. Delete the job role and its resource allocation: Select None from the drop-down list. Important: Deleting a job role deletes all current and past resource allocation related to that job role for all projects. For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted. Click Yes, Delete It.
-->

##  

