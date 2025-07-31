---
product-area: projects
navigation-topic: financials
title: Manage Project Expenses
description: The process for creating and managing expenses is the same for both project and task-related expenses. Any expenses that are added to the project in the Business Case are added to the Expenses tab as planned expenses. 
author: Lisa
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
---
# Manage project expenses

<!-- Audited: 6/2025 -->

The process for creating and managing expenses is the same for both project and task-related expenses. Any expenses that are added to the project in the Business Case are added to the Expenses tab as planned expenses. For more information, see [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

The total amount of your expenses from all the tasks and project contributes to the total cost of the project. The Planned Amount of the expenses contributes to the Planned Cost of the project, and the Actual Amount of the expenses contributes to the project's Actual Cost.

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
   <p>Current: Work or higher</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>Edit access to Projects and Financial Data</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>Contribute or higher permissions to the project with permissions to View or Manage Finance</td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Add Expenses

1. Go to the project or task you want to enter expenses for.
1. Click **Expenses** in the left panel.
1. Click **Add an Expense**. The **Add an Expense** dialog box appears.
1. Enter the following information:

   * **Description:** Enter a description of the expense.
   * **Expense Type:** (Required) Select the category that best describes the expense.
   * **Task:** Type in the name of the task that this expense is associated with, then click it when it appears in the drop-down list.
   * **Planned Amount:** Enter the planned budgeted amount for the expense. This affects the Budgeted Cost of the project.
   
   * **Actual Amount:** Enter the amount that the expense actual cost. This affects the Actual Cost of the project.
   
   * **Planned Date:** Enter the expected date for the expense to occur. You can type the date in the field using the *mm/dd/yy* format, or you can click the **Calendar** icon ![Calendar icon](assets/calendar-icon.png) and select the date dynamically.
   
   * **Date Paid:** Enter or select the date the expense was paid.
   * **Billable:** Select this option if you want to bill this expense. Categorizing an expense as billable is important when creating billing records.
   * **Reimbursable:** Select this option if the expense needs to be reimbursed. You can then mark the expense as reimbursed after the expense has been reimbursed.

1. Select a **Custom Form** and specify any additional information required.

    >[!NOTE]
    >
    >You must create a custom form before you can associate it with an expense. Only active custom forms display in the list. For information about creating custom forms, see the article [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click **Save**.

## Delete Expenses

1. Go to the project you want to delete an expense for.
1. Click **Expenses** in the left panel.
1. Select the expense that you want to delete, then click the **Delete** icon ![Delete](assets/delete.png).
1. In the **Delete Expense** dialog, click **Yes, Delete It**.
