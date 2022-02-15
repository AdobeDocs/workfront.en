---
filename: publish-scenarios-update-projects
product-area: enterprise-scenario-planner-product-area
keywords: publish,plans,projects,scenario,scenarios
navigation-topic: enterprise-scenario-planner-navigation-topic
---



# Update or create projects by publishing initiatives in the *`Adobe Workfront Scenario Planner`* {#update-or-create-projects-by-publishing-initiatives-in-the-adobe-workfront-scenario-planner}

Publishing a scenario from the *`Adobe Workfront Scenario Planner`* accomplishes the following:



*  Creates projects from the initiatives on the scenario and links them together.
*  Updates projects already linked to initiatives on the scenario with information from the linked initiative. Projects can also be linked to initiatives when you import them in to a plan. For information, see [Import projects to plans in the Adobe Workfront Scenario Planner](import-projects-to-plans.md)




## Access requirements {#access-requirements}

You must have the following:

<table class="TableStyle-TableStyle-HeaderRow" style="mc-table-style: url('../Resources/TableStyles/TableStyle-HeaderRow.css');caption-side: bottom;" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 300px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;"> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"><span class="mc-variable WFVariables.WFPlan-Business variable varname">Business</span> or higher</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;"> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Review variable varname">Review</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;"><span class="bold">Product</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>You must purchase an additional license for the <span class="mc-variable WFVariables.FullProdNameWFScenPlan variable varname">Adobe Workfront Scenario Planner</span> to access functionality described in this article.</p> <p>For information about obtaining the <span class="mc-variable WFVariables.ProdNameWorkfrontScenarioPlanner variable varname">Workfront Scenario Planner</span>, see <a href="access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Adobe Workfront Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;"> <p>&nbsp;</p> <p><span class="bold">Access level*</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li>Edit for <span class="mc-variable WFVariables.Scenario_Planner_-_feature_name variable varname">Scenario Planner</span> and Projects</li> 
    </ul> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="text-align: left;font-weight: bold;"> <p><span class="bold">Object permissions</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> 
    <ul> 
     <li>Manage permissions for the plan </li> 
     <li>Manage permissions for published projects</li> 
    </ul> <p>For information on requesting additional access to projects, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> <p>For information on requesting additional access to a plan, see <a href="request-access-to-plan.md" class="MCXref xref">Request access to a plan in the Adobe Workfront Scenario Planner</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


For additional information about access to the *`Workfront Scenario Planner`*, see [Access needed to use the Adobe Workfront Scenario Planner](access-needed-to-use-sp.md).


## Prerequisites {#prerequisites}

Before you begin:



* You must use *`the new Adobe Workfront experience`* to be able to access the *`Scenario Planner`*. 

* You must create and save a plan before you can publish initiatives from it. 




## Considerations about publishing initiatives to projects {#considerations-about-publishing-initiatives-to-projects}




* You can publish only one scenario from a plan. 
* One initiative can be linked to only one project.
*  One project can be linked to more than one initiative when the initiatives belong to different plans. 


  >[!TIP] {type="tip"}
  >
  >`When a project exists on multiple plans and you publish information to the project from all plans, the latest publish overwrites the existing *`Scenario Planner`* information on the project.` 



*  If initiatives were created on the plan by importing projects to the plan, publishing the initiative also updates the linked projects with initiative information. 


  >[!TIP] {type="tip"}
  >
  >You can import the same project into multiple plans. Publishing might overwrite initiative information on a project that is linked to multiple initiatives. 


  For information about creating initiatives by importing projects, see [Import projects to plans in the Adobe Workfront Scenario Planner](import-projects-to-plans.md). 

*  Any changes made to the project do not transfer to the linked initiative. 


&nbsp;


## Publish initiatives  {#publish-initiatives}



>[!IMPORTANT] {type="important"}
>
>If you make any changes to initiatives on the plan, including resolve conflicts, you must republish the initiative in order for the new information to be visible on the project. This information displays on the projects linked to initiatives only when you publish the corresponding the initiative. For information about resolving conflicts between initiatives, see [Resolve initiative conflicts in the Adobe Workfront Scenario Planner](resolve-conflicts-in-sp.md)





