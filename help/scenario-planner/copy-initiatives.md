---
filename: copy-initiatives
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
---



# Copy initiatives in the *`Adobe Workfront Scenario Planner`* {#copy-initiatives-in-the-adobe-workfront-scenario-planner}

You can create initiatives by copying existing ones. You can copy initiatives on a plan that you create or on a plan that someone shares with you. 


## Access requirements {#access-requirements}


<table class="TableStyle-TableStyle-HeaderRow" style="mc-table-style: url('../Resources/TableStyles/TableStyle-HeaderRow.css');caption-side: bottom;" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><span style="font-weight: bold;" class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span><b> plan*</b> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"><span class="mc-variable WFVariables.WFPlan-Business variable varname">Business</span> or higher</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span style="font-weight: bold;" class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span><b> license</b>*</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Review variable varname">Review</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><b>Product</b> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>You must purchase an additional license for the <span class="mc-variable WFVariables.FullProdNameWFScenPlan variable varname">Adobe Workfront Scenario Planner</span> to access functionality described in this article.</p> <p>For information about obtaining the <span class="mc-variable WFVariables.ProdNameWorkfrontScenarioPlanner variable varname">Workfront Scenario Planner</span>, see <a href="access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Adobe Workfront Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Access level configurations*</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Edit access or higher to the <span class="mc-variable WFVariables.Scenario_Planner_-_feature_name variable varname">Scenario Planner</span></p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="text-align: left;"> <p><span class="bold">Object permissions</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Manage permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="request-access-to-plan.md" class="MCXref xref">Request access to a plan in the Adobe Workfront Scenario Planner</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Copy initiatives {#copy-initiatives}

Consider the following when copying initiatives:



*  Copying an initiative places the copy on the same plan as the original initiative. 
* Copying an initiative copies and adds the following information from the original initiative to the new initiative:
    
    
    * Duration
    * Job roles
    * People and Fixed Costs
    * Planned Benefit
    
    
* Copying an initiative can modify the following information for the plan, if the information exists on the original initiative:
    
    
    * Required amount of job roles 
    * Costs
    * Plan Utilization
    * Job role utilization
    * Net Value
    
    
*  Copying an initiative that was created by importing a project or has been published to a project at least once has the following implications: 

    
    
    *  It does not duplicate the project associated with the initiative.
    *  It does not connect the copied initiative to the project. 
    *  It does not modify the Scenario Planner section on the project, for projects that have been published at least once. 
    
    
      For information about publishing initiatives to projects, see [Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner](publish-scenarios-update-projects.md).
    
    
      For information about creating initiatives by importing projects, see [Import projects to plans in the Adobe Workfront Scenario Planner](import-projects-to-plans.md) . 
    
    
    





## Copy initiatives {#copy-initiatives-1}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png), then click  *`Scenarios`*.


   A list of plans displays. 

1. Click the name of a plan to open it, then locate the initiatives you want to copy.
1.  Select the box to the left of the initiative or initiatives that you want to copy, then click `Copy` from the menu that appears at the bottom of the plan.


   ![](assets/bottom-manage-initiative-menu-350x45.png)




   *`Workfront`* copies the initiatives immediately and places them underneath the last selected initiative. 


   The name of the copied initiative is *Copy of <Name of original initiative>*.


   >[!NOTE]
   >
   >`Depending on where you insert the new initiatives, the numbers of existing initiatives may change.`



1.  Update the name of the copied initiative. 


   >[!TIP] {type="tip"}
   >
   >We recommend that you always update the name of the initiative to avoid confusion in case you want to copy them again. 



1.  (Optional) Update the priority of your newly created initiatives. 


   For information about prioritizing initiatives, see [Update initiative priorities in the Adobe Workfront Scenario Planner](prioritize-initiatives.md). 

1. Click `Save Plan` to save your changes. 


