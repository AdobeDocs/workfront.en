---
filename: remove-results-activities-from-goals
product: workfront-goals
product-area: projects
navigation-topic: results-and-activities
---



# Remove results, activities, and projects from goals in *`Adobe Workfront Goals`* {#remove-results-activities-and-projects-from-goals-in-adobe-workfront-goals}

You can remove results, activities, and projects from goals if they are no longer relevant. 


For information about creating goals, and adding results and activities to them, see the following articles:



* [Create goals in Adobe Workfront Goals](create-goals.md) 
* [Add activities to goals in Adobe Workfront Goals](add-activities-to-goals.md) 
* [Add results to goals in Adobe Workfront Goals](add-results-to-goals.md) 
* [Edit results and activities in Adobe Workfront Goals](edit-results-and-activities.md) 




## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Request variable varname">Request</span> or higher</p> <p>For more information, see <a href="wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>You must purchase an additional license for the <span class="mc-variable WFVariables.FullProdNameWFGoals variable varname">Adobe Workfront Goals</span> to access functionality described in this article. </p> <p>For information, see <a href="access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Adobe Workfront Goals</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Edit access to Goals or higher</p> <p>Note:  <p>If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see:</p> 
     <ul> 
      <li> <p><a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li> 
      <li> <p><span href="grant-access-goals.md"><a href="grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> 
    <div> 
     <p>Manage permissions to the goal</p> 
     <p>For information about sharing goals, see <a href="share-a-goal.md" class="MCXref xref">Share a goal in Adobe Workfront Goals</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

You must have the following before you can start:



*  A Layout Template that includes the Goals area in the Main&nbsp;Menu.
*  A goal with results or activities.




## Considerations for removing results, activities, and disconnecting projects from goals {#considerations-for-removing-results-activities-and-disconnecting-projects-from-goals}

`<li>  <ul>   <li> <p>You can remove results and activities only from active goals that are in a current or future time period. </p> </li>  </ul> </li>` 


* You can remove results and activities from a goal by deleting them. Deleted results and activities cannot be recovered. 
*  You cannot delete a project from a goal, but you can disconnect it. By disconnecting the project from the goal the percent complete of the project no longer affects the progress of the goal. 


  For information about how projects affect goal progress, see [Overview of connecting projects to goals in Adobe Workfront Goals](connect-projects-to-goals-overview.md). 

*  You cannot remove or disconnect a result or an activity from a goal if they are the last progress indicator for the goal. 


  ` `**Warning: **``You can delete a project from a goal, even if it is the last progress indicator on the goal.&nbsp;The goal remains Active, but it shows no progress. 





## Delete results and activities from goals {#delete-results-and-activities-from-goals}

Removing results and activities from goals is identical. 



1.  Click the `Main Menu icon` ![](assets/main-menu-icon.png) in the upper-right corner of your screen, then click `Goals`.


   This opens the *`Workfront Goals`* area. 


   The *`Goal List`* displays by default. 

1.  Click the name of a goal you want to remove results and activities from. 


   This opens the Goal Details panel on the right.

1. Click `Results` to remove results or `Activities` to remove activities. 

1.  Click the `gear icon` ![](assets/settings-gear-icon.png) to the right of the result or activity name, then click `Delete` > `Yes, delete`. 


   ![](assets/delete-result-goal-details-350x108.png)




   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result. 





## Disconnect projects from goals {#disconnect-projects-from-goals}




1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) > `Goals` in the upper-right corner of your screen.


   This opens the *`Workfront Goals`* area. 


   The *`Goal List`* displays by default. 

1.  Click the name of a goal you want to remove results and activities from. 


   This opens the Goal Details panel on the right.

1. Click the `right-pointing arrow` to the left of the Activities sections to expand it. 
1.  Click the `gear icon` ![](assets/settings-gear-icon.png) to the right of the project name, then click `Disconnect`.


   ![](assets/disconnect-project-goal-details-350x94.png)




   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.



