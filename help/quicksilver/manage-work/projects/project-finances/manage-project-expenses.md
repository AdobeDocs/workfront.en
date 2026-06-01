---
product-area: projects
navigation-topic: financials
title: Manage Project Expenses
description: The process for creating and managing expenses is the same for both project and task-related expenses. Any expenses that are added to the project in the Business Case are added to the Expenses tab as planned expenses.
author: Lisa
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
TQID: https://experienceleague.adobe.com/b6lcN97EhJ4bD8w12SRE9TGLycM9Y8Si8ZSm8VBlHlA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
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
   <td>Adobe Workfront package</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td>
   <p>Standard</p>
   <p>Work or higher</p></td> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>Edit access to Projects and Financial Data</td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td>Contribute or higher permissions to the project, with permissions to View or Edit General Finance</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
