---
filename: calculate-bcwp
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
---



# Calculate Budgeted Cost of Work Performed (BCWP)  {#calculate-budgeted-cost-of-work-performed-bcwp}



## Overview of Budgeted Cost of Work Performed (BCWP) {#overview-of-budgeted-cost-of-work-performed-bcwp}

Also known as the Earned Value, the Budgeted Cost of Work Performed (BCWP) is a project performance metric that represents the amount of the task that has actually completed at the time when this metric is calculated.


*`Adobe Workfront`* calculates the Budgeted Cost of Work Performed (BCWP) for both projects and tasks.


Consider the following when reviewing the values for the BCWP on a task or project:



*  *`Workfront`* calculates the BCWP for a task based on your configuration for the Performance Index Method (PMI) of the project.


  You can configure your project to calculate the PMI using hours or cost and the BCWP is also calculated using the same values.


  For information about configuring how the BCWP is calculated, see the section [Configure how BCWP is calculated](#configur) in this article.

*  *`Workfront`* calculates the BCWP for a project by adding all the BCWP values from all the parent tasks and individual tasks on the project.


  The values from children tasks are not added to the BCWP of the project.






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


## Configure how BCWP is calculated {#configure-how-bcwp-is-calculated}

You can configure whether the BCWP is calculated in hours or costs by configuring how the Performance Index Method (PIM) of the project is calculated.



1.  


   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Go to a project and expand  <span class="bold">Project Details</span> in the left panel.</MadCap:conditionalText>` 

1.  In the `Finance` area, locate the `Performance Index Method` field and double click to edit it. 


   ![](assets/pim-options-hour-cost-based-350x144.png)



1.  Select from the following options:


1.  Click  `Save Changes`.


   The BCWP of the tasks on the project is calculated using hours or costs.





## Calculate BCWP {#calculate-bcwp}

*`Workfront`* calculates the Budgeted Cost of Work Performed (BCWP) for a task or project using the following formulas:



* 

  ```
  Task BCWP = Actual Percent Complete x Task Budget
  ```

* 

  ```
  Project BCWP = SUM(BCWP values of all parent and individual tasks)
  ```



The following values are used in these calculation:

For example, if the actual percent complete of the task is 25% and the Task Budget or the Planned Cost is $10,000, then the BCWP for the task is: 




```
BCWP = 25% x $10,000 = $2,500
```




## Locate the BCWP for a project or a task {#locate-the-bcwp-for-a-project-or-a-task}

You can view the value of the Budgeted Cost of Work Performed in a report or list, by adding the BCWP column to your view.



1. Go to a list of tasks or projects.
1. Expand the `View` menu and select `New View` or `Customize View`.

1. Click `Add Column`.
1.  In the `Show in this column:` field start typing `BCWP` and click to select it when it displays in the list.


   ![](assets/bcwp-project-view.png)



1. Click `Save View`.
1. The BCWP field displays in the view.


