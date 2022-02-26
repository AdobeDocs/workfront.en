---
filename: project-activity-overview
title: Project activity overview
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: View the Project activity visualization in Enhanced analytics
description: The Project activity visualization shows an aggregate view of activities on the project level—the activities of each person assigned to the project—that happened during a specific time frame. You can narrow your focus to understand the activities within a project, or you can compare project activities against other projects in Adobe Workfront.
---

# View the Project activity visualization in *Enhanced analytics*

The Project activity visualization shows an aggregate view of activities on the project level—the activities of each person assigned to the project—that happened during a specific time frame. You can narrow your focus to understand the activities within a project, or you can compare project activities against other projects in *Adobe Workfront*.

>[!NOTE]
>
>The Activity by team visualization behaves similarly to this visualization, but the Activity by team visualization shows home team activity for all projects.  
>For information on the Activity by team visualization, see [View the Activity by team visualization in Enhanced analytics](../enhanced-analytics/activity-by-team-overview.md).

[ ![](assets/project-activity-350x114.png)](../Resources/Images/Analytics/Activity by Team.png)

Project activities display in different colors to summarize specific events in a project over a period of time:

<ul> 
 <li> <p><span class="bold">Users logged in</span>: Purple boxes show that people assigned to the project logged in on that day. A darker shade indicates a higher number of people logging in.</p> <p> <img src="assets/project-activity-users-logged-in.png"> </p> </li> 
 <li> <p><span class="bold">Task status change</span>: Pink boxes show that people changed the status of a task for the project on that day. A darker shade indicates a higher number of task statuses changing.</p> <p> <img src="assets/project-activity-task-status-changes.png"> </p> </li> 
 <li> <p><span class="bold">Tasks completed</span>: Blue boxes show that people completed a task for the project. A darker shade indicates a higher number of tasks being completed.</p> <p> <img src="assets/project-activity-tasks-completed.png"> </p> </li> 
</ul>

Hovering over a box shows the exact number of times the action was completed in a given day. You can select a project to see a breakdown of these activities by each individual contributor on the project.

Seeing this information helps you determine:

* The activity on a specific project.
* The activity of one project compared to other projects.
* Which users are working on a project and at what frequency.

To learn how to get the best data for this visualization, see [Enhanced analytics overview](../enhanced-analytics/enhanced-analytics-overview.md).

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><em>Workfront</em> plan</a>*</td> 
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

## View the Project activity visualization

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
 <li value="2"> <p>(Optional) To use a different date range, select new start and end dates from the date range filter.</p> <p> <img src="assets/filters-select-date-range-350x344.png" style="width: 350;height: 344;"> </p> <p>For information on using the date range filter, see <a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Apply filters in Enhanced analytics</a>.</p> <note type="note">
   If you select a date range for a period greater than 3 months, the Project activity visualization does not display any data.
  </note> </li> 
 <li value="3"> <p>(Conditional) If you need to limit the project data set, select and apply the filters that you want to use.</p> <p>For more information on adding filters in <em>Enhanced analytics</em>, see <a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Apply filters in Enhanced analytics</a>.</p> <p>After you add filters, data for up to 50 projects displays and the filters remain active even after you leave the page or log out of <em>Workfront</em>.</p> </li> 
 <li value="4"> <p>(Optional) To zoom in on a date range, select a point on the visualization for the start of your date range and drag to the end of your date range.</p> <p>All other visualizations update to the same date range and a timeframe filter is created.</p> <p> <img src="assets/timeframe-filter-350x220.png" style="width: 350;height: 220;"> </p> </li> 
 <li value="5"> <p>(Optional) To change how the projects are sorted, click the <b class="bold">Sort by</b> menu, then select a new sorting option:</p> 
  <ul> 
   <li> <p><span class="bold">A - Z</span> </p> </li> 
   <li> <p><span class="bold">Z - A</span> </p> </li> 
   <li> <p><span class="bold">Planned completion date</span> </p> </li> 
   <li> <p><span class="bold">Planned start date</span> </p> </li> 
  </ul> <p>All other visualizations on the page update to match your sorting selection.</p> </li> 
 <li value="6"> <p>(Conditional) If there are more than 50 projects in your data set, use the arrows in the bottom-left corner of the visualization to navigate from one group of 50 projects to the next.</p> <p>All other visualizations on the page update to match your page selection.</p> <p> <img src="assets/pagination-350x118.png" style="width: 350;height: 118;"> </p> </li> 
 <li value="7"> <p>Click a project in the visualization to see more details for the project.</p> <p>The list expands to display the activities of each individual contributor on the project.</p> </li> 
 <li value="8"> <p>Mouse over a box to see the date that users completed an action, as well as the number of times the action was completed for that day.</p> <p> <img src="assets/project-activity-activity-pop-up-350x137.png" style="width: 350;height: 137;"> </p> </li> 
 <li value="9"> <p>(Optional) To export the visualization data, click the <b>Export icon</b> <img src="assets/export.png"> in the top-right corner of the visualization, then select the export format:</p> 
  <ul> 
   <li> <p><b>Chart (PNG)</b> </p> </li> 
   <li> <p><b>Data Table (XSLX)</b> </p> </li> 
  </ul> </li> 
</ol>

## Video walk-through

View the following video to learn more about the Project activity visualization. This video was recorded in *the new Workfront experience*. However, the content also applies to *Workfront Classic*.

[ ![](assets/video-walk-through--350x197.png)](https://vimeo.com/441154105/7181a0dedf) 
