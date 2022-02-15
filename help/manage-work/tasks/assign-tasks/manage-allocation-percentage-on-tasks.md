---
filename: manage-allocation-percentage-on-tasks
product-area: projects;user-management
navigation-topic: assign-tasks
---



# Manage allocation percentage on tasks {#manage-allocation-percentage-on-tasks}

Allocation percentage represents the amount of time an assigned resource is planned to work on a task in a day. It is the percent of a work day (according to the user or project schedule) at which a resource is allocated throughout the duration of the task. You cannot modify the percentage allocation of a resource assigned to an issue.


>[!NOTE]
>
>Consider the following when assigning work to users:
>
>
>
>* You must have a Plan or a Work license and have at least Contribute permissions to a task to be able to make or manage assignments to the task.
>* When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks and issues. For information about schedules, see [Create a schedule](create-schedules.md). 
>
>






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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Modify the percent allocation for a task {#modify-the-percent-allocation-for-a-task}




1. Go to a task for which you are changing the percent allocation.
1.  Click the `More` menu ![](assets/qs-more-icon-on-an-object.png) next to the name of the task, then click `Edit`.
1. In the `Overview` section, ensure that the Duration Type of the task is one of the following:  

    
    
    * Calculated Work
    * Effort Driven
    
      ` `**Tips: **``    
        
        
        * For the Calculated Assignment Duration Type, *`Workfront`* uses the following formula to calculate the allocation percentage of the assignees: 
        
        
        
        
          ```        
          Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day
          ```        
        
          .
        
        
        
    
        
        
        * For the Simple Duration Type, you can estimate the hours assigned to each resource, not the allocation percentage. 
        
        
    
    
    

1.  Click `Assignments`, then modify the `Allocations` for each task assignee. 


   You can only modify the allocation percentage for user and job role assignments. 


   You cannot modify the allocation percentage for a team assigned to a task.

1. Click `Save`.


