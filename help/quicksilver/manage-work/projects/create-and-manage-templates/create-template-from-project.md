---
product-area: templates
navigation-topic: templates-navigation-topic
title: Create template from project
description: You can create templates when you save an existing project as a template.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
---
# Create template from project

<!--Audited: 10/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

You can create templates when you save an existing project as a template.

After you save an existing project as a template, you can use the new template to create new projects. This simplifies and expedites the project creation process.

>[!NOTE]
>
>When saving a project as a template, the actual dates of the tasks and of the project do not save for the template. 
>
>A template and its tasks do not have actual dates, but rather an indication of which day (from when the future project might start) a task might start and on which day the task might need to complete. When using templates to create the future projects, the projects will receive actual dates. For information, see [Create a project](../create-projects/create-project.md).

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
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you create it</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

 +++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you create it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Create template from project

1. Go to the project that you want to save as a template. 
1. Click the **More** menu ![More icon](assets/more-icon.png), then **Save as Template**. 
1. Specify the following information for the template:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Template Name</td> 
      <td>Specify a name for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Provide a description for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Is Active</td> 
      <td> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Yes</strong>: Other users can find the template and attach it to projects.</p> </li> 
        <li><strong>No</strong>: Other users cannot find the template and cannot attach it to projects.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Custom Forms** in the left panel.   
1. Click the **Add custom form** field and either start typing the name of a project custom for, or select one from the list. 

   If any custom forms are already associated with the project, all of the information in the existing fields from those custom forms displays on the forms.
   
   You can include up to 10 custom forms on a single template.

1. Hover over a form's name, then click to drag and drop it in a new place.

   ![Save project as template top of the box](assets/save-project-as-template-top-of-the-form.png)

1. Click **Options** in the left panel, then select the fields or items you want to transfer to the template.

   All items are checked by default. Deselected items are not transferred to the template. 

   ![Save as template options](assets/save-project-as-template-options-area.png)

1. Click **Exclude** in the left panel, then select any tasks that you want to exclude from the project.

   ![Save as template exclude](assets/save-project-as-template-exclude-area.png)

1. Click **Finish and Save Template.**

   Your template now appears in the list of available templates. Users can either attach the new template to an existing project or use it to create a project. 


