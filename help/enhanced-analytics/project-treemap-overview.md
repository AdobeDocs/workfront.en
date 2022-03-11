---
filename: project-treemap-overview
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: View the Project treemap visualization in Enhanced analytics
description: The Project treemap visualization is a view of hours—or days—that have been worked in a specific window of time compared against other work efforts in size. This helps you understand how much time people have dedicated to a project.
---

# View the Project treemap visualization in `Enhanced analytics`

The Project treemap visualization is a view of hours—or days—that have been worked in a specific window of time compared against other work efforts in size. This helps you understand how much time people have dedicated to a project.

![](assets/project-treemap-350x126.png)

The boxes in the Project treemap visualization represent projects and the size of the boxes shows a comparison of how much time was spent on different projects. The larger the box is, the more time spent on the project.

The Project treemap visualization is comprised of:

<ul> 
 <li> <p><span class="bold">Smaller, light blue boxes</span>: Projects that have fewer hours—or days—display as smaller boxes with a light blue color.</p> <p> <img src="assets/project-treemap-smaller-box.png"> </p> </li> 
 <li> <p><span class="bold">Larger, dark blue boxes</span>: Projects that have more hours—or days—display as larger boxes with a dark blue color.</p> <p> <img src="assets/project-treemap-larger-box-350x205.png" style="width: 350;height: 205;"> </p> </li> 
 <li> <p><span class="bold">Medium-sized, blue boxes</span>: Projects that fall in between the two categories display as medium-sized boxes with a shade of blue between the dark blue and light blue colors. There are 3 possible shades of blue for the medium-sized boxes.</p> </li> 
</ul>

The legend on the right side shows a breakdown of completed hours for each shade of blue. This legend is dynamic and updates according to the data.

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>If you are looking at the Project treemap visualization by duration instead of by planned hours, this legend shows a breakdown of days worked for each shade of blue.  
>![](assets/project-treemap-days-worked.png)>

Seeing this information helps you determine:

* The priority of things being worked on during the selected date range.
* What teams are spending time on.
* If teams are focusing on the right things.
* When a specific project is clicked, how much the scope of a project changed over that time period.

To learn how to get the best data for this visualization, see [Enhanced analytics overview](../enhanced-analytics/enhanced-analytics-overview.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span>Adobe Workfront</span> plan</a>*</td> 
   <td> <p>Business or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Projects</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level.<br>For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View</p> <p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Prerequisites

For prerequisites to using Enhanced Analytics, see [Prerequisites](../enhanced-analytics/enhanced-analytics-overview.md#prerequi) in [Enhanced analytics overview](../enhanced-analytics/enhanced-analytics-overview.md).

## View the Project treemap visualization

<ol> 
 <li value="1"> <p> Click the Main Menu icon , thenselect <b>Analytics</b>.</p> </li> 
 <li value="2"> <p>(Optional) To use a different date range, select new start and end dates from the date range filter.</p> <p> <img src="assets/filters-select-date-range-350x344.png" style="width: 350;height: 344;"> </img> </p> <p>For information on using the date range filter, see <a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Apply filters in Enhanced analytics</a>.</p> </li> 
 <li value="3"> <p>(Conditional) If you need to limit the project data set, select and apply the filters that you want to use.</p> <p>For more information on adding filters in <span>Enhanced analytics</span>, see <a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Apply filters in Enhanced analytics</a>.</p> <p>After you add filters, data for up to 50 projects displays and the filters remain active even after you leave the page or log out of <span>Workfront</span>.</p> </li> 
 <li value="4"> <p>(Optional) To change how the projects are sorted, click the <b class="bold">Sort by</b> menu in the upper-right corner of the Project treemap visualization, then select a new sorting option:</p> 
  <ul> 
   <li> <p><span class="bold">A - Z</span> </p> </li> 
   <li> <p><span class="bold">Z - A</span> </p> </li> 
   <li> <p><span class="bold">Planned completion date</span> </p> </li> 
   <li> <p><span class="bold">Planned start date</span> </p> </li> 
  </ul> <p>All other visualizations on the page update to match your sorting selection.</p> </li> 
 <li value="5"> <p>(Conditional) If there are more than 50 projects in your data set, use the arrows in the bottom-left corner of the visualization to navigate from one group of 50 projects to the next.</p> <p>All other visualizations on the page update to match your page selection.</p> <p> <img src="assets/pagination-350x118.png" style="width: 350;height: 118;"> </p> </li> 
 <li value="6"> <p>(Optional) Change the view from <b>planned hours</b> to <b>duration</b>.</p> <p>Planned hours is selected by default.</p> </li> 
 <li value="7"> <p>Hover over a project to see the project condition, as well as the number of total planned hours, the number of total completed hours, and the average number of hours spent on the project per day.</p> <p> <img src="assets/project-treemap-project-details-350x404.png" style="width: 350;height: 404;"> </p> <note type="note"> 
   <p>If you selected the <b>duration</b> view, you'll see the following duration details:</p> 
   <ul> 
    <li> <p><b class="bold">Planned Timeframe</b>: The number of days planned to complete the project.</p> </li> 
    <li> <p><b class="bold">Days Worked</b>: The planned duration for each task that was completed within the date range selected at the top, divided by the number of hours in a day.</p> </li> 
   </ul> 
   <p> <img src="assets/duration-treemap-350x159.png" style="width: 350;height: 159;"> </p> 
   <p>For more information on duration, see the section "Duration view" in <a href="../enhanced-analytics/enhanced-analytics-overview.md" class="MCXref xref">Enhanced analytics overview</a>.</p> 
  </note> </li> 
 <li value="8"> <p>(Optional) To export the visualization data, click the <b>Export icon</b> <img src="assets/export.png"> in the top-right corner of the visualization, then select the export format:</p> 
  <ul> 
   <li> <p><b>Chart (PNG)</b> </p> </li> 
   <li> <p><b>Data Table (XSLX)</b> </p> </li> 
  </ul> </li> 
 <li value="9"> <p>Click a project to open the Burndown and Tasks in flight visualizations to gain a deeper insight of how tasks and hours—or days—contributed to the size of a project.</p> </li> 
</ol>

For more information on the Burndown visualization, see [View the Burndown visualization in Enhanced analytics](../enhanced-analytics/burndown-overview.md). For more information on the Tasks in flight visualization, see [View the Tasks in flight visualization in Enhanced analytics](../enhanced-analytics/tasks-in-flight-overview.md).

## Video walk-through

View the following video to learn more about the Project treemap visualization. This video was recorded in `the new Workfront experience`. However, the content also applies to `Workfront Classic`.

[ ![](assets/video-walk-through--350x197.png)](https://vimeo.com/441151801/59d2fa726b) 
