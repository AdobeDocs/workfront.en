---
filename: transfer-custom-form-data-larger-item
title: Transfer Custom Form data to a larger work item
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Transfer custom form data to a larger work item
description: Depending on the business needs of your organization, the work defined in a task or an issue might become too large to manage it within the task or the issue. In this case, you can convert them to a larger work item:
---

# Transfer custom form data to a larger work item

Depending on the business needs of your organization, the work defined in a task or an issue might become too large to manage it within the task or the issue. In this case, you can convert them to a larger work item:

* You can convert issues to tasks or projects. For more information, see [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).
* You can convert tasks to projects. For more information, see [Convert a task to a project](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md).

To transfer custom form data from an issue to a task or a project, you must complete the 2 tasks in this article, in the order below.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> Adobe Workfront plan* Any 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> Access level configurations* Administrative access to custom forms For information about how Workfront administrators grants this access, see Grant users administrative access to certain areas. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Copy a custom form

You can retain custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form and attach it to the new object.

To copy a custom form for an issue and save it as a custom form for a task or project:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Custom Forms</span>.</li> 
 <li value="3">Select an Issue custom form, then click <span class="bold">Copy</span>.</li> 
 <li value="4">In the <span class="bold">Custom Form</span> dialog box, specify a name for the new form.<br></li> 
 <li value="5"> <p>From the <span class="bold">Form Type</span> drop-down menu, select the object for which you want to create the new custom form.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If you want to transfer the custom form data to a project, select Project.</p> </li> 
 <li value="6"> <p>Click <span class="bold">Copy Form</span>.<br></p> <p>This creates an identical copy of the Issue custom form. This new custom form can now be attached to a task or project as described in the following section.</p> </li> 
</ol>

## Convert an issue or task and transfer custom form data

Transferring custom form data from issues to tasks is identical with transferring custom form data from issues to projects, or from tasks to projects.

To transfer custom form data from an issue to a task as you are converting the issue:

1. Copy the custom form on the task or issue you are converting.

   For more information, see [Copy a custom form](#copying-a-custom-form).

1. Go to the issue you want to convert.

   For information about converting issues, see [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Click `Issue Actions`, then click `Convert to Task`.

1. In the `Convert to Task` dialog box, click the `Add Forms`&nbsp;drop-down menu and select the form you copied in the previous section.

   The information captured in the custom fields of the issue is now transferred to the custom form on the task.

1. Click `Save Changes`.

