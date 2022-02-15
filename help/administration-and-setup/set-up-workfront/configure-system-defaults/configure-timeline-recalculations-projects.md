---
filename: configure-timeline-recalculations-projects
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
---



# Configure timeline recalculations for projects {#configure-timeline-recalculations-for-projects}

Recalculating timelines allows managers to see how forces outside of the project are impacting the project's timeline. A project's timeline refers to the planned dates and projected dates for the project.


As an *`Adobe Workfront administrator`*, you can manually recalculate timelines for all projects in the system. 


Project owners can recalculate timelines for individual projects, as described in [Recalculate project timelines](recalculate-project-timeline.md).


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Configure automatic recalculations {#configure-automatic-recalculations}

As an *`Adobe Workfront administrator`*, you can configure when  *`Workfront`* recalculates project timelines. *`Workfront`* can recalculate project timelines either every night or when the project scope changes, or both. 



1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, then click  <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</MadCap:conditionalText>` 
1. Click `Project Preferences` > `Projects.`

1.  In the `Timelines` section, enable or disable one or both of the settings below. By default, both settings are enabled. 

    
    
    *  `Every night`: *`Workfront`*​​​ recalculates timelines at night only for projects where both of the following conditions are met:
    
        
        
        * Have a status of Current
        * Have had an update in the past three months
        
        
    
    *  `When a project's scope changes`: For information about what constitutes a project scope change, see [Recalculate project timelines](recalculate-project-timeline.md).
    
    





## Recalculate timelines for the entire  *`Workfront`* instance {#recalculate-timelines-for-the-entire-workfront-instance}

You can run the Recalculate Timeline diagnostic to immediately recalculate all timelines in the *`Workfront`* system. This allows all Project Managers to see the influence of external changes immediately on both planned and projected dates. For more information, see [Use Diagnostics to trigger automated processes](use-diagnostics-to-trigger-automated-processes.md).
