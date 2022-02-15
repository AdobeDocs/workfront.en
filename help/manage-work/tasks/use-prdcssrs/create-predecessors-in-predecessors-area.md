---
filename: create-predecessors-in-predecessors-area
product-area: projects
navigation-topic: use-predecessors
---



# Create a predecessor relationship using the Predecessors area {#create-a-predecessor-relationship-using-the-predecessors-area}

You can use predecessor tasks (or just predecessors) to link tasks that depend on other tasks to start or complete. For example, you would not want to host a party (dependent task) before you send out the invitations (predecessor task).


This article shows how you can set predecessors using the Predecessors tab within a task.


For information about setting predecessors in a list of tasks, see [Create a predecessor relationship on the task list](create-predecessors-on-task-list.md).


You can view the predecessors of tasks in the following areas of *`Adobe Workfront`*:



* In the Predecessors `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section </MadCap:conditionalText>`of the dependent tasks
* In the Gantt Chart
* In the task list in the Predecessors column


For information about predecessors, see [Overview of task predecessors](predecessors-overview.md). 



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


## Create a predecessor for a task {#create-a-predecessor-for-a-task}




1.  Go to a task that you want to designate as a dependent task, then click `Predecessors` in the left panel. 


   You might need to click `Show More`, then `Predecessors`. 

1.  Click `+Add Predecessor`. 
1.  (Optional) To add a cross-project predecessor, replace the name of the project in the `Parent Project` field with another project, then type the name of the task or tasks that you want as the predecessors. 


   For information about adding cross-project predecessors, see [Create cross-project predecessors](cross-project-predecessors.md).

1.  Type in the name of the task or tasks that you want to designate as the predecessors. 


   ![](assets/add-predecessor-box-nwe-350x465.png)



1.  Select a `Dependency Type`.


   For information about task Dependency Types, see a [Overview of task dependency types](task-dependency-types.md).

1.  Specify a `Lag` amount in days. 


   For information about Lag Types, see ​ [Overview of Lag Types](lag-types.md).

1.  Select `Enforced` if you want to enforce the predecessor relationship between the two tasks. 


   For information about enforcing predecessors, see [Enforce predecessors](enforced-predecessors.md).

1.  Click `Save`. 



