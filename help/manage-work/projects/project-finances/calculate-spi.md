---
filename: calculate-spi
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
---



# Calculate Schedule Performance Index (SPI)  {#calculate-schedule-performance-index-spi}

The Schedule Performance Index (SPI) describes the relationship between the planned schedule and actual schedule.  *`Adobe Workfront`* calculates SPI&nbsp;at the project and task levels. Project managers review this metric to identify whether tasks or projects are currently tracking ahead of or behind schedule. &nbsp;



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


## Schedule Performance Index (SPI) overview {#schedule-performance-index-spi-overview}




* [What the SPI value shows](#understanding-the-cpi-value) 
* [How Workfront calculates SPI](#understanding-how-spi-is-calculated) 




### What the SPI&nbsp;value shows {#what-the-spi-value-shows}

Project managers understand that a SPI&nbsp;value of 1 means the project is on plan or on schedule. &nbsp;Values greater than 1 indicate a project is ahead of schedule, and values less than 1 mean a project is behind schedule. &nbsp;The further from 1, the greater deviation from the plan.



### How *`Workfront`* calculates SPI  {#how-workfront-calculates-spi}

*`Workfront`* calculates SPI by the following formula:




```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```




*&#42;If Planned Hours Scheduled to Date = 0, SPI = 1*.


Planned Hours Schedule to Date are calculated at the minute when you perform the calculations. It shows the number of Planned Hours planned to the current date. It can be recalculated automatically when you change your finance data to be accurate. There is no field in *`Workfront`* that indicates&nbsp;this value. 


For example, if you have a project with 1 task and the task has 10 planned hours and a 10-day Duration, the Planned Hours Schedule to Date on the 5th day are&nbsp;5.&nbsp; 


## Locate SPI in a project or task {#locate-spi-in-a-project-or-task}




1. Go to the project or task where you want to view SPI.
1.  Depending on whether you want to view SPI on a project or a task, do one of the following:

    
    
    1. Click `Project Details` in the left panel, then view the `Finance` area.
    
    1. Click `Task Details` in the left panel, then view the `Finance` area. 
    
    
    

1. Find the `CPI/ SPI/ CSI` field. 


