---
filename: project-planned-completion-date
content-type: overview
product-area: projects
navigation-topic: plan-a-project
---



# Overview of the project Planned Completion Date  {#overview-of-the-project-planned-completion-date}

The Planned Start and the Planned Completion Dates of a project rely on the dates of the tasks on the project.&nbsp;This article describes the Planned Completion Date of a project as well as that of a task. 


The Planned Completion Date of a project can be set manually or automatically, depending on whether you schedule the project from the Start or from the Completion Date.&nbsp;


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Manually set the Planned Completion Date of a project {#manually-set-the-planned-completion-date-of-a-project}

You must manually set the Planned Completion Date of a project when you schedule the project from Completion Date.&nbsp;


To schedule a project from Completion Date:



1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner, then click  <span class="bold">Projects</span>. </MadCap:conditionalText>`
1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click&nbsp; <span class="bold">New Project </span>then <span class="bold"> New Project</span>. </MadCap:conditionalText>`


   For more information about creating projects, see the article [Create a project](create-project.md).

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Select  <span class="bold">Project Details</span> in the left panel, then click the  <span class="bold">Edit Project</span> icon in the upper-right corner. </MadCap:conditionalText>`
1. In the `Schedule From` field, select `Completion Date`.

1. Specify the `Planned Completion Date` of the project.
1.  Click `Save Changes`.


   As you start adding tasks to your project, the `Planned Start Date` of the project calculates based on the total Duration of all of the tasks.&nbsp;





## Automatically set the Planned Completion Date of a project {#automatically-set-the-planned-completion-date-of-a-project}

The Planned Completion Date of a project is automatically calculated by *`Adobe Workfront`* when you schedule the project from Start Date.&nbsp;


To schedule a project from Start Date:



1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner, then click  <span class="bold">Projects</span>. </MadCap:conditionalText>`
1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click&nbsp; <span class="bold">New Project </span>then <span class="bold"> New Project</span>. </MadCap:conditionalText>`


   For more information about creating projects, see the article [Create a project](create-project.md).

1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Select  <span class="bold">Project Details</span> in the left panel, then click the  <span class="bold">Edit Project</span> icon in the upper-right corner. </MadCap:conditionalText>`
1. In the `Schedule From` field, select `Start Date`.

1. Specify the `Planned Start Date` of the project.
1.  Click `Save Changes`.


   As you start adding tasks to your project, the `Planned Completion Date` of the project calculates based on the total Duration of all of the tasks.&nbsp;


   For more information about Task Duration, see the article [Overview of Task Duration and Duration Type](task-duration-and-duration-type.md).


   The Planned Completion Date of the project coincides, in this case, with the Planned Completion Date of the last task on the project.





## The Planned Completion Date of a task {#the-planned-completion-date-of-a-task}

You can either specify the Planned Completion Date of a task, or you can leave it up to *`Workfront`* to calculate it depending on certain criteria.&nbsp;



* [Manually set the Planned Completion Date of a task](#manually-setting-the-planned-completion-date) 
* [How the Planned Completion Date is calculated for a task](#understanding-how-the-planned-completion-date-is-calculated) 




### Manually set the Planned Completion Date of a task {#manually-set-the-planned-completion-date-of-a-task}

Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task.&nbsp;


You can manually set the Planned Completion Date&nbsp;when creating a task, as described in&nbsp;the article [Create tasks in a project](create-tasks-in-project.md).


You can manually specify the Planned Completion Date when you select any of the following Task Constraints:&nbsp;

<table style="width: 649px;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" border="1" cellspacing="15" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Task Constraint Type</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p><span class="bold">Effect of Manually Changing the Planned Completion Date</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>Fixed Dates</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td> 
  </tr> 
 </tbody> 
</table>



### How the Planned Completion Date is calculated for a task {#how-the-planned-completion-date-is-calculated-for-a-task}

When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:



*  Task Constraint


  For more information about Task Constraints, see the article [Task Constraint overview](task-constraint-overview.md).

*  Task predecessor relationship


  For more information about task predecessors, see the article [Overview of task predecessors](predecessors-overview.md).

* Project Completion Date, when the project is scheduled from Completion Date.
*  The time off schedule of the Primary&nbsp;Assignee of the task. 


  When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the `Consider user time off in task durations` setting is selected for the `User Time Off` field. New projects inherit this setting from the Project&nbsp;Preferences area, but you can edit the setting at the project level. 


  For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. 


  For information about the `User Time Off` preference, see the articles [Configure system-wide project preferences](set-project-preferences.md) or [Edit projects](edit-projects.md).



When set automatically, the Planned Completion Date&nbsp;is determined based on the following calculation:&nbsp;




```
Planned Completion Date = Planned Start Date + Duration
```




For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26.


>[!NOTE]
>
>&nbsp;The Update Type for the project must also be&nbsp;set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically&nbsp;adjusted.   
>For more information about the Update Type, see the article [Select the project Update Type](select-project-update-type.md).


