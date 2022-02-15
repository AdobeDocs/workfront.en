---
filename: create-predecessors-on-task-list
product-area: projects
navigation-topic: use-predecessors
---



# Create a predecessor relationship on the task list {#create-a-predecessor-relationship-on-the-task-list}

You can use predecessor tasks (or just predecessors) to link tasks that depend on other tasks to start or complete. For example, you would not want to host a party (dependent task) before you send out the invitations (predecessor task). 


This article shows you how to create predecessors on the task list. 


You can view the predecessors of tasks in the following areas of *`Adobe Workfront`*:



* In the task list in the Predecessors column. 
* In the Gantt chart
* In the Predecessors `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section </MadCap:conditionalText>`of a dependent task 


For more information, see [Overview of task predecessors](predecessors-overview.md).



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


## Create a predecessor {#create-a-predecessor}




1. Go to a project. 
1.  Click `Tasks` in the left panel. 
1.  Ensure that your current view displays the `Predecessor` column. 


   If the view doesn't display the Predecessors column, change to a view that does, or add the column to your view. 

1.  Select the task that you want to designate as the dependent task. 
1. Click inside the `Predecessors` column.
1.  Type the task number that you want to designate as the predecessor of the selected task, then press `Enter`.


   The predecessor icon turns green when the predecessor task is marked complete. This signals that the dependent task is ready for work.


   For more information about the relationship types available in the Predecessors column, see [Overview of task predecessors](predecessors-overview.md) in [Overview of task predecessors](predecessors-overview.md).





## View predecessor details {#view-predecessor-details}

You can quickly view details about the predecessor from the task list.



1.  On the task list, mouse over the predecessor number in the `Predecessors` column.


   A box with the details of the predecessor displays. 


   ![](assets/cpr4-350x175.png)




   The following details are displayed:


   `Predecessor name:` The name of the predecessor that is being referenced. In the above example, the predecessor is Market Research.


   `Project name:` The name of the project where the predecessor resides. In the above example, the project name is Target Markets.


   `Number of predecessors (left of details box):` The number of predecessors for the predecessor being referenced. In the above example, the predecessor being referenced has 0 predecessors.


   `Requested:` The date when the predecessor task was requested.


   `Due Date:` The date when the predecessor task is due.


   `Number of successors (right of details box):` The number of successor (or dependent) tasks for the predecessor being referenced. In the above example, the predecessor being referenced has 1 successor.



