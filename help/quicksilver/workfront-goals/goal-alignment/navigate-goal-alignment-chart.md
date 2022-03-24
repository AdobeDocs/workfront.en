---
filename: navigate-goal-alignment-chart
product: workfront-goals
navigation-topic: goal-alignment
title: Navigate the Goal Alignment section in Adobe Workfront Goals
description: Use the Goal Alignment section to display a holistic view of goal alignment across the entire organization in a flowchart. Aligned goals display on cards that interconnect in a hierarchical tree.
---

# Navigate the Goal Alignment section in Adobe Workfront Goals

Use the Goal Alignment section to display a holistic view of goal alignment across the entire organization in a flowchart. Aligned goals display on cards that interconnect in a hierarchical tree.

For information about goal alignment and how to achieve it, also see the following articles:

* [Goal alignment overview in Adobe Workfront Goals](../../workfront-goals/goal-alignment/goal-alignment-overview.md) 
* [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)

## Access requirements

You must have the following to perform the activities described in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontlicense*</td> 
   <td> <p>Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Adobe Workfront Goals</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Goals</p> <p>Note:   <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> 
    <div> 
     <p>View or higher permissions to goals</p> 
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Adobe Workfront Goals</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

You must have the following before you can start:

* A Layout Template that includes the Goals area in the Main&nbsp;Menu.

## Navigate the Goal Alignment section

