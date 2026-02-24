---
content-type: overview
product-area: templates
keywords: overwrite,field,overwritten
navigation-topic: templates-navigation-topic
title: Overview of attaching a template to a project
description: When you attach a template to an existing project, you are modifying some of the information on the project according to that of the template. Some of the information on the project remains unchanged.
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
---
# Overview of attaching a template to a project

When you attach a template to an existing project, you are modifying some of the information on the project according to that of the template. Some of the information on the project remains unchanged.

For information about how to attach a template to a project, see [Attach a template to a project](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Considerations when adding templates to projects

Consider the following when adding templates to projects:

* You can attach only active templates to projects.
* You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator or a group administrator has enabled this functionality in the Project Preferences area. For information about setting project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project.
* Most template settings are added to the project. Some project settings are preserved. For information, see the section [Understand changes to project fields when attaching a template](#understand-changes-to-project-fields-when-attaching-a-template) in this article.

## Understand changes to project fields when attaching a template {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template, all template fields transfer to the new project. Attaching a template leaves some of the existing project fields unchanged.

Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved.

However, not all project fields are available to manage in the process of attaching a template to a project. For information, see [Attach a template to a project](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

The following table describes the default for what happens to project fields when you attach a template and which fields you can manage during the attachment process to override the default behavior:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Field</td> 
   <td>What happens in the process of attaching a template, by default</td> 
   <td>Ability to manage the field updates in the attachment process </td> 
  </tr> 
  <tr> 
   <td>Description</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Status</p> </td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>Transferred from template, if the field is empty on the project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Priority</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Condition Type</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Schedule Mode</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planned Dates</td> 
   <td>Might change based on the added tasks</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Actual Dates</td> 
   <td>Might change based on the added tasks</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Program</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Group</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Company</td> 
   <td>Transferred from template, if the field is empty on the project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planned Hours</td> 
   <td>Might change based on the added tasks</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Project Owner</td> 
   <td>Transferred from template, if the field is empty on the project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Project Sponsor</td> 
   <td>Transferred from template, if the field is empty on the project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Resource Manager</td> 
   <td>Added to the list of existing resource managers on the project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Custom Forms</td> 
   <td>Added to the project, in addition to forms that are already on the project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Budget</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Currency</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>PIM</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>EAC</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planned Benefit</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Actual Benefit</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Milestone Path</td> 
   <td>Transferred from template, if the field is empty on the project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Completion Mode</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Summary Completion Mode</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Update Type</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Schedule</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>User Time Off</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Resource Leveling Mode</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risk (project field)</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Resource Pools</td> 
   <td>Added to the list of existing resource pools on the project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hour Types</td> 
   <td> <p>If deselected during the attachment process, the Hour Types setting on the project remains unchanged. </p> <p>If selected, the template setting transfers to the project. If Hour Type filtering is set to Yes both on the project and the template, the hour types from the template are added to the ones on the project.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Reminder Notifications</td> 
   <td> <p>Added to the list of existing reminders on the project. </p> <p>If deselected during the attachment process, the project reminder notifications remain unchanged. </p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Task Default Approval Process</td> 
   <td>Project information is preserved</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Task Default Custom Forms</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Work Effort</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Allow users to add issues inline</span> </td> 
   <td><span>Project information is preserved</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>All settings</td> 
   <td>Template settings overwrite those of the project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tasks</td> 
   <td>Added to the bottom of the task list, in addition to the existing project tasks</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>Added to the project, in addition to existing project documents</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Risks (objects in the Risks area of the project)</td> 
   <td>Added to the project, in addition to existing project risks </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Approval Process</td> 
   <td>Transferred from template</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Billing Rates</td> 
   <td> <p>Transferred from template in addition to the existing billing rates on the project. </p> <p>If there is a different rate for the same job role on both the project and the template, the rate on the project remains unchanged. </p> </td> 
   <td> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Billing Records</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Expenses</td> 
   <td>Transferred from template in addition to the existing expenses on the project</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Financial Information</td> 
   <td> <p>When this is selected in the attachment process, the following fields are either transferred or added to the project: </p> 
    <ul> 
     <li> <p>Fixed Cost</p> <p>When the option is selected, the updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>Fixed Revenue</p> <p>When the option is selected, the updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>Cost Type on tasks</p> <p>Transferred from template</p> </li> 
     <li> <p>Revenue Type on tasks</p> <p>Transferred from template</p> </li> 
    </ul> <p>If this field is deselected during the attachment process, the following occurs:</p> 
    <ul> 
     <li> <p>The Fixed Cost and Fixed Revenue on the project are preserved.</p> </li> 
     <li> <p>The Cost and Revenue Types on the tasks added from the template are set to No Cost and Not Billable</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Hours</td> 
   <td>Project information is preserved</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Queue Details, Topic Groups, Queue Topics, Routing Rules</td> 
   <td> <p>Transferred from template</p> <p>If you select the <strong>Queue Properties &amp; Issues Setup</strong> option during the attachment process, the Queue Details of the template overwrite those of the project. In this case, the Routing Rules, Queue Topics, and Topic Groups of the template are added to those of the project. <br>If the project is set up as a request queue and the template you attach to the project is not set up as a request queue, the queue information of the project is removed if you leave the <strong>Queue Properties &amp; Issues Setup</strong> box checked. <br>If you deselect the <strong>Queue Properties &amp; Issue Setup</strong> box, all the Queue Setup settings of the project are preserved and no Queue Setup settings from the template are attached.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Task Constraints</td> 
   <td> <p>Transferred from template </p> <p>If deselected during the attachment process, the task constraints are set to As Soon As Possible or As Late As Possible, depending on the project Schedule From setting. </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr> 
   <td>Task Predecessors</td> 
   <td> <p>Transferred from template</p> <p>If deselected during the attachment process, all predecessor connections between the template tasks are removed.</p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Sharing Options</td> 
   <td> <p>If deselected during the attachment process, project permissions remain unchanged.</p> <p>If selected during the attachment process, the template permissions are added to or overwrite those of the project. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If User A has View permission to the project, but they have Manage permissions on the template, after attaching the template User A will gain Manage access to the project.</p> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

  

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2> </h2>
<h2>Understand changes to project fields when attaching a template</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and replaced with the table above, per Anna)</p>
-->
<!--
<p>Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved. </p> <note type="important">
Not all project fields are available to manage in the process of attaching a template to a project. For information, see
<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md" class="MCXref xref">Attach a template to a project</a>.
</note>
<p>The following scenarios exist when attaching a template to an existing project: </p>
<ul>
<li> <p><a href="#project-fields-that-are-empty-and-the-template-information-updates-them" class="MCXref xref">Project fields that are empty and the template information updates them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-the-template-information-overwrites-them" class="MCXref xref">Project fields that are populated and the template information overwrites them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-they-remain-unchanged-after-attaching-the-template" class="MCXref xref">Project fields that are populated and they remain unchanged after attaching the template</a> </p> </li>
</ul> <note type="important">
Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template all template fields transfer to the new project. Attaching a template leaves some of the existing project's fields unchanged.
</note>
<p><strong>Project fields that are empty and the template information updates them</strong></p>
<p>Most project fields that are empty are populated with template information when attaching the template to an existing project. </p>
<p><strong>Project fields that are populated and the template information overwrites them</strong></p>
<p>The following fields always overwrite or update existing project information with template information when you attach a template to the project and they cannot be managed during attaching the template: </p>
<ul>
<li> <p><b>Resource manager</b>: The template Resource Managers are added to the list of existing resource managers on the project.</p> </li>
</ul>
<ul>
<li> <p><b>Financial Information</b>: You can indicate whether you want financial information to transfer from the template or to keep the existing financial information on the project in the process of attaching a template. However, when the Financial Information option is selected to indicate that you intend to keep the information from the template, the following fields are updated on the project: </p>
<ul>
<li> <p> The updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li>
<li> <p>The updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li>
</ul> </li>
</ul>
<ul>
<li> <p><b>Filter Hour Types</b> </p> </li>
</ul>
<ul>
<li> <p><b>Access settings</b> </p> </li>
</ul>
<ul>
<li> <p><b>Custom Forms</b>: Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project Sponsor</p> </li>
<li> <p style="font-weight: bold;">Group</p> </li>
<li> <p style="font-weight: bold;">Company</p> </li>
<li> <p style="font-weight: bold;">Currency</p> </li>
<li> <p style="font-weight: bold;">Milestone Path</p> </li>
<li> <p><b>Completion Mode</b> </p> </li>
<li> <p style="font-weight: bold;">Resource Pool</p> </li>
<li> <p style="font-weight: bold;">Tasks Settings fields</p> </li>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p style="font-weight: bold;">Issue Settings fields</p> </li>
</ul>
</div>
<p> </p>
</div>
-->

 
