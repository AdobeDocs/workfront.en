---
title: Customize the Details View Using a Layout Template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: As a Workfront administrator, you can use a layout template to determine what information appears when a user selects the Details section in the left panel while viewing a task, issue, document, program, or portfolio.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
---
# Customize the Details view using a layout template

{{preview-fast-release-general}}

As an Adobe Workfront administrator, you can use a layout template to determine what information appears when a user clicks the Details icon ![Details icon](assets/project-details-icon.png) in the left panel while viewing a task, issue, document, program, or portfolio.

<!--
or billing record
-->

You can also change the order of the information in which this information appears. For example, for all tasks that your users see, you can move Custom Forms information to the top of the Details view for all tasks that your users see.

For information about creating layout templates, see [Create and manage layout templates](../use-layout-templates/create-and-manage-layout-templates.md). 

For information about layout templates for groups, see [Create and modify a group's layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

After configuring a layout template, you must assign it to users for changes you made to be visible to others. For information about assigning a layout template to users, see [Assign users to a layout template](../use-layout-templates/assign-users-to-layout-template.md).

The changes you make to the Details view for an object also determine the availability and order of fields that users see in the following areas:


* "Create object" boxes, such as Create Task

  ![New task dialog](assets/new-task-dialog.png)


* "Edit object" screens when editing an object, such as Edit Task, Edit Issue, and Edit Project

  ![Edit task screen](assets/edit-task-screen.png)


* "Edit objects" screens when editing objects in bulk. Currently this is supported for editing projects in bulk.

  ![Customize edit projects](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)
  

* Summary panel ![Summary panel](assets/summary-panel-icon.png) for lists of tasks and issues

  ![Summary area](assets/summary-area.png)

  >[!NOTE]
  >
  >Changes to the layout templates affect the order and availability of fields in the Summary panel only for the tasks and issues that are assigned to the logged-in user.

* Conversion boxes, such as the Convert issue to task or Convert issue to project boxes. 

  ![Convert issue to task box](assets/convert-issue-to-task-box.png)

For information about layout templates for groups, see [Create and modify a group's layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td> <p>To perform these steps at the system level, you need the System Administrator access level.</p>
        <p>To perform them for a group, you must be a manager of that group.</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Customize what users see in the Details view

1. Begin working on a layout template, as described in [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Click the down arrow ![Down arrow](assets/dropdown-arrow-12x12.png) under **Customize what users see**, then click **Project**, **Task**, **Issue**, **Program**, or **Portfolio.**
<!--
, or billing record
-->

1. In the **Details** section, do any of the following to customize what users see in the Details view:

   * Drag any section headers ![Move icon](assets/move-icon---dots.png) to change their order.
   * Enable or disable options under the various areas (such as **Overview**, **Finance**, and **Custom Forms**) to show or hide them.

     If you hide all fields in one of these sections, the entire section is hidden.

     All of the fields are enabled by default. You can select or clear the **Select all** check box in an area to display or hide all of the fields in that area.

   ![Details view in layout template](assets/layout-template-details-view.png)

1. <span class="preview">In the Preview environment: Continue customizing the layout template. You can click **Apply** at any time to save your progress.</span>

   <span class="preview">Or</span>

   <span class="preview">If you are finished customizing, click **Save and Close**.</span>

1. In the Production environment: Continue customizing the layout template.

   Or

   If you are finished customizing, click **Save**.

   >[!TIP]
   >
   >You can click **Save** at any time to save your progress, then continue to modify the template later.
