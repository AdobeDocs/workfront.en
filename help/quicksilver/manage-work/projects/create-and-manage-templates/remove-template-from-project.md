---
filename: remove-template-from-project
product-area: templates
navigation-topic: templates-navigation-topic
title: Remove template information from a project
description: You cannot remove a template from a project. You can only manually remove information that was added to the project after a template was attached to the project. For information about attaching templates, see Attach a template to a project.
---

# Remove template information from a project

You cannot remove a template from a project. You can only manually remove information that was added to the project after a template was attached to the project. For information about attaching templates, see [Attach a template to a project](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

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
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to tasks </p> <p>Contribute or higher access to the project </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Options to remove template information from a project

To remove template information that was added to the project, you can do one of the following:

* Manually remove information from the project after the template was attached.

  For information, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

* Delete the tasks in the project which were added with the template.

  For information, see the [Delete tasks created from a template](#delete-tasks-created-from-a-template) section in this article.

* Delete the template from&nbsp;Workfront. Deleting the template from Workfront does not delete the tasks added from the template from projects.

  For information, see [Delete project templates](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Delete tasks created from a template {#delete-tasks-created-from-a-template}

1. Go to the **Tasks** section of the project.
1. Do one of the following:

   * Create a filter for the task list to display only tasks that were created from a template using the following statement:

     ```   
     Task >> Template Task ID >>Is Not Blank
     ```

     For information about creating a filter, see [Create or edit filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

     When you apply the filter, only tasks associated with a Template Task ID display in the list. 
   
   * Create a view for the task list to display the **Template Task ID** or **Template Task Name** fields in a column.

     When you apply the view, the tasks that contain information in the Template Task ID or Template Task name column were created using a template.

     For information about creating a view, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Select all the tasks identified in Step 2 as created from a template, then click&nbsp;**the Delete icon****> Yes, Delete it**. For more information, see [Delete tasks](../../../manage-work/tasks/manage-tasks/delete-tasks.md).