1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click `Scenarios`
1.  (Optional and conditional) If you want to publish from an existing plan, click the `Filter` icon ![](assets/filter-nwepng.png) in the upper-right corner of the plan and select one of the following options:

<table style="width: 100%;mc-table-style: url('../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">All</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Displays all plans that you own or are shared with you. This is the default. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">My plans</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Displays plans that you created.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Shared with me</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Displays plans you did not create but are shared with you.</p> <p>Important: You must have Manage permissions to plans shared with you to be able to publish them. </p> </td> 
  </tr> 
 </tbody> 
</table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)



1.  (Optional) Click the `Search` icon ![](assets/search-icon.png) and start typing the name of a plan to quickly find it in the list.
1.  (Conditional)&nbsp;To publish from a new plan, create a plan.


   For information about creating plans, see [Create and edit plans in the Adobe Workfront Scenario Planner](create-and-edit-plans.md) . 

1.  (Optional) Click the name of an existing plan and create new scenarios for the plan.


   For information about creating scenarios for a plan, see [Create and compare plan scenarios in the Adobe Workfront Scenario Planner](create-and-compare-scenarios-for-a-plan.md). 

1.  (Optional) Update the initiatives of an existing or a new plan or create new ones.


   For information about creating initiatives, see [Create and edit initiatives in the Adobe Workfront Scenario Planner](create-and-edit-initiatives.md).

1. Click `Save plan`. 
1.  Select the scenario you want to publish from the `Initial scenario` drop-down menu, then click `Go to Publish` ![](assets/go-to-publish-button-icon.png) in the upper-right corner.


   Or


   Click `Compare scenarios`, hover over the scenario card that you want to publish from, then click `Go to Publish` ![](assets/go-to-publish-button-icon.png). 


   The Publish initiatives page displays, showing a list of all initiatives in the scenario. If any of the initiatives was previously published, the project icon ![](assets/project-icon-sp.png) displays after their name and the `Last published` date is populated in the list. 


   >[!TIP] {type="tip"}
   >
   >Initiatives that have been created by importing projects also display the project icon ![](assets/project-icon-sp.png) to the right of their name


   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)



1.  (Optional and conditional) If you want to publish from an existing plan, click the `Filter` icon ![](assets/filter-nwepng.png) in the upper-right corner of the plan and select one of the following options:

<table style="width: 100%;mc-table-style: url('../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 90px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">All</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Displays all initiatives of the selected scenario. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Published</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Displays initiatives that you or another user published before. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Unpublished</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Displays unpublished initiatives. </p> </td> 
  </tr> 
 </tbody> 
</table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)



1.  (Optional) Click the `Search` icon ![](assets/search-icon.png) and start typing the name of an initiative to quickly find it in the list.
1.  Select one or multiple initiatives to publish and create or update projects from them, then click `Publish initiatives`. 


   This creates a new project from each selected initiatives or updates the existing connected projects, if the published initiatives were already linked to a project. 


   >[!TIP] {type="tip"}
   >
   >New projects have the same name as the published initiatives. 



1.  (Conditional) Do one of the following: 

    
    
    *  If you published one initiative, click `See associated project` to open the project created or updated from the initiative. 
    *  If you published more than one initiative, click  `See associated projects` to open a list of projects published from initiatives. *`Workfront`* applies the Scenario Planner Projects filter to the list of projects by default. The projects published most recently display at the top of the list. 
    
    
      ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)    
    

    
    
    

