---
content-type: overview
product-area: projects
navigation-topic: financials
title: Override User Cost Rates at the Project Level
description: This article describes how you can override the system user cost rates for a project.
author: Lisa
feature: Work Management
exl-id: ff1110fd-2d24-48a7-8000-712e551ca61a
---
# Override user cost rates at the project level

You can specify what the cost rate is for a user on a specific project. This project-level cost rate overrides the cost rate at the system level for this user. Workfront uses the project-level cost rate of the job role to calculate cost, instead of using the system-level cost rate.

This article describes how you can override the system user cost rates for a project.

For more information about calculating cost on the project, see [Overview of revenue and cost hierarchy](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) and [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

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

## Prerequisites

The user must have the **Cost rate override allowed** field enabled on their user profile. When a user does not have the cost override field enabled, cost overrides are not allowed for that user on any project, and the system uses the rate on the user profile to calculate cost.

For more information, see [Edit a user's profile](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Override user cost rates at the project level

1. Go to the project you want to override cost rates for.
1. Click **Rates** in the left panel. You might have to first click **Show More**.
1. Click the **Cost** tab if it is not already selected.
1. Click **Add Cost Rate** > **New User Cost Rate**.

   The New User Cost Rate box opens.

1. In the **User** field, select the user you want to change the cost rate for.
1. Select the **Currency** for the cost rate override.
1. In the **Cost Rate** field, enter the first cost rate override.
1. (Optional) Click **Add date effective rate** to add more cost rate overrides.

   >[!NOTE]
   >
   >If you enter a single rate override, it applies for the entire life of the project.
   >If you want to have different rates over time, you can add multiple date-effective overrides.

1. (Conditional) If you are adding multiple cost rate overrides, specify the following information for each row:

   * **Cost Rate**: the value of the cost rate during the specified time period.
   * **Start Date**: the date when the cost rate override begins.
   * **End Date**: the date when the cost rate override ends.

   ![New User Cost Rate box showing effective dates](assets/new-user-cost-rate-box.png)

   Workfront applies the override job role rate to the hours that occur during these time frames when calculating cost on the project.

   There should be no gaps between the time frames of two override rates. The **Start Date** of an override rate should be the day immediately following the **End Date** of the previous override date.

   You are not required to specify a Start Date for the first override rate, nor an End Date for the last override rate.

   We recommend that you use the Default Rate for the first override rate.
   
   Workfront assumes that the first override rate is applied for all hours with a date older than the End Date of the first override, and that the last override rate is applied for all hours with a date newer than the Start Date of the last override.

   If an hour is logged before the Planned Start Date of the project, the very first cost rate is used.

   If an hour is logged after the Planned Completion Date of the project, the very last cost rate is used.

1. Click **Save**.
