---
filename: edit-tasks
product-area: projects
navigation-topic: manage-tasks
---



# Edit tasks {#edit-tasks}

You can edit information on tasks that you have created, or that you have Contribute or Manage permissions to. 


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Tasks and&nbsp;Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> 
    <ul> 
     <li> <p>Contribute permissions to a task to edit it in the Task Details area </p> </li> 
     <li> <p>Manage permissions to a task to edit it in the Edit Task box</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Contribute or higher permissions to the project</p> </li> 
    </ul> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Limitations for editing tasks {#limitations-for-editing-tasks}

There are some limitations that might prevent you from editing tasks. 


Consider the following when editing tasks: 



* Updating tasks triggers notifications for projects that are a Current status. To avoid confusion for users who are assigned to the tasks, limit editing tasks as much as possible when the project is in the Current status. 
*  You cannot edit tasks that are in an Approval Process. You can only log time or update the Status for a task in an approval process. 


  ![](assets/edit-task-in-approval-process-nwe-350x148.png)



* You can edit and add documents to tasks on a project that has a status of Complete, Dead, or is Pending Approval only when your *`Workfront administrator`* `or a *`group administrator`*` enabled this functionality in the Project Preferences area. For information about setting project preferences, see [Configure system-wide project preferences](set-project-preferences.md). 

* You can always edit the following information on a task when the project has been marked Complete, Dead, or is in an Approval Process:
    
    
    * Log time
    * Edit existing expenses
    * Attach a custom form
    
    






## Edit a task in a list {#edit-a-task-in-a-list}

You can edit task information in a list of tasks, by inline editing fields displayed in the view of the list. 


For information about editing tasks in lists, see [Edit tasks in a list](edit-tasks-in-a-list.md).



## Edit a task in a list using the Summary {#edit-a-task-in-a-list-using-the-summary}

You can edit a task in a list using the Summary panel. For information about editing a task in the Summary panel, see the "Edit a task in the Summary" section in the [Edit tasks in a list](edit-tasks-in-a-list.md) article.


## Edit a task in the Edit Task box {#edit-a-task-in-the-edit-task-box}

You can edit a task using the Edit Task or Task Details areas. The following steps describe editing a task in the Edit Task box. 




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*.

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <span class="bold">Projects</span>, then <span class="bold"> </span></MadCap:conditionalText>`click the name of a project to open it.
1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <span class="bold">Tasks</span> in the left panel.</MadCap:conditionalText>` 
1.  Click the task you want to edit.
1.  
   (Optional) To edit limited information about a task, click `Task Details` in the left panel. 


   ![](assets/nwe-task-details-expanded-350x273.png)




   Consider editing information in the following areas in the Task Details section:

    
    
    *  `Overview` 
    
    
      This area is expanded by default.
    
    *  `Custom Forms` 
    
    
      Names of customs forms display only if there are custom forms attached to the object.
    
    *  `Finance` 
    
    


   >[!NOTE]
   >
   >Depending on how your *`Workfront administrator`* or *`Group administrator`* modified your Layout Template, the fields in the Task Details area might be rearranged or not display. For information, see [Customize the Details view using a layout template](customize-details-view-layout-template.md).


   For information about the fields visible in the Task Details section,


   continue with editing the task in the Edit Task box as described below.


   To edit information in the Details section, do the following: 

    
    
    1.  (Optional) Click the `Collapse All` icon ![](assets/collapse-all-icon.png) in the upper-right corner to collapse all areas. 
    1.  (Optional and conditional) When an area is collapsed, click the `right-pointing arrow` ![](assets/right-pointing-arrow.png) next to each area to expand the area you want to edit. 
    1.  `<MadCap:snippetBlock src="assets/edit-fields-in-details-section-all-objects-step.flsnp" />` For more information about editing information in the Task Details tab, see the following articles:
    
        
        
        *  [Manage task information in the Task Details Overview area](task-information-in-overview.md) 
        *  [Manage task finances in the Task Details section](task-finances-in-details.md) 
        
        
    
    1.  (Optional) If there are no custom forms attached to the task, start typing the name of a form in the `Add custom form` field, then select it when it displays in the list, then click `Save Changes`.
    1.  (Optional) Click the `Export` icon ![](assets/export.png) to export the Overview and custom forms information to a PDF file, then click `Export`. Select from the following:
    
        
        
        *  Select all (displays only when there is at least one custom form attached)
        *  Overview
        *  The name of one or multiple custom forms
        
        
       The PDF file downloads to your computer. 
    
    
       ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)    
    

    
    
       For more information, see [Export custom forms and object details in Adobe Workfront](export-custom-forms-details.md).
    
    
    
