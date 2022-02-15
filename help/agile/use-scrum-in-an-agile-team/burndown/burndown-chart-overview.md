---
filename: burndown-chart-overview
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
---



# Agile burndown chart overview {#agile-burndown-chart-overview}

The burndown chart provides a visual representation of how stories are progressing through the iteration . The actual burndown rate is measured against the ideal burndown rate for the iteration timeline.


The burndown chart adjusts based on the selected day. The current day is the default. When a previous day is selected, all data in the burndown chart and&nbsp;all values in the completion status section above the burndown chart are recalculated to represent the data as it was at the end of the selected day. (You can select past days or the current day; you cannot select days in the future.)


![](assets/agile-iteration-burndown-350x88.png)




## Visual indicators {#visual-indicators}

The burndown chart contains the following visual indicators:

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col style="width: 40%;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col style="width: 60%;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt=""> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Ideal burndown rate based on when the iteration began.</p> <p>This line is not displayed if the scope of the iteration never changes (hours or points are never added or removed).</p> <p>This line is displayed as flat when work is done on a day off. For more information, see <a title="Using the Agile Burndown Chart" href="#understanding-how-days-off-affect-the-burndown-chart" class="MCXref xref">How days off affect the burndown chart</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt=""> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Ideal burndown rate based on current stories or tasks.</p> <p>The current ideal burndown rate (solid blue line) differs from the original ideal burndown rate (dotted blue line) when hours or points are added to or removed from the iteration after the iteration begins.</p> <p>This line is displayed as flat when work is done on a day off.</p> <p>For more information, see <a title="Using the Agile Burndown Chart" href="#understanding-how-days-off-affect-the-burndown-chart" class="MCXref xref">How days off affect the burndown chart</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt=""> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Actual burndown rate is shown in red when the burndown rate is less than the ideal (more points or hours remaining per day than the ideal burndown calculation).</p> <p>The following formula is used to calculate the actual burndown rate:</p> <p>[SUM(Point or Hour Value of In-Progress Work * Percent Complete) + Point or Hour Value of Completed Work]</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt=""> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Actual burndown rate is shown in green when the burndown rate is equal to or better than the ideal (equal or fewer points remaining per day than the ideal burndown calculation).</p> <p>The following formula&nbsp;is used to calculate the actual burndown rate:</p> <p>[SUM(Point or Hour Value of In-Progress Work * Percent Complete) + Point or Hour Value of Completed Work]</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Change in scope (hours or points are added or removed from the iteration).</p> <p>Scope changes are always shown as a vertical line&nbsp;in the middle of the day. In addition, a blue dot is displayed in the middle of any day where a scope change has occurred.</p> <p>The vertical axis of the burndown chart shows the story points or hours.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Change in date range (iteration duration is either increased or decreased).</p> <p>A blue dot is displayed in the middle of any day where the iteration duration was changed.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>A green or red dot is displayed on the actual burndown rate any time work is burned down. (When the actual burndown rate on that day is red, the dot is red; when the actual burndown rate on that day is green, the dot is green.)</p> <p>Work is burned down when any of the following occur:</p> 
    <ul> 
     <li> The Percent Complete is increased on the story.<br>Percent Complete is increased when: </li> 
     <ul> 
      <li> <p>Manually changed</p> </li> 
      <li> <p>The number of points or hours are updated on the story</p> </li> 
     </ul> 
     <li>The status of the story is changed to&nbsp;Complete</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## How days off affect the burndown chart {#how-days-off-affect-the-burndown-chart}

The default schedule defined in *`Workfront`* affects the burndown&nbsp;chart&nbsp;by excluding days off (weekends and holidays) from the burndown. The burndown chart uses the&nbsp;default schedule to define working days (as described in&nbsp; [Create a schedule](create-schedules.md)).


Agile teams can incorporate team-specific non-working days by defining&nbsp;an alternate schedule (as described in the article [Use an alternate team schedule for burndown charts](use-alt--team-schedule-burndown-charts.md)). This alternate schedule is then reflected in the burndown chart of any iteration assigned to the team. The alternate schedule affects only the burndown chart. 


Days off are reflected in the burndown chart only if:



*  Work was previously logged on a day off. (The day when work was logged is displayed.)


  When work is logged on a day off:

    
    
    *  Any work logged is not included when calculating&nbsp;the ideal burndown because the team is not scheduled to do any work.
    *  The ideal burndown lines (the solid blue line and dashed blue line) are displayed as flat in the burndown chart for any day when work was done or on the day you are viewing the burndown chart (if you are viewing on a day off).
    *  Work logged is included when calculating other burndown statistics such as the&nbsp;estimated completion and the average points or hours per day.
    
    

*  You are viewing the burndown chart on a day off. (The day that you are viewing is shown on the burndown chart.)
*  You complete the total remaining work for the iteration on a day off.


  When a user completes the total remaining work for the iteration on a day off, the Estimated Completion field displays the date the iteration was completed.


  When planning the iteration, if you set the iteration end date for a non-working day and the iteration is tracking to finish on time, the Estimated Completion date is set for the last working day prior to the iteration end date that you set (because work is not scheduled to be burned down on non-working days).


  The end date for the iteration is specified when the iteration is planned, as described in the article [Create an iteration](create-an-iteration.md).   




