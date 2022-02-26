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
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects </p> <p>For information about project access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> <p>View access to&nbsp;Templates</p> <p>For information about template permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Sharing a template</a>. </p> <p>For information about template access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Grant access to templates</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>. </p> <p>View permissions or higher to the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="access-limitations"></a>Considerations when adding templates to projects</h2>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your <em>Adobe Workfront administrator</em> <span>or a <em>group administrator</em></span> has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
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

## Considerations when adding templates to projects

Consider the following when adding templates to projects:

* You can attach only active templates to projects. 
* You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your *Adobe Workfront administrator* `or a *group administrator*` has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md). 
* Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. 
* Most template settings are added to the project. 
* Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. 

  ` `**Example: **`` For example, these settings are added to the project:

  * Start&nbsp;From field
  * Custom forms and the information on them
  * Queue Details 
  * Financial settings

## Attach a template to an existing project

<!--
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h3><a name="Attach2"></a> </h3>
<ol>
<li value="1">Go to the project where you want to attach a template. </li>
<li value="2"> <p>Click the <span class="bold">More</span> menu <img src="assets/qs-more-icon-on-an-object.png">, then click <span class="bold">Attach Template</span>. </p> <p>The Attach Template box displays. <br></p> </li>
<li value="3"> <p>Begin typing the name of the template that you want to attach in the <span class="bold">Search Templates</span> field, then click it when it displays.in the list</p>
<div>
<p>Or</p>
<p>Click the name of a template in the <span class="bold">Other Templates</span> area. </p>
<p>A preview of the template displays to the right that contains the following information about the template:</p>
<ul>
<li> <p>Duration</p> </li>
<li> <p>Owner</p> </li>
<li> <p>The number of top-level tasks (includes a list of the first three top-level tasks)</p> </li>
<li> <p>Total number of tasks </p> </li>
<li> <p>Names of attached custom forms</p> </li>
</ul>
<p> <img src="assets/attach-template-box-template-preview-area-nwe-350x281.png" style="width: 350;height: 281;"> </p>
</div> </li>
<li value="4"> <p>(Optional) Click the <span class="bold">Favorites</span> icon <img src="assets/favorites-icon-small.png"> to the left of the template name to mark it as a favorite. This moves the template in the Favorites list. </p> <p> <img src="assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png" style="width: 350;height: 79;"> </p> </li>
<li value="5"> <p>(Optional)&nbsp;Click the <span class="bold">Favorites</span> icon <img src="assets/favorites-icon-selected.png"> again to remove it from the Favorites list. </p> </li>
<li value="6"> <p>Click <span class="bold">Customize and attach</span>. </p> <p> <img src="assets/attach-template-large-box-nwe-350x262.png" style="width: 350;height: 262;"> </p> </li>
<li value="7"> <p>Update information in the following sections before attaching the template (or, click <span class="bold">Attach Template</span> at any time):</p>
<table cellspacing="0">
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
<td> <p>Click the field to display a list of project tasks. Select which project task you want finished before the template tasks can start. Alternatively, you can skip this step and set up relationships within the project after the template is attached. </p> <p> Select the <span class="bold">Dependency Type</span>, <span class="bold">Lag</span> information, and whether you want the predecessor to be <span class="bold">Enforced</span> or not. </p> </td>
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
<td> <p>Deselect the check-boxes beside any information you want to clear from the template before attaching it to the project. This information is not transferred from the template to the project. For more information on each field, see <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Overview of attaching a template to a project</a>. </p> <note type="important">
If you check the
<span class="bold">Queue Properties & Issues Setup</span> box, the Queue Details of the template overwrite those of the project. In this case, the Routing Rules, Queue Topics, and Topic Groups of the template are added to those of the project.
<br>If the project is set up as a request queue and the template you attach to the project is not set up as a request queue, the queue information of the project is removed if you leave the
<span class="bold">Queue Properties and Issues Setup</span> box checked.
<br>If you deselect the
<span class="bold">Queue Properties and Issue Setup</span> box, all the Queue Setup settings of the project are preserved and no Queue Setup settings from the template are attached.
</note> </td>
</tr>
<tr>
<td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Custom Forms section</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td>
</tr>
<tr>
<td role="rowheader">Custom&nbsp;Forms</td>
<td> <p>When custom forms are attached to the template, their names display in the left panel. </p> </td>
</tr>
</tbody>
</table> </li>
<li value="8"> <p>(Optional) Update information in the custom forms. This information transfers to the project. </p>
<div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
<span class="autonumber"><span><b>Tip: </b></span></span>
<ul>
<li> <p>This step is mandatory when the custom forms on the template contain required fields that are empty. </p> </li>
<li> <p>If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
</div> </li>
<li value="9"> <p>Click <span class="bold">Attach&nbsp;Template.</span></p> </li>
<li value="10"> <p>Click&nbsp;<span class="bold">Cancel attachment</span> to stop attaching the template. </p> <p>Or</p> <p>Allow the attachment to finish to add the template to the project. </p> <p>After attaching the template, you can edit the project and adjust any tasks, information, or settings as needed. <br></p> </li>
<li value="11"> <p>(Optional) Click&nbsp;<span class="bold">Project&nbsp;Details</span>, then <span class="bold">Overview</span> to view the name of the template you attached in the <span class="bold">Project relationships</span> area. </p> <note type="tip">
If you attach more than one template to the project, only the template you attached first displays in this field. For information, see the
<a href="#attaching-multiple-templates-and-viewing-template-information" class="MCXref xref">Attach multiple templates to an existing project and view template information</a> section in this article.
</note> </li>
<li value="12"> <p>(Optional)&nbsp;Remove template information from the project where you attached the template. For information, see <a href="../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md" class="MCXref xref">Remove template information from a project</a>. </p> </li>
</ol>
</div>
-->

