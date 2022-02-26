---
filename: resource-availability-allocation-resource-planner
product-area: resource-management
navigation-topic: resource-planning
title: Review resource availability and allocation using the Resource Planner
description: You can view the availability of your resources and the amount of planned or budgeted work for your projects in the Resource Planner. These values are displayed in Hours, FTE (Full Time Equivalent), or Cost amounts and are organized in columns.
---

# Review resource availability and allocation using the *Resource Planner*

You can view the availability of your resources and the amount of planned or budgeted work for your projects in the *Resource Planner*. These values are displayed in Hours, FTE (Full&nbsp;Time Equivalent), or Cost amounts and are organized in columns.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> and higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Review</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Financial Data</p> </li> 
     <li> <p>Users</p> </li> 
     <li> <p>Projects</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects you want to view in the <em>Resource Planner</em></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

You must meet all the prerequisites required to work with the *Resource Planner*.&nbsp;For more information, see [Resource Planner overview](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>If any of the prerequisites required for the correct functionality of the *Resource Planner* are missing, some of the numbers may be zero, or the Budgeted Hours might be dimmed.

## Availability and allocation of resources

The columns that display the availability and allocation of your resources change depending on which view you apply to the *Resource Planner*. For information about displaying the information in the *Resource Planner* by Project, Role, or User see [Resource Planner navigation overview](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Consider the following when changing your view to the *Resource Planner*:

* When you apply the `View by Project` or `View by Role` views, you can see the following columns:

  * Available Hours, FTE, or Cost
  * Planned Hours, FTE, or Cost
  * Budgeted Hours, FTE, or Cost
  * Hours, FTE, or Cost Variance
  * Net Hours, FTE, or Cost

* When you apply the `View by User` view, you can see the following columns:

  * Available Hours or FTE 
  * Planned Hours or FTE 
  * Hour or FTE Difference 
  * Planned Hours Allocation Percentage

` `**Tips: **``  The information is not available as Cost when applying the `View by User` view to the *Resource Planner*.

For more information about what each column displays, mouse over the name of the column in which the number is displayed.  
![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)

For more information about the data displayed in each column, see the following articles:

* [Overview of hours, FTE, and cost information in the Project and Role views of the Resource Planner](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md) 
* [View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)

## View information by Hour, FTE, or Cost

<ol> 
 <li value="1"> <p> Go to the <span class="bold">Planner</span>.</p> <p>By default, information displays by Hours in the <em>Resource Planner</em>.<br></p> </li> 
 <li value="2"> Expand the drop-down menu. <br><img src="assets/hours-fte-or-cost-dropdown.png" alt="Hours_fte_or_cost_dropdown.png"></li> 
 <li value="3"> <p> Select from the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Hours</td> 
     <td>Displays availability and allocation information in Hours.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">FTE</td> 
     <td> <p>Displays availability and allocation information in FTE.</p> <p>For more information about how the FTE is calculated in the <em>Resource Planner</em>, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md">Calculating Hours and FTE in the Resource Planner</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Cost</td> 
     <td> <p>Displays availability and allocation information by cost, if you are viewing the <em>Resource Planner</em> in the Project or Role views. The information displays values in the currency of your system. Your <em>Workfront administrator</em> defines the system currency. For more information about setting up the system currency in <em>Workfront</em>, see <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <note type="note">
       You must associate users and job roles with Cost per Hour rates in order to display Cost information in the 
       <em>Resource Planner</em>.
       <br style="font-style: italic;">For more information about associating Cost per Hour rates with job roles, see 
       <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.
       <br style="font-style: italic;">For more information about associating Cost per Hour rates with users, see 
       <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.
       <br style="font-style: italic;">For more information about how Cost is calculated in the 
       <em>Resource Planner</em>, see 
       <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">Calculate costs in the Resource Planner </a>.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Customize</td> 
     <td>Creates a custom view of the columns that display in the <em>Resource Planner</em>. Select the options that you want to display in the <em>Resource Planner</em>, as described in the steps below. </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4"> <p>(Conditional) If you selected <b>Customize</b>, indicate options in the <span class="bold">Customize displayed metrics</span> box to set up your custom view. </p> <p> <img src="assets/planner-customize-view-box-350x114.png" style="width: 350;height: 114;"> </p> </li> 
 <li value="5"> <p>In the <span class="bold">View type</span> column on the left, select one of the following views:</p> 
  <ul> 
   <li>Project </li> 
   <li>Role</li> 
   <li>User</li> 
  </ul> </li> 
 <li value="6"> <p>In the <span class="bold">Display selected items</span> section, select the type of information you want to display in the columns of the selected view.&nbsp;The following table shows what options are available in each view:</p> 
  <table cellspacing="3"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td rowspan="2"><b>Option</b> </td> 
     <td colspan="3"><b>View</b> </td> 
    </tr> 
    <tr> 
     <td>User</td> 
     <td>Project </td> 
     <td>Role </td> 
    </tr> 
    <tr> 
     <td>Available</td> 
     <td>✔</td> 
     <td>✔</td> 
     <td>✔</td> 
    </tr> 
    <tr> 
     <td>Planned </td> 
     <td>✔</td> 
     <td>✔</td> 
     <td>✔</td> 
    </tr> 
    <tr> 
     <td>Budgeted</td> 
     <td>&nbsp;</td> 
     <td>✔</td> 
     <td>✔</td> 
    </tr> 
    <tr> 
     <td>Variance</td> 
     <td>&nbsp;</td> 
     <td>✔</td> 
     <td>✔</td> 
    </tr> 
    <tr> 
     <td>Net</td> 
     <td>&nbsp;</td> 
     <td>✔</td> 
     <td>✔</td> 
    </tr> 
    <tr> 
     <td>Actual</td> 
     <td>✔</td> 
     <td>&nbsp;</td> 
     <td>&nbsp;</td> 
    </tr> 
    <tr> 
     <td>Difference</td> 
     <td>✔</td> 
     <td>&nbsp;</td> 
     <td>&nbsp;</td> 
    </tr> 
    <tr> 
     <td>Percent</td> 
     <td>✔</td> 
     <td>&nbsp;</td> 
     <td>&nbsp;</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="7"> <p>Select <span class="bold">Use Planned (PLN)&nbsp;values in NET calculations</span> to use Planned instead of Budgeted information when calculating the Net values in the Project and Role views. </p> <p>When selecting this option <em>Workfront</em> calculates the Net values using the following formula: </p> <p><code>Net = Available - Planned</code> </p> <note type="tip">
   <span>This option is applied only when you select at least one option to customize the view in the Display selected items section.</span> 
  </note> </li> 
 <li value="8"> <p>Click <span class="bold">Save</span>. </p> <p>The customized view that includes your selected columns displays. </p> <p>The <em>Resource Planner</em> lists the customized view as Custom in the Hours drop-down menu. </p> <note type="note">
   You can have only one customized view. 
  </note> <p> <img src="assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png" style="width: 183;height: 281;"> </p> </li> 
</ol>

## View the User Allocation chart

You can display the Planned Allocation of users against their availability in a chart.

To display the allocation of users in a chart:

<ol> 
 <li value="1"> <p>Go to the <span class="bold">Planner</span>.</p> <p>For more information about accessing the <em>Resource Planner</em>, see the <a href="../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner" class="MCXref xref">Locate the Resource Planner</a> section in the article <a href="../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p> </li> 
 <li value="2"> <p>Select <span class="bold">View by User</span>.</p> <note type="tip">
   You can view the User Allocation Chart only in the User View. 
  </note> </li> 
 <li value="3"> <p>Click the <span class="bold">User allocation chart</span> icon <img src="assets/rp-user-allocation-chart.png" alt="RP_user_allocation_chart.png"> to display the following information:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Availability % with no overallocation for all users</td> 
     <td>This is the amount of time that all users are available for work in a time period, shown as a percentage from their total available time. </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Overallocation % for all users</span> </td> 
     <td> <p>This is the amount of time that users are overallocated in a time period, shown as a percentage from the total available time.</p> <note type="note">
        An overallocation happens when the Planned Hours are higher than the Available Hours. 
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Underutilization % for all users</td> 
     <td> <p>This is the amount of time that users are underutilized in a time period, shown as a percentage from the total available time.</p> <note type="note">
       Underutilization happens when the Planned Hours are lower than the Available Hours. 
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">There is an overallocation for at least one user during this time period</td> 
     <td>This indicates that there is an overallocation for at least one user in a time period, although the total amount of time of all users is not overallocated for the time period.<br>You must scroll through the list of users and the hours for the user who is overallocated are highlighted in red.</td> 
    </tr> 
   </tbody> 
  </table> <p> <img src="assets/rp--user-allocation-chart-dec.-7--2017-350x148.png" alt="RP__user_allocation_chart_Dec._7__2017.png" style="width: 350;height: 148;"> </p> </li> 
 <li value="4"> <p>(Optional) Click the <span class="bold">Overallocation % for all users</span> area in the chart.<br>All users that are overallocated are highlighted in red.</p> </li> 
 <li value="5">(Optional) Click the <span class="bold">Underutilization % for all users</span> area in the chart.<br>All users that are underutilized are highlighted in blue.</li> 
 <li value="6">(Optional) Click the indicator icon <img src="assets/one-user-overallocation-marker.png" alt="one_user_overallocation_marker.png"> that shows where you have at least one user overallocated.<br>The users that are overallocated are highlighted in red. </li> 
 <li value="7">(Optional) Refresh the page to collapse the chart. </li> 
</ol>

