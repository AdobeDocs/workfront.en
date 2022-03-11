---
filename: attach-template-to-project
product-area: templates
navigation-topic: templates-navigation-topic
title: Attach a template to a project
description: You can attach a template to a project either during the initial creation phase of the project or after it has been created.
---

# Attach a template to a project

You can attach a template to a project either during the initial creation phase of the project or after it has been created.

For more information about creating a project using a template, see [Create a project using a template](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Access requirements

You must have the following to perform the steps described in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects </p> <p>For information about project access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> <p>View access to&nbsp;Templates</p> <p>For information about template permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Sharing a template</a>. </p> <p>For information about template access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Grant access to templates</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>. </p> <p>View permissions or higher to the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

<!--
Considerations when adding templates to projects Consider the following when adding templates to projects: You can attach only active templates to projects. You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator or a group administrator has enabled this functionality in the Project Preferences area. For information about setting project preferences, see Configure system-wide project preferences. Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. Most template settings are added to the project. Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. Example: For example, these settings are added to the project: Start From field Custom forms and the information on them Queue Details Financial settings
-->

## Attach a template to an existing project

Go to the project where you want to attach a template. Click the More menu , then click Attach Template. The Attach Template box displays. Begin typing the name of the template that you want to attach in the Search Templates field, then click it when it displays.in the list Or Click the name of a template in the Other Templates area. A preview of the template displays to the right that contains the following information about the template: Duration Owner The number of top-level tasks (includes a list of the first three top-level tasks) Total number of tasks Names of attached custom forms (Optional) Click the Favorites icon to the left of the template name to mark it as a favorite. This moves the template in the Favorites list. (Optional) Click the Favorites icon again to remove it from the Favorites list. Click Customize and attach. Update information in the following sections before attaching the template (or, click Attach Template at any time): Tasks section The selected template tasks below are imported to the project. Deselect the ones you want to exclude. Deselect any tasks that you want to exclude from the template before attaching it to the project. Select the project task you want as the predecessor for the tasks in this template. Click the field to display a list of project tasks. Select which project task you want finished before the template tasks can start. Alternatively, you can skip this step and set up relationships within the project after the template is attached. Select the Dependency Type, Lag information, and whether you want the predecessor to be Enforced or not. Select the project task that you want as the parent of the tasks in this template. Select which project task you want to designate as the parent task for all of the template tasks. If you do not make a selection, all of the template tasks appear at the end of your current project tasks. You can skip this step and move tasks around in the project after the template is attached. Options section The selected items below are transferred to the project. Deselect the ones you want to exclude. Deselect the check-boxes beside any information you want to clear from the template before attaching it to the project. This information is not transferred from the template to the project. For more information on each field, see Overview of attaching a template to a project. Important: If you check the Queue Properties & Issues Setup box, the Queue Details of the template overwrite those of the project. In this case, the Routing Rules, Queue Topics, and Topic Groups of the template are added to those of the project. If the project is set up as a request queue and the template you attach to the project is not set up as a request queue, the queue information of the project is removed if you leave the Queue Properties and Issues Setup box checked. If you deselect the Queue Properties and Issue Setup box, all the Queue Setup settings of the project are preserved and no Queue Setup settings from the template are attached. Custom Forms section Custom Forms When custom forms are attached to the template, their names display in the left panel. (Optional) Update information in the custom forms. This information transfers to the project. Tip: This step is mandatory when the custom forms on the template contain required fields that are empty. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. Click Attach Template. Click Cancel attachment to stop attaching the template. Or Allow the attachment to finish to add the template to the project. After attaching the template, you can edit the project and adjust any tasks, information, or settings as needed. (Optional) Click Project Details, then Overview to view the name of the template you attached in the Project relationships area. Tip: If you attach more than one template to the project, only the template you attached first displays in this field. For information, see the Attach multiple templates to an existing project and view template information section in this article. (Optional) Remove template information from the project where you attached the template. For information, see Remove template information from a project. 

## Attach multiple templates to an existing project and view template information

You can attach multiple templates (one at a time) to the same project, following the steps described in the section [Attach a template to an existing project](#attaching-a-template) in this article. This adds the tasks and other information from each template to the project.

>[!TIP]
>
>When you attach several templates to a project, only the one you attached first displays in the Project Details area.

To understand what template is applied to a project:

1. Navigate to a project which has a template attached.
1. Click Project Details in the left panel.
1. Find the name of the template attached to the project in the `Template` field at the bottom of the Overview section under Project relationships.

&nbsp;

&nbsp;

##  

