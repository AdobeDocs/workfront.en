---
product-area: templates
navigation-topic: templates-navigation-topic
title: Attach a template to a project
description: You can attach a template to a project either during the initial creation phase of the project or after it has been created.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
---
# Attach a template to a project

You can attach a template to a project either during the initial creation phase of the project or after it has been created.

For more information about creating a project using a template, see [Create a project using a template](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Access requirements

You must have the following to perform the steps described in this article:

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
   <td> <p>Edit access to Projects </p> <p>For information about project access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> <p>View access to&nbsp;Templates</p> <p>For information about template permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Share a template</a>. </p> <p>For information about template access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Grant access to templates</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>. </p> <p>View permissions or higher to the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations when adding templates to projects</h2>
<p>(NOTE: moved this to an Overview article of its own) </p>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator <span>or a group administrator</span> has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
<li> <p>Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. </p> </li>
<li> <p>Most template settings are added to the project. </p> </li>
<li> <p>Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>For example, these settings are added to the project:</p>
<ul>
<li>Start&nbsp;From field</li>
<li>Custom forms and the information on them</li>
<li>Queue Details </li>
<li>Financial settings </li>
</ul>
</div> </li>
</ul>
</div>
-->

## Attach a template to an existing project {#attach-a-template-to-an-existing-project}

You can attach a template to a project in Workfront from the project page or from a project list or report.

1. Go to the project where you want to attach a template and click the **More** icon ![](assets/qs-more-icon-on-an-object.png) to the right of the project name

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Or

   Go to a project list or report and select a project then click the **More** icon ![](assets/qs-more-icon-on-an-object.png) at the top of the list.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

   
1. Click **Attach Template**.

   The Attach Template box displays.

1. Begin typing the name of the template that you want to attach in the **Search Templates** field, then click it when it displays.in the list

   Or

   Click the name of a template in the **Other Templates** area.

   A preview of the template displays to the right that contains the following information about the template:

   * Duration
   * Owner
   * The number of top-level tasks (includes a list of the first three top-level tasks)
   * Total number of tasks 
   * Names of attached custom forms

   ![](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (Optional) Click the **Favorites** icon ![](assets/favorites-icon-small.png) to the left of the template name to mark it as a favorite. This moves the template in the Favorites list.

   ![](assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png)

1. (Optional)&nbsp;Click the **Favorites** icon ![](assets/favorites-icon-selected.png) again to remove it from the Favorites list. 
1. Click **Customize and attach**.

   ![](assets/attach-template-large-box-nwe-350x262.png)

1. Update information in the following sections before attaching the template (or, click **Attach Template** at any time):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Tasks section</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">The selected template tasks below are imported to the project.&nbsp;Deselect the ones you want to exclude. </td> 
      <td>Deselect any tasks that you want to exclude from the template before attaching it to the project.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Select the project task you want as the predecessor for the tasks in this template.</td> 
      <td> <p>Click the field to display a list of project tasks. Select which project task you want finished before the template tasks can start. Alternatively, you can skip this step and set up relationships within the project after the template is attached. </p> <p> Select the <strong>Dependency Type</strong>, <strong>Lag</strong> information, and whether you want the predecessor to be <strong>Enforced</strong> or not. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Select the project task that you want as the parent of the tasks in this template.</td> 
      <td> Select which project task you want to designate as the parent task for all of the template tasks. If you do not make a selection, all of the template tasks appear at the end of your current project tasks. You can skip this step and move tasks around in the project after the template is attached.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Options section</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">The selected items below are transferred to the project. Deselect the ones you want to exclude.</td> 
      <td> <p>Deselect the check-boxes beside any information you want to clear from the template before attaching it to the project. This information is not transferred from the template to the project. For more information on each field, see <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Overview of attaching a template to a project</a>. </p> <p>Important: If you check the <strong>Queue Properties &amp; Issues Setup</strong> box, the Queue Details of the template overwrite those of the project. In this case, the Routing Rules, Queue Topics, and Topic Groups of the template are added to those of the project. <br>If the project is set up as a request queue and the template you attach to the project is not set up as a request queue, the queue information of the project is removed if you leave the <strong>Queue Properties and Issues Setup</strong> box checked. <br>If you deselect the <strong>Queue Properties and Issue Setup</strong> box, all the Queue Setup settings of the project are preserved and no Queue Setup settings from the template are attached. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Custom Forms section</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom&nbsp;Forms</td> 
      <td> <p>When custom forms are attached to the template, their names display in the left panel. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Update information in the custom forms. This information transfers to the project.

   >[!TIP]
   >
   >* This step is mandatory when the custom forms on the template contain required fields that are empty. 
   >* If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. 

1. Click **Attach Template.**
1. Click&nbsp;**Cancel attachment** to stop attaching the template.

   Or

   Allow the attachment to finish to add the template to the project.

   After attaching the template, you can edit the project and adjust any tasks, information, or settings as needed.

1. (Optional) Click&nbsp;**Project Details**, then **Overview** to view the name of the template you attached in the **Project relationships** area.

   >[!TIP]
   >
   >If you attach more than one template to the project, only the template you attached first displays in this field. For information, see the [Attach multiple templates to an existing project and view template information](#attach-multiple-templates-to-an-existing-project-and-view-template-information) section in this article.

1. (Optional)&nbsp;Remove template information from the project where you attached the template. For information, see [Remove template information from a project](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## Attach multiple templates to an existing project and view template information {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

You can attach multiple templates (one at a time) to the same project, following the steps described in the section [Attach a template to an existing project](#attach-a-template-to-an-existing-project) in this article. This adds the tasks and other information from each template to the project.

>[!TIP]
>
>When you attach several templates to a project, only the one you attached first displays in the Project Details area.

To understand what template is applied to a project:

1. Navigate to a project which has a template attached.
1. Click **Project Details** in the left panel.
1. Find the name of the template attached to the project in the **Template** field at the bottom of the **Overview** section under **Project relationships** .

   ![](assets/nwe-template-info-on-project-350x356.png)


