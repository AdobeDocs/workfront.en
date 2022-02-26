---
filename: hour-types
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Manage hour types
description: You can associate hour types with your hour entries. Hour types are labels you use to define your hour entries.
---

# Manage hour types

You can associate hour types with your hour entries. Hour types are labels you use to define your hour entries. &nbsp;

There are two sets of hour types:

<ul> 
 <li> <p><span class="bold">Project Specific Hour Types</span>: This is time logged on projects, tasks, and issues. Project-specific hour types can be associated with hour entries anywhere in <em>Adobe Workfront</em> where you can log time for projects, tasks, and issues.</p> <p>When logging time in <em>Workfront</em>, the project-specific hour types that are available depend on configuration options set at the system, project, and user levels.</p> <p>The following default project-specific hour types are always available: </p> 
  <ul> 
   <li> <p>Project Time</p> </li> 
   <li> <p>Task Time</p> </li> 
   <li> <p>Issue Time</p> </li> 
  </ul> <p>The <em>Workfront administrator</em> determines which project-specific hour types are made available, as described in <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability for timesheets</a>. </p> <note type="note">
   If you enable&nbsp;any project-specific hour types in your 
   <em>Workfront</em> system, at least one project-specific hour type must be enabled on each project in your system. You cannot enable a project-specific hour type at the system level, and have no project-specific hour types available at the project level.
  </note> </li> 
 <li><span class="bold">General Hour Types</span>: General hours cannot be associated with a project, task, or issue, and are logged directly into a timesheet. For more information about&nbsp;logging time, see <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Log time</a>.</li> 
</ul>

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Built-in hour types

*Workfront* comes with a set of built-in hour types. These hour types cannot be edited and cannot be hidden.&nbsp;

The hour types that come with *Workfront* are:&nbsp;

* `Sick Time`: A&nbsp;general hour type that&nbsp;cannot be associated with hour entries on a project, task, or issue.
* `Vacation Time`: A&nbsp;general hour type that&nbsp;cannot be associated with hour entries on a project, task, or issue.
* `General Overhead`: A&nbsp;general hour type that&nbsp;cannot be associated with hour entries on a project, task, or issue. However, it can count as revenue in your project planning process.&nbsp;
* `Project Time`: A general hour type that can be associated only with hour entries on a project.
* `Task Time`: A general hour type that&nbsp;can be associated only with hour entries on&nbsp;a task.
* `Issue Time`:A general hour type that can be associated only with hour entries on&nbsp;an issue.&nbsp;

## Create hour types

As a *Workfront administrator*, you can create new hour types for your organization on both system and project levels. After you create hour types on the system and project levels, users can define which hour types are available for specific projects and users. For more information, see the [Define hour types and availability for timesheets](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

To create new hour types:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2">Click <span class="bold">Timesheet & Hours</span> > <span class="bold"> Hour Types</span>.&nbsp;</li> 
 <li value="3">Click<span class="bold"> New Hour Type.</span></li> 
 <li value="4"> <p>Specify the following information on the <span class="bold">New Hour Type</span> form:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Name</td> 
     <td>Give your new hour type a name which is easily recognizable in the system.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Description</td> 
     <td>Add a description for your hour type.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Scope</td> 
     <td> <p>Define whether the hour type is a general or project-specific hour type by selecting the correct scope in the drop-down menu.</p> <p>General hour types are visible only in timesheets and cannot be associated with projects, tasks, or issues.</p> <note type="important">
       If you have a custom Hour Type that is&nbsp;Project Specific, then you change it to&nbsp;General, all the existing Task, Issues and Project hours are set to their system default types.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Count As Revenue</td> 
     <td>Select this option if you want&nbsp;the hour entry associated with this hour type to affect your revenue calculations.</td> 
    </tr> 
   </tbody> 
  </table> <p><span class="bold">Count As Revenue</span>:Select this option if you want&nbsp;the hour entry associated with this hour type to affect your revenue calculations.&nbsp;</p> </li> 
 <li value="5">Click <span class="bold">Create Hour Type.</span></li> 
</ol>

## Deactivate hour types

If hour types become obsolete and you no longer want users to associate their hour entries with them, you can deactivate the hour types.&nbsp;

Deactivating hour types hides the hour types from anywhere in *Workfront* where hour types are visible.

To deactivate an hour type:

1. Click `Setup` near the upper-right corner of *Adobe Workfront* on the Global Navigation Bar.  

1. Expand  `Timesheet & Hours Preferences`, then click `Hour Types`.&nbsp;

1. Select the hour type you want to deactivate.
1. Click `Deactivate`.&nbsp;

