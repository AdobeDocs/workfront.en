---
product-area: projects
navigation-topic: manage-tasks
title: Convert a task to a project
description: When a task in a project requires a larger amount of effort to complete than you originally planned, you can convert it to a project.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
---
# Convert a task to a project

When a task in a project requires a larger amount of effort to complete than you originally planned, you can convert it to a project.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
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

* You can convert a task to a blank project or to a project using a template. 
* The original task is deleted.
* All sub-tasks, issues and notes roll up to the new project.
* Documents, document versions, and proofs are moved to the new project.
* Status and percent complete of all sub-tasks and issues are preserved.
* Shared users of the task become shared users on the project.
* The project start date is set to the start date of the task.
* The following table lists project information and whether it transfers from the template or from the task: 

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td>Description</td> 
    <td> <p>The Description of the task transfers to the new project. </p> <p> If there is no description on the task, the Description from the template transfers to the project. </p> <p>If the Description field is empty both for the task and for the template, the field is empty on the project. </p> </td> 
    </tr> 
    <tr> 
    <td>Status</td> 
    <td> Default status selected for the group on the template. If the template is not associated with the group, the project status is set to the default status set by the Workfront administrator in the Project Preferences area of Setup. For information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">Configure system-wide project preferences</a>

    The following scenarios exist for updating the Status of the project: 
    <ul>
    <li> If the task status is 'New' the project status is set to 'Planning.'</li>
    <li> If the task status is 'In Progress' the project status is set to 'Current.'</li>
    <li> If the task status is 'Complete' the project status is set to 'Complete.'</li></ul>
    
    </td> 
    </tr> 
    <tr> 
    <td>Priority</td> 
    <td>Transfers from the task to the project, or it transfers from the template, if you use one in the conversion. </td> 
    </tr> 
    <tr> 
    <td>URL</td> 
    <td> <p>The URL from the task transfers to the new project. </p> <p> If there is no URL specified on the task, the URL from the template transfers to the project. </p> <p>If the URL field is empty both for the issue and for the template, the field is empty on the project. </p> </td> 
    </tr> 
    <tr> 
    <td>Project Condition Type</td> 
    <td>Transfers from the template.</td> 
    </tr> 
    <tr> 
    <td>Project Condition</td> 
    <td>Matches the system-level default preference as determined by the Workfront administrator in the Setup area. For information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md">Set a custom condition as the default for projects</a>
    </td> 
    </tr> 
    <tr> 
    <td>Schedule From</td> 
    <td>Transfers from the template.</td> 
    </tr> 
    <tr> 
    <td>Project dates</td> 
    <td> 
      <ul> 
      <li> <p><b>Planned Start Date</b>: The closest working time based on the template schedule's working time should be preselected, according to the timezone of the template's schedule. This field is disabled if the Schedule From field is set to From Completion. </p> </li> 
      <li> <p><b>Planned Completion Date</b>: The closest working time based on the template schedule's working time should be preselected, according to the timezone of the template's schedule. This field is disabled if the Schedule From field is set to From Start. </p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td>Portfolio</td> 
    <td>Transfers from the template. Otherwise, this field is empty.</td> 
    </tr> 
    <tr> 
    <td>Program</td> 
    <td>Transfers from the template. Otherwise, this field is empty.</td> 
    </tr> 
    <tr> 
    <td>Group</td> 
    <td><p> The following scenarios exist:</p>
      <ul><li>If a group is specified during the conversion, that becomes the group of the project</li>
      <li>If you convert to a project using a template, and there is a group on the template, and during the conversion you do not specify a group, then the group of the template becomes the group of the new project</li>
      <li> If there is no group on the template and you do not specify a group during the conversion, then the group of the original issue's project becomes the group of the new project</li> </ul>
        </td> 
    </tr> 
    <tr> 
    <td>Company</td>    
    <td>  Transfers from the template. Otherwise, this field is empty.</td>
      
    </tr> 
    <tr> 
    <td>Project Owner</td> 
    <td>Transfers from the Template Owner field on the template. Otherwise, it is set to the logged-in user who is performing the conversion. </td> 
    </tr> 
    <tr> 
    <td>Project Sponsor</td> 
    <td>Transfers from the Template Sponsor field on the template. Otherwise, this field is empty.</td> 
    </tr> 
    <tr> 
    <td>Resource Manager</td> 
    <td>Transfers from the template. Otherwise, this field is empty.</td> 
    </tr> 
    <tr> 
    <td>Task Settings</td> 
    <td>Transfer from the template.</td> 
    </tr> 
    <tr> 
    <td>Issue Settings</td> 
    <td>Transfer from the template. </td> 
    </tr> 
    <tr> 
    <td>Access</td> 
    <td> <p>Transfers from the Access section on the template. </p> </td> 
    </tr> 
    <tr> 
    <td>Approvals</td> 
    <td>Transfer from the template. The approvals associated with the task are removed during the conversion. </td> 
    </tr> 
  </tbody> 
  </table>


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
     >To update fields in the Finance section in the Convert to Project box you must have Edit access to Financial&nbsp;Data in your access level.&nbsp;If you have View access to Financial Data in your access level all financial information from the template transfers to the new project and you cannot edit it while you convert the issue. For information, see [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) and [Share a template](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Optional) Add **Custom Forms** to the new project.

     >[!TIP]
     >
     >If a multi-object custom form attached to the task is configured for use with both tasks and projects, all information saved in the form is retained when you make the conversion.
     >
     >
     >If you are using a template for the conversion and a custom form attached to the template contains a custom field also found in a custom form attached to the task, the field value from the task is used for the new project. However, if the custom field is blank on the task, the value from the template is used.

1. Click **Save Changes**.
