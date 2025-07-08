---
navigation-topic: financials
title: Create Billing Records
description: In addition to setting up revenue and tracking expenses, you can create billing records on a project for information that needs to be billed.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
---
# Create billing records

 <!-- Audited: 6/2025 -->

In addition to setting up revenue and tracking expenses, you can create billing records on a project for information that needs to be billed.

You can't create billing records for tasks; you can only create billing records for projects.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>New: Standard</p>
   <p>or</p>
   <p>Current: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>Edit access to Projects and Financial Data</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>Manage permissions to the project with permissions to Manage Finance</td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Billing records overview

Billing records are created as attachments to a project and contain financial data from the project as well as the project tasks' financial information.

Consider the following when planning to use billing records:

* You create a billing record when you want to bill an amount of money related to the project to an external vendor or partner. In addition to billing a fixed amount to an external source, there are times when you need to bill out the amount of work on the project (from logged hours) to an external contractor, as well as the expenses incurred or the amount of fixed revenues. You can include all this information in the same billing record.
* Once a billing record is set to Billed, it can't be edited.

  >[!IMPORTANT]
  >
  >This is important when your rates vary and you want to lock the revenue and expense information on your project. Adding it to a billing record and marking it as Billed prevents it from being updated when the rates update in your system.

* A project with billing records that have been marked as Billed can't be deleted.

## Create a billing record

{{step1-to-projects}}

1. On the **Projects** page, select a project.
1. Click **Billing Records** in the left panel.
1. Click **New Billing Record**.
1. In the **New Billing Record** box that displays, specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>(Required) Enter a description for the billing record.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Billing Status</td> 
      <td> <p>Select <strong>Not Billed</strong> if this record hasn't been billed yet.</p> <p>Select <strong>Billed</strong> if the billing record has been billed.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Billing Date</td> 
      <td>Select the date that this billing record was billed by clicking the calendar icon.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">PO Number</td> 
      <td>Enter the PO Number associated with this billing record.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Invoice ID</td> 
      <td>Enter the Invoice associated with this billing record.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Additional Amount</td> 
      <td>Enter the fixed amount of your billing record. This is the amount you intend to bill an external customer, contractor, or partner for this project. This amount can't be modified after the billing record status is changed to Billed.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Under **Custom Forms**, select a billing records custom form that you want to add to the record.

   A billing records custom form must be created before you can select it here. Only active custom forms display in the list. For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click **Save.** The billing record is created. 

## Include Billable Hours, Expenses and Fixed Revenues in a billing record

### Include Billable Hours in a billing record {#include-billable-hours-in-a-billing-record}

You can include hours that have been logged on tasks, issues, or the project in your billing records.

If the user who logs the hours or their Primary Job Role is associated with a Billing per Hour Rate, the revenue from these hours is added to the billing record.

