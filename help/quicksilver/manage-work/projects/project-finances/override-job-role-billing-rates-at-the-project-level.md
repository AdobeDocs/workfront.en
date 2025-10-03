---
product-area: projects
navigation-topic: financials
title: Override Job Role Billing Rates at the Project Level
description: As a project manager, you can specify what the billing rate is for a job role on a specific project. This project-level billing rate overrides the billing rate at the system level for this job role. Workfront uses the project-level billing rate of the job role to calculate revenue, instead of using the system-level billing rate.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
---
# Override Job Role Billing Rates at the project level

{{highlighted-preview}}

As a project manager, you can specify what the billing rate is for a job role on a specific project. This project-level billing rate overrides the billing rate at the system level for this job role. Workfront uses the project-level billing rate of the job role to calculate revenue, instead of using the system-level billing rate.

This article describes how you can override the system job role billing rates for a project.

For general information about overriding job role billing rates for projects and calculating project&nbsp;Revenue, see [Overview of overriding Job Role Billing Rates and calculating Revenue on a project](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

For more information about which job role is used to calculate revenue on the project, see the "Understanding Revenue Calculations for Tasks Based on User and Role Assignments" section in the article [Overview of Billing and Revenue](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>In the case of Actual Revenue, the billing rates applied to hours that are added to a Billing Record which is marked as Billed, should not be affected by billing rate overrides that occur after the Billing Record has been billed.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td> <p>Edit access to Projects and Financial Data</p> <p>Administrative access for job roles</p></td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td>Manage permissions to the project that includes Edit Financial Data </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Override Job Role Billing Rates at the project level

You can override the billing rate of a job role on a project in the following ways:

* One time, by selecting a new rate for the job role.  
  The new rate is used for the entire duration of the project, to calculate revenue.

* Several times, by selecting several new rates for specific date ranges.   
  A different rate can be used during each specified date range.

* You can add new billing rates to a project template and those become project billing rates when you create the project from that template. For information about editing templates, see [Edit project templates](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md). 

>[!TIP]
>
>You cannot override user billing rates for a project.

To override a billing rate for a project:

1. Go to the project you want to override billing rates for.
1. Click **Billing Rates** in the left panel.
1. Click **Add Billing Rate** > **New Billing Rate**.

   The New Billing Rate box opens. 

1. In the **Job Role** field, select the job role you want to change the billing rate for.

   The **Default Billing Rate** field displays the system-level rate for this job role.

1. In the **Billing Rates 1** field, enter the one time billing rate override, then click **Save** to override the billing rate one time

   Or

   Click **Add Rate** to add more billing rate overrides.

1. (Conditional) If you are adding more than one billing rate override, specify the following information:

   * **Billing Rates 1**: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the **Default Rate**.
   * **Start Date**: this is the date when the Default Rate ends.
   * **End Date**: the date when the new billing rate override ends.

   <span class="preview">Sample image in the Preview environment:</span>
   ![Billing rates with override dates](assets/billing-rates-093025.png)

   Sample image in the Production environment:
   ![Billing rates with override dates](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. The timezone for the dates you select displays at the bottom of the New Billing Rate box. This is the timezone associated with your Workfront&nbsp;instance, as shown in the Customer Info area of Setup. For information, see [Configure basic information for your system](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. Workfront applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.
1. There should be no gaps between the time frames of two override rates. The **Start Date** of an override rate should be the day immediately following the **End Date** of the previous override date.

1. You cannot specify a Start Date for the first override rate, nor an End Date for the last override rate.   
   We recommend that you use the Default Rate for the first override rate.   
   Workfront assumes that the first override rate is applied for all hours with a date older than the End Date of the first override, and that the last override rate is applied for all hours with a date newer than the Start Date of the last override.   
   If an hour is logged before the Planned Start Date of the project the very first billing rate is used.   
   If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.

1. Click **Save**.
