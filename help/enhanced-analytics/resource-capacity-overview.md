---
filename: resource-capacity-overview
title: Resource capacity overview
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: View the Resource capacity visualization in Enhanced analytics
description: The Resource capacity visualization shows whether a team is over, under, or at capacity. This calculation is based on:
---

# View the Resource capacity visualization in *Enhanced analytics*

The Resource capacity visualization shows whether a team is over, under, or at capacity. This calculation is based on:

<ul> 
 <li> <p> <b>Available capacity</b>: The total amount of hours a home team has available to work in the filtered period of time</p> <note type="note">
   If you are looking at a future time period, the available capacity is calculated based on the team's capacity for the last 7 days. For this reason, any scheduled PTO is not taken into account.
  </note> </li> 
 <li> <p> <b>Planned capacity</b>: The total amount of planned hours of work expected from the home team in the filtered period of time</p> </li> 
</ul>

This comparison of a home team's planned hours and actual scheduled hours can help you determine if you're not assigning enough work to the home team or if they may be experiencing burnout from a heavy workload.

![](assets/resource-capacity-350x110.png)

On the Resource capacity visualization, you can see the following details:

<ul> 
 <li> <p><span class="bold">Planned capacity</span>: Inline with a home team name, the blue circle represents the number of planned hours assigned to the home team.</p> <p> <img src="assets/resource-capacity-blue-circle.png"> </p> </li> 
 <li> <p><span class="bold">Actual capacity</span>: Inline with a home team name, the vertical line represents the number of hours available for the home team.</p> <p> <img src="assets/resource-capacity-vertical-line.png"> </p> </li> 
 <li> <p><span class="bold">Over capacity</span>: When the horizontal line and the blue circle display to the right of the vertical line, the home team was assigned more work than they can complete in the number of available hours. This means that the team may be over capacity for the filtered time period. The remaining number of hours the team needs to complete displays to the right of the blue circle.</p> <p> <img src="assets/resource-capacity-over-capacity.png"> </p> </li> 
 <li> <p><span class="bold">Under capacity</span>: When the horizontal line and the blue circle display to the left of the vertical line, the home team has more available hours than the number of planned hours of work they were assigned. This means that the team may be under capacity for the filtered time period. The additional number of available hours for the home team to complete work displays to the left of the blue circle.</p> <p> <img src="assets/resource-capacity-under-capacity.png"> </p> </li> 
</ul>

Hovering over a row shows the exact number of hours for planned capacity and available capacity, as well as the number of hours the home team is over or under capacity.

Seeing this information helps you determine:

* If the home team was overallocated or underallocated.
* What the largest projects were that the home team was focused on.
* Which home teams are available for work.

To learn how to get the best data for this visualization, see [Enhanced analytics overview](../enhanced-analytics/enhanced-analytics-overview.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><em>Adobe Workfront</em> plan</a>*</td> 
   <td> <p>Business or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level.<br>For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View</p> <p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

For prerequisites to using Enhanced Analytics, see [Prerequisites](../enhanced-analytics/enhanced-analytics-overview.md#prerequi) in [Enhanced analytics overview](../enhanced-analytics/enhanced-analytics-overview.md).

## View the Resource capacity visualization

<ol> 
 <li value="1"> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the Main Menu icon 
     <img src="assets/main-menu-icon-16x12.png" style="width: 16;height: 12;">, then 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the Main Menu icon 
    <img src="assets/main-menu-icon-16x12.png" style="width: 16;height: 12;">, then 
   </MadCap:conditionalText>select <b>Analytics</b>.</p> </li> 
 <li value="2"> <p>In the left panel, select <span class="bold">People</span>.</p> <p> <draft-comment>
    <img src="assets/people-area-cropped-qs-350x276.png" style="width: 350;height: 276;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/people-area-cropped-qs-350x276.png" style="width: 350;height: 276;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="3"> <p>(Optional) To use a different date range, select new start and end dates from the date range filter.</p> <p> <img src="assets/filters-select-date-range-350x344.png" style="width: 350;height: 344;"> </img> </p> <p>For information on using the date range filter, see <a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Apply filters in Enhanced analytics</a>.</p> </li> 
 <li value="4"> <p>(Conditional) If you haven't set your Team filter, add the Team filter and select each team that you want to see data for.</p> <p>For more information on adding filters in <em>Enhanced analytics</em>, see <a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Apply filters in Enhanced analytics</a>.</p> <p>After you add filters, data for up to 50 projects displays and the filters remain active even after you leave the page or log out of <em>Workfront</em>.</p> </li> 
 <li value="5"> <p>(Optional) To zoom in on a date range, select a point on the visualization for the start of your date range and drag to the end of your date range.</p> <p>All other visualizations update to the same date range and a timeframe filter is created.</p> <p> <img src="assets/timeframe-filter-350x220.png" style="width: 350;height: 220;"> </img> </p> </li> 
 <li value="6"> <p>Hover over the home team line to see how many hours are still available to be scheduled, the amount of hours planned for the home team to complete, and the total number of hours worked, which is labeled as over, under, or at capacity.</p> <p> <img src="assets/resource-capacity-capacity-pop-up-350x213.png" style="width: 350;height: 213;"> </p> </li> 
 <li value="7"> <p>(Optional) To export the visualization data, click the <b>Export icon</b> <img src="assets/export.png"> in the top-right corner of the visualization, then select the export format:</p> 
  <ul> 
   <li> <p><b>Chart (PNG)</b> </p> </li> 
   <li> <p><b>Data Table (XSLX)</b> </p> </li> 
  </ul> </li> 
 <li value="8"> <p>Click a home team name to see more information in the Team capacity visualization.</p> <p>To learn more about the Team capacity visualization, see <a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">View the Team capacity visualization in Enhanced analytics</a>.</p> </li> 
</ol>

## Video walk-through

View the following video to learn more about the Resource capacity visualization. This video was recorded in *Workfront Classic*. However, the content also applies to *the new Workfront experience*.

[ ![](assets/video-walk-through--350x197.png)](https://vimeo.com/368320000/cc5bb66ac8) 
