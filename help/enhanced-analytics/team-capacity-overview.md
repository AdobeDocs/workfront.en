---
filename: team-capacity-overview
title: Team capacity overview
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: View the Team capacity visualization in Enhanced analytics
description: The Team capacity visualization shows the total amount of capacity a home team has, whether they are overallocated or underallocated, and how dynamic the capacity is over time.
---

# View the Team capacity visualization in *Enhanced analytics*

The Team capacity visualization shows the total amount of capacity a home team has, whether they are overallocated or underallocated, and how dynamic the capacity is over time.

![](assets/team-capacity-350x110.png)

The Team capacity visualization displays the volume of work assigned to the home team on a given day.

<ul> 
 <li> <p><span class="bold">Burnout</span>: When the darker blue fill color is above the dotted line, the home team has more work hours assigned to them than they can complete in the number of hours the team is available to work. This indicates that the team is overallocated and may be approaching burnout.</p> <p> <img src="assets/team-capacity-over-capacity.png"> </p> </li> 
 <li> <p><span class="bold">Unchallenged</span>: When the darker blue fill color is below the dotted line, the home team has more hours available to work than the amount of work assigned to them. This indicates that the team is underallocated and may be unchallenged.</p> <p> <img src="assets/team-capacity-under-capacity.png"> </p> </li> 
 <li> <p><span class="bold">Balance</span>: When the lighter or more transparent blue fill color is just above, just below, or at the dotted line, the home team has an amount of work hours assigned to them that they should be able to complete within their available work hours. This indicates that the team's workload is more balanced.</p> <p> <img src="assets/team-capacity-at-capacity.png"> </p> </li> 
</ul>

Hovering over any point on the visualization shows the following details for a given day:

* `Scheduled hours`: This is the number of planned hours of work the team needs to complete.
* `Available hours`: This is the number of work hours the team is available to work.
* `Capacity`: In addition to a capacity percentage, the designations At capacity, Under capacity, or Over capacity also display.

Seeing this information helps you determine:

* When the home team was overallocated or underallocated.
* If the home team is overallocated or underallocated on a daily basis.
* How consistent a home team's workload is from day to day.
* If you're creating capacity issues with new work.

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

## View the Team capacity visualization

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
 <li value="5"> <p>On the Resource capacity visualization, click a team to see more information.</p> <p>The Team capacity visualization displays.</p> <p>For more information on the Resource capacity visualization, see <a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">View the Resource capacity visualization in Enhanced analytics</a>.</p> </li> 
 <li value="6"> <p>(Optional) To zoom in on a date range, select a point on the visualization for the start of your date range and drag to the end of your date range.</p> <p>All other visualizations update to the same date range and a timeframe filter is created.</p> <p> <img src="assets/timeframe-filter-350x220.png" style="width: 350;height: 220;"> </img> </p> </li> 
 <li value="7"> <p>Hover over a point on the graphed line to see the scheduled hours and planned hours for the given date, as well as the capacity percentage and whether the home team was over, under, or at capacity at the time.</p> <p> <img src="assets/team-capacity-capacity-pop-up-350x351.png" style="width: 350;height: 351;"> </p> </li> 
 <li value="8"> <p>(Optional) To export the visualization data, click the <b>Export icon</b> <img src="assets/export.png"> in the top-right corner of the visualization, then select the export format:</p> 
  <ul> 
   <li> <p><b>Chart (PNG)</b> </p> </li> 
   <li> <p><b>Data Table (XSLX)</b> </p> </li> 
  </ul> </li> 
</ol>

## Video walk-through

View the following video to learn more about the Team capacity visualization. This video was recorded in *Workfront Classic*. However, the content also applies to *the new Workfront experience*.

[ ![](assets/video-walk-through--350x197.png)](https://vimeo.com/368320039/6551197797) 
