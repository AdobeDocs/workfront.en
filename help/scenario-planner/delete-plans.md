---
filename: delete-plans
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
---



# Delete plans in the *`Adobe Workfront Scenario Planner`* {#delete-plans-in-the-adobe-workfront-scenario-planner}

You can delete plans that you created. You cannot delete plans that are shared with you. 


## Access requirements {#access-requirements}


You must have the following:

<table class="TableStyle-TableStyle-HeaderRow" style="mc-table-style: url('../Resources/TableStyles/TableStyle-HeaderRow.css');caption-side: bottom;" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><span style="font-weight: bold;" class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span><b> plan*</b> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"><span class="mc-variable WFVariables.WFPlan-Business variable varname">Business</span> or higher</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p><span style="font-weight: bold;" class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span><b> license*</b> </p> </td> 
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

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Delete plans {#delete-plans}



>[!IMPORTANT] {type="important"}
>
>You cannot recover deleted plans. 


You can delete a plan or you can delete one scenario in a plan. 



* [Delete plans](#delete3) 
* [Delete scenarios](#delete4) 




### Delete plans {#delete-plans-1}



>[!IMPORTANT] {type="important"}
>
>Consider the following when deleting plans:
>
>
>
>*  All information related to the plan is also deleted. This includes all the scenarios and initiatives associated with the plan including information about job roles and costs. This information cannot be recovered.
>*  >
>  If the plan contains a published scenario, the projects linked to the deleted initiatives are preserved and the *`Scenario Planner`* area remains in the Project&nbsp;Details section. 
>
>
>  For information about publishing initiatives to projects, see [Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner](publish-scenarios-update-projects.md).
>
>



To delete a plan:



1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png), then click  *`Scenarios`*.


   A list of plans displays. 

1. Click the name of a plan to open it.
1.  Click the `More menu` ![](assets/more-menu.png) to the right of the plan name, then click `Delete` > `Yes, delete it`.


   The plan is deleted and you return to the list of plans. 





### Delete scenarios {#delete-scenarios}



>[!IMPORTANT] {type="important"}
>
>Consider the following when deleting a scenario:&nbsp;
>
>
>
>* Deleting a scenario deletes all initiatives and their information from the scenario. If they are copied to other scenarios, the initiatives remain on the other scenarios. 
>* When deleting a scenario, the subsequent scenario takes on the number of the deleted scenario and the counting order is preserved.&nbsp;For example, if you delete Scenario 4, Scenario 5 becomes Scenario 4. 
>* `If some initiatives on the scenario are published, the project linked to the initiative is preserved and the *`Scenario Planner`* area remains on the linked projects.` 
>*  >
>  If the published initiatives exist on another scenario, they remain on that scenario, including their link to the project. Publishing those initiatives from the other scenarios updates the linked projects with new information from those scenarios. 
>
>
>  For information about publishing initiatives to projects, see [Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner](publish-scenarios-update-projects.md).
>
>



To delete a scenario:



1.  Go to the plan for which you want to delete a scenario. 


   By default, the Initial scenario displays.

1. Click `Compare scenarios`.
1.  From the upper-right corner of the scenario card, click the `More` menu ![](assets/more-menu.png), then click `Delete`. 


   The scenario is deleted.

1. Click `Save plan` to save your changes. 


&nbsp;
