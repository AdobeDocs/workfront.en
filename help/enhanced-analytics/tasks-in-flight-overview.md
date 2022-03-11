---
filename: tasks-in-flight-overview
title: Tasks in flight overview
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: View the Tasks in flight visualization in Enhanced analytics
description: The Tasks in flight visualization shows how many tasks (within the applied filter criteria) are in progress for a project, the percentage of work completed for each task, and how on schedule the tasks are.
---

# View the Tasks in flight visualization in `Enhanced analytics`

The Tasks in flight visualization shows how many tasks (within the applied filter criteria) are in progress for a project, the percentage of work completed for each task, and how on schedule the tasks are.

![](assets/tasks-in-flight-possible-replacement-350x104.png)

The Tasks in flight plan visualization shows the following task details:

<ul> 
 <li> <p><span class="bold">Planned task duration</span>: The length of a task bar indicates the planned duration, which is based on the task's start date and completion date.</p> <p> <img src="assets/tasks-in-flight-duration-350x80.png" style="width: 350;height: 80;"> </p> </li> 
 <li> <p><span class="bold">Work effort completed</span>: The dark blue color within a task bar indicates the amount of work completed for a task. This completion percentage displays to the right of the task bar.</p> <p> <img src="assets/tasks-in-flight-dark-blue-350x35.png" style="width: 350;height: 35;"> </p> </li> 
 <li> <p><span class="bold">Work effort remaining</span>: The light blue color within a task bar indicates the amount of work that needs to be completed for a task.</p> <p> <img src="assets/tasks-in-flight-light-blue-350x35.png" style="width: 350;height: 35;"> </p> </li> 
</ul>

This information can help you determine:

* Where work effort has been focused.
* Which tasks could be putting a project at risk.
* How close a task is to completion.
* Who you need to talk to about a specific task.

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
   <td> <p>View access to Projects</p> <p>View access to Tasks (To update tasks, you need Edit access to Tasks.)</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level.<br>For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permission to both project and task objects</p> <p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Prerequisites

For prerequisites to using Enhanced Analytics, see [Prerequisites](../enhanced-analytics/enhanced-analytics-overview.md#prerequi) in [Enhanced analytics overview](../enhanced-analytics/enhanced-analytics-overview.md).

## View the Tasks in flight visualization

<ol> 
 <li value="1"> <p> Click the Main Menu icon , thenselect <b>Analytics</b>.</p> </li> 
 <li value="2"> <p>(Optional) To use a different date range, select new start and end dates from the date range filter.</p> <p> <img src="assets/filters-select-date-range-350x344.png" style="width: 350;height: 344;"> </img> </p> <p>For information on using the date range filter, see <a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Apply filters in Enhanced analytics</a>.</p> </li> 
 <li value="3"> <p>(Conditional) If you need to limit the project data set, select and apply the filters that you want to use.</p> <p>For more information on adding filters in <span>Enhanced analytics</span>, see <a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Apply filters in Enhanced analytics</a>.</p> <p>After you add filters, data for up to 50 projects displays and the filters remain active even after you leave the page or log out of <span>Workfront</span>.</p> </li> 
 <li value="4"> <p>On the Flight plan or Project treemap visualization, click a project to view more information.</p> <p>The Burndown and Tasks in flight visualizations display.</p> <note type="note"> 
   <p>To learn more about these other visualizations, see:</p> 
   <ul> 
    <li><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">View the Flight plan visualization in Enhanced analytics</a> </li> 
    <li><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">View the Project treemap visualization in Enhanced analytics</a> </li> 
    <li><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">View the Burndown visualization in Enhanced analytics</a> </li> 
   </ul> 
  </note> </li> 
 <li value="5"> <p>(Optional) To zoom in on a date range, select a point on the visualization for the start of your date range and drag to the end of your date range.</p> <p>All other visualizations update to the same date range and a timeframe filter is created.</p> <p> <img src="assets/timeframe-filter-350x220.png" style="width: 350;height: 220;"> </img> </p> </li> 
 <li value="6"> <p>(Optional) To change how the tasks are sorted, click the <b class="bold">Sort by</b> menu, then select a new sorting option:</p> 
  <ul> 
   <li> <p><span class="bold">Completion date</span> </p> </li> 
   <li> <p><span class="bold">Alphabetically A-Z</span> </p> </li> 
   <li> <p><span class="bold">Work breakdown structure</span> (This option matches the order that the tasks appear in the project.)</p> </li> 
  </ul> <p>All other visualizations on the page update to match your sorting selection.</p> </li> 
 <li value="7"> <p>Review the progress of tasks in the selected project, then hover over a specific task to see the number of planned hours, the planned due date, and the completion percentage.</p> <p> <img src="assets/tasks-in-flight-task-details-350x242.png" style="width: 350;height: 242;"> </p> </li> 
 <li value="8"> <p>Click a task to open the task Detailson the right side of the screen, where you can see more information about the task, view or enter updates, or make changes to the task.</p>  </li> 
 <li value="9"> <p>(Optional) To export the visualization data, click the <b>Export icon</b> <img src="assets/export.png"> in the top-right corner of the visualization, then select the export format:</p> 
  <ul> 
   <li> <p><b>Chart (PNG)</b> </p> </li> 
   <li> <p><b>Data Table (XSLX)</b> </p> </li> 
  </ul> </li> 
</ol>

## Video walk-through

View the following video to learn more about the Tasks in flight visualization. This video was recorded in `the new Workfront experience`. However, the content also applies to `Workfront Classic`.

[ ![](assets/video-walk-through--350x197.png)](https://vimeo.com/441153099/45304dcf9c) 
