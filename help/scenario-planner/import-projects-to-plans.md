---
filename: import-projects-to-plans
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
---



# Import projects to plans in the *`Adobe Workfront Scenario Planner`* {#import-projects-to-plans-in-the-adobe-workfront-scenario-planner}

You can import existing projects into a plan. The imported projects are converted to initiatives and you can manage them within the plan as you would manage a new initiative. The original project remains linked to the new initiative. 


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


## Considerations about importing projects into plans as new initiatives {#considerations-about-importing-projects-into-plans-as-new-initiatives}




* You must create projects before you can import them into a plan as new initiatives. 
* You must have at least View permissions to the projects to be able to import them into a plan as new initiative. 
*  You can import the same project into multiple plans. 
* The projects you want to import must have dates included in the time frame of your plan. You cannot import projects with a Planned Completion Date earlier than the start of the plan or a Planned Start Date later than the end of the plan. 
* You cannot import more than 100 projects at a time. 
* Some project information is also imported into the plan and becomes initiative information. For information about what project information is imported into the plan and becomes initiative information, see the [Project information imported into the plan](#project) section in this article. 
* Changes that occur on the linked projects do not affect the initiatives on the plan. 
* Changes that occur on the initiatives on the plan do not automatically affect the linked projects `Initiative changes affect the linked projects only when you publish the initiative from the plan.` `For information about how publishing initiatives affects the linked projects, see` ` [Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner](publish-scenarios-update-projects.md)`. 

* Deleting an initiative that has been created by importing a project does not delete the project. 
* Deleting a project linked to an initiative does not delete the initiative. 




## Project information imported into the plan {#project-information-imported-into-the-plan}

When you import a project into a plan some project information is also imported into the plan and it becomes initiative information. The following table shows what project information becomes initiative information when you import a project into a plan: 

<table style="width: 100%;mc-table-style: url('../Resources/TableStylesheets/Standard.css');" class="TableStyle-Standard" cellspacing="3"> 
 <col class="TableStyle-Standard-Column-Column1"> 
 <col class="TableStyle-Standard-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray" style="font-weight: bold;">Project information</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray" style="font-weight: bold;">Initiative information </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Project&nbsp;Name</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray">Initiative name</td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-LightGray">Project Planned Dates</td> 
   <td class="TableStyle-Standard-BodyD-Column1-LightGray"> <p>Initiative start and end months.</p> <p>If a project starts or ends in the middle of a month, the imported dates are extended to cover a full month in the plan.&nbsp;For example, if the Project Planned Dates are March 20 - May 5, 2020, then the dates of the imported initiative are March - May, 2020.</p> <p>If the Planned Start or Completion Date is beyond the duration of the plan, there is a visual indication that the imported initiative starts before or ends after the plan. </p> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-MediumGray"> 
   <td class="TableStyle-Standard-BodyE-Column1-MediumGray">Job roles assigned to tasks and issues</td> 
   <td class="TableStyle-Standard-BodyD-Column1-MediumGray"> <p>Initiative Job&nbsp;Roles. </p> <p>Note:  <p>If a user changes roles during the life of the project, the roles that are imported depend on the status of the assignment when you import the project. The following scenarios exist:</p> 
     <ul> 
      <li> <p>If a user assigned to a task or an issue changed their role after they marked their assignment as Done, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> imports to the initiative the role the user fulfilled before they marked the assignment as Done.</p> </li> 
      <li> <p>If a user assigned to a task or issue changed the role during the life of the project but their assignment on the task or issue is not marked as Done when you import the project, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> imports only the current role of the assigned user. </p> </li> 
     </ul> <p>For information about the status of an assignment, see "Assignment Status" in <a href="workfront-terminology-glossary.md" class="MCXref xref">Glossary of Adobe Workfront terminology</a>. </p> </p> </td> 
  </tr> 
  <tr class="TableStyle-Standard-Body-LightGray"> 
   <td class="TableStyle-Standard-BodyB-Column1-LightGray">Project Planned Hours associated with job roles assigned to tasks or issues</td> 
   <td class="TableStyle-Standard-BodyA-Column1-LightGray"> <p><span>Depending on whether the plan is set up to use FTEs or hours, the Planned Hours from the tasks on the project become either</span> Required FTEs <span>or Required hours on the plan</span>. </p> <p>For information about setting up a plan to use&nbsp;FTEs or hours, see <a href="create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Adobe Workfront Scenario Planner</a>. </p> <p>Consider the following:</p> 
    <ul> 
     <li> <p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> uses the job roles assigned to tasks and issues or the job roles that the users assigned to tasks or issues are associated with on the project and transfers them to the new initiative as Required Job&nbsp;Roles. </p> </li> 
     <li> <p>When the plan is set up to use FTEs, the Planned Hours associated with the job roles on the tasks and issues of the project are first converted to FTE.&nbsp;This FTE is then assigned to the initiative’s job role. <span>Planned Hours are equally distributed in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. If a task or an issue spans multiple months, the amount of Planned Hours for each month in the duration of the initiative is converted in monthly FTE and transferred to each month of the initiative. </span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span>For example, if a task is assigned to a job role for 80 Planned Hours in September, then the imported job role displays 0.5 FTE for the initiative in September. </span> </p> </li> 
     <li> <p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates the FTE of the Required Job&nbsp;roles associated with the initiative using the following formula:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Tip: The <span class="mc-variable WFVariables.Scenario_Planner_-_feature_name variable varname">Scenario Planner</span> assumes that there are 160 working hours in a month.</p> <p>For example, if a project has a Duration of 1200 minutes and a job role on the project is associated with 600 minutes of Planned Hours, their FTE is 0.5. When importing the project, the Required Job Role FTE on the newly created initiative is 0.5 for each month of the initiative. </p> </li> 
     <li>When a job role is assigned to a task on the project with zero Planned Hours, the Required FTE for the job role of the initiative is zero by default. </li> 
     <li>When a job role is assigned to a task on the project with a zero Duration, the Required FTE&nbsp;<span>or hours</span> for the job role of the initiative is zero by default, even if the task has Planned Hours. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;


## Import projects into a plan {#import-projects-into-a-plan}



>[!IMPORTANT] {type="important"}
>
>After importing projects into a plan, they become initiatives on the plan. Although the two items are linked, they exist as independent entities and do not automatically affect each other when they are updated. 
>
>
>The following occur:
>
>
>
>*  Changes to the project never affect the initiative after you import the project into the plan.These changes include changes to the job role allocations. 
>*  Changes to the initiative affect the information in the *`Scenario Planner`* area on the project only when you publish the initiative to the corresponding project. Otherwise, they do not affect the Planned Hours information for the tasks and issues of the project. 
>
>
>  `For information about how publishing initiatives affects the linked projects, see` ` [Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner](publish-scenarios-update-projects.md)`. 
>
>
>






1. Click the `Main Menu` ![](assets/main-menu-icon.png) in the upper-right corner of *`Workfront`*, then click  *`Scenarios`* to access the *`Scenario Planner`*. 

1. Click the name of a plan where you want to import projects. 
1.  Click `New Initiative`, then click `Import Projects`. 


   The Import Projects box displays. Projects that have dates included in the time frame of your plan display in a list.


   ![](assets/project-import-ui-projects-selected-350x72.png)




   >[!TIP] {type="tip"}
   >
   >Projects in any status display in the list.



1. (Optional) Click the `Filter icon` ![](assets/filter-nwepng.png)and select an available filter from the list to reduce the amount of projects on your list. By default, the list of projects is filtered by the user's currently selected project filter in a list of projects. 

1. (Optional) Click the `Search icon` ![](assets/search-icon.png) and add a keyword displayed on any field on the screen. The items containing the search word display in the list automatically and all items are hidden. 

1. (Conditional) Click the `X icon` to remove the search and display all projects. 
1.  Select up to 100 projects and click `Import`. 


   The projects are imported as new initiatives. 


   Notice the following:

    
    
    * A project icon ![](assets/project-icon-sp.png) displays to the right of the initiative name.
    *  If the project timeline exceeds the duration of the plan, the bar of the initiative ends with a pointed margin to the left (when the Start Date is earlier than the plan's date) or to the right (when the End Date is later than the plan's date).
    
    
      ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)    
    

    
    *  The number of months and job roles have been updated to match those of the project. 
    
    


   >[!TIP] {type="tip"}
   >
   >The costs associated with the job roles update at the initiative level and are not imported from the project. 



