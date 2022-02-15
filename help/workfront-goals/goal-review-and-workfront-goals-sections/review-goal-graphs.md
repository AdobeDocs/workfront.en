---
filename: review-goal-graphs
product: workfront-goals
navigation-topic: goal-review-and-sections
---



# Review graphs to understand goal progress trends in *`Adobe Workfront Goals`* {#review-graphs-to-understand-goal-progress-trends-in-adobe-workfront-goals}

You can view the overall health of your goals and their progress trend in time in the Graphs section of *`Adobe Workfront Goals`*. The charts in this section do not break down the progress of each goal, but instead give you a holistic snapshot of all goals' progress status as well as their progress trend in time during a specified period. 


>[!IMPORTANT] {type="important"}
>
>You can see a total count for your goals in the Graphs section for a selected period of time. However, *`Workfront Goals`* takes into account only goals with a status of Active and Closed when calculating the overall goal progress status and percent complete. 




## Access requirements {#access-requirements}

You must have the following access to perform the actions described in this article:

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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Access level*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>View or higher access to&nbsp;Goals</p> <p>Note:  <p>If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see:</p> 
     <ul> 
      <li> <p><a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li> 
      <li> <p><span href="grant-access-goals.md"><a href="grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> 
    <div> 
     <p>View or higher permissions on goals</p> 
     <p>For information about sharing goals, see <a href="share-a-goal.md" class="MCXref xref">Share a goal in Adobe Workfront Goals</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

You must have the following before you can start:



*  A Layout Template that includes the Goals area in the Main&nbsp;Menu.




## Types of graphs in *`Workfront Goals`*  {#types-of-graphs-in-workfront-goals}

The following charts are available in the Graphs section or *`Workfront Goals`*: 

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 184px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">The Goal&nbsp;Health Chart</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>A gauge chart that displays the following:</p> 
    <ul> 
     <li>A total number of goals for the selected period of time. Goals with any status are taken into account. </li> 
     <li>The progress status of goals with a status of Active and Closed.</li> 
    </ul> <p>For information about how <span class="mc-variable WFVariables.Workfront_Align_(Goals) variable varname">Workfront Goals</span> calculates progress status, see <a href="calculate-goal-progress.md" class="MCXref xref">Calculate goal progress in Adobe Workfront Goals</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">The Goal Progress Chart</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>A line chart that displays updates made to goals in weekly increments during the goal's duration. The goal progress chart displays the following:</p> 
    <ul> 
     <li>An average expected and actual percent complete of all&nbsp;active and closed goals in the selected period.&nbsp;The percent complete progress is broken down into weekly increments marked by nodes. </li> 
     <li>The overall average percentage of progress for active and&nbsp;closed goals since the previous week. </li> 
    </ul> <p>Tip: The goal progress chart might not display any information when updates are made on the goals outside of the time period selected. </p> </td> 
  </tr> 
 </tbody> 
</table>



## Review goal progress in graphs {#review-goal-progress-in-graphs}




1.  Click the `Main Menu icon` ![](assets/main-menu-icon.png) in the upper-right corner of your screen, then click `Goals`.


   This opens the *`Workfront Goals`* area. 

1.  Click `Graphs` in the left panel. 


   ![](assets/graphs-in-left-panel.png)




   The Graphs section displays. 


   By default, the goals displayed in the Graphs section are limited by the following criteria:&nbsp;

    
    
    * The filters applied to the Graphs area. 
    *  Goals that are in a status of Active and Draft. 
    
    

1.  (Optional) Select the type of information you want to display by updating the filters in the upper-right corner of the Graphs section. 


   For more information about filtering goals, see [Filter information in Adobe Workfront Goals](filter-information-wf-goals.md).


   >[!TIP] {type="tip"}
   >
   >If you selected to display more than one time period, a health chart (gauge) as well as a progress chart (line) displays for each time period. 



1.  Review the information in the table below when you review the Goal Health Chart.


   ![](assets/gauge-graph-wf-align-350x230.png)




1.  Review the information in the table below when you review the Goal&nbsp;Progress Chart. 


   ![](assets/line-graph-wf-align-350x161.png)



<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 346px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Baseline progress</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">The green slope line indicates the expected overall percent complete average of active and closed goals for the selected time period. All goals within a period are expected to complete, so the baseline progress is always 100% at the end of the period. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Actual progress</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>The blue line indicates the actual overall percent complete average of active and closed goals for the selected time period in weekly increments. Each week during the duration of the goal is marked by a node in the line. </p> </td> 
  </tr> 
 </tbody> 
</table>


1.  Hover a week node in the goal progress chart and review the following:

    
    
    * `Week date`: The month, day, and year of the selected week.
    * `Progress`:&nbsp;An average of the actual percent complete of all goals for the selected week.
    * `Baseline`: An average of the expected percent complete of all goals for the selected week.
    
    

1.  (Optional) Click `Progress` at the bottom of the progress chart to remove the actual overall progress line


   Or


   Click `Baseline` at the bottom of the progress chart to remove the expected progress from the chart. 



&nbsp;
