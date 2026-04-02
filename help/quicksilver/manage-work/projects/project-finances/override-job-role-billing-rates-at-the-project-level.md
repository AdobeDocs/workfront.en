---
product-area: projects
navigation-topic: financials
title: Override Job Role Billing Rates at the Project Level
description: As a project manager, you can specify what the billing rate is for a job role on a specific project. This project-level billing rate overrides the billing rate at the system level for this job role. Workfront uses the project-level billing rate of the job role to calculate revenue, instead of using the system-level billing rate.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
---
# Override Job Role Billing Rates at the project level

{{highlighted-preview}}

As a project manager, you can specify what the billing rate is for a job role on a specific project. This project-level billing rate overrides the billing rate at the system level for this job role. Workfront uses the project-level billing rate of the job role to calculate revenue, instead of using the system-level billing rate.

This article describes how you can override the system job role billing rates for a project.

For general information about overriding job role billing rates for projects and calculating project Revenue, see [Overview of overriding billing rates and calculating revenue on a project](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

For more information about which job role is used to calculate revenue on the project, see [Overview of revenue and cost hierarchy](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) and the [Revenue Calculations for Tasks Based on User and Role Assignments](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) section in the article [Overview of Billing and Revenue](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

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
   <td> <p>To override a job role billing rate for a project:: Any Workfront or Workflow package</p>
        <p>To apply attributes to the job role: Workflow Ultimate</p> </td> 
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

When you override the billing rate of a job on a project, you can assign effective dates and each date range has a different rate. If you do not assign effective dates, then the billing rate override you enter is used for the entire duration of the project to calculate revenue.

You can add new billing rates to a project template and those become project billing rates when you create the project from that template. For information about editing templates, see [Edit project templates](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md). 

>[!TIP]
>
>You cannot override user billing rates for a project unless you have the Workflow Ultimate package.

To override a billing rate for a project:

1. Go to the project you want to override billing rates for.
1. Click **Billing Rates** in the left panel.

   Or

   <span class="preview">Click **Rates** in the left panel and click the **Billing** tab if it is not already selected.</span>

1. Click **Add Billing Rate** > **New Billing Rate**.

   Or

   <span class="preview">Click **Add Billing Rate > New Job Role Billing Rate**.</span>

   The New Billing Rate box opens. 

1. In the **Job Role** field, select the job role you want to change the billing rate for.

1. <span class="preview">(Optional) Select any attributes for the billing rate, such as agency or location.</span>

   <span class="preview">The system administrator defines rate attributes in the Setup area.</span>

1. Select the **Currency** for the billing rate override.
1. In the **Billing Rate** field, enter the billing rate override, then click **Save** to override the billing rate one time

   Or

   Click **Add Rate** to add more billing rate overrides.

1. (Conditional) For date effective billing rate overrides, enter the following information for each row:

   * **Billing Rate**: The value of the Billing Rate from the beginning of the project to the first date of the first override.
   * **Start Date**: The date when the billing rate override begins.
   * **End Date**: The date when the billing rate override ends.

   ![Billing rates with override dates](assets/new-job-role-billing-rate-on-project2.png)

   Workfront applies the override job role rate to the hours that occur during these time frames when calculating revenue on the project.

   Workfront allows you to leave gaps between override timeframes, but you will receive a warning to confirm this is intentional.
   
   You are not required to specify a Start Date for the first override rate, nor an End Date for the last override rate.

   If you enter only one billing rate override, that rate applies for the entire duration of the project. If you add multiple date-effective overrides, Workfront assumes that the first override applies to all hours before its End Date, and the last override applies to all hours after its Start Date.
   
   Workfront assumes that the first override rate is applied for all hours with a date older than the End Date of the first override, and that the last override rate is applied for all hours with a date newer than the Start Date of the last override.

   If an hour is logged before the Planned Start Date of the project, the very first billing rate is used.

   If an hour is logged after the Planned Completion Date of the project, the very last billing rate is used.

1. Click **Save**.
