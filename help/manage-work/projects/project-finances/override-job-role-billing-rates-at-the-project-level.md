---
filename: override-job-role-billing-rates-at-the-project-level
product-area: projects
navigation-topic: financials
title: Override Job Role Billing Rates at the project level
description: As a project manager, you can specify what the billing rate is for a job role on a specific project. This project-level billing rate overrides the billing rate at the system level for this job role. Workfront uses the project-level billing rate of the job role to calculate revenue, instead of using the system-level billing rate.
---

# Override Job Role Billing Rates at the project level

As a project manager, you can specify what the billing rate is for a job role on a specific project. This project-level billing rate overrides the billing rate at the system level for this job role. `Workfront` uses the project-level billing rate of the job role to calculate revenue, instead of using the system-level billing rate.

This article describes how you can override the system job role billing rates for a project.

For general information about overriding job role billing rates for projects and calculating project&nbsp;Revenue, see [Overview of overriding Job Role Billing Rates and calculating Revenue on a project](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

For more information about which job role is used to calculate revenue on the project, see the "Understanding Revenue Calculations for Tasks Based on User and Role Assignments" section in the article [Overview of Billing and Revenue](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>In the case of Actual Revenue, the billing rates applied to hours that are added to a Billing Record which is marked as Billed, should not be affected by billing rate overrides that occur after the Billing Record has been billed.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Financial Data</p> <p>Administrative access for Job&nbsp;roles</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project that includes Edit Financial&nbsp;Data </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Override Job Role Billing Rates at the project level

You can override the billing rate of a job role on a project in the following ways:

* One time, by selecting a new rate for the job role.  
  The new rate is used for the entire duration of the project, to calculate revenue.

* Several times, by selecting several new rates for specific date ranges.   
  A different rate can be used during each specified date range.

>[!TIP]
>
>You cannot override user billing rates for a project.

To override a billing rate for a project:

<ol> 
 <li value="1">Go to the project you want to override billing rates for.</li> 
 <li value="2"> Click Billing Rates in the left panel. You might have to first click Show More. </li> 
 <li value="3">Click <span class="bold">Add Billing Rate</span>.</li> 
 <li value="4">Click <span class="bold">New Billing Rate</span>.</li> 
 <li value="5">In the <span class="bold">Job Role</span> field, select the job role you want to change the billing rate for.<br><img src="assets/new-billing-rate-350x267.png" alt="new_billing_rate.png" style="width: 350;height: 267;"><br>The <span class="bold">Default Billing Rate</span> field displays the system-level rate for this job role.</li> 
 <li value="6">In the <span class="bold">Billing Rates 1</span> field, enter the one time billing rate override, then click <span class="bold">Save</span> to override the billing rate one time, <br>Or Click <span class="bold">Add Rate</span> to add more billing rate overrides.</li> 
 <li value="7">(Conditional) If you are adding more than one billing rate override, specify the following information:<br>- <span class="bold">Billing Rates 1</span>: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the <span class="bold">Default Rate</span>.<br>- <span class="bold">Start Date</span>: this is the date when the Default Rate ends.<br>- <span class="bold">End Date</span>: the date when the new billing rate override ends. <br><img src="assets/new-billing-rate-with-adjustment-dates-350x266.png" alt="new_billing_rate_with_adjustment_dates.png" style="width: 350;height: 266;"><br><span>Workfront</span> applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.<br>There should be no gaps between the time frames of two override rates. The <span class="bold">Start Date</span> of an override rate should be the day immediately following the <span class="bold">End Date</span> of the previous override date.<br><note type="note">
    You cannot specify a 
   <span class="bold">Start Date</span> for the first override rate, nor an 
   <span class="bold">End Date</span> for the last override rate. We recommend that you use the Default Rate for the first override rate.
   <br>
   <span>Workfront</span> assumes that the first override rate is applied for all hours with a date older than the
   <span class="bold"> End Date</span> of the first override, and that the last override rate is applied for all hours with a date newer than the 
   <span class="bold">Start Date</span> of the last override.
   <br>If an hour is logged before the Planned Start Date of the project the very first billing rate is used.
   <br>If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.
  </note><br></li> 
 <li value="8">Click <span class="bold">Save</span>.</li> 
</ol>

