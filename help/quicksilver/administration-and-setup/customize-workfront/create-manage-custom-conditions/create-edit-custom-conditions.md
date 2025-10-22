---
title: Create or Edit a Custom Condition
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: As an Adobe Workfront administrator, you can create or edit a custom condition for projects, tasks, and issues to match the needs of your organization.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
---
# Create or edit a custom condition

As an Adobe Workfront administrator, you can create or edit a custom condition for projects, tasks, and issues to match the needs of your organization.

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
  <tr> 
   <td>Access level configurations</td> 
   <td>System Administrator</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create or edit a custom condition

{{step-1-to-setup}}

1. Click **Project Preferences** > **Conditions**.  

1. Click the tab of the object type (**Project**, **Task**, or **Issue**) that you want to associate with the condition.

1. To create a new condition, click **Add a new condition**.

   Or

   To edit an existing condition, click **Edit** next to the condition name.

   ![Edit custom condition](assets/custom-conditions-0825.png)

1. Configure your custom condition using the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Condition name</td> 
      <td>(Required) Type a descriptive name for the condition.</td> 
     </tr> 
     <tr> 
      <td>Description</td> 
      <td>(Optional) Type a description of the condition's purpose for those who will use it.</td> 
     </tr> 
     <tr> 
      <td>Color</td> 
      <td>(Optional) Click the color icon, then choose the color you want for the condition when it displays in projects, task, or issues. You can also type a hex number.</td> 
     </tr> 
     <tr> 
      <td>Equates with </td> 
      <td><p>(Required, for projects only) Click the option in the drop-down list that best describes the function of your new condition. For example, for a condition named Tracking Well, you would click On Target. This determines how your default conditions work. Every condition you create must equate with one of the options in the drop-down menu.</p>
      <p>For information about default conditions, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Set a custom condition as the default for projects</a> and <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">Set a custom condition as the default for tasks and issues</a>.</p>
      <p>This option cannot be modified after you finish creating the condition.</p></td> 
     </tr> 
     <tr> 
      <td>Key</td> 
      <td><p>(Required) For a project condition, type an alphanumeric abbreviation that users will be able to recognize. For a task or issue condition, type a two-digit numeric code from 01 to 99. </p>
      <p>This key, which is used in the API and can be used for reporting purposes, must be unique for each object.</p>
      <p>You cannot change the key for a condition after you save the condition. </p></td> 
     </tr> 
     <tr> 
      <td>Hide condition</td> 
      <td><p>(Optional) This option is available for custom conditions that you no longer want people to use, but want to keep for historical reasons. </p>
      <p>If you hide a custom condition that has been used on work items, it continues to appear on those work items after you hide it. </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >You can standardize condition terminology and colors across all three object types. To do this, copy the condition Name and the Color hex code from one tab (Project, Task, Issue) to the corresponding condition on the other two tabs.

1. (Optional) Drag ![Move icon](assets/move-icon---dots.png) any condition to a new position to re-order the list.

   This changes the order in which conditions display in projects, tasks and issues:

   * When a user is editing a project

     ![Change condition when editing project](assets/change-condition-edit-project-0825.png)

   * When a user is changing the condition for a task or issue in a list view:

     ![Change condition in list](assets/change-conditions-list-dropdown-0925.png)

     >[!NOTE]
     >
     >In the default Condition view, the **Condition** field is a type of field that can't be edited inline. When you add the **Condition** field separately to a view, it is editable. For information about inline editing, see [Inline edit items in a list in Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

1. Click **Save**.

You can set your custom condition as a default condition for projects or for tasks and issues. For more information, see [Set a custom condition as the default for projects](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) and [Set a custom condition as the default for tasks and issues](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

For more information about custom conditions, see [Custom conditions](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).


   <!-- THIS WAS ORIGINALLY BETWEEN THE OTHER TWO BULLETS.
   * When a user is changing the condition for a task or issue on the Updates tab:

     ![Change condition when updating comment](assets/change-condition-update-comment.png)
   -->
