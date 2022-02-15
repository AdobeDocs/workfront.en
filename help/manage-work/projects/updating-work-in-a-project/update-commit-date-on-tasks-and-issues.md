---
filename: update-commit-date-on-tasks-and-issues
product-area: projects
navigation-topic: update-work-in-a-project
---



# Update Commit Dates on tasks and issues {#update-commit-dates-on-tasks-and-issues}

You can manually update the Commit date of a task or an issue that you are assigned to. For more information about Commit Dates in  *`Adobe Workfront`*, see [Commit Date overview](overview-of-commit-dates.md).


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Tasks and Issues</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions on the task or issue</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

Before you begin, you must be assigned to the task or issue you need to update the Commit Date for. 


## Update Commit Dates on tasks and issues {#update-commit-dates-on-tasks-and-issues-1}

Updating the Commit Date is identical for tasks and issues.



1.  Go to a task or issue that you are assigned to as the `Task Owner`.


   For more information about finding out who the Task Owner for an issue or task is, see the section [Edit tasks](edit-tasks.md#assignments) in the article [Edit tasks](edit-tasks.md).

1.  Click `<MadCap:conditionalText style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Work on it</MadCap:conditionalText>``<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> in the task or issue header</MadCap:conditionalText>`


   Or


   Click `Start Task` or `Start Issue` if the `<MadCap:conditionalText style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Work on it</MadCap:conditionalText>` button has been customized in your environment to indicate that you are now working on the work item. 


   At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.

1.  (Optional) If you clicked Start Task or Start Issue, click `Undo` in the lower-left corner of the screen. The Commit Date is removed. 


   For information about replacing the Work On It button with a Start button, see ` [Replace the Work On It button with a Start button](work-on-it-button-to-start-button.md)`.


   >[!TIP] {type="tip"}
   >
   >`The option to undo your selection to start your work is not available when you click` `Work on it` `.` 



1.  
   Click `Updates` in the left panel, then click the `Start a new update` > `Commit Date`


   Or


   Click `Task Details` or `Issue Details` in the left panel, then double click  `Commit Date` and select a new date from calendar, then click  `Save Changes`. 
   ![](assets/commit-date-calendar-picker-in-updates-stream-nwe-350x452.png)



   The following things happen after making this change:&nbsp;

    
    
    *  The Commit Date and the Planned Completion date are no longer the same. 
    
    
      Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.
    
    
      ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)    
    

    
    *  The changes are saved automatically when you select a new date from the Updates area.
    *  The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. 
    
    
      ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)    
    

    
    
      For information about the notifications and updates that are triggered by this change, see the section [Notifications and updates triggered by changing the Commit Date](overview-of-commit-dates.md#notifica) in the article [Commit Date overview](overview-of-commit-dates.md).
    
    
    



