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

1. Setup
1. In the left panel, click**Job Roles.**
1. Click **New Job Role.**

   ![](assets/new-job-role-box-with-currency-override-classic-350x273.png)

1. Update the following fields: 

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>Indicate a name for the job role.&nbsp;This is the name that displays everywhere in&nbsp;Workfront where the Job&nbsp;Role field displays. </p> <p>Tip: The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of Workfront. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Is Active</span> </td> 
      <td> 
       <ul> 
        <li> <p>Select <strong>Yes</strong> if you want the role to be active and available everywhere in Workfront to be associated with users, work items, etc. </p> </li> 
        <li> <p>Select <strong>No</strong>, if you want the role to be deactivated and not available to assign to users, work items, etc. </p> </li> 
       </ul> <p><span>For information about deactivating job roles, see</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deactivate job roles</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Enter a description for the role that indicates what is unique about it. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Base Currency</span> </td> 
      <td> <p><span>This is the Base Currency, as set in the Setup area by your Workfront administrator. For information, see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a> .</p> <p>Tip: <span>You cannot edit the Base Currency at the job role level.&nbsp;This field is dimmed and serves as a reminder for what the base currency is for your system.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cost/ Hr.</td> 
      <td>This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. <span>Enter the rate using the Base Currency.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bill/ Hr. </td> 
      <td>This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the Base Currency. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Override Currency</span> </td> 
      <td> 
       <div> 
        <p>Select a currency associated with this job role. This is the currency that Workfront uses for calculating costs and revenue associated with this job role. </p> 
        <p><span>This is a different than the Base Currency set up by your Workfront administrator in the Setup area, and can be different than the currency associated with a project.</span> </p> 
        <p>Tip: Only currencies available in the Exchange Rates area in your system are available in this field.</p> 
       </div> <p><span>For information about setting up the Base Currency in Workfront, see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <p><span>For information about changing the currency of a project, see</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Change the project currency</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Override Currency Cost/ Hour</span> </td> 
      <td> 
       <div> 
        <p>This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. </p> 
        <p><span>Enter the rate in the Override Currency specified above. This also updates the Cost/ Hour rate for this job role when using the Base Currency.</span> </p> 
        <p>For information about how Workfront calculates cost, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> 
       </div> <p>Tip: When updating an existing job role that already has a Cost/ Hour rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost/ Hour, the Cost/ Hour of the job role also updates automatically.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Override Currency Billing/ Hour</span> </td> 
      <td> 
       <div> 
        <p>This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. </p> 
        <p><span>Enter the rate in the Override Currency specified above. This also updates the Billing/ Hour rate for this job role when using the Base Currency.</span> </p> 
        <p>For information about how Workfront calculates revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> 
       </div> <p>Tip: When updating an existing job role that already has a Billing/ Hour rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing/ Hour, the Billing/ Hour of the job role also updates automatically. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Job roles are an integral&nbsp;part of managing resources. To use the resource planning tools, job roles need a cost and billing rate associated with them. For information, see [Get started with Resource Management](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Click **Create Job Role**. The job role is now available to be assigned to tasks, issues, approvals, or you can share layout templates or other objects with it. For information about all uses of job roles in&nbsp;Workfront, see [Job role overview](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). For information about deleting a job role, see [Delete job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="deleting-a-job-role"></a>Delete a job role</h2>
<ol data-mc-continue="false"> Click <strong>Setup</strong> near the upper-right corner of Adobe Workfront on the Global Navigation Bar.
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that&nbsp;are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are&nbsp;associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to&nbsp;them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong>&nbsp;from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Delete It.</strong> </li>
</ol>
</div>
-->

##  

