---
filename: activity-by-team-overview
title: Activity by team overview
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
---



# View the Activity by team visualization in *`Enhanced analytics`* {#view-the-activity-by-team-visualization-in-enhanced-analytics}

The Activity by team visualization shows activities that happen during a specific time frame for a home team, allowing you to understand how different home teams spent their time in *`Adobe Workfront`*. Depending on how your home team is set up in *`Workfront`*, this visualization can give you different insights and answer different questions.


>[!NOTE]
>
>The Project activity visualization is similar to this visualization, but it displays activity based on people assigned to projects rather than people assigned to a home team.  
>For information on the Project activity visualization, see [View the Project activity visualization in Enhanced analytics](project-activity-overview.md).


![](assets/activity-by-team-350x113.png)




The different activities display in different colors to summarize specific events over the filtered time period:



*  `Users logged in`: Purple boxes show that people on the home team logged in on that day. A darker shade indicates a higher number of people logging in.


  ![](assets/project-activity-users-logged-in.png)



*  `Task status change`: Pink boxes show that people on the home team changed the status of a task on that day. A darker shade indicates a higher number of task statuses changing.


  ![](assets/project-activity-task-status-changes.png)



*  `Tasks completed`: Blue boxes show that people on the home team completed a task on that day. A darker shade indicates a higher number of tasks being completed.


  ![](assets/project-activity-tasks-completed.png)





Hovering over a box shows the exact number of times the action was completed in a given day. You can select a team to see a breakdown of these activities by each person on the home team.


Seeing this information helps you determine:



* What activities are occurring within a home team and at what rate.
* What home teams are being overworked or are using the system more.
* If the distribution of work is appropriate for the home team.


To learn how to get the best data for this visualization, see [Enhanced analytics overview](enhanced-analytics-overview.md).


## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> plan</a>*</td> 
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


## View the Activity by team visualization {#view-the-activity-by-team-visualization}




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



1.  Click a team name to see more details for activities completed by the home team.


   The list expands to display the activities of each person assigned to the home team.

1.  Hover over a colored box to see the date when users completed an action, as well as the number of times the action was completed that day.


   Darker colors indicate higher activity.


   ![](assets/activity-by-team-activity-pop-up-350x155.png)



1.  (Optional) To export the visualization data, click the **Export** icon ![](assets/export.png) in the top-right corner of the visualization, then select the export format:

    
    
    *  **Chart (PNG)** 
    *  **Data Table (XSLX)** 
    
    





## Video walk-through {#video-walk-through}

View the following video to learn more about the Activity by team visualization. This video was recorded in *`Workfront Classic`*. However, the content also applies to *`the new Workfront experience`*.


[ ![](assets/video-walk-through--350x197.png)](https://vimeo.com/368319785/c8ec75887b) 
