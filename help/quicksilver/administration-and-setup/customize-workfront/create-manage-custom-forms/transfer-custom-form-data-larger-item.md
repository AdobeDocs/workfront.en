---
filename: transfer-custom-form-data-larger-item
title: Transfer Custom Form data to a larger work item
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Transfer custom form data to a larger work item
description: Deprecate this article when multi-object custom forms goes to Prod?
---

# Transfer custom form data to a larger work item

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Deprecate this article when multi-object custom forms goes to Prod?</p>
-->

Depending on the business needs of your organization, the work defined in a task or an issue might become too large to manage it within the task or the issue. In this case, you can convert them to a larger work item:

* You can convert issues to tasks or projects. For more information, see [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).
* You can convert tasks to projects. For more information, see [Convert a task to a project](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md).

To transfer custom form data from an issue to a task or a project, you must complete the two tasks in this article, in the order below.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to custom forms</p> <p>For information about how Workfront administrators grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Copy a custom form {#copy-a-custom-form}

You can retain custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form and attach it to the new object.

To copy a custom form for an issue and save it as a custom form for a task or project:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select an Issue custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the object for which you want to create the new custom form.

   ``` ```**Example: **``````If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This creates an identical copy of the Issue custom form. This new custom form can now be attached to a task or project as described in the following section.

## Convert an issue or task and transfer custom form data

Transferring custom form data from issues to tasks is identical with transferring custom form data from issues to projects, or from tasks to projects.

To transfer custom form data from an issue to a task as you are converting the issue:

1. Copy the custom form on the task or issue you are converting.

   For more information, see [Copy a custom form](#copy-a-custom-form).

1. Go to the issue you want to convert.

   For information about converting issues, see [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Click **Issue Actions**, then click **Convert to Task**.

1. In the **Convert to Task** dialog box,&nbsp;click the **Add Forms**&nbsp;drop-down menu and select the form you copied in the previous section.

   The information captured in the custom fields of the issue is now transferred to the custom form on the task.

1. Click **Save Changes**.

