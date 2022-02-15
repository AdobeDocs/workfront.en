---
filename: attach-template-to-project-overview
content-type: overview
product-area: templates
keywords: overwrite,field,overwritten
navigation-topic: templates-navigation-topic
---



# Overview of attaching a template to a project {#overview-of-attaching-a-template-to-a-project}

When you attach a template to an existing project, you are modifying some of the information on the project according to that of the template. Some of the information on the project remains unchanged.


For information about how to attach a template to a project, see [Attach a template to a project](attach-template-to-project.md).



## Considerations when adding templates to projects {#considerations-when-adding-templates-to-projects}

Consider the following when adding templates to projects:



*  You can attach only active templates to projects.
*  You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your *`Adobe Workfront administrator`* `or a *`group administrator`*` has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see [Configure system-wide project preferences](set-project-preferences.md).
*  Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project.
*  Most template settings are added to the project. Some project settings are preserved. For information, see the section [Understand changes to project fields when attaching a template](#understa2) in this article.




## Understand changes to project fields when attaching a template {#understand-changes-to-project-fields-when-attaching-a-template}



>[!IMPORTANT] {type="important"}
>
>Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template, all template fields transfer to the new project. Attaching a template leaves some of the existing project fields unchanged.


Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved.


However, not all project fields are available to manage in the process of attaching a template to a project. For information, see [Attach a template to a project](attach-template-to-project.md).


The following table describes the default for what happens to project fields when you attach a template and which fields you can manage during the attachment process to override the default behavior:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStylesheets/Standard.css');" class="TableStyle-Standard" cellspacing="3"> 
 <col class="TableStyle-Standard-Column-Column1"> 
 <col class="TableStyle-Standard-Column-Column1"> 
 <col class="TableStyle-Standard-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Field</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">What happens in the process of attaching a template, by default</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="font-weight: bold;">Ability to manage the field updates in the attachment process </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="font-weight: bold;" colspan="3">Overview fields</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Description</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td style="text-align: center;" class="TableStyle-Standard-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;"> <p>Status</p> </td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">URL</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Transferred from template, if the field is empty on the project</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Priority</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Condition&nbsp;Type</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Schedule Mode</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Planned Dates</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Might change based on the added tasks</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Actual&nbsp;Dates</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Might change based on the added tasks</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Portfolio</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Program</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Group</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Company</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Transferred from template, if the field is empty on the project</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Planned Hours</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Might change based on the added tasks</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Project Owner</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Transferred from template, if the field is empty on the project</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Project Sponsor</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Transferred from template, if the field is empty on the project</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Resource Manager</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Added to the list of existing resource managers on the project</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="font-weight: bold;" colspan="3">Custom&nbsp;Forms section</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Custom&nbsp;Forms</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Added to the project, in addition to forms that are already on the project</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="font-weight: bold;" colspan="3">Finance fields</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Budget</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Currency</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">PIM</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">EAC</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Planned Benefit</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Actual Benefit</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="font-weight: bold;" colspan="3">Project Settings fields</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Milestone Path</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Transferred from template, if the field is empty on the project</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Completion Mode</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Summary Completion&nbsp;Mode</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Update Type</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Schedule</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">User&nbsp;Time Off</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Resource Leveling Mode</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Risk (project field)</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Resource Pools</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Added to the list of existing resource pools on the project</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Hour Types</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray"> <p>If deselected during the attachment process, the Hour Types setting on the project remains unchanged. </p> <p>If selected, the template setting transfers to the project. If Hour Type filtering is set to Yes both on the project and the template, the hour types from the template are added to the ones on the project.</p> </td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;"> <p>&nbsp;</p> <p>&nbsp;</p> <p>&nbsp;</p> <p>✓</p> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Reminder Notifications</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray"> <p>Added to the list of existing reminders on the project. </p> <p>If deselected during the attachment process, the project reminder notifications remain unchanged. </p> </td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="font-weight: bold;" colspan="3">Task Settings fields</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Task Default Approval Process</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Task Default Custom&nbsp;Forms</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Work&nbsp;Effort</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="font-weight: normal;" colspan="3"><span style="font-weight: bold;">Issue Settings fields</span> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;"><span>Allow users to add issues inline</span> </td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray"><span>Project information is preserved</span> </td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="font-weight: bold;" colspan="3">Access section </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">All settings</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Template settings overwrite those of the project</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="font-weight: bold;" colspan="3">Other objects and fields</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Tasks</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Added to the bottom of the task list, in addition to the existing project tasks</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Documents</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Added to the project, in addition to existing project documents</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Risks (objects in the Risks area of the project)</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Added to the project, in addition to existing project risks </td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Approval Process</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Transferred from template</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Billing Rates</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray"> <p>Transferred from template in addition to the existing billing rates on the project. </p> <p>If there is a different rate for the same job role on both the project and the template, the rate on the project remains unchanged. </p> </td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;"> <p>&nbsp;</p> <p>✓</p> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Billing Records</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Expenses</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Transferred from template in addition to the existing expenses on the project</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Financial Information</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray"> <p>When this is selected in the attachment process, the following fields are either transferred or added to the project:&nbsp;</p> 
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
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;"> <p>&nbsp;</p> <p>&nbsp;</p> <p>&nbsp;</p> <p>&nbsp;</p> <p>&nbsp;</p> <p>&nbsp;</p> <p>✓</p> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Hours</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project information is preserved</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="text-align: center;">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Queue Details, Topic Groups, Queue Topics, Routing Rules</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray"> <p>Transferred from template</p> <p>If you select the <span class="bold">Queue Properties &amp; Issues Setup</span> option during the attachment process, the Queue Details of the template overwrite those of the project. In this case, the Routing Rules, Queue Topics, and Topic Groups of the template are added to those of the project. <br>If the project is set up as a request queue and the template you attach to the project is not set up as a request queue, the queue information of the project is removed if you leave the <span class="bold">Queue Properties &amp; Issues Setup</span> box checked. <br>If you deselect the <span class="bold">Queue Properties &amp; Issue Setup</span> box, all the Queue Setup settings of the project are preserved and no Queue Setup settings from the template are attached.</p> </td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;"> <p>&nbsp;</p> <p>&nbsp;</p> <p>&nbsp;</p> <p>&nbsp;</p> <p>&nbsp;</p> <p>&nbsp;</p> <p>&nbsp;</p> <p>✓</p> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: normal;">Task Constraints</td> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray"> <p>Transferred from template </p> <p>If deselected during the attachment process, the task constraints are set to As Soon As Possible or As Late As Possible, depending on the project Schedule From setting. </p> </td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray"> <p>&nbsp;</p> <p>&nbsp;</p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: normal;">Task Predecessors</td> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray"> <p>Transferred from template</p> <p>If deselected during the attachment process, all predecessor connections between the template tasks are removed.</p> </td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray" style="text-align: center;">✓</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyB-Column1-LightGray" style="font-weight: normal;">Sharing Options</td> 
   <td class="TableStyle-Standard-BodyB-Column1-LightGray"> <p>If deselected during the attachment process, project permissions remain unchanged.</p> <p>If selected during the attachment process, the template permissions are added to or overwrite those of the project. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If User A has View permission to the project, but they have Manage permissions on the template, after attaching the template User A will gain Manage access to the project.</p> </td> 
   <td class="TableStyle-Standard-BodyA-Column1-LightGray" style="text-align: center;">✓</td> 
  </tr> 
 </tbody> 
</table>

&nbsp; &nbsp;