* [What hours can be added to a billing record](#what-hours-can-be-added-to-a-billing-record) 
* [Add Hours to a billing record](#add-hours-to-a-billing-record)

#### What hours can be added to a billing record {#what-hours-can-be-added-to-a-billing-record}

You can add hours to a billing record when the following conditions are met:

* Hours have been logged for the tasks, issues, or project.
* The Hour Type of the hours logged is marked as Count as Revenue.

  For more information, see the article [Manage hour types](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* All hours logged for issues or the project can be added to a billing record if the user who logs the time has a Billing per Hour rate associated with them or their Primary Job Role. 
* If the hours are logged on a task, the task must have the following Revenue Type:

   * The Revenue Type can't be set to Not Billable.
   * If the Revenue Type is set to User Hourly, the user who logs the time must have a Billing per Hour rate set in their profile. 
   * If the Revenue Type is set to Role Hourly, the Primary Role of the user who logs the time must have a Billing per Hour rate.

     >[!NOTE]
     >
     >You can override billing rates for job roles at the project level.  
     >For more information, see the section Overriding Job Role Billing Rates at the Project Level in the article [Overview of overriding Job Role Billing Rates and calculating Revenue on a project](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* If the Require time to be approved for this project option is checked under Project Settings, then the Project Owner must approve the hours logged.  
  For more information, see [Require time to be approved for a project](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Add hours to a billing record {#add-hours-to-a-billing-record}

{{step1-to-projects}}

1. On the **Projects** page, select a project.
1. Click **Billing Records** in the left panel.
1. Click the billing record **Description** to open the **Billing Record Details** tab.
1. Click **Billable Hours** in the left panel.
1. If there are hours that could be included in a billing record, click **Add Hours**. The **Add Billable Hours** box opens.

   >[!NOTE]
   >
   >If there are no hours logged or if the hours logged don't meet the conditions required to be added to a billing record, the **Add Hours** button will not display. For more information, see the following section in this article: [What hours can be added to a billing record](#what-hours-can-be-added-to-a-billing-record).

1. Select the hour entries you want to include in the billing record, then click **Add Hours**. The Actual Cost of the hours is added as the **Billable Hours** amount to the **Billing Record Total**. 

1. (Optional) Click **Billing Records Details** to review the **Billable Hours** and **Billing Record Total** amounts, and the billing record total in the billing record header.

### Include Billable Expenses in a billing record {#include-billable-expenses-in-a-billing-record}

If you are adding Billable Expenses to the billing record, ensure the expenses on the tasks and the project are marked as Billable. Expenses that are not marked as Billable are not available to add in a billing record. For more information about adding expenses, see the article [Manage project expenses](../../../manage-work/projects/project-finances/manage-project-expenses.md).

To add billable expenses to a billing record:

{{step1-to-projects}}

1. On the **Projects** page, select a project.
1. Click **Billing Records** in the left panel.
1. Click the billing record **Description** to open the **Billing Record Details** tab.
1. Click **Billable Expenses** in the left panel. 
1. (Conditional) If you've added expenses to your tasks or the project and marked them as Billable, click **Add Expenses**.

   >[!NOTE]
   >
   >If you have expenses but they're not marked as Billable, the **Add Expenses** button does not display. Only billable expenses with an Actual Amount greater than zero are eligible to be included in a billing record.

1. Select the billable expenses that are available to be added to the billing record, then click **Add Expenses**.  The Actual Amount of the expenses is added as the **Billable Expenses** amount to the **Billing Record Total**.

1. (Optional) Click **Billing Records Details** to review the **Billable Expenses** and **Billing Record Total** amounts, and the billing record total in the billing record header.

### Include Fixed Revenues in a billing record {#include-fixed-revenues-in-a-billing-record}

You can add Fixed Revenues to your billing records if you have tasks that have Fixed Revenue available. No other type of task or project revenue is available to be added in a billing record. For more information about revenue types, see the Overview of Billing and Revenue section in the article [Overview of Billing and Revenue](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

{{step1-to-projects}}

1. On the **Projects** page, select a project.
1. Click **Billing Records** in the left panel.
1. Click the billing record's **Description** to open the **Billing Record Details** tab.
1. Select the **Fixed Revenues** tab.
1. If you have added fixed revenues to your tasks, click **Add Fixed Revenues**.

   >[!NOTE]
   >
   >If you have revenue amounts on tasks but they aren't marked as Fixed, the **Add Fixed Revenue** button will not display.

1. Select the tasks whose fixed revenues you want to include in the billing record, then click **Add Tasks**.  The **Fixed Revenue** amount of the tasks is added as the **Billable Revenues** amount to the **Billing Record Total**.

1. (Optional) Click **Billing Records Details** to review the **Billable Revenues** and **Billing Record Total** amounts, and the billing record total in the billing record header.

## Edit a billing record

After creating a billing record and adding hours, expenses, and revenues to it, you can edit some information on the existing record before it's marked as Billed.

1. Navigate to the billing record.
1. Select **Billing Record Details** in the left panel.
1. Edit information in any available fields.

   Or

   Click the **Edit** icon ![Edit icon](assets/edit-icon.png) in the upper-right corner, then edit information in any available fields.

   Update the following:

   * **Description** 
   * **Billing Date**
   * **Billing Status**

     >[!TIP]
     >
     >If you select **Billed** for the Billing Status, the billing record can't be edited after you save your changes.
 
   * **Invoice ID** 
   * **PO Number** 
   * **Additional Amount**

   The following fields are not available for editing:

   * **Billable Hours:** The total of the Actual Revenue of the hours included in the billing record. For more information, see the following section in this article: [Include Billable Hours in a billing record](#include-billable-hours-in-a-billing-record).
   
   * **Billable Expenses**: The total of the Actual Amount of the billable expenses included in the billing record. For more information, see the following section in this article: [Include Billable Expenses in a billing record](#include-billable-expenses-in-a-billing-record).
   
   * **Billable Revenues**: The total of the Fixed Revenue of the tasks included in the billing record. For more information, see the following section in this article: [Include Fixed Revenues in a billing record](#include-fixed-revenues-in-a-billing-record).
   
   * **Billing Record Total**: The total of all billable amounts. This is calculated by the following formula:

     ```   
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Click **Save Changes**.
