---
filename: budgeted-cost
content-type: reference
product-area: projects
navigation-topic: financials
---



# Calculate Budgeted Cost {#calculate-budgeted-cost}

The Budgeted Cost of a project is the total cost associated with the project as estimated when you plan the project.


## Overview of Budgeted Cost in a project {#overview-of-budgeted-cost-in-a-project}

You cannot manually change the Budgeted Cost of a project. *`Adobe Workfront`* calculates the Budgeted Cost using the following formula: 




```
Budgeted Cost = Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project
```





*  The `Budgeted Labor Cost` in the calculation above is the cost associated with the job roles in the project.


  You can track the Budgeted Labor Cost of a project in the following area of *`Workfront`*:

    
    
    * Resource Budgeting area of the Business Case or the *`Resource Planner`*
    
    
  For information about Budgeted Labor Costs, see the article [Understand Budgeted Labor Cost and Budgeted Hours for projects](budgeted-labor-cost.md). 

* The `Budgeted Expenses Cost` in the calculation above is the Planned Cost associated with the expenses on the project, as they are calculated in the Expenses area of the Business Case or the Expenses tab of the project.  
  For more information about Expenses on a project, see the article [Manage project expenses](manage-project-expenses.md).

* The `Fixed Cost` in the calculation above is the fixed amount associated with the Cost of the project, as defined in the Finances `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> area of the Details section </MadCap:conditionalText>`of the project.  
  For more information about the Finance sub-tab of a project, see the article [Manage information in the project Finance area](manage-project-finance-area.md).





>[!NOTE]
>
>*`Workfront`* calculates all cost information using the currency of the project. If you specify Budgeted Hours for your resources in the *`Resource Planner`*, the option to change project currency is disabled. 
>
>
>For more information about changing the currency of a project, see the article [Change the project currency](change-project-currency.md).





## Locate the Budgeted Cost of a project {#locate-the-budgeted-cost-of-a-project}

You can view the following Budgeted Cost information in *`Workfront`*:



*  The Budgeted Cost as reflected in the Resource Budgeting area of the Business Case or the *`Resource Planner`* displays in the following areas of *`Workfront`* under the following names:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Budgeted Cost display name</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" style="font-weight: bold;">Area of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Budgeted Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Business Case Summary</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Portfolio Optimizer</p> <p>Tip: The total of all project Budgeted Cost values is the Budgeted Cost of the portfolio.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Project Budgeted Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Project report</p> <p>Project (Financial Data) report</p> <p>Task report</p> <p>Issue report</p> <p>Budgeted Hour report</p> <p>For more information about creating a report, see the article <a href="create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>




