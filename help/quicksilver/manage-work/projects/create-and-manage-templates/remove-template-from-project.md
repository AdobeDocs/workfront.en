---
product-area: templates
navigation-topic: templates-navigation-topic
title: Remove template information from a project
description: You cannot remove a template from a project. You can only manually remove information that was added to the project after a template was attached to the project. For information about attaching templates, see Attach a template to a project.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
---
# Remove template information from a project

You cannot remove a template from a project. You can only manually remove information that was added to the project after a template was attached to the project. For information about attaching templates, see [Attach a template to a project](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p>
   <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to tasks </p> <p>Contribute or higher access to the project</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to tasks </p> <p>Contribute or higher access to the project </p>  </td> 
  </tr> 
 </tbody> 
</table>-->

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
