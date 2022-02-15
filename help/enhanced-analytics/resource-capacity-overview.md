---
filename: resource-capacity-overview
title: Resource capacity overview
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
---



# View the Resource capacity visualization in *`Enhanced analytics`* {#view-the-resource-capacity-visualization-in-enhanced-analytics}

The Resource capacity visualization shows whether a team is over, under, or at capacity. This calculation is based on:



*   **Available capacity**: The total amount of hours a home team has available to work in the filtered period of time


  >[!NOTE]
  >
  >If you are looking at a future time period, the available capacity is calculated based on the team's capacity for the last 7 days. For this reason, any scheduled PTO is not taken into account.



*   **Planned capacity**: The total amount of planned hours of work expected from the home team in the filtered period of time


This comparison of a home team's planned hours and actual scheduled hours can help you determine if you're not assigning enough work to the home team or if they may be experiencing burnout from a heavy workload.


![](assets/resource-capacity-350x110.png)




On the Resource capacity visualization, you can see the following details:



*  `Planned capacity`: Inline with a home team name, the blue circle represents the number of planned hours assigned to the home team.


  ![](assets/resource-capacity-blue-circle.png)



*  `Actual capacity`: Inline with a home team name, the vertical line represents the number of hours available for the home team.


  ![](assets/resource-capacity-vertical-line.png)



*  `Over capacity`: When the horizontal line and the blue circle display to the right of the vertical line, the home team was assigned more work than they can complete in the number of available hours. This means that the team may be over capacity for the filtered time period. The remaining number of hours the team needs to complete displays to the right of the blue circle.


  ![](assets/resource-capacity-over-capacity.png)



*  `Under capacity`: When the horizontal line and the blue circle display to the left of the vertical line, the home team has more available hours than the number of planned hours of work they were assigned. This means that the team may be under capacity for the filtered time period. The additional number of available hours for the home team to complete work displays to the left of the blue circle.


  ![](assets/resource-capacity-under-capacity.png)





Hovering over a row shows the exact number of hours for planned capacity and available capacity, as well as the number of hours the home team is over or under capacity.


Seeing this information helps you determine:



* If the home team was overallocated or underallocated.
* What the largest projects were that the home team was focused on.
* Which home teams are available for work.


To learn how to get the best data for this visualization, see [Enhanced analytics overview](enhanced-analytics-overview.md).


## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Business or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><a href="wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Review or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>View access to Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level.<br>For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

For prerequisites to using Enhanced Analytics, see [Prerequisites](enhanced-analytics-overview.md#prerequi) in [Enhanced analytics overview](enhanced-analytics-overview.md).


## View the Resource capacity visualization {#view-the-resource-capacity-visualization}




1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the Main Menu icon  <img src="assets/main-menu-icon-16x12.png" style="width: 16;height: 12;">, then </MadCap:conditionalText>`select **Analytics**.
1.  In the left panel, select `People`.


   ![](assets/people-area-cropped-qs-350x276.png)



1.  (Optional) To use a different date range, select new start and end dates from the date range filter.


   ![](assets/filters-select-date-range-350x344.png)




   For information on using the date range filter, see [Apply filters in Enhanced analytics](use-enhanced-analytics-filters.md).

1.  (Conditional) If you haven't set your Team filter, add the Team filter and select each team that you want to see data for.


   For more information on adding filters in *`Enhanced analytics`*, see [Apply filters in Enhanced analytics](use-enhanced-analytics-filters.md).


   After you add filters, data for up to 50 projects displays and the filters remain active even after you leave the page or log out of *`Workfront`*.

1.  (Optional) To zoom in on a date range, select a point on the visualization for the start of your date range and drag to the end of your date range.


   All other visualizations update to the same date range and a timeframe filter is created.


   ![](assets/timeframe-filter-350x220.png)



1.  Hover over the home team line to see how many hours are still available to be scheduled, the amount of hours planned for the home team to complete, and the total number of hours worked, which is labeled as over, under, or at capacity.


   ![](assets/resource-capacity-capacity-pop-up-350x213.png)



1.  (Optional) To export the visualization data, click the **Export icon** ![](assets/export.png) in the top-right corner of the visualization, then select the export format:

    
    
    *  **Chart (PNG)** 
    *  **Data Table (XSLX)** 
    
    

1.  Click a home team name to see more information in the Team capacity visualization.


   To learn more about the Team capacity visualization, see [View the Team capacity visualization in Enhanced analytics](team-capacity-overview.md).





## Video walk-through {#video-walk-through}

View the following video to learn more about the Resource capacity visualization. This video was recorded in *`Workfront Classic`*. However, the content also applies to *`the new Workfront experience`*.


[ ![](assets/video-walk-through--350x197.png)](https://vimeo.com/368320000/cc5bb66ac8) 
