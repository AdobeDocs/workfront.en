---
filename: create-advanced-assignments
product-area: projects;user-management
navigation-topic: assign-tasks
---



# Create advanced assignments {#create-advanced-assignments}

You can manage task or issue assignments by using Advanced Assignments. 


You can adjust the following assignment information when making advanced assignments:



* Assign users to the task or issue (this can be accomplished outside of an advanced assignment).
* Adjust and redistribute the number of hours each assignee is allocated.
* Determine which user should be designated as the owner of the task or issue.
* Specify which role each user is fulfilling when working on the task or issue.




>[!NOTE]
>
>When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks and issues. For information about schedules, see [Create a schedule](create-schedules.md).




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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to&nbsp;Tasks and Issues</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Contribute or higher permissions to a the task or issue</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Make advanced assignments {#make-advanced-assignments}




1. Go to the project where you want to assign a task or an issue. 
1.  Click `Tasks` or `Issues` in the left panel, then click the name of a task or issue in the list. 


   >[!TIP] {type="tip"}
   >
   >You can make advanced assignments directly on the task or issue list if there are two or more people assigned. Click inside the `Assignments` field on the same line as the task or issue, then click the `People icon` to open the Advanced Assignments window. Skip to step 5 to continue creating advanced assignments.  
   >![](assets/nwe-advanced-assignments-350x55.png)   >
   >




1.  Click `Assign to` in the `Assignments` field in the header of the task or issue. 
1.  Click `Advanced`. 
1.  In the `Search people, role and teams` field, start typing the name of a user, role, or team then click the name when it appears in the drop-down list. 


   >[!NOTE]
   >
   >If the user's name contains a special character, you must include the special character in the search field. 



1.  (Optional) Continue adding assignees in the `Search people, role or teams`box to add multiple resources to the task or issue.

   ` `**Tip: **`` You can assign multiple users, or job roles, and you can assign only one team. `You can assign only active users, `job roles`, and teams.`


   `If a user, `job role`, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:` 

    
    
    *  `Reassign the work item to active resources.` 
    *  `Associate the users in a deactivated team with an active team and reassign the work item to the active team.` 
    
    

1.  For each user in the `Assignee` column, specify the following information:

    
    
    *  `Owner`: Hover over the name of the assignee and click `Make Primary` in the Owner field if you want to mark the assignee as the Task Owner. A green checkbox indicates that the specified user is the Primary Contact of the task or issue. *`Adobe Workfront`* marks the first user or job role that you assign to a task or issue as the Owner or Primary Assignment. A team cannot be designated the Primary Owner of a task or issue. 
    
    
      >[!IMPORTANT] {type="important"}
      >
      >Depending on how your *`Workfront administrator`* `or *`group administrator`*` set up your project preferences, *`Workfront`* might use the schedule of the task owner to calculate the timeline of the task when you have multiple users assigned to the task. For information about multiple task assignees, see the "Assign multiple users to a task" section in the article [Assign tasks](assign-tasks.md). 
    
    
    
    *   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span class="bold"> Allocations</span> </MadCap:conditionalText>`: When the Duration Type of a task is Simple, specify the number of hours each user should be assigned to the task or issue. The sum of all assigned hours for each user is equal to the number in the `Planned Hours` field at the bottom of the `Hours` column. In all other cases, specify the percentage of time (or allocation)&nbsp;that you want the assignee to spend solving the task or issue. 
    *  `Assignee's Role:` Select the role the user should use when fulfilling this assignment. `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> The Primary Role of the user displays by default. Click in the Assignee's Role box to select another role. </MadCap:conditionalText>``<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  When you assign the task or the issue to a role first, and then add a user who can fulfill that role as a second assignment, the list of suggested users is filtered for the users who can fulfill the roles already assigned to the task and issue. </MadCap:conditionalText>`
    
    
      ![](assets/advanced-assignments-box-select-a-role-350x243.png)    
    

    
    * `Duration Type`: This is only available for tasks. Click the name of the Duration Type and select a Duration Type from the drop-down menu. For information about Duration Types, see [Overview of Task Duration and Duration Type](task-duration-and-duration-type.md).
    
    *  `Duration:` You can update this field for a task when you have Manage permissions to the task. 
    
    
      For more information, see [Overview of Task Duration and Duration Type](task-duration-and-duration-type.md). When bulk editing assignment information, a similar dialogue box appears to assign users, hours, allocation, and task owner.
    
    *  `Planned Hours`: When the Duration Type is Calculated Assignment or Simple, update the number of Planned Hours. The allocation percentages or the hours for each resource are distributed evenly as a result. *`Workfront`* calculates the Planned Hours when the Duration Type is Calculated Work or Effort Driven. For more information, see [Overview of Task Duration and Duration Type](task-duration-and-duration-type.md).
    
    
      ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x239.png)    
    

    
    
    

1.  Click `Save`. 