1.  Go to the following areas to view initiative information on the project:


    
    
    *  **The Updates section**: An update publishes to indicate that the project was created or updated from the initiative. The update contains the name of the initiative that created or updated the project and the linked name of the plan that contains the initiative. You can click the name of the plan in the update to open the plan in the *`Scenario Planner`*. 
    
    
      ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)    
    

    
    *  **The Overview area of the Project Details section**: A new Scenario Planner section is created in this area that contains information from the linked initiative. 
    
    
      >[!TIP] {type="tip"}
      >
      >This information is visible only when viewing Project Details in *`the new Adobe Workfront experience`*. 
    
    
      ![](assets/scenario-planner-on-project-details-350x135.png)    
    

    
    
      The following initiative information is published in the Scenario Planner area of the Project&nbsp;Details section:
    
    
    
    
    <table style="margin-left: 0;margin-right: auto;mc-table-style: url('../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col style="width: 273px;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col style="width: 873px;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span>Initiative Duration*</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><span>The duration of the corresponding initiative when the project is linked to an initiative. This field is not editable. </span> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span>Last Published Date*</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><span>The date when the project was last published from a corresponding initiative.</span> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span>Initiative Start Date*</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><span>The first day of the start month of the initiative, when the project is linked to an initiative. </span> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span>Initiative End Date*</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><span>The last day of the end month of the initiative, when the project is linked to an initiative.&nbsp; </span> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span>Initiative Job&nbsp;Roles in FTEs and Hours*</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Information about the associated job roles and their time allocations for the initiative.&nbsp;This includes:</p> 
    <ul> 
     <li>Job&nbsp;Role name</li> 
     <li>Number of FTEs</li> 
     <li> <p>Number of Hours for all&nbsp;FTEs</p> <p>You can estimate the amount of job roles needed for your plan or initiative using hours or FTEs.&nbsp;</p> <p>For more information, see <a href="create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Adobe Workfront Scenario Planner</a>. </p> </li> 
    </ul> <p>Tip: <span>If the number of job role is different for each month in the initiative, this field displays the maximum amount of roles needed for the initiative. For example, if you need 1 Consultant for January and 2 for February, the column displays 2FTE and the corresponding amount of hours for 2 FTEs for all months. </span> </p> </td> 
  </tr> 
 </tbody> 
</table>    
    

    
    
      >[!NOTE]
      >
      >All users with View access to the project can see the *`Scenario Planner`* section in the Overview area. You can control whether this area displays in the Details section by using a layout template. If users do not have a layout template associated with them, this area displays by default. 
      >
      >    
      >    
      >    *  For information about adding or removing areas in the Details section using a layout template, see [Customize the Details view using a layout template](customize-details-view-layout-template.md). 
      >    *  For more information about viewing information in the Overview area of the Project&nbsp;Details, see [Manage information in the project Overview area](understand-project-overview-area.md).
      >    
      >    

    
    
    
    *  **The Role Allocation panel in the ** *`Workload Balancer`*** or the task list of the project**: Information about role allocation on the initiative populates in this area, in addition to role allocations on the project. 
    
    
      For more information, see [Overview of reconciling resource allocations between projects and initiatives](overview-reconcile-allocations-between-projects-initiatives.md). 
    
    
      ![](assets/role-allocation-panel-350x174.png)    
    

    
    
      Any changes to the dates or resources of the project do not affect the corresponding initiative or any of the areas on the project that contain initiative information. 
    
    *  **The Resource Budgeting area of the Business Case of the project**: A new option for managing project resources using *`Scenario Planner`* information is added in the Resource Budgeting area of the Business Case of the project. 
    
    
      For more information, see [Budget resources in the Business Case using the Adobe Workfront Scenario Planner](budget-resources-in-business-case-use-scenario-planner.md). 
    
    
      ![](assets/sp-in-business-case-selected-350x110.png)    
    

    
    
    

1.  (Optional) Review the following information in the *`Scenario Planner`* after you published a scenario: 

    
    
    * The published scenario becomes the first scenario after you publish initiatives from it. 
    * You cannot publish from any other scenario after you have published a scenario at least once. 
    * The Go to Publish option is removed from all other scenarios after at least one initiative has been published from a scenario. 
    *  A green indicator displays next to the published initiatives' project icons in the plan. 
    
    
      ![](assets/indicator-for-published-initiative-icon-350x119.png)    
    

    
    *  A green "Published"&nbsp;indicator displays at the top of the scenario and on the scenario card and the Published field is populated on the scenario card indicating the number of initiatives in the scenario that have been published. 
    
    
      ![](assets/published-scenario-highlighted-350x632.png)    
    

    
    
      >[!TIP] {type="tip"}
      >
      >If all the projects published from the scenario's initiatives are deleted, the indication that the scenario has been published is removed. For information, see [Delete projects](delete-projects.md). 
    
    
    
    
    

1.  (Optional) Update information on the initiative and repeat the process described above to republish the initiative and update initiative information on the linked project. 


   For information about editing initiatives, see [Create and edit initiatives in the Adobe Workfront Scenario Planner](create-and-edit-initiatives.md). 



&nbsp;
