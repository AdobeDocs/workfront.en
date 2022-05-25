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

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **Linked to Creating Billing Record</p>
-->

You can associate hour types with your hour entries. Hour types are labels you use to define your hour entries. &nbsp;

There are two sets of hour types:

* **Project Specific Hour Types**: This is time logged on projects, tasks, and issues. Project-specific hour types can be associated with hour entries anywhere in Adobe Workfront where you can log time for projects, tasks, and issues.

  When logging time in Workfront, the project-specific hour types that are available depend on configuration options set at the system, project, and user levels.

  The following default project-specific hour types are always available:

   * Project Time
   * Task Time
   * Issue Time

  The Workfront administrator determines which project-specific hour types are made available, as described in [Define hour types and availability for timesheets](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >If you enable&nbsp;any project-specific hour types in your Workfront system, at least one project-specific hour type must be enabled on each project in your system. You cannot enable a project-specific hour type at the system level, and have no project-specific hour types available at the project level.

* **General Hour Types**: General hours cannot be associated with a project, task, or issue, and are logged directly into a timesheet. For more information about&nbsp;logging time, see [Log time](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Access requirements

You must have the following access to perform the steps in this article: 

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Built-in hour types

Workfront comes with a set of built-in hour types. These hour types cannot be edited and cannot be hidden.&nbsp;

The hour types that come with Workfront are:&nbsp;

* **Sick Time**: A&nbsp;general hour type that&nbsp;cannot be associated with hour entries on a project, task, or issue.
* **Vacation Time**: A&nbsp;general hour type that&nbsp;cannot be associated with hour entries on a project, task, or issue.
* **General Overhead**: A&nbsp;general hour type that&nbsp;cannot be associated with hour entries on a project, task, or issue. However, it can count as revenue in your project planning process.&nbsp;
* **Project Time**: A general hour type that can be associated only with hour entries on a project.
* **Task Time**: A general hour type that&nbsp;can be associated only with hour entries on&nbsp;a task.
* **Issue Time**:A general hour type that can be associated only with hour entries on&nbsp;an issue.&nbsp;

## Create hour types

As a Workfront administrator, you can create new hour types for your organization on both system and project levels. After you create hour types on the system and project levels, users can define which hour types are available for specific projects and users. For more information, see the [Define hour types and availability for timesheets](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

To create new hour types:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  

1. Click **Timesheet & Hours** > **Hour Types**.&nbsp;

1. Click**New Hour Type.**
1. Specify the following information on the **New Hour Type** form:

   <table> 
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
      <td> <p>Define whether the hour type is a general or project-specific hour type by selecting the correct scope in the drop-down menu.</p> <p>General hour types are visible only in timesheets and cannot be associated with projects, tasks, or issues.</p> <p><b>IMPORTANT</b>: If you have a custom Hour Type that is&nbsp;Project Specific, then you change it to&nbsp;General, all the existing Task, Issues and Project hours are set to their system default types.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Count As Revenue</td> 
      <td>Select this option if you want&nbsp;the hour entry associated with this hour type to affect your revenue calculations.</td> 
     </tr> 
    </tbody> 
   </table>

   **Count As Revenue**:Select this option if you want&nbsp;the hour entry associated with this hour type to affect your revenue calculations.&nbsp;

1. Click **Create Hour Type.**

## Deactivate hour types

If hour types become obsolete and you no longer want users to associate their hour entries with them, you can deactivate the hour types.&nbsp;

Deactivating hour types hides the hour types from anywhere in Workfront where hour types are visible.

To deactivate an hour type:

1. Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.  

1. Expand&nbsp;**Timesheet & Hours Preferences**, then click**Hour Types**.&nbsp;

1. Select the hour type you want to deactivate.
1. Click **Deactivate**.&nbsp;

