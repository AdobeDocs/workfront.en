---
filename: create-baselines
product-area: projects
navigation-topic: create-projects
---



# Create project baselines {#create-project-baselines}

A baseline is a project snapshot that represents key pieces of information included in the initial project plan or at any given time during the life of the project. 


You can use baseline to compare those pieces of information from the current plan to the original plan or any other point in time, to identify problem tasks, scope creep, and other trends over time. 


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information about access to projects, see <a href="grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Considerations for working with baselines {#considerations-for-working-with-baselines}




* You can capture a snapshot of the progress on a project multiple times during the lifetime of the project, creating multiple baselines. 
* You can view the information included in the baselines of a project by creating a baseline or by building a Baseline report. 
* When you create a baseline, the task information is also captured on the baseline tasks of that baseline. 
* You can view the information of the baseline tasks by building a Baseline Task report. 




>[!IMPORTANT] {type="important"}
>
>A baseline takes a snapshot of the name, dates, and financial information of the project. The baseline does not include the values of custom fields on the project. For information about financial information included in the baseline, see [Project finances included in project baselines](project-finances-included-in-project-baselines.md).




## Create a baseline {#create-a-baseline}

You can create a baseline in the following ways:



*  Automatically: Your *`Workfront administrator`* `or a *`group administrator`*` sets the project preference for *`Workfront`* to automatically create a baseline when a project becomes Current. When this setting is enabled, a baseline is created when the project status becomes Current. When this setting is not enabled, you must manually create baselines. 


  For more information about configuring project preferences and setting up automatic baseline creation, see [Configure system-wide project preferences](set-project-preferences.md). 


  ` `**Warning: **`` Enabling this setting automatically creates a baseline for a project every time a project's status changes to Current. The first created baseline is the default one. You must manually create all other baselines during the life of the project .

* Manually: You can create new baselines for the project as needed as the project progresses. You can then compare baselines to see how the project progressed over time. 





1. Navigate to a project. 
1.   In the left panel, click `Baselines`. 


   Or


   Click `Show More`, then click `Baselines`. 


   ![](assets/nwe-baselines-section-on-project-with-header-350x78.png)



1. Click `New Baseline.`
1. Specify the name for the baseline.
1.  (Optional) If this is the first baseline, you may want to choose it as the default. 
1.  Click `Save`.


   By default, the following information displays about the baseline you created:

    
    
    * Baseline name
    * Baseline Entry Date
    * Planned Start Date of the project when the baseline was created
    * Projected Start Date of the project when the baseline was created
    * Actual Duration of the project when the baseline was created
    * % Complete of the project when the baseline was created
    *  Default Baseline indicator that shows whether a baseline is the Default baseline of the project 
    
    
      >[!TIP] {type="tip"}
      >
      >You cannot view information from any two baselines at the same time in the same view or report. You can only view information from a given baseline and the Default baseline in the same report. You can modify which baseline you consider to be the Default baseline any time during the life of the project. 
    
    
    
    
    

1. (Optional) Click the drop-down arrow next to the View, then `Customize View` to add fields to your view and compare additional information between baselines. 




## Create a Baseline or a Baseline Task report {#create-a-baseline-or-a-baseline-task-report}

To view baseline information, you can also create a Baseline or Baseline Task report. This allows you to display any number of fields about the baselines or baseline tasks to compare them in one view. 


>[!TIP] {type="tip"}
>
>You must create a baseline before you can create a Baseline or Baseline Task report. 


For information about creating a report, see [Create a custom report](create-custom-report.md).


We recommend that you add a Project Name grouping to your Baseline or Baseline report to make it easier to read. 


For information about creating a grouping, see [Create groupings](create-groupings.md). 