1.  Click the bar representing the new initiative to open the initiative details panel to the right. 


   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)




   In the `Initiative Duration` area review the following information: 

<table style="width: 100%;mc-table-style: url('../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Initiative Duration</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">This is the duration of the initiative in months. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Initiative</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The Start and End dates of the initiative. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Project</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>The Planned Start and Completion dates of the linked project.</p> <p>Tip: If the Project information is missing, the project was deleted.</p> </td> 
  </tr> 
 </tbody> 
</table>


1. Edit the name of the initiative. By default, it matches the name of the project. 
1. (Optional) Do one of the following:
    
    
    * Update job roles in the `Required Job Roles` section
    * Update the `Fixed Costs` in the `Costs` section
    
    * Click `Update available job roles` or `Update available budget` to resolve conflicts between the new initiative and other initiatives on the plan.
    
    
    
1. (Conditional) Click `Apply` to save changes to your initiative. 
1. Click  `Save Plan` to save the changes to your plan. 
1. (Optional) To update the changes you make to the initiative back to the project it was imported from, publish the project from the plan.&nbsp;For information about publishing plans, see [Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner](publish-scenarios-update-projects.md). 
1.  (Optional) Click the project icon to access the linked project. 


   ![](assets/project-icon-on-initiative-highlighted-350x49.png)





