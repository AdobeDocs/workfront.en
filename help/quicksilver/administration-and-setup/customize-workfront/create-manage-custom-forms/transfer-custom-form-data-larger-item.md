---
title: Transfer custom form data when converting an object
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: When the work defined in a work item becomes too large, you can convert it to a larger work item.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
---
# Transfer custom form data when converting an object

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Depending on the business needs of your organization, the work defined in a task or an issue might become too large to manage within the task or the issue. In this case, you can convert them to a larger work item:

* You can convert issues to tasks, or to projects
* You can convert tasks to projects

To transfer custom form data from an issue to a task or a project, you must complete the two tasks in this article, in the order below.

For more information, see [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) or [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Access requirements

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>New: Standard</p>
   <p>or</p>
   <p>Current: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Administrative access to custom forms</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## First: Add additional objects to the custom form

{{step-1-to-setup}}

1. Click **Custom Forms**.
1. Find the form you need, then click **Edit** <span class="preview">or ![Edit icon](assets/edit-icon.png).</span>
1. At the top of the form, add the object you plan to convert the task or issue to.

   >[!INFO]
   >
   >**Example**: If you want to transfer the custom form data to a project, select Project.

1. Click **Apply** at the bottom of the form.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Second: Convert the issue or task and transfer the custom form data {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Add additional objects to the custom form on the issue or task you are converting, as explained in the section [First: Add additional objects to the custom form](#first-add-additonal-objects-to-the-custom-form) in this article.
1. Convert the issue or task using the **Custom Forms** option in the box that displays to select the custom form you need. For instructions, see the following articles:

   * [Convert an issue to a project in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Convert an issue to a task in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Convert a task to a project](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. In the **Convert to (object type)** dialog box that displays, click the **Add Forms** drop-down menu and select the form you copied in the previous section.

   The information captured in the custom fields of the issue is now transferred to the custom form on the task.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see the section [Start editing a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) in the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->