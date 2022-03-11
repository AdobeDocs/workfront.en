---
filename: navigate-the-workload-balancer
product-area: resource-management
navigation-topic: the-workload-balancer
title: Navigate the Workload Balancer
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Navigate the `Workload Balancer`

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

Use the `Workload Balancer` to understand the availability of your resources as well as to assign work to your users. This article walks you through using the icons and settings available to update the view for and navigate the `Workload Balancer`.

>[!NOTE]
>
>The `Workload Balancer` is a resource scheduling tool that will eventually replace the current resource scheduling tools which are currently deprecated. 
>
>For more information about removing the resource scheduling tools and replacing them with the `Workload Balancer`, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).
>
>We recommend that you use the `Workload Balancer` for scheduling your resources.

The `Workload Balancer` is available in multiple areas of `Adobe Workfront`. Navigating it is similar in all areas. This article describes how to navigate the `Workload Balancer` for multiple projects in the Resourcingarea. For more information about where the `Workload Balancer` is located, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

Also consider reading the following articles:

* For information about assigning work using the `Workload Balancer`, see ` [Overview of assigning work in the Adobe Workfront Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)`. 

* For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to&nbsp;the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Considerations for viewing items in the `Workload Balancer`

Consider the following when viewing the `Workload Balancer`:

<ul> 
 <li>Projects display in the Workload Balancer only when the Group by Project setting is enabled. This setting is enabled by default.</li> 
 <li> <p>When a project has no tasks during a period of time, the bar at the project level becomes a dimmed color. </p> <p> <img src="assets/wb-break-in-project-timeline-with-no-tasks-highlight-350x80.png" style="width: 350;height: 80;"> </p> </li> 
 <li> <p>When you don't have permissions to see certain items, they display as <span class="bold">Inaccessible work items</span> or <span class="bold">Inaccessible projects</span>. </p> <p> <img src="assets/balancer-inaccessible-items-and-projects-highlighted-350x108.png" style="width: 350;height: 108;"> </p> </li> 
 <li>The names of the work items display on the left and within the timeline selected on the right. </li> 
 <li>The total of Planned Hours for each work item displays to the right of the name of the work items on the left. </li> 
 <li> <p>The total of the Planned Hours for each project displays to the right of the name of the project on the left. </p> <p>The Planned Hours information for the project is a total of Planned Hours from all items listed in the Workload Balancer, and not a total of Planned Hours on the project. </p> </li> 
</ul>

##  Overview of the Unassigned Work and Assigned Work areas

The `Workload Balancer` displays work items in two separate areas, depending on their assignments.

The two areas of the `Workload Balancer` display the following information:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Unassigned Work</td> 
   <td> <p>This area displays tasks unassigned to users. It does not display issues. </p> <p>This area does not display any work items by default. We recommend using filters to display relevant information for you in this area.</p> <p>After you apply a filter, this area displays the following work items:</p> 
    <ul> 
     <li>unassigned</li> 
     <li>assigned to a team </li> 
     <li>assigned to a job role</li> 
     <li> <p>assigned to a team and a role at the same time</p> </li> 
    </ul> <p>Tip: Items assigned to a user as the primary assignee do not display in the Unassigned Work area. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assigned Work</td> 
   <td> <p> All active users in the system display in this area by default. We recommend using filters to limit the amount of information in this area. </p> <p>Both tasks and issues display in the Assigned Work area. </p> <p>The work items that the users are assigned to display under their names. </p> <p>If a work item is assigned to multiple users, the item displays under each assigned user. </p> </td> 
  </tr> 
 </tbody> 
</table>

