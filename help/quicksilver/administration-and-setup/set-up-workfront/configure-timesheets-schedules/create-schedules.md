---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Create a schedule
description: You can define your users' work weeks by using schedules. You can associate a schedule with a user or a project. This allows [!DNL Workfront] to calculate timelines and user availability.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
---
# Create a schedule

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

As an [!DNL Adobe Workfront] administrator, you can define your work week by using schedules. You can associate a schedule with a user or a project. This allows [!DNL Workfront] to calculate timelines and user availability.

When you have users that work in different timezones, creating a schedule in each of the timezones and associating it with those users ensures that their work is recorded in [!DNL Workfront] in real time and that their availability is always accurate according to when they work.

For information about associating schedules with users and projects, see the following articles:

* [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
* [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md)

Group administrators can also create schedules that are associated with the groups they manage. For more information, see [Create and modify a group's schedules](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

For information about using schedules to help users collaborate in [!DNL Workfront] across time zones, see [Working across time zones](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

For information about how schedules are used in resource planning, see [Schedules overview](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) and [Resource Planner overview](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a [!DNL Workfront] administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Create a schedule

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe] Workfront, then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Click **[!UICONTROL Schedules]**.
1. Click **[!UICONTROL New Schedule]**.
1. Specify a name for the schedule.
1. (Optional) Select **[!UICONTROL Default Schedule]** to identify this schedule as your default.

   You can have more than one schedule in [!DNL Workfront], but you can only have one default schedule.

   You must have at least one schedule in [!DNL Workfront]. If you only have one, that is designated as the default schedule.

   >[!NOTE]
   >
   >You cannot designate a schedule as the default schedule if you are a group administrator. Only a [!DNL Workfront] administrator can designate a schedule as the default for the system.

   ![](assets/new-schedule.png)

1. In the **[!UICONTROL Schedule]** tab, select a daily schedule by dragging the blue outline across hour blocks to highlight them.

   We recommend that you select 8 one-hour blocks over a 9 hour period of time. This accommodates for lunch or other breaks.

   ![](assets/new-schedule-with-exceptions.png)

1. On the **[!UICONTROL Details]** tab, specify the following information:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Group with Administration Access]</td>
     <td><p>Indicate the group whose administrators have the permission to edit this schedule.</p>
     <p><b>IMPORTANT</b>:</p>
      <ul>
       <li>
       <p>If you are a group administrator creating a schedule, this field is mandatory.</p>
       <p>As a group administrator, you can create a schedule only if it is designated for a group or subgroup for which you are designated as the administrator.</p>
       <p>If you manage only one group, that group is selected in this field, by default.</p>
       <p>If you manage several groups, you must select a group in this field before you can save the schedule.</p></li>
       <li>If you are a [!DNL Workfront] administrator creating a schedule, this field is optional. When you create a schedule without associating it with a group, it is saved as a system-level schedule and cannot be managed by a group administrator of any group.
       <p>Schedules assigned to accounts or projects are visible to all users who can edit these objects. This is true for both system-level and group-level schedules.</p>
       </li>
       <p>Specifying a Group with Administration Access for a schedule does not assign the schedule to the users in the group; it only allows the group administrators in the group to edit, delete, and copy the schedule.</p>
       <p>Group Administrators cannot edit, delete, or copy system-level schedules. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Groups with View Access]</td>
     <td><p>Select the groups with [!UICONTROL View] access which this schedule is visible to.</p>
     <p>Only the users in the groups specified here can find the schedule in the drop-down menu when they are assigning it to users or projects.</p></tr>
    <tr>
     <td>[!UICONTROL Time Zone]</td>
     <td><p>Select the time zone for your schedule.</p>
     <p>If you associate the schedule with a user, we recommend that the Time Zone of the schedule matches that of the user.For information about user's time zones, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile.
     </td>
    </tr>
   </table>


1. On the **[!UICONTROL Exceptions]** tab, specify the exceptions to the schedule.

   Exceptions are full or half days which need to be excluded from the schedule, such as holidays or company events.

   >[!NOTE]
   >
   >If you already know what your recurring schedule exceptions are, you can define your schedule exceptions for many years in the future.

   Full or partial days can be excluded from the work schedule. Click the date to select it as an exception, then select the **[!UICONTROL All day]** field to indicate whether the exception is a full day or not.

   ![](assets/schedule-adding-an-all-day-exception.png)

1. Specify the start and end time for the partial day exceptions.

   ![partial-day-exception-on-schedules.png](assets/partial-day-exception-on-schedules.png)

1. Click **[!UICONTROL Save]**, then click **[!UICONTROL Save] Changes**.

1. (Optional) Associate the schedule with a user.

   For information, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Optional) Associate the schedule with a project.

   For information, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).
