---
content-type: overview
product-area: projects
navigation-topic: financials
title: Override User Billing Rates at the Project Level
description: This article describes how you can override the system user billing rates for a project.
author: Lisa
feature: Work Management
exl-id: eb7dbb6f-a31c-4569-be54-9a151dcf4135
---
# Override user billing rates at the project level

{{highlighted-preview-article-level}}

As a project manager, you can specify what the billing rate is for a user on a specific project. This project-level billing rate overrides the billing rate at the system level for this user. Workfront uses the project-level billing rate of the user to calculate revenue, instead of using the system-level billing rate.

This article describes how you can override the system user billing rates for a project.

For general information about overriding billing rates for projects and calculating project revenue, see [Overview of overriding billing rates and calculating revenue on a project](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

For more information about calculating revenue on the project, see [Overview of revenue and cost hierarchy](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) and the [Revenue Calculations for Tasks Based on User and Role Assignments](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) section in the article [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

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
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td> <p>Edit access to Projects and Financial Data</p>
       <p><p>You must also have one of the following:</p> 
        <ul> 
          <li> <p>The System Administrator access level. </li> 
          <li> <p><b>Users</b> setting in your access level configured to <b>Edit</b> access, with <b>Create</b> and at least one of the two <b>User Admin</b> options enabled under <b>Fine-tune your settings</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Of these two options, if <b>User Admin (Group Users)</b> is enabled, you must be a group administrator of a group where the user is a member.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td>Manage permissions to the project that includes Edit Financial Data </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Override User Billing Rates at the project level

When you override the billing rate of a user on a project, you can assign effective dates and each date range has a different rate. If you do not assign effective dates, then the billing rate override you enter is used for the entire duration of the project to calculate revenue.

To override a user billing rate for a project:

1. Go to the project you want to override billing rates for.
1. Click **Rates** in the left panel. You might have to first click **Show More**.
1. Click the **Billing** tab if it is not already selected.
1. Click **Add Billing Rate** > **New User Billing Rate**.

   The New User Billing Rate box opens.

1. In the **User** field, select the user you want to change the billing rate for.
1. Select the **Currency** for the billing rate override.
1. In the **Billing Rate** field, enter the first billing rate override.
1. (Optional) Click **Add date effective rate** to add more billing rate overrides.
1. (Conditional) If you are adding multiple billing rate overrides, specify the following information for each row:

   * **Billing Rate**: the value of the billing rate during the specified time period.
   * **Start Date**: the date when the billing rate override begins.
   * **End Date**: the date when the billing rate override ends.

   ![New User Billing Rate box showing effective dates](assets/new-user-billing-rate-on-project2.png)

   Workfront applies the override user rate to the hours that occur during these time frames when calculating revenue on the project.

   Workfront allows you to leave gaps between override timeframes, but you will receive a warning to confirm this is intentional.

   You are not required to specify a Start Date for the first override rate, nor an End Date for the last override rate.

   If you enter only one billing rate override, that rate applies for the entire duration of the project. If you add multiple date-effective overrides, Workfront assumes that the first override applies to all hours before its End Date, and the last override applies to all hours after its Start Date.

   Workfront assumes that the first override rate is applied for all hours with a date older than the End Date of the first override, and that the last override rate is applied for all hours with a date newer than the Start Date of the last override.

   If an hour is logged before the Planned Start Date of the project, the very first billing rate is used.

   If an hour is logged after the Planned Completion Date of the project, the very last billing rate is used.

1. Click **Save**.
