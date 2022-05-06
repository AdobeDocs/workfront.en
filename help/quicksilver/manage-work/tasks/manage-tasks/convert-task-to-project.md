---
filename: convert-task-to-project
product-area: projects
navigation-topic: manage-tasks
title: Convert a task to a project
description: When a task in a project requires a larger amount of effort to complete than you originally planned, you can convert it to a project.
---

# Convert a task to a project

When a task in a project requires a larger amount of effort to complete than you originally planned, you can convert it to a project.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and&nbsp;Projects</p> <p>View or higher access to&nbsp;Templates, when converting to a project using a template</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>View permissions on a template, if converting to a project using a template</p> <p>After creating the project, you have Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations for converting tasks to projects

* The original task is deleted.
* Task approvals are deleted.
* All sub-tasks, issues and notes roll up to the new project.
* Documents, document versions, and proofs are moved to the new project.
* Status and percent complete of all sub-tasks and issues are preserved.
* Shared users of the task become shared users on the project.
* The project start date is set to the start date of the task.
* If the task status is 'New' the project status is set to 'Planning.'
* If the task status is 'In Progress' the project status is set to 'Current.'
* If the task status is 'Complete' the project status is set to 'Complete.'

## Convert a task to a project

1. Go to the task that you want to convert to a project.
1. Click the **More** icon ![](assets/more-icon.png), then **Convert to Project**. 
1. Choose either the following options:

   * **New Project** 
   * A template in the **Select From Templates** section

     ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Click **Continue** on the notification that appears.
1. In the **Convert to Project** box, specify the following:

   * **Name**: Name your project. The default name is the name of the task.
   * (Optional) **Description**: Describe the purpose for this project.
   * (Optional and conditional) If you have selected to create a project from a template, update the available fields in the **Convert to Project** dialog box.

     For more information about editing fields on projects, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >To update fields in the Finance section in the Convert to Project box you must have Edit access to Financial&nbsp;Data in your access level.&nbsp;If you have View access to Financial Data in your access level all financial information from the template transfers to the new project and you cannot edit it while you convert the issue. For information, see [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) and [Sharing a template](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Optional) Add **Custom Forms** to the new project.

     >[!TIP]
     >
     >If a multi-object custom form attached to the task is configured for use with both tasks and projects, all information saved in the form is retained when you make the conversion.
     >
     >
     >If you are using a template for the conversion and a custom form attached to the template contains a custom field also found in a custom form attached to the task, the field value from the task is used for the new project. However, if the custom field is blank on the task, the value from the template is used.

1. Click **Save Changes**.

