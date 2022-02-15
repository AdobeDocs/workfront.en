---
filename: show-role-allocation-task-list-nwe
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
---



# Show role allocation for projects and initiatives in the task list {#show-role-allocation-for-projects-and-initiatives-in-the-task-list}



>[!IMPORTANT] {type="important"}
>
>Your organization must purchase an additional license for the *`Adobe Workfront Scenario Planner`* so that you can view initiative information on a project. For information about obtaining the *`Workfront Scenario Planner`*, see [Access needed to use the Adobe Workfront Scenario Planner](access-needed-to-use-sp.md). 


After you connect projects and initiatives, you can manage their resource allocation side-by-side to ensure they match. This avoids overallocating or underutilizing them. 


This article describes how you can reconcile resources using the Role Allocation panel in the task list of a project. 


For general information about reconciling resources between projects and initiatives, including prerequisites, see [Overview of reconciling resource allocations between projects and initiatives](overview-reconcile-allocations-between-projects-initiatives.md). 


## Access requirements {#access-requirements}

You need to following: 

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
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>View or higher access to Projects </p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="text-align: left;"> <p><span class="bold">Object permissions</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>View or higher permissions to the project</p> <p>For information on requesting additional access to a plan, see <a href="request-access-to-plan.md" class="MCXref xref">Request access to a plan in the Adobe Workfront Scenario Planner</a>.</p> <p>For information about requesting additional access to a project, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.



## Show role allocation for projects and initiatives in the task list {#show-role-allocation-for-projects-and-initiatives-in-the-task-list-1}

If your company has purchased a *`Workfront Scenario Planner`* license, you can reconcile the resource allocations between the initiative and the project linked to it in the Tasks section of the project. 



1.  (Conditional) Connect a project with an initiative using one of the methods described in the [Show role allocation for projects and initiatives in the task list](#connect) of this article. 


   >[!IMPORTANT] {type="important"}
   >
   >If you make changes to resources on the initiative, you must re-publish the scenario that the initiative belongs to in order for the latest resource information from the initiative to update on the project. 



1.  Go to the project where you want to review the allocation of job roles for the project as well as for the associated initiative. 
1.  Click `Tasks` in the left panel. 
1.  Click the `Show role allocation` icon ![](assets/show-role-allocation-icon.png) in the upper-right corner of the toolbar. 


   The Role&nbsp;Allocation panel displays.

1.  Review the following information in the `Project Totals` area of the Role Allocation panel: 

<table style="width: 100%;mc-table-style: url('../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Job&nbsp;Role</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The names of the job roles associated with any of the following:</p> 
    <ul> 
     <li> <p>tasks on the project</p> </li> 
     <li> <p>issues on the project</p> </li> 
     <li> <p>initiative linked to the project</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Initiative Hours</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The number of required hours associated with each job role on the initiative for the total duration of the initiative. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Planned Hours</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">The number of Planned Hours associated with each job role in the tasks or issues on the project for the total duration of the project. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Variance</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>The difference between the hours required on the initiative and the planned hours associated with work on the project.&nbsp;<span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> calculates the Variance using this formula:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>When resources are planned for more hours than required on the initiative, the Variance is negative and it displays in red. This means your resources are overallocated. </p> </td> 
  </tr> 
 </tbody> 
</table>


   ` `**Tip: **`` Planned Hours from the project do not display in the following scenarios: 

    
    
    *  When tasks or issues are not assigned to job roles, or users with a job role associated with them.
    *  When tasks or issues have a Duration of zero. 
    
    
   &nbsp;

1.  (Optional) If the Variance column shows that your resources are overallocated, adjust one of the following:

    
    
    *  Lower the number of Planned Hours for one job role that shows overallocated or add more resources to the tasks and distribute more Planned Hours to the new resources. You can update assignments or the number of Planned Hours on tasks or issues when editing them.&nbsp;For more information see the following articles:
    
        
        
        *  [Edit tasks](edit-tasks.md) 
        *  [Edit issues](edit-issues.md) 
        
        
    
    
      >[!NOTE]
      >
      >You must have additional access and permissions to edit tasks and issues.
    
    
    
    *  Increase the number of required hours for role that shows the overallocation on the initiative. For more information, see [ Create and edit initiatives in the *`Adobe Workfront`* *`Scenario Planner`*](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&topicId=Content%2FScenario_Planner%2Fcreate-and-edit-initiatives.htm&_LANG=enus). 
    
    
      >[!NOTE]
      >
      >You must have additional access and permissions to edit plans. 
    
    
    
    
    



&nbsp;
