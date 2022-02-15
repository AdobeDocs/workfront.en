---
filename: calculate-bcws
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
---



# Calculate Budgeted Cost of Work Scheduled (BCWS) {#calculate-budgeted-cost-of-work-scheduled-bcws}



## Overview of Budgeted Cost of Work Scheduled (BCWS) {#overview-of-budgeted-cost-of-work-scheduled-bcws}

Also known as the Planned Value, the Budgeted Cost of Work Scheduled (BCWS) is a project performance metric that represents the amount of the task that should have completed at the time when this metric is calculated.


*`Adobe Workfront`* calculates the Budgeted Cost of Work Scheduled (BCWS) for both projects and tasks.


Consider the following when reviewing the values for the BCWS on a task or project:



*  *`Workfront`* calculates the BCWS for a task based on your configuration for the Performance Index Method (PIM) of the project.


  You can configure your project to calculate the PIM using hours or cost and the BCWS is also calculated using the same values.


  For information about configuring how the BCWS is calculated, see the section [Configure how BCWS is calculated](#configur) in this article.

*  *`Workfront`* calculates the BCWS for a project by adding all the BCWS values from all the parent tasks and individual tasks on the project.


  The values from children tasks are not added to the BCWS of the project.






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


## Configure how BCWS is calculated {#configure-how-bcws-is-calculated}

You can configure whether the BCWS is calculated in hours or costs by configuring how the Performance Index Method (PIM) of the project is calculated.



1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Go to a project and click  <span class="bold">Project Details</span> in the left panel.</MadCap:conditionalText>`
1.  In the `Finance` area, locate the `Performance Index Method` field and double click it to edit it.


   ![](assets/pim-options-hour-cost-based-350x144.png)



1.  Select from the following options:


1.  Click  `Save Changes`.


   The BCWS of the tasks on the project is calculated using hours or costs.





## Calculate BCWS {#calculate-bcws}

*`Workfront`* calculates the Budgeted Cost of Work Scheduled (BCWS) for tasks or projects by using the following formulas:



* 

  ```
  Task BCWS = Planned Percent Complete x Task Budget
  ```

* 

  ```
  Project BCWS = SUM(BCWS values of all parent and individual tasks)
  ```



The following values are used in this calculation:

For example, if it is February 12 today, and a task is scheduled to last from February 10 to February 20, the task should be 20% complete today. If the Task Budget (Planned Cost) is $10,000, then the BCWS for the task is:




```
Task BCWS = 20% x $10,000 = $2,000
```




## Locate the BCWS for a project or a task {#locate-the-bcws-for-a-project-or-a-task}

You can view the value of the Budgeted Cost of Work Scheduled in a report or list, by adding the BCWS column to your view.



1. Go to a list of tasks or projects.
1. Expand the `View` menu and select `New View` or `Customize View`.

1. Click `Add Column`.
1.  In the `Show in this column:` field start typing `BCWS` and click to select it when it displays in the list.


   ![](assets/bcws-in-project-view.png)



1. Click `Save View`.
1. The `BCWS` field displays in the view.


