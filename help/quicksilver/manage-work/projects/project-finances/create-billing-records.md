---
navigation-topic: financials
title: Create billing records
description: In addition to setting up revenue and tracking expenses, you can create billing records on a project for information that needs to be billed.
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
---
# Create billing records

In addition to setting up revenue and tracking expenses, you can create billing records on a project for information that needs to be billed.

You cannot create billing records for tasks. You can only create billing records for projects.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Financial&nbsp;Data</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Billing records overview

Billing records are created as attachments to a project and contain financial data from the project as well as some financial information for the tasks in a project.

Consider the following when planning to use billing records:

* You create a billing record when you want to bill an amount of money related to the project to an external vendor or partner. In addition to billing a fixed amount to an external source, there are times when you need to bill out the amount of work on the project (from logged hours) to an external contractor, as well as the expenses incurred or the amount of fixed revenues. You can include all this information in the same billing record.
* Once a billing record is set to Billed it can not be edited.

  >[!IMPORTANT]
  >
  >This is important when your rates vary and you want to lock the revenue and expense information on your project. Adding it to a billing record and marking it as Billed prevents it from being updated when the rates update in your system.

* A project with billing records that have been marked as Billed cannot be deleted.

## Create a billing record

1. Navigate to a project.
1. Click **Billing Records** in the left panel.

   This section might be located under **Show More**.