###

<ol> 
 <li value="1">Go to the project where you want to attach a template. </li> 
 <li value="2"> <p>Click the <span class="bold">More</span> menu <img src="assets/qs-more-icon-on-an-object.png">, then click <span class="bold">Attach Template</span>. </p> <p>The Attach Template box displays. <br></p> </li> 
 <li value="3"> <p>Begin typing the name of the template that you want to attach in the <span class="bold">Search Templates</span> field, then click it when it displays.in the list</p> 
  <div> 
   <p>Or</p> 
   <p>Click the name of a template in the <span class="bold">Other Templates</span> area. </p> 
   <p>A preview of the template displays to the right that contains the following information about the template:</p> 
   <ul> 
    <li> <p>Duration</p> </li> 
    <li> <p>Owner</p> </li> 
    <li> <p>The number of top-level tasks (includes a list of the first three top-level tasks)</p> </li> 
    <li> <p>Total number of tasks </p> </li> 
    <li> <p>Names of attached custom forms</p> </li> 
   </ul> 
   <p> <img src="assets/attach-template-box-template-preview-area-nwe-350x281.png" style="width: 350;height: 281;"> </p> 
  </div> </li> 
 <li value="4"> <p>(Optional) Click the <span class="bold">Favorites</span> icon <img src="assets/favorites-icon-small.png"> to the left of the template name to mark it as a favorite. This moves the template in the Favorites list. </p> <p> <img src="assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png" style="width: 350;height: 79;"> </p> </li> 
 <li value="5"> <p>(Optional)&nbsp;Click the <span class="bold">Favorites</span> icon <img src="assets/favorites-icon-selected.png"> again to remove it from the Favorites list. </p> </li> 
 <li value="6"> <p>Click <span class="bold">Customize and attach</span>. </p> <p> <img src="assets/attach-template-large-box-nwe-350x262.png" style="width: 350;height: 262;"> </p> </li> 
 <li value="7"> <p>Update information in the following sections before attaching the template (or, click <span class="bold">Attach Template</span> at any time):</p> 
  <table cellspacing="0"> 
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
     <td> <p>Click the field to display a list of project tasks. Select which project task you want finished before the template tasks can start. Alternatively, you can skip this step and set up relationships within the project after the template is attached. </p> <p> Select the <span class="bold">Dependency Type</span>, <span class="bold">Lag</span> information, and whether you want the predecessor to be <span class="bold">Enforced</span> or not. </p> </td> 
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
     <td> <p>Deselect the check-boxes beside any information you want to clear from the template before attaching it to the project. This information is not transferred from the template to the project. For more information on each field, see <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Overview of attaching a template to a project</a>. </p> <note type="important">
       If you check the 
       <span class="bold">Queue Properties & Issues Setup</span> box, the Queue Details of the template overwrite those of the project. In this case, the Routing Rules, Queue Topics, and Topic Groups of the template are added to those of the project. 
       <br>If the project is set up as a request queue and the template you attach to the project is not set up as a request queue, the queue information of the project is removed if you leave the 
       <span class="bold">Queue Properties and Issues Setup</span> box checked. 
       <br>If you deselect the 
       <span class="bold">Queue Properties and Issue Setup</span> box, all the Queue Setup settings of the project are preserved and no Queue Setup settings from the template are attached. 
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Custom Forms section</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Custom&nbsp;Forms</td> 
     <td> <p>When custom forms are attached to the template, their names display in the left panel. </p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="8"> <p>(Optional) Update information in the custom forms. This information transfers to the project. </p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <ul> 
    <li> <p>This step is mandatory when the custom forms on the template contain required fields that are empty. </p> </li> 
    <li> <p>If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li> 
   </ul> 
  </div> </li> 
 <li value="9"> <p>Click <span class="bold">Attach&nbsp;Template.</span></p> </li> 
 <li value="10"> <p>Click&nbsp;<span class="bold">Cancel attachment</span> to stop attaching the template. </p> <p>Or</p> <p>Allow the attachment to finish to add the template to the project. </p> <p>After attaching the template, you can edit the project and adjust any tasks, information, or settings as needed. <br></p> </li> 
 <li value="11"> <p>(Optional) Click&nbsp;<span class="bold">Project&nbsp;Details</span>, then <span class="bold">Overview</span> to view the name of the template you attached in the <span class="bold">Project relationships</span> area. </p> <note type="tip">
   If you attach more than one template to the project, only the template you attached first displays in this field. For information, see the 
   <a href="#attaching-multiple-templates-and-viewing-template-information" class="MCXref xref">Attach multiple templates to an existing project and view template information</a> section in this article. 
  </note> </li> 
 <li value="12"> <p>(Optional)&nbsp;Remove template information from the project where you attached the template. For information, see <a href="../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md" class="MCXref xref">Remove template information from a project</a>. </p> </li> 