1. ```Use the filters in the upper-right corner of the alignment chart to select only goals that are important to you. For information about using filters in Workfront Goals, see``` [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   The goals that match your filters display in the alignment chart on cards.

   The following information displays on a goal card:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Time period dates </td> 
      <td> <p>This is the period for which the goal is open.&nbsp;The goal must be achieved by the end date of the period. Workfront Goals calculates progress on the goal based on the duration of the goal's period and the current date.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress indicators</td> 
      <td>The number of progress indicators for the goal.&nbsp;Progress indicators can be aligned goals, results, or activities. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Owner name</td> 
      <td>The name of the user, team, group, or the organization designated as the goal&nbsp;Owner. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Goal name</td> 
      <td>The name of the goal. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Goal Progress bar <span>and Progress</span></td> 
      <td> <p>The goal progress indicates how much of the goal has currently been achieved.&nbsp;This is an automatic calculation of the average of the progress of all aligned goals, results, and activities for the goal based on the time elapsed since the start of the goal's time period. For information about calculating progress on goals, see <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Calculate goal progress in Adobe Workfront Goals</a>. </p> 
       <div> 
        <p>The actual progress of the goal by the current date.&nbsp;The following progress values and colors indicate how likely the goal is to being achieved on time: </p> 
        <ul> 
         <li><span>On Target</span> (green indicator): the goal is on time and will be achieved on time.</li> 
         <li> <span>At Risk</span> (yellow indicator):&nbsp;the goal runs behind and might not be achieved on time.</li> 
         <li> <span>In&nbsp;Trouble</span> (red indicator): the goal is in danger of not being achieved on time. </li> 
        </ul> 
       </div> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Updated on date </td> 
       <td>The date when the goal was last updated</td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td><span>Goals in all statuses display in the Goal Alignment section. </span> </td> 
     </tr> 
    </tbody> 
   </table>

   Goals that are aligned to other goals display the number of aligned goals under the goal card.

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

1. Click the **downward-pointing arrow** icon under a goal to further expand and view the children goals.

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

   >[!TIP]
   >
   >Goals that have children goals aligned to them display the number of aligned goals under their respective cards.

1. (Conditional) If the current filter excludes some of the goals that participate in an alignment, a warning message displays to indicate that not all goals display.

   ![](assets/parent-goal-excluded-by-filter-alignment-section-350x230.png)

1. Click&nbsp;**Show them** to display the goals currently eliminated by the filter.

   Notice the following changes in the alignment chart:

   * Connected goals previously eliminated by the filter now display in the alignment chart. 
   * The filter in the upper-right corner is outlined in yellow to indicate that it is currently not applied.

     ![](assets/reapply-filter-link-and-yellow-filter-highlight-350x120.png)

     A Reapply filter link displays to the left of the filter name.

1. (Optional)&nbsp;Click **Reapply filter** to return to the original results and display the goal hierarchy.
1. (Optional) Hover over the progress indicator to understand where the goal progress should be for the current day.

   ![](assets/progress-mouse-over-alignment-chart-350x163.png)

   The following information displays:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">As of today</td> 
      <td>The progress status is always current. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Actual</span> </td> 
      <td>The actual progress (a percentage) of the goal by the current date as calculated by taking into account all the progress indicators on the goal. Goal progress indicators are aligned goals, activities, and results. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Expected</td> 
      <td> <p>The expected progress (a percentage) of the goal by the current date assuming that you will achieve the goal on time.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click a goal card to open the Goal&nbsp;Details panel and edit information about or check in on the goal. For information about editing existing goals, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md). For information about checking in on goals, see [Check in on goals in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
1. Click the ```the upward-pointing arrow``` of the current-level goal to return to the previous level in the hierarchy of the chart.

   Or

   (Optional)&nbsp;Click **Exit goal hierarchy** to display the cards of all the goals that match the current filter, without displaying their connection to each other.

   &nbsp;

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p class="preview">In the Preview environment, do the following:</p>
<ol>
<li value="1"> <p><span class="preview">Use the filters in the upper-right corner of the alignment chart to select only goals that are important to you. For information about using filters in Workfront Goals, see </span><a href="../../workfront-goals/goal-management/filter-information-wf-goals.md" class="MCXref xref">Filter information in Adobe Workfront Goals</a> </p> </li>
<li value="2"> <p>(Conditional) If the current filter excludes some of the goals that participate in an alignment, a warning message displays to indicate that not all goals are displayed:<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
< new screen shot>
</MadCap:conditionalText>
--></p> </li>
<li value="3"> <p>Click&nbsp;<strong>Show them</strong> to display the goals currently eliminated by the filter.</p> <p>Notice the following changes in the alignment chart: </p>
<ul>
<li> <p>Connected goals previously eliminated by the filter now display in the alignment chart. </p> </li>
<li> <p>The filter in the upper-right corner is outlined in yellow to indicate that it is currently not applied. </p> </li>
<li> <p>A Reapply filter link displays to the left of the filter name</p> </li>
</ul> </li>
<li value="4"> <p>(Optional) Click <strong>Reapply filter</strong> to return to the original results and display the goal hierarchy .</p> </li>
<li value="5"> <p>(Optional)&nbsp;Click <strong>Exit goal hierarchy</strong> to display the cards of all the goals that match the current filter, without displaying their connection to each other. </p> </li>
</ol>
<ol>
<li value="1"> <p>In the Production environment, do the following: </p>
<ol>
<li value="1"> <p>(Optional) Click the&nbsp;<strong>Company</strong> tab to view goals that are assigned to your organization and their aligned goals. </p> <p>Goals that are aligned to other goals display with additional stacked cards behind the top goal card. </p> <p> <img src="assets/stacked-aligned-goal-cards-highlighted-350x147.png" style="width: 350;height: 147;"> </p> </li>
<li value="2"> <p>(Optional) Select a different period from the upper-right drop-down menu.&nbsp;The default is the current quarter. You can only select one time period at a time to view goals that are due during that period. Select from quarters or yearly periods for the current year and up to two more years. </p> </li>
<li value="3"> <p>(Optional) Start typing the name of an owner who is designated as a goal owner in the <strong>Search for owner's name</strong> field, the select it when it appears in the list. Goals assigned to the owner you indicate and their aligned goals display in the Goal Alignment section. </p> <p>The goals that match your filter and tab selection display in the alignment chart. </p> </li>
</ol> </li>
</ol>
</div>
-->

&nbsp;