1. With **Billing Record Details** selected in the left panel, click **New Billing Record**.
1. In the **New Billing Record** box that displays, specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>This is a required field. Specify a description for the billing record, to reflect the purpose or the intent for this record.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Billing Status</td> 
      <td> <p>Select <strong>Not Billed</strong>, if this record has not been billed yet.</p> <p>Select <strong>Billed</strong> when the billing record is billed.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Billing Date</td> 
      <td>Select the date for when this billing record is billed, by clicking the calendar icon.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">PO Number</td> 
      <td>If there is a PO Number associated with this billing record, specify this information in this field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Invoice ID</td> 
      <td>If there is an Invoice associated with this billing record, specify this information in this field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Additional Amount</td> 
      <td>Enter the fixed amount of your billing record. This is the amount you intend to bill an external customer, contractor or partner for this project. This amount cannot be modified after the status of the billing record is changed to Billed.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Under **Custom Forms**, select a billing records custom form that you want to add to the billing record.

   You (or another user with access to custom forms) must create a billing records custom form before you can select it here. Only active custom forms display in the list. For information about creating custom forms, see [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   You can repeat this step to add other custom forms that you need for the billing record.

1. Click **Save.**

   The billing record is created. To include Billable Hours, Expenses and Fixed Revenues in the billing record, follow the steps outlined in the following sub-section.

## Include Billable Hours, Expenses and Fixed Revenues in a billing record

* [Include Billable Hours in a billing record](#include-billable-hours-in-a-billing-record) 
* [Include Billable Expenses in a billing record](#include-billable-expenses-in-a-billing-record) 
* [Include Fixed Revenues in a billing record](#include-fixed-revenues-in-a-billing-record)

### Include Billable Hours in a billing record {#include-billable-hours-in-a-billing-record}

You can include hours that have been logged on tasks, issues, or the project in your billing records.  
If the user who logs the hours or their Primary Job Role is associated with a Billing per Hour Rate, the revenue from these hours is added to the billing record.

* [What hours can be added to a billing record](#what-hours-can-be-added-to-a-billing-record) 
* [Add Hours to a billing record](#add-hours-to-a-billing-record)

#### What hours can be added to a billing record {#what-hours-can-be-added-to-a-billing-record}

You can add hours to a billing record when the following conditions are met:

* Tasks, issues, or the project have hours logged. 
* The Hour Type of the hours logged is marked as Count as Revenue.

  For more information about Hour Types, see the article [Manage hour types](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* All hours logged for issues or for the project can be added to a billing record if the user who logs the time has a Billing per Hour rate associated with them or their Primary Job Role. 
* If the hours are logged on a task, the task must have the following Revenue Type:

   * The Revenue Type cannot be set to Not Billable.
   * If the Revenue Type is set to User Hourly, the user who logs the time must have a Billing per Hour rate set in their profile. 
   * If the Revenue Type is set to Role Hourly, the Primary Role of the user who logs the time must have a Billing per Hour rate.

     >[!NOTE]
     >
     >You can override billing rates for job roles at the project level.  
     >For more information about overriding job role billing rates, see the section "Overriding Job Role Billing Rates at the Project Level" in the article [Overview of overriding Job Role Billing Rates and calculating Revenue on a project](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* If **Require time to be approved for this project** is checked under Project Settings, then the Project Owner must approve the hours logged.  
  For more information about requiring approval on project hours, see the article [Require time to be approved for a project](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Add Hours to a billing record {#add-hours-to-a-billing-record}

To add billable hours to a billing record:

1. Go to the project with the billing records.
1. Click **Billing Records** in the left panel.

   This section might be located under **Show More**.

1. Click the **Description** of a billing record to open the **Billing Record Details** tab.

1. Click **Billable Hours** in the left panel.
1. If there are hours that could be included in a billing record, click **Add Hours**.  
   The **Add Billable Hours** box opens.

   >[!NOTE]
   >
   >If there are no hours logged or if the hours logged do not meet the conditions required to be added to a billing record, the **Add Hours** button does not display. For more information about what hours can be logged to a billing record, see the section [What hours can be added to a billing record](#what-hours-can-be-added-to-a-billing-record) in this article.

1. Select the hour entries you want to include in the billing record, and click **Add Hours**.   
   The Actual Cost of the hours is added as the **Billable Hours** amount to the **Billing Record Total**. 

1. (Optional) Click **Billing Records Details** to review the **Billable Hours** and **Billing Record Total** amounts. You can also see the billing record total in the header of the billing record.

### Include Billable Expenses in a billing record {#include-billable-expenses-in-a-billing-record}

If you are adding Billable Expenses to the billing record, ensure the expenses on the tasks and the project are marked as Billable. Expenses that are not marked as Billable are not available to add in a billing record. For more information about adding expenses, see the article [Manage project expenses](../../../manage-work/projects/project-finances/manage-project-expenses.md).

To add billable expenses to a billing record:

1. Go to the project with the billing records.
1. Click **Billing Records** in the left panel.

   You might have to click **Show More**, then **Billing Records**. 

1. Click the **Description** of a billing record to open the **Billing Record Details** tab.

1. Click **Billable Expenses** in the left panel. 
1. (Conditional) If you have added expenses to your tasks or the project and have marked them as Billable, click **Add Expenses**.

   >[!NOTE]
   >
   >If you have expenses but they are not marked as Billable, the **Add Expenses** button does not display. Only billable expenses with an Actual Amount greater than zero are eligible to be included in a billing record.

1. Select the billable expenses that are available to be added to the billing record, then click **Add Expenses**.  
   The Actual Amount of the expenses is added as the **Billable Expenses** amount to the **Billing Record Total**.

1. (Optional) Click **Billing Records Details** to review the **Billable Expenses** and **Billing Record Total** amounts. You can also see the billing record total in the header of the billing record.

### Include Fixed Revenues in a billing record {#include-fixed-revenues-in-a-billing-record}

You can add Fixed Revenues to your billing records if you have tasks that have Fixed Revenue available. No other types of task or project revenue is available to be added in a billing record. For more information about revenue types, see the [Overview of Billing and Revenue](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) section in [Overview of Billing and Revenue](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

To add fixed revenues to a billing record:

1. Go to the project with the billing records.
1. Click **Billing Records** in the left panel.

   You might have to click **Show More**, then **Billing Records**.

1. Click the **Description** of a billing record to open the **Billing Record Details** tab.

1. Select the **Fixed Revenues** tab.
1. If you have added fixed revenues to your tasks, click **Add Fixed Revenues**.

   >[!NOTE]
   >
   >If you have revenue amounts on tasks but they are not marked as "Fixed', the **Add Fixed Revenue** button does not display.

1. Select the tasks whose fixed revenues you want to include in the billing record, then click **Add Tasks**.  
   The **Fixed Revenue** amount of the tasks is added as the **Billable Revenues** amount to the **Billing Record Total**.

1. (Optional) Click **Billing Records Details** to review the **Billable Revenues** and **Billing Record Total** amounts. You can also see the billing record total in the header of the billing record.

## Edit a billing record

After creating a billing record and including hours, expenses and revenues in the billing record, you can edit some information on the existing record, before it is marked as Billed.

1. Go to the billing record.
1. With **Billing Record Details** selected in the left panel , edit information in any available fields

   Or

   Click the **Edit icon** ![](assets/edit-icon.png) in the upper-right corner, then edit information in any available fields.

   Update the following:

   * **Description** 
   * **Billing Status**

     >[!TIP]
     >
     >If you select **Billed** for the Billing Status, the billing record cannot be edited, after you save your changes.

   * **Billing Date** 
   * **PO Number** 
   * **Invoice ID** 
   * **Additional Amount**

   The following fields are not available for editing:

   * **Billable Hours:** The total of the Actual Revenue of the hours included in the billing record. For more information about including hours in a billing record, see the section [Include Billable Hours in a billing record](#include-billable-hours-in-a-billing-record) in this article.
   
   * **Billable Expenses**: The total of the Actual Amount of the billable expenses included in the billing record. For more information about including billable expenses in a billing record, see the section [Include Billable Expenses in a billing record](#include-billable-expenses-in-a-billing-record) in this article.
   
   * **Billable Revenues**: The total of the Fixed Revenue of the tasks included in the billing record. For more information about including fixed revenues in a billing record, see the section [Include Fixed Revenues in a billing record](#include-fixed-revenues-in-a-billing-record) in this article.
   
   * **Billing Record Total**: The total of all billable amounts. This is calculated by the following formula:

     ```   
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Click **Save****Changes**.
