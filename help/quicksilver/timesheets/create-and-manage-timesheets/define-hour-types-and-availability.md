---
filename: define-hour-types-and-availability
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Define hour types and availability for timesheets
description: There are two sets of hour types in Adobe Workfront:
---

# Define hour types and availability for timesheets

There are two sets of hour types in Adobe Workfront:

* **General hours:** Hours that are not associated with a project, such as sick time or administration. You can log general hours only on the timesheet.
* **Project-specific hours:** Hours logged on projects, tasks, and issues. You can log project-specific hours from any&nbsp;locations where you can log time.

When logging&nbsp;time in Workfront, the project-specific hour types that are available depend on configuration options set at the system, project, and user levels. (The following default project-specific hour types are always available: Project Time, Task Time, and Issue Time.)

An Hour Type is a label that allows you&nbsp;to categorize time entry. Depending on the reporting requirements of your organization for hours, this can&nbsp;be an essential part of logging time.

The hour types that are available to select when logging time (on projects, tasks, and issues) are determined first by the hour types made available system-wide by the system administrator, and then by the hour types&nbsp;selected at the project and user levels.

After the appropriate hour types have been configured, you can log time from multiple locations in Workfront, as described in [Log time](../../timesheets/create-and-manage-timesheets/log-time.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
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

The system administrator determines which project-specific hour types are made available system-wide, as described in&nbsp;the [Manage hour types](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md) section in&nbsp; [Manage hour types](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Define availability&nbsp;at the project level

The project owner determines whether all hour types defined at the system level are available on the project (and tasks and issues within the project), or whether only a subset of those hour types are available.&nbsp;

1. Go to the project where you want to determine the&nbsp;availability of&nbsp;hour types.
1. More
1. Edit
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

If you make an hour type available at the user level as described in this section, but you do not see that hour type when logging time on a project, task, or issue, that hour type has not been made available on the project (as described in [Define availability at the project level](#defining-availability-at-the-project-level)).

To define the hour types that are available to a user:

1. Main Menu
1. 
1. More
1. Edit
1. Only a system administrator can edit other users. If you have a Plan license, you can edit the hour types on your own profile.
1. In the **Resource Planning** section, in the **Available Hour Types** drop-down menu, do either of the following, depending on which hour types you want to make available when logging time on a project, task, or issue:

  * **To make all hour types available for the user:**&nbsp;Select all the hour types.  
    If you leave all hour types unselected, this is technically the same as selecting all hour types. However, in this case, all hour type are available for the user only on projects, tasks, and&nbsp;issues where&nbsp;**No** is selected in the **Filter Hour Types** option when editing the project, as described in [Define availability at the project level](#defining-availability-at-the-project-level).
  * **To make only a subset of the hour types available for the user:** Select only the hour types you want to make available.

    In order for the hour types you select at the user level to be available on projects, tasks, and issues, these same hour types must also be selected&nbsp;in the **Filter Hour Types** option when editing the project, as described in [Define availability at the project level](#defining-availability-at-the-project-level).

1. Click **Save Changes**.

   Now when you log hours on a project, task, or issue, the hour types you select are available if those same hour types have been made available at the project level.

