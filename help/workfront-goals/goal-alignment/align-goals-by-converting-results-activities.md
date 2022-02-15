---
filename: align-goals-by-converting-results-activities
product: workfront-goals
navigation-topic: goal-alignment
---



# Align goals by converting results and activities to goals {#align-goals-by-converting-results-and-activities-to-goals}

You can manually align two goals or you can convert the results and activities of an existing goal to another goal.&nbsp;The converted result or activity becomes the child goal of the original goal. For information about manually aligning two goals, see [Align goals by connecting them in Adobe Workfront Goals](align-goals-by-connecting-them.md). 


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
*  An existing goal with existing results and activities.


  For information about creating goals, see [Create goals in Adobe Workfront Goals](create-goals.md).





>[!IMPORTANT] {type="important"}
>
>A goal cannot have more than a total of 50 activities, results, or aligned goals.




## Considerations when converting results and activities into goals {#considerations-when-converting-results-and-activities-into-goals}

Sometimes, a result or an activity may have a larger scope than anticipated and it would make more sense that they would become goals. You can convert results and activities of an existing goal to a new goal.&nbsp;This is a bottom-up approach to aligning goals.


Consider the following when converting results and activities to goals:



* The converted result or activity becomes the child goal of the original goal, and the two goals become aligned.
* The converted result or activity is removed from the original goal and added as a result or activity to the newly created goal. 
* The newly created goal becomes the single progress indicator for the original goal, if there are no additional results or activities on the original goal. 




## Convert a result or activity to a goal {#convert-a-result-or-activity-to-a-goal}




1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the `Goal Details` panel.
1. Expand the `Results` or `Activities` right-pointing arrows to see a list of results or activities for the goal. 

1.  Click the `gear icon` ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click `Convert into a Goal`. 


   ![](assets/convert-to-goal-link-highlighted-350x191.png)



1. (Optional) Remove the name of the original activity or result owner from the `Goal Owner` field and replace it with another user, team, group, or your organization's name. By default, *`Workfront`* selects the owner of the result or the activity as the goal owner. 

1. Click  `Convert`. The activity or result displays as an aligned goal in the Goal&nbsp;Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the `Goal Details` panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](edit-goals.md). 



