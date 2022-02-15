---
filename: convert-issues
product-area: projects
navigation-topic: convert-issues
---



# Overview of converting issues in *`Adobe Workfront`* {#overview-of-converting-issues-in-adobe-workfront}

If more work needs to be done to complete an issue after the issue is submitted, you can convert the issue to a project or to a task.


For information about converting issues to tasks, see [Convert an issue to a task in Adobe Workfront](convert-issue-to-task.md).


For information about converting issues to projects, see [Convert an issue to a project in Adobe Workfront](convert-issue-to-project.md).


## Considerations when converting issues {#considerations-when-converting-issues}




* Your *`Workfront administrator`* or *`group administrator`* has already set the preferences for what happens to an issue, its resolution, and the its Primary&nbsp;Contact's access when it is converted to a project or a task, as outlined in [Configure system-wide task and issue preferences](set-task-issue-preferences.md).

* *`Workfront`* removes any approvals that are associated with issues during conversion.
* *`Workfront`* overwrites the Resolving Object of the issue when you convert it to a task or an project. The new task or issue becomes the new Resolving Object of the issue after conversion. 
* Consider the following: 
    
    
    * During conversion, you might be asked whether you want to keep the issue and its resolution tied to the project or task you are creating.
    * If you keep the issue, the status and percent complete of the project or task automatically update the status and the percent complete of the issue when any changes occur on the project, task, or the issue or when the *`Workfront`* recalculates the timeline. 
    
    
* When converting an issue to a project using a template, most information from the template transfers to the new project. However, some information from the issue can also transfer to the new project.&nbsp;For more information, see the [Overview of project fields when converting an issue to a project using a template](#overview) section in this article. 
*  While converting an issue, not all documents or their information are moved to the new object that the issue is converted to. The following items are included when you convert an issue that has documents or document links attached:

    
    
    *  Document
    *  Document links to third-party services, such as Google Drive or SharePoint.
    *  Versions
    *  Proofs are included only when the option `Keep the original issue and tie its resolution to this task`is unselected.
    * Document approvals are not included when you convert an issue that has documents and document links attached.
    
    

* If you decided to keep the issue in the conversion and it has documents attached, the document and its versions are copied to the project or the task. The *`proofs`* and the document approvals are not copied to the project or the task.  

* If you decided to not keep the issue in the conversion, and it has documents attached, the document, its versions, and the *`proofs`* transfer to the project or the task. The document approvals will not transfer to the project or the task.  

* If you have documents and folders linked to the original issue from third party services, like Google Drive, regardless of whether you are keeping the issue or not during the conversion, those links will be copied to the new object.
* Issue comments are also copied to the task or project converted from the issue, but tagged users will not transfer.
* If you want to transfer custom form information from the issue to the project or task you are converting it to, ensure you have a project or task custom form that include the same fields you want to transfer from the issue. For more information, see [Transfer custom form data to a larger work item](transfer-custom-form-data-larger-item.md). 





## Overview of project fields when converting an issue to a project using a template {#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template}

When converting an issue to a project, you can either convert it to a blank project or use a template. 


For information, see [Convert an issue to a project in Adobe Workfront](convert-issue-to-project.md).


When using a template, some fields that are populated on the template transfer to the project created from the converted issue. Other fields transfer to the project from the converted issue. 


The following table lists project information and whether it transfers from the template or from the issue: 

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStylesheets/Standard.css');" class="TableStyle-Standard" cellspacing="3"> 
 <col class="TableStyle-Standard-Column-Column1" style="width: 109px;"> 
 <col class="TableStyle-Standard-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Description</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray"> <p>The Description of the issue transfers to the new project. </p> <p> If there is no description on the issue, the Description from the template transfers to the project. </p> <p>If the Description field is empty both for the issue and for the template, the field is empty on the project. </p> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: bold;">Status</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray">Default status selected for the group on the template. If the template is not associated with the group, the project status is set to the default status set by the <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> in the Project&nbsp;Preferences area of Setup. For information, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Priority</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray">Transfers from the template. </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: bold;">URL</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray"> <p>The URL&nbsp;from the issue transfers to the new project. </p> <p> If there is no URL specified on the issue, the URL from the template transfers to the project. </p> <p>If the URL&nbsp;field is empty both for the issue and for the template, the field is empty on the project. </p> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Project&nbsp;Condition Type</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray">Transfers from the template.</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: bold;">Project&nbsp;Condition</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray">Matches the system-level default preference as determined by the <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> in the Setup area. For information, see <a href="set-custom-condition-default-projects.md" class="MCXref xref">Set a custom condition as the default for projects</a></td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Schedule From</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray">Transfers from the template.</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: bold;">Project dates</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>Planned Start Date</b>: The closest working time based on the template schedule's working time should be preselected, according to the timezone of the template's schedule. This field is disabled if the Schedule From field is set to From&nbsp;Completion. </p> </li> 
     <li> <p><b>Planned Completion Date</b>: The closest working time based on the template schedule's working time should be preselected, according to the timezone of the template's schedule. This field is disabled if the Schedule From field is set to From&nbsp;Start. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Portfolio</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray">Transfers from the template.&nbsp;Otherwise, this field is empty.</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: bold;">Program</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray">Transfers from the template.&nbsp;Otherwise, this field is empty.</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Group</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray">Transfers from the template.&nbsp;Otherwise, it is set to the Home Group of the logged-in user who is performing the conversion. </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: bold;">Company</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray">Transfers from the template.&nbsp;Otherwise, this field is empty.</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Project Owner</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray">Transfers from the Template Owner field on the template. Otherwise, it is set to the logged-in user who is performing the conversion. </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: bold;">Project Sponsor</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray">Transfers from the Template Sponsor field on the template. Otherwise, this field is empty.</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Resource&nbsp;Manager</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray">Transfers from the template. Otherwise, this field is empty.</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: bold;">Task Settings</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray">Transfer from the template.</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Issue Settings</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray">Transfer from the template. </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray" style="font-weight: bold;">Access</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray"> <p>Transfers from the Access section on the template. </p> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyB-Column1-LightGray" style="font-weight: bold;">Approvals</td> 
   <td class="TableStyle-Standard-BodyA-Column1-LightGray">Transfer from the template. The approvals associated with the issue are removed during the conversion. </td> 
  </tr> 
 </tbody> 
</table>



## View original issue information on projects and tasks {#view-original-issue-information-on-projects-and-tasks}

You can view the original issue information in project and task lists and reports `or in the Project Details area`. For information about building reports, see [Create a custom report](create-custom-report.md). 


The following table illustrates which&nbsp;issue fields are visible from the converted projects and tasks. 

` `**Warning: **``If the Primary&nbsp;Contact of an issue changes or if the issue becomes unlinked from the project or task after the issue has been converted, the Converted Issue Originator Name does not update and it displays the original&nbsp;Primary&nbsp;Contact of the issue at the time the issue was converted. 
