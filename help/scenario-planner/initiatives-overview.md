---
filename: initiatives-overview
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
---



# Initiatives overview in the *`Adobe Workfront Scenario Planner`* {#initiatives-overview-in-the-adobe-workfront-scenario-planner}




##  


This is available only in *`the new Adobe Workfront experience`* and requires an additional license. For information about the *`Workfront Scenario Planner`*, see [The Adobe Workfront Scenario Planner overview](scenario-planner-overview.md). 
As a business manager, you can create initiatives for plans in the *`Adobe Workfront Scenario Planner`*. For information about creating plans, see the article [Create and edit plans in the Adobe Workfront Scenario Planner](create-and-edit-plans.md). 


## Initiatives overview {#initiatives-overview}

Using the *`Workfront Scenario Planner`*, you can estimate and review the following information for each initiative:



* Estimate the kind and number of job roles that might be required to complete the initiative. This adds to the Required job role count for the plan as well as calculates the People Costs that you can review for an initiative. 
* Estimate the Fixed Costs associated with the work needed to complete the initiative.
* Estimate the Planned Benefit that your company might gain when the initiative is completed.


To view information about your initiatives, you can access individual initiatives within a plan. For information about creating and accessing initiatives, see the article [Create and edit initiatives in the Adobe Workfront Scenario Planner](create-and-edit-initiatives.md). 


## Considerations about initiatives {#considerations-about-initiatives}

Consider the following when creating initiatives:



* You must create a plan before you can create an initiative. 
*  You can create initiatives from scratch or you can import projects into a plan. The projects become initiatives within the plan. 


  For information about creating initiative from scratch, see [Create and edit initiatives in the Adobe Workfront Scenario Planner](create-and-edit-initiatives.md).


  For information about importing projects into a plan to create initiatives from projects, see [Import projects to plans in the Adobe Workfront Scenario Planner](import-projects-to-plans.md). 

* Initiatives are smaller planning units than plans and they are created only as part of a plan.
* The shortest initiative can have a duration of 1 month. The longest initiative can have a duration of 5 years. 
* You cannot do actual work on an initiative. At the initiative level, you can define what resources are needed and what cost those resources will incur so you can start executing one of the demands of the plan. For example, if your company has a plan to expand and acquire a new office in a new location, your department might have an initiative to install the network infrastructure for that new location. 
* You can create multiple initiatives in a plan. With each initiative, you can outline a high-level strategy to accomplish the work in your department. 
* You can prioritize initiatives within a plan, to ensure that the most important initiative receives the most budget and the most resources. 
* When you create initiatives within a plan everyone that views that plan can also view all the initiatives within the plan.
* You can publish initiatives to create projects or to update the projects that are linked to them. For information about publishing initiatives, see [Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner](publish-scenarios-update-projects.md).




## Financial information about initiatives {#financial-information-about-initiatives}

You can review financial information about individual initiatives to understand how the initiatives fit within the plan. For information about accessing an initiative, see the article [Create and edit initiatives in the Adobe Workfront Scenario Planner](create-and-edit-initiatives.md).


You can view the following financial indicators about an initiative by accessing it within a plan:

<table style="width: 100%;mc-table-style: url('../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 200px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" style="width: 200px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" style="font-weight: bold;" rowspan="3" role="rowheader">Costs information</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column2-LightGray" style="font-weight: bold;">Costs total amount</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray" style="font-weight: bold;"> <p style="font-weight: normal;">This is a calculation of the total cost of an initiative. </p> <p style="font-weight: normal;"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates the total Costs value of an initiative using this formula:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column2-MediumGray" style="font-weight: bold;">Fixed Costs</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray" style="font-weight: bold;"> <p><span style="font-weight: normal;">This is a manual entry where you can estimate <span>a monthly amount of Fixed Costs for each month of the initiative. </span> This does not include the costs associated with the roles added to the initiative which are captured in the People Cost field. </span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column2-LightGray" style="font-weight: bold;">People Costs</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray" style="font-weight: normal;"> <p style="font-weight: normal;">This is a total calculation of the costs associated with the job roles of the initiative for the duration of the initiative. This number depends on how many FTEs you estimate for a job role for each month of the initiative. </p> 
    <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
     <span class="autonumber"><span><b>Tip: </b></span></span> 
     <ul> 
      <li> <p style="font-weight: normal;">The number of monthly FTEs for the same job role may be different from month to month. </p> </li> 
      <li> <p style="font-weight: normal;"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> considers that there are 160 working hours in one month. </p> </li> 
     </ul> 
    </div> <p style="font-weight: normal;"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates the People Costs of an initiative using the following formula:</p> <p style="font-weight: normal;"><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <div> 
     <p style="font-weight: normal;"> <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates the Monthly People Costs for each month during the Initiative's duration using the following formula:&nbsp;</p> 
     <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
     <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span style="font-weight: normal;"> If you have an initiative with a duration of 6 months that requires 1 Designer with a $50 hourly rate for 1 FTE every month and a Web&nbsp;Designer with an hourly rate of $100 for 2 months of the initiative, the People Costs of the initiative is calculated as follows:</span> <br style="font-weight: normal;"><code style="font-weight: normal;">Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code> </p> 
    </div> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" style="font-weight: bold;" colspan="2" role="rowheader">Planned Benefit</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray" style="font-weight: bold;"><span style="font-weight: normal;">This is a manual entry where you can estimate the overall benefit that your department would gain by completing this initiative. </span> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" style="font-weight: bold;" colspan="2" role="rowheader">Net Value amount</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray" style="font-weight: bold;"> <p style="font-weight: normal;">This represents the value of your initiative when taking into account the overall costs and the Planned Benefit estimated on the initiative. <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates the Net Value of an initiative using the following formula:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
  </tr> 
 </tbody> 
</table>




## Initiative information in reports {#initiative-information-in-reports}

You can display initiative information in reports, as described in the table below. This information is available in your *`Workfront`* instance only when your company has purchased a *`Workfront Scenario Planner`* license. 


>[!NOTE]
>
>You can access the following report information from *`Adobe Workfront Classic`* as well as *`The new Adobe Workfront experience`*. However, you will not be able to access plans or initiatives from *`Adobe Workfront Classic`*. 



<table style="width: 100%;mc-table-style: url('../Resources/TableStylesheets/Standard.css');" class="TableStyle-Standard" cellspacing="3"> 
 <col class="TableStyle-Standard-Column-Column1"> 
 <col class="TableStyle-Standard-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Report type</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="font-weight: bold;">Initiative information</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Initiative </td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray">Name, Duration,&nbsp;Start and&nbsp;End Dates, Entered by, ID, Last Published Date*, All Project fields including custom fields*</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Initiative Job Role</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray">All Initiative information as listed above, (Job Role) ID, Project*, Project&nbsp;Assignment Planned Hours*, Initiative Job Role Hours, (Job Role) Count, All Project fields including custom fields*</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyB-Column1-MediumGray">Project*</td> 
   <td class="TableStyle-Standard-BodyA-Column1-MediumGray"> <p>All Initiative information as listed above*</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; These fields populate with information from the project linked to the initiative, only when the initiative was created from a project or was published to a project at least once. For information about publishing initiatives, see [Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner](publish-scenarios-update-projects.md).
