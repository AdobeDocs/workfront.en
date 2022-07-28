---
title: Customize the Details view using a layout template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: As a Workfront administrator, you can use a layout template to determine what information appears when a user selects the Details section in the left panel while viewing a task, issue, document, program, or portfolio.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
---
# Customize the Details view using a layout template

As an Adobe Workfront administrator, you can use a layout template to determine what information appears when a user clicks the Details icon ![](assets/project-details-icon.png) in the left panel while viewing a task, issue, document, program, or portfolio.

<!--
, or billing record
-->

You can also change the order of the information in which this information appears. For example, for all tasks that your users see, you can move Custom Forms information to the top of the Details view for all tasks that your users see.

The changes you make to the Details view for an object also determine the availability and order of fields that users see in the following areas:

* "New object" boxes, such as New Task and New Issue

  ![](assets/new-task-dialog.png)

* "Edit object" screens, such as Edit Task and Edit Issue

  ![](assets/edit-task-screen.png)

* Summary ![](assets/summary-panel-icon.png) panel for lists of tasks and issues

  ![](assets/summary-area.png)

  >[!NOTE]
  >
  >Changes to the layout templates affect the order and availability of fields in the Summary panel only for the tasks and issues that are assigned to the logged-in user.

* Conversion boxes, such as the Convert issue to task or Convert issue to project boxes. 

  ![Convert issue to task box](assets/convert-issue-to-task-box.png)

For information about layout templates for groups, see [Create and modify a group's layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Access requirements

You must have the following access to perform the steps in this article: 

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>To perform these steps at the system level, you need the System Administrator access level.
To perform them for a group, you must be a manager of that group</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Customize what users see in the Details view

1. Begin working on a layout template, as described in [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Click the down arrow ![](assets/dropdown-arrow-12x12.png) under **Customize what users see**, then click **Project**, **Task**, **Issue**, **Program**, or **Portfolio.**
<!--
, or billing record
-->

1. In the **Details** section, do any of the following to customize what users see in the Details view:

   * Drag any section headers ![](assets/move-icon---dots.png) to change their order.
   * Enable or disable options under **Overview** and **Custom Forms** to show or hide them.

     If you hide all fields in one of these sections, the entire section is hidden.

     All of the fields are enabled by default.

1. Continue customizing the layout template.

   Or

   If you are finished customizing, click **Save**.

   >[!TIP]
   >
   >You can click Save at any time to save your progress, then continue to modify the template later.
