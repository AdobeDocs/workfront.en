---
filename: update-task-status
product-area: projects
navigation-topic: update-work-in-a-project
---



# Update task status {#update-task-status}

You can update a task's status to inform others about where the task is (and the overall project) and how it is progressing.


The default statuses are New, In Progress, and Complete. Your *`Adobe Workfront administrator`* can add custom statuses for your organization. For more information, see [Create or edit a status](create-or-edit-a-status.md).


You can manually update task statuses or you can let *`Workfront`* automatically update them when certain actions take place. 



## Access requirements {#access-requirements}

You must have the following access to manually update tasks: 

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Manually update task status {#manually-update-task-status}

When you are updating a task status, you can also type an explanation about the new status and change other task information such as the due date.



1. Go to a task that you are assigned to for which you want to update the status.
1.  Click the `Status` field in the task header and select a new status. 
1.  (Optional) Do any of the following to provide additional information about the update, then click `Update` or, if the task has the `Complete` status, click `Done:`

    
    
    *  To add a note about the update, go to the `Updates` `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> area </MadCap:conditionalText>`and click `Start a new update`, then type your note.  

    * To notify certain users about the update, type their names in the `Notify` box that appears when you type a note about the update.
    * To update the condition of the task, click `Select Condition` to the right of the `Notify` box (these appear when you type a note about the update), then select the condition that best reflects the current condition of the task.
    
    * To update the Commit Date of the task, expand the `Commit Date` drop-down calendar, and select a new Commit Date. 
    
    





## Automatically update task status {#automatically-update-task-status}

*`Workfront`* automatically updates the existing status of a task to a different status when the actions listed in the table below occur.


>[!NOTE]
>
>The statuses in the following table are default system statuses. Your *`Workfront administrator`* or a *`group administrator`* can rename the statuses in your instance of *`Workfront`*. For information about creating and managing statuses in *`Workfront`*, see [Create or edit a status](create-or-edit-a-status.md).



<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Action</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Original Status</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="font-weight: bold;">New Status</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Update the task percent complete to 100%</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">New or In Progress</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Complete</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Update the task percent complete from 100% to a lower number</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Complete</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">In Progress</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><span>Click the Start Task button to accept working on a task assigned to you</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><span>New</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p><span>Any status associated with the Start Task button in your Home Team settings. </span> </p> <p><span>For information about replacing the Work On It button with a Start Task button, see </span><span href="work-on-it-button-to-start-button.md"><a href="work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span><span>. </span> </p> <p>Tip: <span>Clicking </span><span data-mc-conditions="QuicksilverOrClassic.Quicksilver">the Undo button</span><span> after clicking Start Task reverts the status to New. </span> </p> </td> 
  </tr> 
 </tbody> 
</table>

