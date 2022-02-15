---
filename: add-results-to-goals
product: workfront-goals
product-area: projects
navigation-topic: results-and-activities
---



# Add results to goals in *`Adobe Workfront Goals`* {#add-results-to-goals-in-adobe-workfront-goals}

Results measure the progress of a goal. Without associating results, activities, or aligned goals to a goal, you cannot activate the goal and you cannot record progress on it. 


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
*  An existing goal.


  For information about creating goals, see [Create goals in Adobe Workfront Goals](create-goals.md).





>[!IMPORTANT] {type="important"}
>
>A goal cannot have more than a total of 50 activities, results, or aligned goals.




## Add a result to a goal {#add-a-result-to-a-goal}




1. Go to the goal for which you want to add a result and click the name to open the `Goal Details` panel.
1.  Click `Add results`.


   ![](assets/add-result-inside-goal-details-highlighted-350x145.png)



1. Start typing the result you want to achieve in the `Result` field. This is the name of the result and it displays wherever the goal displays. 
1.  (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the `Owner` field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.


   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.



1.  In the `Value` drop-down menu, select the type of value that you want to measure your success by. 


   ![](assets/results-value-initial-target-boxes-350x49.png)




   Select from the following options:

   For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value. 


   >[!TIP] {type="tip"}
   >
   >The result Type is always Metric and cannot be edited. 




1.  In the `Initial` field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. 
1. In the `Target` field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.
1.  Click `Save`.


   The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result. 



