---
filename: create-schedules
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Create a schedule
description: As an Adobe Workfront administrator, you can define your work week by using schedules. You can associate a schedule with a user or a project. This allows Workfront to calculate timelines and user availability.
---

# Create a schedule

As an `Adobe Workfront administrator`, you can define your work week by using schedules. You can associate a schedule with a user or a project. This allows `Workfront` to calculate timelines and user availability.

For information about associating schedules with users and projects, see the following articles:

* [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) 
* [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md)

`Group administrators` can also create schedules that are associated with the groups they manage. For more information, see [Create and modify a group’s schedules](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

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
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Create a schedule

<ol> 
 <li value="1"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</p> </li> 
 <li value="2">Click<span class="bold"> Schedules</span>.</li> 
 <li value="3">Click<span class="bold"> New Schedule</span>.</li> 
 <li value="4">Specify a name for the schedule.</li> 
 <li value="5"> <p>(Optional) Select <span class="bold">Default Schedule</span> to identify this schedule as your default.</p> <p>You can have more than one schedule in <span>Workfront</span>, but you can only have one default schedule.</p> <p>You must have at least one schedule in <span>Workfront</span>. If you only have one, that is designated as the default schedule.</p> <note type="note">
    You cannot designate a schedule as the default schedule if you are a group administrator. Only a 
   <span>Workfront administrator</span> can designate a schedule as the default for the system.
   <br>
  </note> <p> <img src="assets/new-schedule-350x174.png" style="width: 350;height: 174;"> </p> </li> 
 <li value="6"> <p>In the <span class="bold">Schedule</span> tab, select a daily schedule by dragging the blue outline across hour blocks to highlight them.</p> <p>We recommend that you select 8 one-hour blocks over a 9 hour period of time. This accommodates for lunch or other breaks.<br></p> <p> <img src="assets/new-schedule-with-exceptions-350x167.png" style="width: 350;height: 167;"> <br> </p> </li> 
 <li value="7">On the <span class="bold">Details</span> tab, specify the following information: 
  <ul>
   <li><p><span class="bold">Group with Administration Access</span>: Indicate the group whose Group Administrators have the permission to edit this schedule. </p><note type="important">
     <ul>
      <li><p>If you are a <span>group administrator</span> creating a schedule, this field is mandatory.</p><p>A <span>group administrator</span> can create a schedule only if it is designated for a group or subgroup for which they are designated as the administrator.</p><p>If you manage only one group, that group is selected in this field, by default. </p><p>If you manage several groups, you must select a group in this field before you can save the schedule.<br></p></li>
      <li><p>If you are a <span>Workfront administrator</span> creating a schedule, this field is optional. When you create a schedule without associating it with a group, it is saved as a system-level schedule and cannot be managed by a <span>group administrator</span> of any group.</p><p>Schedules assigned to accounts or projects are visible to all users who can edit these objects. This is true for both system-level and group-level schedules.<br></p></li>
     </ul>
    </note><p>Specifying a <span class="bold">Group with Administration Access</span> for a schedule does not assign the schedule to the users in the group. Specifying a <span class="bold">Group with Administration Access</span> only allows the Group Administrators in the group to edit, delete, and copy the schedule.<br>Group Administrators cannot edit, delete, or copy system-level schedules. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p></li>
   <li>Select the <span class="bold">Groups with View Access</span> to which this schedule is visible to.<br>Only the users in the groups specified here can find the schedule in the drop-down menu when they are assigning it to users or projects. </li>
   <li>Select the <span class="bold">Time Zone</span> for your schedule. </li>
  </ul></li> 
 <li value="8"> <p>On the <span class="bold">Exceptions</span> tab, specify the exceptions to the schedule. </p> <p>Exceptions are full or half days which need to be excluded from the schedule, such as holidays or company events. </p> <note type="note">
   If you already know what your recurring schedule exceptions are, you can define your schedule exceptions for many years in the future.
  </note> <p>Full or partial days can be excluded from the work schedule. Click the date to select it as an exception, then select the <span class="bold">All day</span> field to indicate whether the exception is a full day or not.</p> <p> <img src="assets/schedule-adding-an-all-day-exception-350x177.png" style="width: 350;height: 177;"> <br> </p> </li> 
 <li value="9"> <p>Specify the start and end time for the partial day exceptions.</p> <p> <img src="assets/partial-day-exception-on-schedules-350x285.png" alt="partial_day_exception_on_schedules.png" style="width: 350;height: 285;"> </p> </li> 
 <li value="10">Click <span class="bold">Save</span>, then click <span class="bold">Save Changes</span>.</li> 
 <li value="11"> <p>(Optional) Associate the schedule with a user.</p> <p>For information, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
 <li value="12"> <p>(Optional)&nbsp;Associate the schedule with a project.</p> <p>For information, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li> 
</ol>

##  

