---
product-area: templates
navigation-topic: templates-navigation-topic
title: Create a project template
description: You can create and delete templates from the Templates area. When building a new template, you can enter the information for all of the tasks and all information for your future project settings. This information will then transfer to the project, when you create it from the template.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
---
# Create a project template

You can create and delete templates from the Templates area. When building a new template, you can enter the information for all of the tasks and all information for your future project settings. This information will then transfer to the project, when you create it from the template.

>[!NOTE]
>
>A template and its tasks do not have actual dates, but rather an indication of which day (from when the future project might start) a task might start and on which day the task might need to complete. When using templates to create the future projects, the projects will receive actual dates. For information, see [Create a project](../create-projects/create-project.md).


You can create a new template in the following ways:

* From scratch, as described in this article.
* From existing projects, by saving a project as a template.

  For more information about creating templates from existing projects, see [Save a project as a template](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* By copying it from another template.

  For more information about copying an existing template, see [Copy a project template](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* If you are a Workfront administrator, you can create templates by importing Blueprints. For information, see [Configure a blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Access requirements

You must have the following:

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
   <td> <p>Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">System administrator for importing templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Create a template

1. From the **Main Menu** ![](assets/main-menu-icon.png) click **Templates**. 

1. Click **New Template**.

   The template is untitled.

   ![New template](assets/create-template-nwe-2022-350x102.png)

1. Specify a name for the new template in the template header, then press **Enter.**
1. Click the **Template Tasks** section in the left panel. 
1. Click**Start Adding Template Tasks**.

   Or

   Click **New Template Task** to start adding tasks to your template.

   Adding template tasks to a template is identical to adding tasks to a project.

   For more information about adding tasks to a project, see [Create tasks in a project](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >You cannot add recurring tasks to a template.

1. (Optional) Click the **Gantt chart** icon in the upper-right corner of the Task List to see a visual representation of the template's task list.

   >[!TIP]
   >
   >You cannot edit tasks directly from this Gantt chart.

1. To add information to your new template, click the **More** menu ![](assets/more-icon.png), then click **Edit**.

   For information about editing a template, see [Edit project templates](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Click **Save Changes**.
1. (Optional) If you want to add additional items to the template, see the section [Add additional items to a template](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) in the article [Edit project templates](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Template settings determined by group association

A project template's association with a group (or lack thereof) affects how project, task, and issue preferences determine certain settings in the template. For more information, see the section [Create and modify a group's project templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) in the article [Create and modify a group's project templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