For information about applying a filter in the `Workload Balancer`, see [Manage filters in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

![](assets/balancer-empty-unassiged-area-350x179.png)

## Navigate the `Workload Balancer`

You can update the view in the `Workload Balancer` to display exactly the information you need to focus on in the time frame that makes the most sense to you.

After selecting the settings you want to apply to your view, the `Workload Balancer` remembers these settings every time you access it from any browser or device.

<ol> 
 <li value="1"> Click the Main Menu icon in the upper-right corner of Workfront, then click Resourcing. </li> 
 <li value="2"> <p> Click Workload Balancer in the left panel.<span></span> </p> <p>You might need to click <span class="bold">Scheduling</span>, then select <span>Workload Balancer</span> in the upper-left corner. </p> 
  <div> 
   <p>The <span>Workload Balancer</span> displays work assignment information starting with the current week. The names of work items are listed on the left side as well as represented by bars on the right side of the of the <span>Workload Balancer</span> within their respective timelines. <span>By default, blue bars represent the timelines of projects and tasks and maroon bars represent issues.</span></p> Tip: You can change the color of the bars for projects and tasks when you select your color scheme to match the project. For more information, continue reading this procedure. 
   <div> 
    <p>The work items that display under the name of users in the <span>Workload Balancer</span> are sorted by the following criteria, in this order: </p> 
    <ol> 
     <li value="1">Planned Start Date (oldest first)</li> 
     <li value="2">Planned Completion Date (oldest first)</li> 
     <li value="3">Alphabetical by project (only when the first two criteria are identical for multiple work items)</li> 
    </ol> 
   </div> 
  </div> </li> 
 <li value="3"> <p>Click the <span class="bold">Filter icon</span> <img src="assets/filter-icon.png"> in the upper-right corner of the <span class="bold">Unassigned Work</span> or the <span class="bold">Assigned Work</span> areas to select the type of information to display in the Workload Balancer.</p> <p>For information about filtering information in the <span>Workload Balancer</span>, see <a href="../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md" class="MCXref xref">Manage filters in the Workload Balancer</a>. </p> </li> 
 <li value="4"> <p>Click the right-pointing arrow next to <span class="bold">Unassigned Work</span> to expand this area or the down-pointing arrow to collapse it. </p> <note type="tip">
   No items display in this area by default. You must apply a filter to view unassigned work items.
  </note> </li> 
 <li value="5"> <p>Drag and drop the separation line between the <span class="bold">Unassigned Work</span> and <span class="bold">Assigned Work</span> areas to adjust their size.</p> <p> <img src="assets/modern-scheduler-separation-line-between-areas-350x278.png" style="width: 350;height: 278;"> </p> </li> 
 <li value="6">Click the back or forward icons <img src="assets/back-and-forward-icons.png"> to navigate the timeline, then click <span class="bold">Today</span> to return to the current week. </li> 
 <li value="7"> <p>Click the <span class="bold">time frame drop-down menu</span> on the toolbar, then click the beginning date of the period selected in step 8 on the calendar that displays. By default, the first week selected on the calendar is the week you navigated to.</p> <p> <img src="assets/calendar-date-picker-balancer-350x208.png" style="width: 350;height: 208;"> </p> 
  <div class="tips" data-mc-autonum="<b>Tips: </b>">
   <span class="autonumber"><span><b>Tips: </b></span></span> 
   <ul> 
    <li> <p>When you view the <span>Workload Balancer</span> on smaller screens the time frame drop-down menu is replaced by the calendar icon <img src="assets/calendar-icon-wb.png">. </p> </li> 
    <li> <p>A dual calendar displays only when you select to view 12 weeks at a time. </p> </li> 
   </ul> 
  </div> </li> 
 <li value="8"> <p>Click one of the following options in the toolbar to display information by different time frames:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Day</td> 
     <td>Displays information by day for four weeks starting with today's date, by default. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Week</td> 
     <td>Displays information by week for four weeks. </td> 
    </tr> Month Displays information by month for three months. 
   </tbody> 
  </table> </li> 
 <li value="9"> <p>Select the number of weeks you want to display at one time in the Workload Balancer from the following options:</p> 
  <ul> 
   <li>2 weeks</li> 
   <li>4 weeks.&nbsp;This is the default setting.</li> 
   <li>6 weeks</li> 
   <li> <p>12 weeks</p> 
    <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
     <span class="autonumber"><span><b>Tip: </b></span></span> 
     <ul> 
      <li> <p><span>When you display the <span>Workload Balancer</span> by month, the option for 12 weeks becomes 3 months.</span> </p> <p> <img src="assets/3-months-12-weeks-drop-down-wb-350x140.png" class="preview" style="width: 350;height: 140;"> </p> </li> 
      <li> <p><span>When you display the <span>Workload Balancer</span> by a time frame shorter than 3 months or 12 weeks, the time frame switches automatically from Month to Week.</span> </p> </li> 
     </ul> 
    </div> </li> 
  </ul> </li> 
 <li value="10"> Click the Settings icon . The Settings panel displays. Select from the options listed below to update the information you view in the Workload Balancer, then click the X icon in the upper-right of the Settings box to close it. Group by Project: When this is selected, the items in the Unassigned and Assigned Work areas are grouped by project. This is selected by default. Include hours from issues: When this is selected, issues assigned to users display under the user's name in the Assigned Work area and the Planned Hours from the issues also display for the issues, the project, and the user. Tip: Issues don't display in the Unassigned Work area of the Workload Balancer. Show Projected Dates: When this is selected, the projected timeline of work items displays in addition to the planned timeline. Notice the following: The projected timeline of tasks and projects displays in light blue bars with a line underneath. The projected timeline of issues displays in light maroon bars with a line underneath. The projected timeline for the items that you have no access to view displays in light gray with a line underneath. When a task or issue completes before the due Planned Completion Date the allocation numbers for the remaining days are struck through and do not count towards the user's allocation. This displays only when both the Show Projected Dates setting and the Show allocation icon are enabled. Tip: Notice that work items display in the Workload Balancer when either their planned or the projected timelines (not necessarily both at the same time) occur during the timeframe selected. Show completed work: When this is enabled, tasks and issues that are completed display in the Assigned Work area. This is enabled by default. A green checkmark icon displays to the upper-right corner of a task or issue bar when they are completed. The same icon displays for a project when the tasks or issues for the selected time frame of the project are completed. Show remaining time: When this is enabled, Workfront displays the difference between the daily time for which the user is available to work based on their schedules and the hours for which they are allocated in the Assigned Work area for the users. This is disabled by default and allocated time displays by default. In the Select color theme section, select from the following: Default: The bars for all projects and their work items display in blue. Project: The bars associated with each project and its work items change according to the name of the project. All tasks that belong to the project display in bars that match the color of the project. Project Status: The bars associated with each project and its work items change to the color of the status of the project. Tip: The project status is that associated with the Group of the project. If the Group does not have group-specific statuses, the color of the work item bars is that of the system-level project status. Both system as well as custom statuses display. For information about group statuses, see Create or edit a group status. In the Display user allocation in section, select from the following: Hours: Displays allocated time as hours. This is the default. Percentage: Displays allocated time as a percentage of the total available time </li> (Optional and conditional) If you changed the color theme to Project Status, hover over the name of a project on the left to view the status of the project. 
 <li value="12"> <p>Click the <span class="bold">Chart icon</span> <img src="assets/user-allocation-chart-icon.png"> to display the user allocation in a chart format. Days where the user is overallocated display as red blocks, and days where the user is underallocated or at capacity display as blue blocks. The size of the blocks indicates the amount of the allocation: the larger the box, the more time the user is allocated to work items for that day or week. </p> <p> <img src="assets/user-allocation-chart-350x237.png" style="width: 350;height: 237;"> </p> </li> 
 <li value="13"> <p>Click the <span class="bold">Show allocations icon</span> <img src="assets/show-allocations-icon-small.png"> to view the daily or weekly Planned Hours for work items.</p> <p>This replaces the name in the bars of the work items with the amount of daily or weekly Planned Hours in the Unassigned and Assigned Work areas. This setting is disabled by default. </p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <ul> 
    <li>The Show allocations setting only affects what displays for projects, tasks, <span>issues</span> and inaccessible items. Daily Planned Hours for users display by default and cannot be hidden.</li> 
    <li>You must enable the Group by Project setting to display daily Planned Hours for projects. </li> 
    <li>When you view the <span>Workload Balancer</span> by week, the hours displayed are the weekly Planned Hours. </li> 
   </ul> 
  </div> <p>Days that show overallocations display in red. </p> </li> 
 <li value="14"> <p>(Optional) Hover over the allocated time in the user line to understand what the capacity and allocation of the user. The capacity is the availability of the user according to their schedule. </p> <p> <img src="assets/overallocation-vs-capacity-tooltip-wb-nwe.png"> </p> </li> 
 <li value="15"> <p>(Optional)&nbsp;Click the <span class="bold">Hide allocations icon</span> <img src="assets/show-allocations-icon-small.png"> to display the name of the tasks in the bars of the work items. </p> </li> 
 <li value="16"><span>Click the <span class="bold">More menu</span> icon <img src="assets/more-icon.png"> to the right of a task or issue name,</span> then click one of the following:
  <ul>
   <li><p><span class="bold">Assign this to</span>, then start typing the name of a user, role, or team you want to assign the work item to. </p><p><img src="assets/more-menu-right-of-task-350x104.png" style="width: 350;height: 104;"></p>
    <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
     <span class="autonumber"><span><b>Tip: </b></span></span>
     <p><span>You can also use the following shortcuts to assign tasks or issues:</span></p>
     <ul>
      <li><span>In Windows: CTRL+click the task or issue bar.</span></li>
      <li><span>In&nbsp;Mac: CMD+click the task or issue bar.</span></li>
     </ul>
    </div><p>For more information about assigning work items to users in the <span>Workload Balancer</span>, see <a href="../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md" class="MCXref xref">Overview of assigning work in the Adobe Workfront Workload Balancer</a>. </p></li>
   <li><span class="bold">Edit allocations</span>, then edit the daily or weekly allocations for the user. For information about managing user allocations, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>. </li>
  </ul></li> Click the Open Summary icon , then click the bar of a task or issue to open the Summary panel. For information about updating task information in the Summary in the Workload Balancer, see Update work items in the Workload Balancer using the Summary in the new Adobe Workfront experience. Tip: This option is available for tasks in the Unassigned Work area and for tasks and issues in the Assigned Work area. This is not available for projects or users. Click Bulk Assignments to assign work items in bulk. For more information, see Assign work in bulk using the Adobe Workfront Workload Balancer. 
 <li value="19">(Optional) Double-click a daily or weekly allocation for a user inside the bar of a work item to edit the number of allocated hours. For information about managing user allocations, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>. </li> 
 <li value="20">Click the name of a work item on the left to access it. </li> 
 <li value="21"> <p>Click the <span class="bold">Shareable link icon</span> <img src="assets/wb-shearable-link-icon-small.png"> to copy the direct URL for the <span>Workload Balancer</span> to your clipboard. </p> </li> 
 <li value="22"> <p>(Optional) Share the link with any user who does not have direct access to the <span>Workload Balancer</span>.</p> <p>For information about sharing the <span>Workload Balancer</span> with a link, see <a href="../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md" class="MCXref xref">Share the Workload Balancer with a link</a>. </p> </li> 
 <li value="23"> <p>(Conditional) From the <span>Workload Balancer</span> of a project, click the <span class="bold">Show role allocations</span> icon <img src="assets/show-role-allocation-icon.png">. </p> <p>The Role Allocation panel displays. You can view information about Planned Hours associated with job roles on the project and job roles associated with initiatives from the <span>Scenario Planner</span>. For more information, see <a href="../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md" class="MCXref xref">Overview of reconciling resource allocations between projects and initiatives </a>. </p> <note type="tip">
   You cannot view initiative job role information if your organization has not purchased a license for the 
   <span>Workfront Scenario Planner</span>. In this case, you can only view the planned hours associated with job roles on the project. For more information, see 
   <a href="../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Adobe Workfront Scenario Planner</a>. 
  </note> </li> 
 <li value="24"> (Optional) Select Scheduling from the drop-down menu in the upper-left corner to access the scheduling area. </li> 
</ol>

