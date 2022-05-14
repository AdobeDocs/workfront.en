---
filename: convert-task-to-project
product-area: projects
navigation-topic: manage-tasks
title: Convert a task to a project
description: When a task in a project requires a larger amount of effort to complete than you originally planned, you can convert it to a project.
---

# Convert a task to a project

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

When a task in a project requires a larger amount of effort to complete than you originally planned, you can convert it to a project.

## Access requirements

You must have the following access to perform the steps in this article:

<table> 
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
1. Click **Actions**.
1. Choose either the following options:

   * **New Project** 
   * **New from Template**

     ![](assets/cattap-350x262.png)

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
     >You can transfer custom form information from the task to the project by adding a duplicate project-type custom form (with the same fields that are on the task-type custom form) to the new project. For more information, see [Transfer custom form data when converting an object](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md).

1. Click **Save Changes**.