</ol>

## Attach multiple templates to an existing project and view template information

You can attach multiple templates (one at a time) to the same project, following the steps described in the section [Attach a template to an existing project](#attaching-a-template) in this article. This adds the tasks and other information from each template to the project.

>[!TIP]
>
>When you attach several templates to a project, only the one you attached first displays in the Project Details >
><!-->
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">>
>area>
></MadCap:conditionalText>>
>-->
>`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> area</MadCap:conditionalText>`.

To understand what template is applied to a project:

<ol> 
 <li value="1">Navigate to a project which has a template attached.</li> 
 <li value="2"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Project Details</span> in the left panel
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Project Details</span> in the left panel
  </MadCap:conditionalText>.</li> 
 <li value="3"> Find the name of the template attached to the project in the <span class="bold">Template</span> field <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    at the bottom of the 
    <span class="bold">Overview</span> section under 
    <span class="bold">Project relationships</span> 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   at the bottom of the 
   <span class="bold">Overview</span> section under 
   <span class="bold">Project relationships</span> 
  </MadCap:conditionalText>. <p>
   <draft-comment>
    <img src="assets/nwe-template-info-on-project-350x356.png" style="width: 350;height: 356;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/nwe-template-info-on-project-350x356.png" style="width: 350;height: 356;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li> 
</ol>

&nbsp;

&nbsp;

##  