1.  To edit all information about the task, click the `More` menu ![](assets/more-icon.png) next to the name of the task, then click `Edit`.


   Or


   From a list of tasks, select a task, then click the `Edit` icon ![](assets/edit-icon.png) at the top of the list.


   The Edit Task box opens. 


   >[!IMPORTANT] {type="important"}
   >
   >You must have Manage permissions to the task in order to see the Edit option.


   All task fields are available in the Edit Task box and are grouped by the areas listed in the left panel.


   >[!NOTE]
   >
   >Depending on how your *`Workfront administrator`* or *`Group administrator`* modified your Layout Template, the fields in the Task Details area might be rearranged or not display. For information, see [Customize the Details view using a layout template](customize-details-view-layout-template.md).


   Consider specifying information in any of the following sections: 

    
    
    *  [Task Name](#task) 
    *  [Overview](#overview) 
    *  [Assignments](#assignme) 
    *  [Custom Forms](#custom%c2%a0f) 
    *  [Finance](#finance) 
    *  [Settings](#settings) 
    
    


   >[!NOTE]
   >
   >Depending on how your *`Workfront administrator`* or *`Group administrator`* sets up our Layout Template, the fields in the Edit Task box might be rearranged or not display. For information, see [Customize the Details view using a layout template](customize-details-view-layout-template.md).







### Task Name {#task-name}




1.  Begin editing your task as described above.
1.  Click `Task Name` in the left panel. 


   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)



1.  Update the name of the task.  

1.  Click  `Save` or continue with the following sections. 




### Overview {#overview}




1.  Begin editing your task as described above.
1.  Click `Overview` in the left panel. 


   ![](assets/nwe-overview-section-edit-task-box-350x257.png)



1.  Update the following information about the task: 

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Add additional information about the task. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-MediumGray" colspan="2" role="rowheader"><span style="font-weight: bold;">Basic information section</span> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Status</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select the status of the task which indicates what stage of development the task is in.</p> <p>Tip: You can update the task Status in the task header. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Priority</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>This is a visual flag for you which allows you to prioritize your tasks. </p> <p>Select from the following options: </p> 
    <ul> 
     <li> <p> None</p> </li> 
     <li> <p> Low </p> </li> 
     <li> <p>Normal </p> </li> 
     <li> <p>High </p> </li> 
     <li> <p> Urgent </p> </li> 
    </ul> <p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For information about task priorities, see <a href="task-priority.md" class="MCXref xref">Update Task Priority</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-LightGray" colspan="2" role="rowheader"><span style="font-weight: bold;">Task&nbsp;dates and constraints section</span> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Task Constraint</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Decide when the task must be completed by specifying a Task Constraint. </p> <p>Select from the following options: </p> 
    <ul> 
     <li> <p><span>Fixed Dates</span> </p> <p>Specify a <span class="bold" style="font-weight: bold;">Planned Start</span> and a <span class="bold" style="font-weight: bold;">Planned Completion Date</span>. </p> </li> 
     <li> <p><span>Must Start On</span> </p> <p>Specify a <span class="bold">Planned Start Date</span>. </p> </li> 
     <li> <p><![CDATA[
]]><span>Must Finish On </span></p> <p>Specify a <span class="bold">Planned Completion Date</span>. </p> </li> 
    </ul> 
    <ul> 
     <li> <p><![CDATA[
]]><span>As Soon as Possible</span><![CDATA[
]]></p> </li> 
     <li> <p><span>As Late as Possible</span><![CDATA[

]]></p> </li> 
     <li> <p><span>Earliest Available Time</span><![CDATA[

]]></p> </li> 
     <li> <p> <span>Latest Available Time</span><![CDATA[

]]></p> </li> 
     <li> <p><span>Start No Later Than</span> </p> </li> 
     <li> <p>Specify a Planned Start Date</p> </li> 
     <li> <p><span>Start No Earlier Than</span> </p> <p>Specify a <span class="bold">Planned Start Date</span>. </p> </li> 
     <li> <p> Finish <span>No Later Than</span></p> <p>Specify a <span class="bold">Planned Completion Date</span>. </p> </li> 
     <li> <p> Finish <span>No Earlier Than</span></p> <p>Specify a <span class="bold">Planned Completion Date</span></p> </li> 
    </ul> <p>For more information on Task Constraint, see <a href="task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Commit Date and time</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>This is the date by which the user assigned to the task commits to have it completed. This can be different than the Planned Completion Date. Only assignees can edit this field. For information about Commit Dates in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, see <a href="overview-of-commit-dates.md" class="MCXref xref">Commit Date overview</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Planned Start Date and time</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>When the task is planned to start. The planned start date of a task is set and influenced by a number of factors:</p> 
    <ul> 
     <li>Depending on the system-wide preference for the task planned start date, the start date of a new task on a project can either be today, or the start date of the project, by default. <span>The <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> for the group associated with the project can also set this preference for the group.</span> For more information about the system-level or group-level task preferences, see <a href="set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</li> 
     <li>Depending on the predecessors of the task, the planned start date is picked by <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> to be the next available date after the predecessors finish, or start, depending on the predecessor relationship. For more information about predecessor relationships, see <a href="predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</li> 
     <li>The project manager or the task owner can manually set the planned start date when the task constraint is either Fixed Dates or Must Start On. For more information about task constraints, see <a href="task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Planned Completion Date and time</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The anticipated completion date as shown when the task is planned. The planned completion date can be set by a number of factors:</p> 
    <ul> 
     <li>The planned completion date is calculated from the planned start date by adding the Duration of the task to the planned start date. When the project manager or <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> specifies the Duration of the task, this triggers an update to the planned completion date. If the planned date changes, it will often be because the Duration of the has been updated.</li> 
     <li>The project manager or the task owner can manually set the planned completion date when the task constraint is either Fixed Dates or Must Finish On. For more information about task constraints, see <a href="task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</li> 
     <li>If the Duration Type of the task changes, and the number of resources on the tasks changes at the same time, the planned completion date will change, as well. For more information about duration types, see <a href="task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Actual Start Date and time</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Specify an Actual Start Date for the task. The default is typically automatically populated when you change the status of the task to In Progress. The actual start date can also be manually modified by the project manager, or the task owner. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Actual Completion Date and time</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Specify the actual date and time when the task completes. The default date and time when a task is completed always coincides with the actual time when the status becomes Completed. The actual completion date can also be manually modified by the project manager, or the task owner. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column1-MediumGray" role="rowheader" colspan="2">Working time section</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.Work_Effort variable varname">Work Effort</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> 
    <div> 
     <p>The amount of effort required to complete the task. Your project manager might decide to use this field instead of Planned Hours to estimate the effort needed to complete a task. This field is visible only when the following conditions are met:</p> 
     <ul> 
      <li> <p>The task has a Simple Duration&nbsp;Type. </p> <p>Tip: If you update the task Duration&nbsp;Type, this field becomes dimmed. </p> </li> 
      <li>Your project manager has enabled the Use <span style="font-weight: normal;" class="mc-variable WFVariables.Work_Effort variable varname">Work Effort</span> to automatically calculate task Planned Hours field on the project. </li> 
     </ul> 
     <p>Select from the following options:</p> 
     <ul> 
      <li>Small</li> 
      <li>Medium <span style="font-weight: normal;">(this is the default value for a new task)</span></li> 
      <li>Large</li> 
     </ul> 
     <p>Note: Updating the amount of effort could update the task Planned Hours. The update is immediate if the project Update Type is Automatic. When the project Update Type is Manual you must recalculate timeline to see the updated Planned Hours. </p> 
     <p>For information about using <span class="mc-variable WFVariables.Work_Effort variable varname">Work Effort</span> instead of Planned Hours to estimate task effort, see <a href="work-effort.md" class="MCXref xref">Work Effort overview</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>


1.  Click  `Save` or continue with the following sections. 




### Assignments {#assignments}




1.  Begin editing your task as described above.
1.  Click  `Assignments` in the left panel. 


   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)



1.  Click `Search people, role and teams` and start typing the name of a user, role, or team that you want to assign to the task, then click it or press Enter when it displays on the list. You can assign multiple users or job roles to a task. You can assign only one team to a task. 

   ` `**Tip: **`` You can assign multiple users, or job roles, and you can assign only one team. `You can assign only active users, `job roles`, and teams.`


   `If a user, `job role`, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:` 

    
    
    *  `Reassign the work item to active resources.` 
    *  `Associate the users in a deactivated team with an active team and reassign the work item to the active team.` 
    
    

1.  (Optional) Indicate whether an assignee is the primary assignee on the task, by selecting the `Owner` radio button next to their name. A team cannot be the primary assignee of a task. 
1.  (Conditional and optional) Update the following fields: 

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Duration Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>This identifies the relationship between the following: </p> 
    <ul> 
     <li> <p>The number of resources assigned to a task </p> </li> 
     <li> <p>The total effort required to complete the task </p> </li> 
     <li> <p> The total duration of the task. </p> </li> 
    </ul> <p>Your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> <span> or a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span></span> selects the default Duration Type setting for the tasks in your system or your group. For information about setting project defaults, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> <p>Duration Types enable you to set consistent resource assignments based on the needs of the task. For more information about the Duration Type of a task, see <a href="task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>. </p> <p>Select from the following options: </p> 
    <ul> 
     <li> <p>Calculated Assignment </p> </li> 
     <li> <p> Calculated Work </p> </li> 
     <li> <p>Effort Driven </p> </li> 
     <li> <p>Simple</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Duration per Occurrence</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>This displays only on the parent of recurring tasks. It displays the duration of each recurring task. For information about creating recurring tasks, see <a href="create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>. </p> <p>Note: Durations modified in individual recurring tasks do not display the value indicated in this field. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Duration</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> 
    <div> 
     <div> 
      <p>This is the amount of time that you allow a task to remain open before it is completed. </p> 
      <p>Important: Because the task duration is typically the amount of time between the Planned Start and the Planned Completion Dates, it affects the timeline of the project.</p> 
      <p>To indicate the Duration of the task and the unit of time do the following:</p> 
      <ul> 
       <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Type the length of time and select from the units of time available in the drop-down menu.</p> <p>Tip: When you update the Duration of tasks in a task list, you can use the abbreviation for the unit of time. </p> </li> 
      </ul> 
      <p> You can choose from the regular time or elapsed time options in the following table: </p> 
      <table style="width: 100%;mc-table-style: url('../../../Resources/TableStylesheets/Standard.css');" class="TableStyle-Standard" cellspacing="3"> 
       <col class="TableStyle-Standard-Column-Column1"> 
       <col class="TableStyle-Standard-Column-Column1" data-mc-conditions=""> 
       <tbody> 
        <tr class="TableStyle-Standard-Body-LightGray"> 
         <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Unit of Time</td> 
         <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="font-weight: bold;">Abbreviation</td> 
        </tr> 
        <tr class="TableStyle-Standard-Body-MediumGray"> 
         <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Minutes</td> 
         <td class="TableStyle-Standard-BodyD-Column1-MediumGray">M</td> 
        </tr> 
        <tr class="TableStyle-Standard-Body-LightGray"> 
         <td class="TableStyle-Standard-BodyE-Column1-LightGray">Hours</td> 
         <td class="TableStyle-Standard-BodyD-Column1-LightGray">H</td> 
        </tr> 
        <tr class="TableStyle-Standard-Body-MediumGray"> 
         <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Days.&nbsp;This is the default. </td> 
         <td class="TableStyle-Standard-BodyD-Column1-MediumGray">D</td> 
        </tr> 
        <tr class="TableStyle-Standard-Body-LightGray"> 
         <td class="TableStyle-Standard-BodyE-Column1-LightGray">Weeks</td> 
         <td class="TableStyle-Standard-BodyD-Column1-LightGray">W</td> 
        </tr> 
        <tr class="TableStyle-Standard-Body-MediumGray"> 
         <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Months</td> 
         <td class="TableStyle-Standard-BodyD-Column1-MediumGray">T</td> 
        </tr> 
        <tr class="TableStyle-Standard-Body-LightGray"> 
         <td class="TableStyle-Standard-BodyE-Column1-LightGray">Elapsed Minutes</td> 
         <td class="TableStyle-Standard-BodyD-Column1-LightGray">EM</td> 
        </tr> 
        <tr class="TableStyle-Standard-Body-MediumGray"> 
         <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Elapsed Hours</td> 
         <td class="TableStyle-Standard-BodyD-Column1-MediumGray">EH</td> 
        </tr> 
        <tr class="TableStyle-Standard-Body-LightGray"> 
         <td class="TableStyle-Standard-BodyE-Column1-LightGray">Elapsed Days</td> 
         <td class="TableStyle-Standard-BodyD-Column1-LightGray">ED</td> 
        </tr> 
        <tr class="TableStyle-Standard-Body-MediumGray"> 
         <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Elapsed Weeks</td> 
         <td class="TableStyle-Standard-BodyD-Column1-MediumGray">EW</td> 
        </tr> 
        <tr class="TableStyle-Standard-Body-LightGray"> 
         <td class="TableStyle-Standard-BodyB-Column1-LightGray">Elapsed Months</td> 
         <td class="TableStyle-Standard-BodyA-Column1-LightGray">ET</td> 
        </tr> 
       </tbody> 
      </table> 
      <p>Note: Elapsed time is a unit of time for a task's Duration. It is the time between the Planned Start Date and the Planned Completion Date of a task that includes holidays, weekends, and time off. In other words, elapsed time is the passage of calendar days. Regular time takes into account holidays, weekends, and time off and excludes them from the Duration of the task. For more information about task duration, see <a href="task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>. </p> 
      <p> </p> 
     </div> 
    </div> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Planned Hours</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Specify the amount of Planned Hours for the task, in hours. This is the amount of actual time it would take the assignees of the task to complete it. You can only specify the amount of Planned Hours for a task when the Duration Type is set to Calculated Assignment. For more information about duration types, see <a href="task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Allocation</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>If your Task Constraint is Calculated Work or Effort Driven, specify the <span class="bold">Allocation %</span> (allocation percentage) for each assignee. This is the amount of time from the schedule of the assignee that they can spend on this task. Changing the allocation percentage for an assignee will change the Planned Hours of a task. </p> <p>When the Task Constraint is Simple, you can specify the following:</p> 
    <ul> 
     <li> <p>Allocation Hours of each assignee.</p> </li> 
     <li> <p>Planned Hours of the task</p> </li> 
     <li> <p>Duration of the task</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Assignee's&nbsp;Role</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Select a role from the <span class="bold">Assignee's Role</span> drop-down menu when you selected a person as an assignee. This is the role that the assignee can fulfill on this task. </p> <p>Tip: Only the job roles associated with each assignee in their profile appear in the drop-down menu.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  Click  `Save` or continue with the following sections. 





### Custom&nbsp;Forms {#custom-forms}

You can define default custom forms to be automatically attached to tasks when the tasks are added to a project. For information about setting up the project to include default task custom forms for all new tasks, see the "Tasks"section in the article [Edit projects](edit-projects.md). 



1.  Begin editing the task as described above.
1.  Click `Custom Forms` in the left panel, or click the name of a custom form if it is already attached. 


   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)



1.  Click `Add custom form` and select the custom form or forms that you want to associate with the task. You must build the custom forms before they are available to select in this field. Only active custom forms display in the list. 


   For more information about building custom forms, see [Create or edit a custom form](create-or-edit-a-custom-form.md).You can add up to ten custom forms to a task.

1.  (Conditional) If you attached a custom form to the task, edit any fields on the form. You must specify all required fields before you can save the task.


   >[!NOTE]
   >
   >Depending on how your *`Workfront administrator`* set the permissions for the sections in your custom form, not everyone can view or edit the same fields on a given custom form. The permissions to edit fields within a section of a custom form depend on the permissions you have on the task itself. `For information about setting task permissions, see [Share a task in Adobe Workfront](share-a-task.md).`



1.  Click  `Save` or continue with the following sections. 




### Finance {#finance}




1.  Begin editing your task as described in the [Edit tasks](#edit2) section&nbsp;in this article.
1.  Click  `Finance` in the left panel. 


   ![](assets/nwe-finance-section-edit-task-box-350x298.png)



1.  Update the following fields:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Cost Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Specify the Cost Type for the task. This is going to determine how the cost of the task is calculated, based on the number of hours on the tasks. </p> <p>Select from the following options: </p> 
    <ul> 
     <li> <p>No Cost</p> </li> 
     <li> <p>Fixed Hourly </p> </li> 
     <li> <p> User Hourly </p> </li> 
     <li> <p> Role Hourly</p> </li> 
    </ul> <p>For more information about tracking costs, see <a href="track-costs.md" class="MCXref xref">Track costs</a> . Your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> or a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> selects the default Cost Type setting for the tasks in your system or your group. For information about setting project defaults, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> .</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Revenue Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Specify the Revenue Type for the task. This is going to determine how the Revenue on the task is calculated, based on the number of hours on the tasks. </p> <p>Select from the following options: </p> 
    <ul> 
     <li> <p> Not Billable </p> </li> 
     <li> <p>User Hourly </p> </li> 
     <li> <p>Role Hourly </p> </li> 
     <li> <p>Fixed Hourly </p> </li> 
     <li> <p>User Hourly w/Cap </p> </li> 
     <li> <p>Role Hourly w/Cap </p> </li> 
     <li> <p>User Hourly Plus Fixed </p> </li> 
     <li> <p>Role Hourly Plus Fixed </p> </li> 
     <li> <p>Fixed Revenue </p> </li> 
    </ul> <p>For more information about tracking revenue, see<a href="billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a> . </p> <p>Your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> or <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> selects the default Revenue Type setting for the tasks in your system or your group. For information about setting project defaults, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Save` or continue with the following section.




### Settings {#settings}




1.  Begin editing your task as described in the [Edit tasks](#edit2) section&nbsp;in this article. 
1.  Click `Settings` in the left panel.


   ![](assets/nwe-settings-section-edit-task-box-350x304.png)



1.  Update the following fields: 

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Tracking Mode</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Specify how the progress status of the task is tracked. </p> <p>Select from the following options: </p> 
    <ul> 
     <li> <p> User Must Update </p> </li> 
     <li> <p>Assume on Time </p> </li> 
     <li> <p>Ignore Late Warnings</p> </li> 
     <li> <p> Autocomplete </p> </li> 
     <li> <p>Predecessor </p> </li> 
    </ul> <p>For more information about the Tracking Mode on tasks, see <a href="task-tracking-mode.md" class="MCXref xref">Task Tracking Mode overview</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Resource Leveling</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select the <span class="bold">Exclude from Resource Leveling</span> field if you want the resources assigned to the task to be excluded from leveling.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Leveling Delay</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Specify the Leveling Delay, in hours. </p> <p> For more information about leveling delays, see <a href="task-leveling-delay.md" class="MCXref xref">Update task Leveling Delay</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Approval process</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Select an approval process that you want to associate with the task. Your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> must define system-level Approval Processes before you can associate them with tasks. A user with administrative access to Approval processes can also create group-specific approval processes. </p> <p>For more information about creating Approval Processes, see <a href="create-approval-processes.md" class="MCXref xref">Create an approval process</a>. Consider the following when adding approval processes: </p> 
    <ul> 
     <li> <p>Only active approval processes display in the list. </p> </li> 
     <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list. </p> <p>Important:  If the group of the project changes, the group-specific approval process previously attached becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="how-changes-affect-group-approvals.md" class="MCXref xref">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
     <li> <p>You can define default approval processes to be automatically attached to tasks when the tasks are added to a project. For information about setting up the project to include default task approval processes, see the "Tasks" section in the article <a href="edit-projects.md" class="MCXref xref">Edit projects</a>. </p> </li> 
     <li> <p>When bulk-editing tasks, the following scenarios exist: </p> 
      <ul> 
       <li> <p>When you select multiple tasks from the same group, both system-level and group-level approval processes display in this field. </p> </li> 
       <li> <p>When you select multiple tasks from different groups, only system-level approval processes display in this field. </p> </li> 
       <li> <p>When any of the tasks have a single-use approval process attached, it is replaced by the system-level or group-level approval process you select. </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Save`. 


&nbsp;



## Edit a task in the task header (limited) {#edit-a-task-in-the-task-header-limited}

You can edit a limited amount of information in the task header. 


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)




You can edit the following fields in the task header:



* Task name
* Percent complete
* Assignments
*  Planned Completion Date `and time` 


  ` `**Warning: **``Some Task Constraints and other dependencies might prevent you from editing this field. For information about Task Constraints, see [Task Constraint overview](task-constraint-overview.md).   


* Status
* Make approval decisions if you are set as the approver in a current approval process





## Edit tasks in bulk {#edit-tasks-in-bulk}


You can edit tasks in bulk in a list and update all their information at the same time when you select to automatically save the changes you are making to tasks in the list. 


For information about saving tasks in bulk , see the "Edit tasks in bulk" section in the article [Edit tasks in a list](edit-tasks-in-a-list.md).
