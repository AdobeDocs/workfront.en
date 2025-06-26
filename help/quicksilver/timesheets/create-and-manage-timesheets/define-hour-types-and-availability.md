---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Define Hour Types and Availability
description: An Hour Type is a label that allows you to categorize time entry. Depending on the reporting requirements of your organization for hours, this can be an essential part of logging time.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
---
# Define hour types and availability

<!--Audited: 6/2025-->

An Hour Type is a label that allows you to categorize time entry. Depending on your organization's reporting requirements for hours, this can be an essential part of logging time.

There are 2 sets of hour types in Adobe Workfront:

* **General hours**: Hours that are not associated with a project, such as sick time or administration. You can only log general hours on the timesheet.
* **Project-specific hours**: Hours logged on projects, tasks, and issues. You can log project-specific hours from any location where you can log time.

When logging time in Workfront, the project-specific hour types that are available depend on configuration options set at the system, project, and user levels. (The following default project-specific hour types are always available: Project Time, Task Time, and Issue Time.)

The hour types that are available to select when logging time (on projects, tasks, and issues) are determined first by the hour types made available system-wide by the system administrator, and then by the hour types selected at the project and user levels.

After the appropriate hour types have been configured, you can log time from multiple locations in Workfront. For more information, see [Log time](../../timesheets/create-and-manage-timesheets/log-time.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard</p> 
   <p>Current: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator access to define system-wide hour types and to edit all users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>Manage access on the project to define hour types on a project</td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Define availability at the system level

The system administrator determines which project-specific hour types are made available system-wide. For more information, see [Manage hour types](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md). 

## Define availability at the project level {#define-availability-at-the-project-level}

The project owner determines whether all hour types defined at the system level are available on the project (and tasks and issues within the project), or whether only a subset of those hour types are available. 

{{step1-to-projects}}

1. On the **Projects** page, select the project you want to determine the availability of hour types for.
1. Click the **More** icon ![More icon](assets/more-icon.png) next to the project name in the header, then click **Edit**. The **Edit Project** panel opens. 

1. In the **Project Settings** section, locate the **Filter Hour Types** setting.  

1. Select **No** to make all project-specific hour types available on the project.

   Or

   Select **Yes** to make only a subset of the project-specific hour types available on the project, then select the **Hour Types** you want to make available. You can select multiple hour types.

   >[!NOTE]
   >
   >   Consider the following: 
   >   
   >   * If you select **Yes**, only the hour types you select are made available to select when logging hours on the project (or on tasks and issues within the project). 
   >   
   >   * If you select **Yes** and don't select any hour types, the project displays only general hour types.
   >
   >   * The same selections must be made at the individual user level in order for the user to see these hour type options on the project.
   >
   >   * When the user's Default Hour Type and a project Filtered Hour Type match, that hour type is selected by default when logging time. 

1. Click **Save**.

## Define availability at the user level

You can log hours for a given hour type on projects, tasks, and issues only if that hour type has been made available at the system level, project level, and user level.

If you make an hour type available at the user level as described in this section but don't see that hour type when logging time on a project, task, or issue, that hour type hasn't been made available on the project. For more information, see the following section in this article: [Define availability at the project level](#define-availability-at-the-project-level).

To define the hour types that are available to a user:

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click your user avatar in the upper-left corner.

   Or

   Click the **Main Menu** icon ![Main Menu icon](assets/adobe-main-menu.png) in the upper-right corner, if available, then click **Workfront Profile**.

1. Click the **More** icon ![More icon](assets/more-icon.png) next to the user name, then click **Edit**. The **Edit Person** box opens.

      >[!IMPORTANT]
      >
      >Only a system administrator can edit other users. If you have a Plan license, you can edit the hour types on your own profile.


1. In the **Resource Planning** section, in the **Available Hour Types** drop-down menu, do either of the following, depending on which hour types you want to make available when logging time on a project, task, or issue:

   * **To make all hour types available for the user:** Select all the hour types.  
     If you leave all hour types unselected, this is technically the same as selecting all hour types. However, in this case, all hour type are available for the user only on projects, tasks, and issues where **No** is selected in the **Filter Hour Types** option when editing the project, as described in [Define availability at the project level](#define-availability-at-the-project-level).
   * **To make only a subset of the hour types available for the user:** Select only the hour types you want to make available.

     In order for the hour types you select at the user level to be available on projects, tasks, and issues, these same hour types must also be selected in the **Filter Hour Types** option when editing the project, as described in [Define availability at the project level](#define-availability-at-the-project-level).

1. (Optional) In the **Default Hour Type** drop-down menu, select one hour type. When the user Default Hour Type and a project Filtered Hour Type match, that hour type is selected by default when logging time.

1. Click **Save Changes**. Now, when you log hours on a project, task, or issue, the hour types you select are available if those same hour types have been made available at the project level.

## How user-level and project-level hour types work together

The following list describes what hour types display on an object after you have customized and filtered both the user-level and the project-level hour types when you log time on the object: 

* After you customize the Default Hour Type for the user and the Filtered Project Hour Types, the Hour Type drop-down menu displays one of the following hour types:

   * When the user has a Default Hour Type  on their profile and the project has the same Filtered Hour Type, this Hour Type displays as the selected default when logging time; Project, Task, or Issue Time show as additional options. 

   * When the user doesn't have a Default Hour Type and the project has Filtered Hour Types, the default Hour Type when logging time are Project, Task, or Issue Time, but the filtered Hour Types from the project also displays as additional options.

   * When the user doesn't have a Default Hour Type and the project has no Filtered Hour Types, only the Project, Task, or Issue Time hour types display as defaults depending on the object you're logging time to. 

   * When the user has a Default Hour Type and the project has no Filtered Hour Types, the Project, Task, or Issue Time display as defaults when logging time on the objects, and no other Hour Types are available as options, including the user's Default Hour Type. 

* After you customize Hour Types and define Available Hour Types for your user or filter the Hour Types for a project, the following scenarios exist: 

   * When you selected all the hour types for the Available Hour Type field in your user's profile and the project's Hour Types aren't filtered, you'll see all available hour types when you log time. 
   * When you selected only a subset of hour types for the Available Hour Type field in your user's profile and the project's Hour Types aren't filtered, you'll see only the user's hour types when you log time.
   * When you selected all the hour types for the Available Hour Type field in your user's profile and the project's Hour Types are filtered, you'll see only the project's hour types and the default hour types like Project Time, Task Time, Issue Time depending on the object. 
   * When you selected only a subset of hour types for the Available Hour Type field in your user's profile and the project's Hour Types are filtered, you'll see only the hour types that are common to the user and the project. If no hour types are common to the user and the project, only the default hour types display (Project Time, Task Time, Issue Time). 

>[!TIP]
>
>   If you select a different Hour Type other than the default hour type for an object, the hour type becomes sticky. Next time you log time on the same object, the Hour Type will automatically default to the one you last selected. 
    
