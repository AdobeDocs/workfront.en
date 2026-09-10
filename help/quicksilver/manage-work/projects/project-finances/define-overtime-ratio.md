---
content-type: overview
product-area: projects
navigation-topic: financials
title: Define an Overtime Ratio
description: You can define an overtime ratio on a task to adjust the Planned Revenue calculation for the task assignments.
author: Lisa
feature: Work Management
exl-id: 832d3aab-3e09-4d83-91a6-be0145ce3554
---
# Define an overtime ratio

When an overtime ratio is added to a task, it is applied to all assignments on the task. It multiplies all Planned Hours for that task and affects the Planned Revenue calculations.

The overtime ratio cannot vary for assignments within the same task. If different overtime multipliers are required, you must create separate subtasks under a parent task.

>[!NOTE]
>
>There is no validation preventing the overtime ratio from being added to a non-overtime task.

## Overtime calculation on Planned Revenue

The system first determines the billing rate using the standard billing rate hierarchy. For more information, see [Overview of revenue and cost hierarchy](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

If the overtime ratio exists on the task, then the calculation is:
Planned Revenue = Billing Rate × Overtime Ratio × Planned Hours

If the overtime ratio is blank, then the calculation is:
Planned Revenue = Billing Rate × Planned Hours

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
   <td>Edit access to Tasks, Projects, and Financial Data</td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td><p>Manage permissions to a task that include Edit billing rates</p>
     <p>Contribute or higher permissions to the project</p></td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites

The task Revenue Type must be User and Role Hourly. For more information, see [Overview of revenue and cost hierarchy](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

The **Overtime Ratio** field must be enabled on your layout template.

1. In the layout template, click the down arrow under **Customize what users see**, then click **Task**.
1. In the **Details** section, select the **Overtime Ratio** field in the **Finance** area.

   For more information, see [Customize the Details view using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

## Define the overtime ratio on a task

1. Go to the task that you want to edit.

   For more information, see [Manage task finances in the Task Details section](/help/quicksilver/manage-work/tasks/manage-tasks/task-finances-in-details.md).

1. Click **Task Details** in the left panel.
1. In the **Finance** area, enter the overtime multiplier in the **Overtime Ratio** field.
1. Click **Save Changes**.
