---
filename: calculate-hours-fte-scheduling-area
product-area: resource-management
navigation-topic: resource-scheduling
title: Configure how Workfront calculates resource hour and FTE availability for the Scheduling area
description: We are no longer developing the Resource Scheduling tools and they will soon be removed from Adobe Workfront. We recommend that you use the Workload Balancer for scheduling your resources.
---

# Configure how *Workfront* calculates resource hour and FTE&nbsp;availability for the Scheduling area

>[!NOTE]
>
>We are no longer developing the Resource Scheduling tools and they will soon be removed from *Adobe Workfront*. We recommend that you use the *Workload Balancer* for scheduling your resources. 
>
>For information about scheduling resources using the new *Workload Balancer*, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
>
>For more information about the timeline for removing the Resource Scheduling tools and replacing them with the *Workload Balancer*, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

The *Adobe Workfront administrator* determines how *Workfront* calculates resource availability and user allocation at the system level (considering hours as well as FTE availability) when they configure Resource Management preferences.

They can select to use one of the following:

* The Default Schedule of the system and the user's FTE. 
* The user's schedule.&nbsp;

For more information, see [Configure Resource Management preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

This setting affects user availability in the following circumstances when scheduling resources:

* When allowing *Workfront* to automatically assign resources, as described in [Manually assign unassigned tasks and issues in the Scheduling areas](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

* When displaying allocation indicators, as described in the section "Allocation indicators" in the article&nbsp; [Manage user allocations in the Scheduling areas](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2>Access requirements</h2>
<p>You must have the following:</p>
<table cellspacing="0">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><em>Adobe Workfront</em> plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader"><em>Adobe Workfront</em> license*</td>
<td> <p><em>Plan</em> </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>System administrator</p> <note type="note">
If you still don't have access, ask your
<em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a
<em>Workfront administrator</em> can change your access level, see
<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr> <draft-comment>
<tr data-mc-conditions="QuicksilverOrClassic.Draft mode">
<td role="rowheader">Object permissions</td>
<td> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td>
</tr>
</draft-comment>
<tr data-mc-conditions="QuicksilverOrClassic.Draft mode">
<td role="rowheader">Object permissions</td>
<td> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your <em>Workfront administrator</em>.</p>
</div>
<h2>Configure how <em>Workfront</em> calculates resource availability when scheduling resources</h2>
<ol>
<li value="1">Log in to <em>Workfront</em> as an administrator. </li>
<li value="2"><![CDATA[
]]><draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click the
<span class="bold">Main Menu</span> icon
<img src="assets/main-menu-icon.png"> in the upper-right corner of
<em>Adobe Workfront</em>.
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click the
<span class="bold">Main Menu</span> icon
<img src="assets/main-menu-icon.png"> in the upper-right corner of
<em>Adobe Workfront</em>.
</MadCap:conditionalText><br></li>
<li value="3"> <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click&nbsp;
<span class="bold">Setup</span>.
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click&nbsp;
<span class="bold">Setup</span>.
</MadCap:conditionalText> </li>
<li value="4"> <p> Click&nbsp;<span class="bold">Resource Management</span>.<br></p> <p> <draft-comment>
<img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
</draft-comment><img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <br> </p> </li>
<li value="5"> Select to calculate the availability of users in <em>Workfront</em> using&nbsp;one of the following methods:
<ul>
<li><span class="bold">The Default Schedule</span>:&nbsp;The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user when scheduling resources. The Schedule of the user is ignored. In this case:&nbsp;
<ul>
<li> The&nbsp;<span class="bold">Available Hours</span> for a user when scheduling resources<span class="bold">&nbsp;</span>are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE </code><em><code>value</code>&nbsp;</em><br>For example, if the&nbsp;Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Scheduling area.<br>For more information about schedules, including the Default Schedule, see&nbsp;<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
<li> The&nbsp;<span class="bold">Available FTE&nbsp;</span>for the user when scheduling resources<span class="bold">&nbsp;</span>is the same as the user FTE specified in the user settings.&nbsp;&nbsp;<br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner.&nbsp;For more information about the value of the user FTE as it displays in the user settings, see&nbsp;<a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><span class="bold">The User's Schedule</span>: The Schedule of the user&nbsp;is used to determine the availability of the user when scheduling resources.&nbsp;The value of the user FTE is ignored. In this case:&nbsp;
<ul>
<li> The&nbsp;<span class="bold">Available Hours&nbsp;</span>in the<span class="bold">&nbsp;Resource Planner&nbsp;</span>are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available&nbsp;for work, the user is available to work for 40 hours a week in the Resource Planner.&nbsp; </li>
<li> The&nbsp;<span class="bold">Available FTE&nbsp;</span>in the<span class="bold">&nbsp;Resource Planner</span>&nbsp;is calculated by the following formula:<br><em>User Available FTE =&nbsp;Hours from the Schedule of the User/ Default Schedule Hours<br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in <em>Workfront</em> has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see&nbsp;<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul> <note type="note"> &nbsp;If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note></li>
</ul></li>
</ol>
</div>
-->

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>System administrator</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Configure how *Workfront* calculates resource availability when scheduling resources

<ol> 
 <li value="1">Log in to <em>Workfront</em> as an administrator. </li> 
 <li value="2"><![CDATA[
        ]]><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
   <span class="bold">Main Menu</span> icon 
   <img src="assets/main-menu-icon.png"> in the upper-right corner of 
   <em>Adobe Workfront</em>. 
  </MadCap:conditionalText><br></li> 
 <li value="3"> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click&nbsp; 
   <span class="bold">Setup</span>. 
  </MadCap:conditionalText> </li> 
 <li value="4"> <p> Click&nbsp;<span class="bold">Resource Management</span>.<br></p> <p> <img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <br> </p> </li> 
 <li value="5"> Select to calculate the availability of users in <em>Workfront</em> using&nbsp;one of the following methods: 
  <ul> 
   <li><span class="bold">The Default Schedule</span>:&nbsp;The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user when scheduling resources. The Schedule of the user is ignored. In this case:&nbsp; 
    <ul> 
     <li> The&nbsp;<span class="bold">Available Hours</span> for a user when scheduling resources<span class="bold">&nbsp;</span>are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE </code><em><code>value</code>&nbsp;</em><br>For example, if the&nbsp;Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Scheduling area.<br>For more information about schedules, including the Default Schedule, see&nbsp;<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li> 
     <li> The&nbsp;<span class="bold">Available FTE&nbsp;</span>for the user when scheduling resources<span class="bold">&nbsp;</span>is the same as the user FTE specified in the user settings.&nbsp;&nbsp;<br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner.&nbsp;For more information about the value of the user FTE as it displays in the user settings, see&nbsp;<a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li> 
    </ul></li> 
   <li><span class="bold">The User's Schedule</span>: The Schedule of the user&nbsp;is used to determine the availability of the user when scheduling resources.&nbsp;The value of the user FTE is ignored. In this case:&nbsp; 
    <ul> 
     <li> The&nbsp;<span class="bold">Available Hours&nbsp;</span>in the<span class="bold">&nbsp;Resource Planner&nbsp;</span>are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available&nbsp;for work, the user is available to work for 40 hours a week in the Resource Planner.&nbsp; </li> 
     <li> The&nbsp;<span class="bold">Available FTE&nbsp;</span>in the<span class="bold">&nbsp;Resource Planner</span>&nbsp;is calculated by the following formula:<br><em>User Available FTE =&nbsp;Hours from the Schedule of the User/ Default Schedule Hours<br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in <em>Workfront</em> has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see&nbsp;<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li> 
    </ul> <note type="note"> &nbsp;If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule. 
    </note></li> 
  </ul></li> 
</ol>

