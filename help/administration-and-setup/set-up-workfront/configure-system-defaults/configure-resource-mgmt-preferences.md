---
filename: configure-resource-mgmt-preferences
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configure Resource Management preferences
description: As an Adobe Workfront administrator you can configure the Resource Management Preferences for your system.
---

# Configure Resource Management preferences

As an `Adobe Workfront administrator` you can configure the Resource Management Preferences for your system.

The Resource Management preferences determine how user availability and FTE are calculated for the `Workfront` resource scheduling and planning tools.

For information about planning and scheduling resources in `Workfront`, see [Get started with Resource Management](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure Resource Management preferences

>[!NOTE]
>
>Because this is a global setting, this selection affects all the calculations for the entire system, for all users, in all the resource management tools, and for all Resource Pools.

<ol> 
 <li value="1"> Click the Main Menu icon in the upper-right corner of Workfront, then click Setup . </li> 
 <li value="2"> Click <span class="bold">Resource Management</span>. </li> 
 <li value="3"> Select one of the following methods to calculate the availability of users in <span>Workfront</span>: 
  <ul>
   <li><p><span class="bold">The Default Schedule</span>: <span>Workfront</span> uses the Default Schedule of the system and the individual FTE of the user to calculate the Available Hours of the user in resource management tools. <br>For more information about schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p><p>For more information about the value of the user FTE, see&nbsp;<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a><br>The Available Hours for the user are calculated by the following formula:<br><code>User Available Hours = (Default Schedule Hours - Time off hours) * User FTE value</code></p>
    <div class="example" data-mc-autonum="<b>Example: </b>">
     <span class="autonumber"><span><b>Example: </b></span></span>
     <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week, or 4 hours a day in a five-day week. </p>
     <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>
     <p><code>User Daily Available Hours = (4-1) * 0.5 = 3.5 Hours</code><br></p>
    </div></li>
   <li><p><span class="bold">The User's Schedule</span>: <span>Workfront</span> uses the user's schedule as well as the Default Schedule of the system to calculate the Available FTE value of the user in resource management tools. The Available Hours are calculated according only to the user's schedule. The value of the FTE of the user is ignored. This is the default setting.</p><note type="note">
     If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
    </note><p>The Available FTE for the user is calculated by the following formula:</p><p><code>User Available FTE =&nbsp;(Hours from the Schedule of the User - Time off hours) / Default Schedule Hours</code></p>
    <div class="example" data-mc-autonum="<b>Example: </b>">
     <span class="autonumber"><span><b>Example: </b></span></span>
     <p>For example, if the Default Schedule is 40 hours a week and the schedule of the user is 30 hours a week,&nbsp;the FTE of the user is 0.75.&nbsp;</p>
     <p>If the user has 2 hours of Time off one day, their Weekly Available FTE will be calculated as follows:</p>
     <p><code>User Weekly Available FTE = (30-2) / 40 = 0.70</code></p>
    </div></li>
  </ul></li> 
 <li value="4"> Click <span class="bold">Save</span>.<br></li> 
</ol>

