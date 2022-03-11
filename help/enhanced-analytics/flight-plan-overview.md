---
filename: flight-plan-overview
title: Flight plan overview
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: View the Flight plan visualization in Enhanced analytics
description: The Flight plan visualization shows how many projects (within the applied filter criteria) were in flight, what condition changes happened throughout the life of these projects, and how closely these projects adhered to their planned completion deadlines.
---

# View the Flight plan visualization in Enhanced analytics

The Flight plan visualization shows how many projects (within the applied filter criteria) were in flight, what condition changes happened throughout the life of these projects, and how closely these projects adhered to their planned completion deadlines.

![](assets/flight-plan-350x132.png)

In the actual duration of a project, you can see only the following project conditions:

* On Target
* At Risk
* In Trouble

To learn about project conditions, see [Overview of Project Condition and Condition Type](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

The Flight plan visualization shows the following project details:

<ul> 
 <li> <p><b>Planned duration</b>: The horizontal blue line represents the planned length of the project, with the triangles at either end of the line indicating the start date and end date.</p> <p> <img src="assets/planned-duration-line-350x37.png" style="width: 350;height: 37;"> </p> </li> 
 <li> <p><b>Actual duration</b>: The thick, colored line below the planned duration represents the actual length of the project. The color of the line changes depending on the condition of the project at that particular time in the life of the project.</p> <p> <img src="assets/actual-duration-line.png"> </p> </li> 
 <li> <p><b>Actual condition</b>: The thick, colored line also shows the condition of a project at different moments in time. The color of the line changes depending on the condition of the project:</p> 
  <ul> 
   <li> <p><span class="bold">Green</span>: On Target</p> </li> 
   <li> <p><span class="bold">Orange</span>: At Risk</p> </li> 
   <li> <p><span class="bold">Red</span>: In&nbsp;Trouble</p> </li> 
  </ul> <p> <img src="assets/actual-condition-color.png"> </p> </li> 
</ul>

By hovering over a project row in the Flight Plan visualization, you can see information about the project's planned timeframe, the current project condition, and—if applicable—the custom condition. To get a more in-depth view of what may have affected the duration or condition, you can look at the other visualizations in the Enhanced analytics area.

Seeing this information helps you determine:

* What events extend a project past the original planned completion date.
* When a project starts to run into issues.
* How many projects are open over the same time period.
* How many projects are active.
* Which projects need extra attention or support.

For information on how to get the best data for this visualization, see [Enhanced analytics overview](../enhanced-analytics/enhanced-analytics-overview.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront plan</a>*</td> 
   <td> <p>Business or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to the project</p> <p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

For prerequisites to using Enhanced Analytics, see [Prerequisites](../enhanced-analytics/enhanced-analytics-overview.md#prerequi) in [Enhanced analytics overview](../enhanced-analytics/enhanced-analytics-overview.md).

## View the Flight plan visualization

<ol> 
 <li value="1"> <p> Click the Main Menu icon , thenselect <b>Analytics</b>.</p> </li> 
 <li value="2"> <p>(Optional) To use a different date range, select new start and end dates from the date range filter.</p> <p> <img src="assets/filters-select-date-range-350x344.png" style="width: 350;height: 344;"> </p> <p>For information on using the date range filter, see <a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Apply filters in Enhanced analytics</a>.</p> </li> 
 <li value="3"> <p>(Conditional) If you need to limit the project data set, select and apply the filters that you want to use.</p> <p>For more information on adding filters in Enhanced analytics, see <a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Apply filters in Enhanced analytics</a>.</p> <p>After you add filters, data for up to 50 projects displays and the filters remain active even after you leave the page or log out of Workfront.</p> </li> 
 <li value="4"> <p>(Optional) To zoom in on a date range, select a point on the visualization for the start of your date range and drag to the end of your date range.</p> <p>All other visualizations update to the same date range and a timeframe filter is created.</p> <p> <img src="assets/timeframe-filter-350x220.png" style="width: 350;height: 220;"> </p> </li> 
 <li value="5"> <p>(Optional) To change how the projects are sorted, click the <b class="bold">Sort by</b> menu in the upper-right corner of the Flight plan visualization, then select a new sorting option:</p> 
  <ul> 
   <li> <p><span class="bold">A - Z</span> </p> </li> 
   <li> <p><span class="bold">Z - A</span> </p> </li> 
   <li> <p><span class="bold">Planned completion date</span> </p> </li> 
   <li> <p><span class="bold">Planned start date</span> </p> </li> 
  </ul> <p>All other visualizations on the page update to match your sorting selection.</p> </li> 
 <li value="6"> <p>(Conditional) If there are more than 50 projects in your data set, use the arrows in the bottom-left corner of the visualization to navigate from one group of 50 projects to the next.</p> <p>All other visualizations on the page update to match your page selection.</p> <p> <img src="assets/pagination-350x118.png" style="width: 350;height: 118;"> </p> </li> 
 <li value="7"> <p>Hover over the project bar graph to see the blue date line, as well as the following details:</p> 
  <ul> 
   <li> <p>Planned timeline</p> </li> 
   <li> <p>Current condition</p> </li> 
   <li> <p>Custom condition (if applicable)</p> </li> 
  </ul> <p> <img src="assets/project-bar-graph-350x143.png" style="width: 350;height: 143;"> </p> </li> 
 <li value="8"> <p>(Optional) To export the visualization data, click the <b>Export</b> icon <img src="assets/export.png"> in the top-right corner of the visualization, then select the export format:</p> 
  <ul> 
   <li> <p><b>Chart (PNG)</b> </p> </li> 
   <li> <p><b>Data Table (XSLX)</b> </p> </li> 
  </ul> </li> 
 <li value="9"> <p>To see more project information, click a project on the visualization to open the Burndown and Tasks in flight visualizations.</p> <p>These visualizations can help you gain deeper insight into what caused the project to get off track. They also make it easy to check in on an in-progress project.<br>For more information on the Burndown visualization, see <a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">View the Burndown visualization in Enhanced analytics</a>. For more information on the Tasks in flight visualization, see <a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">View the Tasks in flight visualization in Enhanced analytics</a>.</p> </li> 
</ol>

## Video walk-through

View the following video to learn more about the Flight plan visualization. This video was recorded in the new Workfront experience. However, the content also applies to Workfront Classic.

[ ![](assets/video-walk-through--350x197.png)](https://vimeo.com/441153800/2a336ba497) 
