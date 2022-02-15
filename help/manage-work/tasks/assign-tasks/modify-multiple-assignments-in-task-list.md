---
filename: modify-multiple-assignments-in-task-list
product-area: projects;user-management
navigation-topic: assign-tasks
---



# Modify multiple user assignments in a task list {#modify-multiple-user-assignments-in-a-task-list}

When managing task assignments, you can simultaneously modify them for multiple tasks at a time by using the bulk editing feature in a list of tasks. 

This article refers to modifying multiple user assignments for multiple tasks in a task list. Also see the following articles for modifying assignments on multiple tasks in other areas:



* For information about modifying assignments on multiple tasks in the Scheduling area, see [Modify multiple users assignments to tasks in the Scheduling areas](modify-multipl-assignments-scheduling-areas.md).
* For information about assigning tasks using the *`Workload Balancer`*, see [Overview of assigning work in the Adobe Workfront Workload Balancer](assign-work-in-workload-balancer.md).



For information about assigning a task to one resource in a list, see [Assign tasks](assign-tasks.md).



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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects and Tasks</p> <p>View or higher access to Users</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Contribute or higher permissions to tasks</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


##  



## Modify assignments for multiple tasks {#modify-assignments-for-multiple-tasks}




1. Go to the list that contains the tasks where you want to modify assignments.
1. (Optional) Create a filter to display only tasks assigned to the assignee that you want to modify.


   For example, if your project contains a specific role as the default assignee for multiple tasks, you can create a filter to display only tasks with that role as the assignee. Then, you can replace the role with a specific user. 


   Do the following to create a filter for your assignees:

    
    
    1. Click the `Filter` drop-down list, then click `New Filter.`
    
    
       The New Filter dialog box displays.
    
    1. Click `Add a Filter Rule.`
    1. To filter on a role, expand `Assignment Roles`, then click `ID`.
    
    
       >[!TIP] {type="tip"}
       >
       >Do not use the `Assigned to` field. This finds only the Primary Owner for the task instead of any of the roles that could be assigned to them. 
    
    
       Or
    
    
       To filter for a user, expand `Assignment Users,` then click `ID.`
    
    
       >[!TIP] {type="tip"}
       >
       >Do not use the `Assigned to` field. This finds only the Primary Owner for the task instead of any of the users that could be assigned to them. 
    
    
    
    1. In the drop-down list, select `Equal` as the filter qualifier.
    1. Begin typing the name of the user or role that you want to filter for, then click the name when it appears in the drop-down list.
    1. Click `Save Filter.`
    
    

1.  Select the tasks for which you want to modify assignments, then click the `Edit` icon ![](assets/edit-icon.png).  



  
   The Edit Tasks page displays. The items that you edit display in the upper-left corner of the page.

1. Go to the `Assignments` section.
1. Do one of the following to add or remove assignees:  


   >[!IMPORTANT] {type="important"}
   >
   >Removing assignees can affect the task hours and allocation percentages. For more information, see the section [Modify multiple user assignments in a task list](#removing-assignees-affects-task-hours-and-allocation-percentage) in this article. 



    
    
    1. `<li>&nbsp;To add a new assignee:  <ol>  <li value="1"><p>In the <span class="bold">Assignments</span> section, select <span class="bold">Assignee</span>.&nbsp;</p><p>Information that is common across all tasks selected displays. For example, if the same user is assigned to all tasks, that user displays in the <span class="bold">Assignee</span>&nbsp;column. If information is not common across the tasks selected, no information displays.</p></li>  <li value="2"><p>Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected tasks.</p>   <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">    <span class="autonumber"><span><b>Tip: </b></span></span>    <p>You can assign multiple users, or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams. </span></p>    <p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span></p>    <ul>     <li><p><span>Reassign the work item to active resources. </span></p></li>     <li><p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team. </span></p></li>    </ul>   </div></li> </ol></li>``<li>To remove individual assignees:  <ol>  <li value="1"><p>Click the <span class="bold">X icon</span> next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.</p><p>Or</p><p>(Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the tasks that you have selected, click <span class="bold">Remove Assignee</span> and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.</p></li> </ol></li>``<li>To remove all existing assignees:  <ol style="list-style-type: lower-alpha;">  <li value="1"><p>Click <span class="bold">Remove All Existing Assignees</span>, then click <span class="bold">Yes, Delete All Assignees</span>.</p><p>This removes not only common assignees (assignees that are displayed in the edit&nbsp;dialog box), but also all assignees on all the selected tasks.</p></li> </ol></li>`    
    
       >[!TIP] {type="tip"}
       >
       >Removing users from tasks can affect task hours and allocation percentages.&nbsp;For more information, see [Overview of modifying task assignments](modify-task-assignments-overview.md). 
    
    
    
    
    

1. (Optional) Modify any of the following options for assignees:  

    
    
    * (Conditional) `Allocation % or Hours`: Specify a new allocation percentage or hours. 
    
    
      >[!NOTE]
      >
      >This option can be modified only if the Duration Type is the same across all tasks that are being edited. When the Duration Type is Calculated Work or Effort Driven you can update the Allocation %. When the Duration&nbsp;Type is Simple you can update the Hours. For information about Duration&nbsp;Type, see [Overview of Task Duration and Duration Type](task-duration-and-duration-type.md).
      >
      >
      >If the field is blank, this means that the value is different across tasks; however, you are still able to modify it.

    
    
    
    * `Task Owner`: Select this option to make the assignee the owner of the task for all tasks being edited.
    * `Assignee's Role`: Select a role from the drop-down list. If left unselected, *`Adobe Workfront`* automatically selects the Primary Role of the user. 
    
    
    

1. Click `Save Changes.`


