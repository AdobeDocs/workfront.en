---
filename: calculate-cpi
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
---



# Calculate Cost Performance Index (CPI) {#calculate-cost-performance-index-cpi}

The Cost Performance Index (CPI) describes the relationship at the project or task level between the planned cost and actual cost. Project Managers review this metric to identify tasks or projects currently tracking under or over cost at a given point. Cost can be measured in hours or dollars, depending on your Performance Index Method (PIM). For more information about setting the Performance Index Method, see [Set the Performance Index Method (PIM)](set-pim.md).


Only organizations that require time entry can use CPI. Furthermore, cost-based PIM values are accurate only in organizations that have defined cost rates for task assignees (job roles or users). 



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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Review variable varname">Review</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>View access to Projects and Financial&nbsp;Data</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View or higher permissions to the project with permissions to View Finance</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Overview of the Cost Performance Index (CPI) {#overview-of-the-cost-performance-index-cpi}




* [The CPI value](#understanding-the-cpi-value) 
* [How CPI is calculated](#understanding-how-cpi-is-calculated) 




### The CPI value {#the-cpi-value}

Project managers understand that a CPI value of 1 means the project is exactly on budget. Values greater than 1 indicate a project is under budget (fewer hours or expenses have been recorded than originally planned), and values less than 1 mean a project is over budget (more hours or expenses have been recorded than originally planned). The further from 1, the greater deviation from the plan.



### How CPI is calculated {#how-cpi-is-calculated}

In *`Adobe Workfront`*, the calculation for CPI depends on the Performance Index Method selected for the project. For more information about setting the Performance Index Method, see [Set the Performance Index Method (PIM)](set-pim.md).



* [CPI calculations when using Hour-based PIM](#cpi-calculations-when-using-hour-based-pim) 
* [CPI Calculations when using Cost-based PIM](#cpi-calculations-when-using-cost-based-pim) 




#### `CPI calculations when using Hour-based PIM`  {#cpi-calculations-when-using-hour-based-pim}

If 

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```




Otherwise 

```
CPI = 1
```





* `For a non-parent task:`   


  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```


* `For a parent task:`   
  Total Budgeted Cost Work Performed = the sum of the Total Budgeted Cost Work Performed field for all direct child tasks.

* `For a project:`   
  Total Budgeted Cost Work Performed = the sum of the Total Budgeted Cost Work Performed field for all top level tasks (parents and standalone tasks). 



For information about the total Budgeted Cost Work Performed (BCWP), see [Calculate Budgeted Cost Work Performed (BCWP)](calculate-bcwp.md).


#### `CPI Calculations when using Cost-based PIM`  {#cpi-calculations-when-using-cost-based-pim}

If 

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```

<![CDATA[ ]]>


Otherwise 

```
CPI = 1<![CDATA[ 
]]>
```




The fields in this calculation are described below:



*  Total Actual Cost = Actual (logged) Hours &#42; Hourly Rate of assignees 
* Incurred Actual Expense Cost = the same as Actual Cost 
*  Incurred Expense is the expense on which Actual Cost>0 
*  Planned Cost of Incurred Expenses= Total of Planned Cost of all incurred expenses 
*  Planned Cost of Work Performed is calculated by the following formula:




  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100<![CDATA[
					]]>
  ```





The Total Budgeted Cost Work Performed is calculated for the following:<![CDATA[		]]>



* <![CDATA[			]]> `For a non-parent task:`  


  ```
  Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
  ```


* `For a parent task:`   
  Total Budgeted Cost Work Performed = the sum of the Total Budgeted Cost Work Performed field for all direct child tasks.

* `For a project:`   
  Total Budgeted Cost Work Performed = the sum of the Total Budgeted Cost Work Performed field for all top level tasks. 





## Locate CPI in a project or task {#locate-cpi-in-a-project-or-task}

You can display the CPI of a project or a task in a project or task list or report. In addition, you can view it at the project or task level. 



1. Go to the project or task where you want to view the CPI.
1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Expand  <span class="bold">Project Details</span> or  <span class="bold">Task Details</span> in the left panel, depending on whether you are viewing CPI for a project or task.</MadCap:conditionalText>`
1.  Click `Finance`.


   The CPI displays in the `CPI/ SPI/ CSI` field. 



