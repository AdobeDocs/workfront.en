---
filename: enforced-predecessors
product-area: projects
navigation-topic: use-predecessors
---



# Enforce predecessors {#enforce-predecessors}

Predecessors are tasks on which other tasks are dependent for completion. Predecessor relationships affect the Start and Completion Dates of the tasks and ultimately impact the timeline of the project. 


For information about predecessors, see [Overview of task predecessors](predecessors-overview.md).


By setting predecessor relationships between tasks, you define how the start or finish of a dependent task depends upon the start or finish of their predecessor tasks. This is done by using different Dependency Types. 


For information about Dependency Types, see [Overview of task dependency types](task-dependency-types.md).


## Overview of enforced predecessors {#overview-of-enforced-predecessors}



>[!IMPORTANT] {type="important"}
>
>You must enforce predecessors to require that predecessor relationships are respected. Without enforcing the predecessors, dependent tasks can start and finish independently from the start and finish of their predecessors, regardless of their Dependency Types. 


You can enforce the predecessor relationship when setting predecessors on a project. 


If a predecessor is enforced, the successor task cannot start before the predecessor completes. For example, enforcing a Finish-Start relationship between Task A and Task B means that Task B cannot start (the Status must remain New, and the Percent Complete must remain 0%) until Task A is marked as completed. Enforcing relationships apply to all predecessor types.



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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Enforce a predecessor at the task level {#enforce-a-predecessor-at-the-task-level}




1. Go to the successor task whose predecessor you want to enforce.
1.  Click `Predecessors` in the left panel, then click `Add Predecessor`. You might need to click `Show More`, then `Predecessors`. 
1. (Conditional) If you want to add a cross-project predecessor, remove the name of the project in the `Parent Project` field and replace it with another project. 
1. Specify the name of the predecessor task or tasks in the `Tasks` field. 
1.  Specify the `Dependency Type` between these two tasks.


   The default `Dependency Type` is `Finish-Start`.


   ![](assets/ep-350x408.png)



1. Select the `Enforced` field to enforce the predecessor.
1. Click `Save`.




## Enforce a predecessor in a task list {#enforce-a-predecessor-in-a-task-list}




1. Go to a task list on a project.
1. From the `View` drop-down menu, select the `Standard View`. 

1. Make a mental note of the number of task which you are going to designate as the predecessor.
1. Find the successor task whose predecessor you want to enforce. 
1. In the `Predecessors` column, start entering the number of the predecessor task followed by "e". For example, type "1e" to add task number 1 as a predecessor to the selected task. 
1.  Click Enter to save your predecessor information for the task. 


   ![predecessor_enforced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)





