---
filename: activity-by-team-overview
title: Activity by team overview
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: View the Activity by team visualization in Enhanced analytics
description: The Activity by team visualization shows activities that happen during a specific time frame for a home team, allowing you to understand how different home teams spent their time in Adobe Workfront. Depending on how your home team is set up in Workfront, this visualization can give you different insights and answer different questions.
---

# View the Activity by team visualization in *Enhanced analytics*

The Activity by team visualization shows activities that happen during a specific time frame for a home team, allowing you to understand how different home teams spent their time in *Adobe Workfront*. Depending on how your home team is set up in *Workfront*, this visualization can give you different insights and answer different questions.

>[!NOTE]
>
>The Project activity visualization is similar to this visualization, but it displays activity based on people assigned to projects rather than people assigned to a home team.  
>For information on the Project activity visualization, see [View the Project activity visualization in Enhanced analytics](../enhanced-analytics/project-activity-overview.md).

![](assets/activity-by-team-350x113.png)

The different activities display in different colors to summarize specific events over the filtered time period:

<ul> 
 <li> <p><span class="bold">Users logged in</span>: Purple boxes show that people on the home team logged in on that day. A darker shade indicates a higher number of people logging in.</p> <p> <img src="assets/project-activity-users-logged-in.png"> </img> </p> </li> 
 <li> <p><span class="bold">Task status change</span>: Pink boxes show that people on the home team changed the status of a task on that day. A darker shade indicates a higher number of task statuses changing.</p> <p> <img src="assets/project-activity-task-status-changes.png"> </img> </p> </li> 
 <li> <p><span class="bold">Tasks completed</span>: Blue boxes show that people on the home team completed a task on that day. A darker shade indicates a higher number of tasks being completed.</p> <p> <img src="assets/project-activity-tasks-completed.png"> </img> </p> </li> 
</ul>

Hovering over a box shows the exact number of times the action was completed in a given day. You can select a team to see a breakdown of these activities by each person on the home team.

Seeing this information helps you determine:

* What activities are occurring within a home team and at what rate.
* What home teams are being overworked or are using the system more.
* If the distribution of work is appropriate for the home team.

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

## View the Activity by team visualization

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
 <li value="6"> <p>Click a team name<draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      or role
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
     or role
   </MadCap:conditionalText> to see more details for activities completed by the home team.</p> <p>The list expands to display the activities of each person assigned to the home team.</p> </li> 
 <li value="7"> <p>Hover over a colored box to see the date when users completed an action, as well as the number of times the action was completed that day.</p> <p>Darker colors indicate higher activity.</p> <p> <img src="assets/activity-by-team-activity-pop-up-350x155.png" style="width: 350;height: 155;"> </p> </li> 
 <li value="8"> <p>(Optional) To export the visualization data, click the <b>Export</b> icon <img src="assets/export.png"> in the top-right corner of the visualization, then select the export format:</p> 
  <ul> 
   <li> <p><b>Chart (PNG)</b> </p> </li> 
   <li> <p><b>Data Table (XSLX)</b> </p> </li> 
  </ul> </li> 
</ol>

## Video walk-through

View the following video to learn more about the Activity by team visualization. This video was recorded in *Workfront Classic*. However, the content also applies to *the new Workfront experience*.

[ ![](assets/video-walk-through--350x197.png)](https://vimeo.com/368319785/c8ec75887b) 
