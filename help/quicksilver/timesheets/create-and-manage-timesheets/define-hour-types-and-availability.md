---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Define hour types and availability for timesheets
description: An Hour Type is a label that allows you to categorize time entry. Depending on the reporting requirements of your organization for hours, this can be an essential part of logging time.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
---
# Define hour types and availability for timesheets

An Hour Type is a label that allows you to categorize time entry. Depending on the reporting requirements of your organization for hours, this can be an essential part of logging time.

There are two sets of hour types in Adobe Workfront:

* **General hours:** Hours that are not associated with a project, such as sick time or administration. You can log general hours only on the timesheet.
* **Project-specific hours:** Hours logged on projects, tasks, and issues. You can log project-specific hours from any locations where you can log time.

When logging time in Workfront, the project-specific hour types that are available depend on configuration options set at the system, project, and user levels. (The following default project-specific hour types are always available: Project Time, Task Time, and Issue Time.)

The hour types that are available to select when logging time (on projects, tasks, and issues) are determined first by the hour types made available system-wide by the system administrator, and then by the hour types&nbsp;selected at the project and user levels.

After the appropriate hour types have been configured, you can log time from multiple locations in Workfront, as described in [Log time](../../timesheets/create-and-manage-timesheets/log-time.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>System administrator access to define system-wide hour types and to edit all users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>Manage access on the project to define hour types on a project</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your Workfront administrator.

## Define availability&nbsp;at the system level

The system administrator determines which project-specific hour types are made available system-wide, as described in the [Manage hour types](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md). 

## Define availability&nbsp;at the project level {#define-availability-at-the-project-level}

The project owner determines whether all hour types defined at the system level are available on the project (and tasks and issues within the project), or whether only a subset of those hour types are available.&nbsp;

1. Go to the project where you want to determine the&nbsp;availability of&nbsp;hour types.
1. Click the **More** menu next to the task name, then click **Edit**.

1. Click **Edit Project**.
1. In the **Settings** section, locate the **Filter Hour Types** option.  

1. Select **No**&nbsp;to make all project-specific hour types available on the project.

   Or

   Select **Yes** to make only a subset of the project-specific hour types available on the project,&nbsp;then select the hour types you want to make available. (Hold the Shift key to select multiple hour types.)

   If you select this option, only the hour types you select are made available to select when logging hours on the project (or on tasks and issues within the project). If you select this option and you do not&nbsp;select any hour types, the project displays only general hour types.

   The same selections must be made at the individual user level in order for the user to see these hour type options on the project.

1. Click **Save Changes**.

## Define availability&nbsp;at&nbsp;the&nbsp;user level

You can log hours for a given hour type on projects, tasks, and issues only if that hour type has been made available at the system level, at the project level, and at the user level.

If you make an hour type available at the user level as described in this section, but you do not see that hour type when logging time on a project, task, or issue, that hour type has not been made available on the project (as described in [Define availability at the project level](#define-availability-at-the-project-level)).

To define the hour types that are available to a user:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Click your user avatar in the upper-left corner.
1. Click the **More** menu next to the user name, then click **Edit**.

1. Only a system administrator can edit other users. If you have a Plan license, you can edit the hour types on your own profile.
1. In the **Resource Planning** section, in the **Available Hour Types** drop-down menu, do either of the following, depending on which hour types you want to make available when logging time on a project, task, or issue:

   * **To make all hour types available for the user:**&nbsp;Select all the hour types.  
     If you leave all hour types unselected, this is technically the same as selecting all hour types. However, in this case, all hour type are available for the user only on projects, tasks, and&nbsp;issues where&nbsp;**No** is selected in the **Filter Hour Types** option when editing the project, as described in [Define availability at the project level](#define-availability-at-the-project-level).
   * **To make only a subset of the hour types available for the user:** Select only the hour types you want to make available.

     In order for the hour types you select at the user level to be available on projects, tasks, and issues, these same hour types must also be selected&nbsp;in the **Filter Hour Types** option when editing the project, as described in [Define availability at the project level](#define-availability-at-the-project-level).

1. Click **Save Changes**.

   Now when you log hours on a project, task, or issue, the hour types you select are available if those same hour types have been made available at the project level.


## How user-level and project-level hour types work together

The following list describes what hour types display on an object after you have customized and filtered both the user-level and the project-level hour types: 

* By default, when you open an object to log time, the Hour Type drop-down menu displays the Default Hour Types associated with your user. This happens when you did not customize your hour types. 

* After you customize Hour Types and define Available Hour Types for your user or filter the Hour Types for a project, the following scenarios exist: 

   * If you selected all the hour types for the Available Hour Type field in your user's profile, and the project's Hour Types are not filtered, you will see all available hour types when you log time. 
   * If you selected only a subset of hour types for the Available Hour Type field in your user's profile, and the project's Hour Types are not filtered, you will see only the user's hour types when you log time.
   * If you selected all the hour types for the Available Hour Type field in your user's profile, and the project's Hour Types are filtered, you will see only the project's hour types and the default hour types like Project Time, Task Time, Issue Time depending on the object. 
   * If If you selected only a subset of hour types for the Available Hour Type field in your user's profile, and and the project's Hour Types are filtered, you will see only the hour types that are common to the user and the project. If no hour types are common to the user and the project, only the default hour types display (Project Time, Task Time, Issue Time). 

>[!TIP]
>
>   If you select a different Hour Type rather than the default hour type for an object, the hour type becomes sticky. Next time you log time on the same object, the Hour Type will automatically default to the one you last selected. 
    
