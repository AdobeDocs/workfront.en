---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Edit User Profiles in Bulk
description: As an Adobe Workfront administrator, you can edit user accounts in bulk.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
---
# Edit user profiles in bulk

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

You can edit user accounts in bulk. When bulk editing users, only the fields you specifically select are updated with the same information for all users selected. All other fields that you leave unselected stay the same for each individual user, even if they are different for each user.

>[!NOTE]
>
>* You cannot bulk edit the Personal Info section of the users' profiles because that information must be unique for every user.
>* To ensure accuracy of data and optimal performance, we recommend that you select no more than 2000 users at one time for a bulk edit.
>

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p><p>Or</p><p>Current: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level. </li> 
     <li> <p><b>Users</b> setting in your access level configured to <b>Edit</b> access, with <b>Create</b> and at least one of the two <b>User Admin</b> options enabled under <b>Fine-tune your settings</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Of these two options, if <b>User Admin (Group Users)</b> is enabled, you must be a group administrator of a group where the user is a member.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Edit user accounts in bulk

{{step-1-to-users}}

1. Select more than one user, then click the **Edit** icon ![Edit icon](assets/edit-icon.png).

1. In the **Edit User** box, change the information in any of the sections, and click **Save Changes** <span class="preview">or **Save**</span> at any time.

### Preferences

* **Time Zone**: The user's time zone.

  For information about helping users collaborate in Workfront across time zones, see [Working across time zones](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

* **Email Locale**: The user's preferred email locale. This affects the format of numbers and dates in the emails that come from Workfront to this user.

  >[!NOTE]
  >
  >When your organization is on the Adobe Unified Experience, the user's language preferences are stored in their Adobe profile and the email locale is not used. For information about accessing these preferences, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

### Notifications

Select the email notifications that should be enabled for the users.

You can select instant as well as daily digest notifications. All of the daily digest notifications are delivered sometime after the same time for all the users you selected.

For more information, see [Configure event notifications for everyone in the system](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

### Access

* **Is Active** / <span class="preview">**User is active**</span>: Enable this option to indicate that the users are active. Active users use a Workfront license. Disabling the field deactivates the users and prevents them from logging in to Workfront.

* **Access Level**: Select the access level to assign to these users. All users you selected will have the same access level.

  When you assign an access level to users, you can assign a level equal to or lower than your own access level. (For example, if your access level is Standard, you cannot assign the Administrator access level.)
  
  However, you cannot assign an access level that by default is lower than your own access level if the Workfront administrator has enabled non-default permissions on the access level that are not also enabled in your own access level.

  For example, if you have a Standard license with no access to delete tasks, you cannot assign someone a Light license with access to delete tasks, although the Light license is lower than the Standard license. For more information, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  For more information about access levels, see [Configure access to Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  >[!NOTE]
  >
  >If your organization uses the new access model (Standard/Light/Contributor), you cannot reassign a Standard or Light user to a Contributor access level if that user has already reached their decision limit for the month.
  >
  >For more information on the new access model, see [New access levels overview](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).
  >
  >For information on decision limits, see [Limited document and proof decision for non-paid users overview](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

* **Layout Template**: Choose a layout template for the users. this layout template takes precedence over any layout template assigned to their Home Group, Home Team, or Primary Role. For more information about the assignment priority of layout templates, see [Create and manage layout templates](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

  The following list describes how the list of templates you have available in this field depends on your access:

  * As a Workfront administrator, you can see all system-level and group-level layout templates.
  * As a group administrator, you can see system-level layout template, as well as those associated with the groups that you manage.
  * As a user with a Standard or Plan license and access to edit users, you can see only system-level layout templates.
  
    For more information about group-level layout templates, see [Create and modify a group's layout templates](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

### Organization

* **Company**: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see [Create and edit companies](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* **Home Team**: Specify the home team for the users. Users can only have one home team.
* **Other Teams**: Users can belong to multiple teams.
* **Home Group** / <span class="preview">**Current Home Group**</span>: Select an appropriate group to assign the users. This gives the users the ability to access objects that are shared with the group. You can also share layout templates with the a Home Group.

  This is a required field. Every user must be associated with a home group. If you don't select one, your Home Group is assigned as the Home Group.

  You can assign a group to a user only if one of the following is true:

  * you are a Workfront administrator
  * you are the administrator of the group
  * the group is public

* **Other Groups**: Users can belong to multiple groups. You can assign a group to a user only if you are a Workfront administrator, you are the administrator of the group, or the group is public.

  >[!IMPORTANT]
  >
  >Adding a user to more than 100 groups may cause performance issues in any area of Workfront that loads the list of groups.

  For more information about public groups, see [Create a group](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

  For more information about groups, see [Groups overview](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md).

### Resource Planning

* **Work Time**: Represents the percentage of the Full Time Equivalent (FTE) time that the users are available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

  The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work.

  The system uses this number to calculate the availability of the user for actual, project-related work.

  For more information about creating schedules in Workfront, see [Create a schedule](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  Schedule exceptions and time off might also affect the user's capacity.

  Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see [Configure Resource Management preferences](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  >[!TIP]
  >
  >Set the Work Time value to 1 to indicate that the user is available for project-related work their entire full-time equivalent.

* **Schedule Deactivation** / <span class="preview">**Set deactivation date**</span>: Check this box / <span class="preview">click this button</span> if you want to schedule these users to be deactivated on a certain date and at a certain time.
* **Scheduled Deactivation Date** / <span class="preview">**Deactivation Date**</span>: The date and time on which the users become deactivated. For information about scheduling users for deactivation, see [Schedule users for deactivation](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation) in [Deactivate or reactivate a user](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
* **Primary Role**: This is the primary job role that the users can fulfill in Workfront. Every task and issue that the users are assigned to is also assigned to this job role. Job roles are essential in resource management. You can update this field only if you have a Standard or Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see [Grant access to users](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

  Only active job roles display in the list.

* (Conditional) If you selected a **Primary Role**, the **Percentage of FTE Availability** field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.
* **Other Roles**: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.

  Only active job roles display in the list. For more information about job roles, see [Create and manage job roles](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

  You can update this field only if you have a Standard or Plan license with administrative user access, or if you are a Workfront administrator.

  For more information about setting up users with administrative user access, see [Grant access to users](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

* (Conditional) If you selected one or multiple **Other Roles**, the **Percentage of FTE Availability** field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.

  If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.

  The sum of all **Percentages of FTE Availability** for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.

  The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.

  For information about calculating availability for the user, see [Overview of calculating hours and FTE for users and roles in the Resource Planner](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

  For information about configuring Resource Management preferences, see [Configure Resource Management preferences](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Schedule**: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.

  You must create a schedule before you can associate it with users. For more information about creating schedules, see [Create a schedule](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  >[!IMPORTANT]
  >
  >Workfront uses the schedule of a user only when the **Calculate Resource Availability Using** setting is set to **The User's Schedule**. For information about how this setting affects which schedule is used for Resource Management, see [Configure Resource Management preferences](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Timesheet Profile**: Associate a Timesheet Profile with the users to ensure that timesheets generate automatically.

  The list of profiles you have available in this field depends on your access:

  * As a Workfront administrator, you can see all system-level and all group-level Timesheet Profiles.
  * As a group administrator, you can see system-level Timesheet Profiles, as well as those associated with the groups that you manage.
  * As a user with a Standard or Plan license and access to edit users, you can see only system-level Timesheet Profiles. For more information about group-level Timesheet Profiles, see [Create, edit, and assign timesheet profiles](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Default Hour Type**: Select the default hour type for the users. This is the hour type that is used by default when the users log time.
* **Available Hour Types**: Select the hour types that should be available to the users. These hour types are visible everywhere in Workfront where the users can log time. Users can only see the hour types that are enabled at the project level as well as the user level. For more information about what hour types are available to users, see [Define hour types and availability](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
* **FTE**: This is the Full Time Equivalent of the users. Workfront uses this number to calculate the availability of the users based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule.

  The FTE indicates the amount of time that the users can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.

  The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the users are available for 20 hours a week.

  The field's default is 1.

  Schedule exceptions, time off, and the value of Work Time may affect the availability of the users.

  Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

  If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule.

  For more information, see [Configure Resource Management preferences](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  For more information about creating schedules in Workfront, see [Create a schedule](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Resource Pools**: Associate the users with Resource Pools.

  >[!NOTE]
  >
  >Only the resource pools that are common to all the users selected appear in this field. If the users you selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.

  For more information about resource pools, see [Associate resource pools with users](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

* **Cost Rate**: The amount of cost per hour for the user.

  For date effective cost rates, click **Add Rate**. Enter the value of the cost rate for the time period, and assign a Start Date and End Date as needed. Cost Rate 1 will not have a start date and the last cost rate will not have an end date.

  Some dates are added automatically. For example, if Cost Rate 1 does not have an end date, and you add Cost Rate 2 with a start date of May 1, 2023, an end date of April 30, 2023 is added to Cost Rate 1 so that no gaps exist.

* **Billing Rate**: The amount of billing per hour for the user.

  For date effective billing rates, click **Add Rate**. Enter the value of the billing rate for the time period, and assign a Start Date and End Date as needed. Billing Rate 1 will not have a start date and the last billing rate will not have an end date.

  Some dates are added automatically. For example, if Billing Rate 1 does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to Billing Rate 1 so that no gaps exist.

### Custom Forms

Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. Fields you do not have access to edit are not displayed in an individual custom form.

>[!NOTE]
>
>Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the user record on the details page, not on the Edit User dialog. (From the list of users, click the user name to open the details.)

You can optionally select the **Recalculate Custom Expressions** option to ensure that all calculated custom fields in custom forms that are attached to the selected users are up to date.

For information about creating custom forms, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Comment

Type the comment you want to send to the users and to the Updates area of their user profiles.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferences</td> 
      <td> 
       <ul> 
        <li><b>Time Zone:</b> The users' time zone.</li> 
        <li><b>Locale</b>: The users' preferred locale. This affects the format of numbers and dates in the emails that come from Workfront.</li> 
        <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Select the email notifications which should be enabled for the new user.<p>You can select instant as well as daily digest notifications. All the daily digest notifications are delivered sometime after the same time for all the users selected. For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
        <li><b>Is Active:</b> Select this field to indicate whether the users are active. Active users use a Workfront license. Deselecting the field deactivates the users.</li> 
        <li> 
        <p><b>Access Level:</b> Select the access level to assign to these users. All users selected will have the same access level.
        </p> 
        <p>When you assign an access level to users, you can assign a level equal to or less than your own access level. (For example, if your access level is Planner, you cannot assign the Administrator access level.) </p>
        <p>However, you cannot assign an access level that is lower than your own if the Workfront administrator has enabled permissions on the access level that are not also enabled in your own (via the Fine-Tune settings, as described in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>).</p> 
        <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Template</b>: Choose a layout template for the users. The layout template assigned to the users will take precedence over any layout template assigned to their Home Group, Home Team or primary job role. For more information about the assignment priority of layout template, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> 
        <p><b>NOTE</b>:  The list of layout templates you have available in this field depends on your access:
          <ul>
           <li>As a Workfront administrator, you can see all system-level and group-level layout templates.</li>
           <li>As a group administrator, you can see system-level layout templates, as well as those associated with the groups that you manage.</li>
           <li><p>As a user with a Planner license and access to edit users, you can see only system-level layout templates. </p>
           <p>For information about group-level layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization</td> 
      <td> 
       <ul> 
        <li><b>Company</b>: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see Understanding and Managing Companies.</li> 
        <li><b>Home Team</b>: Specify the home team for the users. Users can only have one home team. </li> 
        <li><b>Other Teams</b>: Users can belong to multiple teams. </li> 
        <li> <p><b>Home Group:</b> Select an appropriate group to assign the users as their Home Group. This gives the user the ability to access objects that are shared with the group.</p> <p><b>NOTE</b>:  This is a required field. You cannot have users not associated with a Home Group.</p> <p>You can assign a group to users only in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li>The group is public.</li> 
         </ul> </li> 
        <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only  in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li> <p>The group is public. </p> 
          <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> 
          <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning</td> 
      <td> 
       <ul> 
      
      <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work. 

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 

      <li><b>Schedule Deactivation</b>: Check this box if you want to schedule users to be deactivated after a period of time.</li> 
       <li><b>Scheduled Deactivation Date</b>: The date after which the users become deactivated. For more information about scheduling users for deactivation, see the section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that a user has in Workfront. Every task and issue that the users are assigned to is also assigned to this job role, by default. Job roles are essential in resource management. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a></p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li>(Conditional) If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.</li> 
       <li> <p><b>Other Roles</b>: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.</p> <p>For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</li> 
       <li> <p>The sum of all Percentages of FTE Availability for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For more information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For more information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schedule</b>: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.</p> <p>A Workfront administrator or a group administrator must create a schedule before it can be associated with users.</p> <p>Select a system-level or a group schedule to assign it to the selected users.</p> <p>For more information about system-level and group schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>IMPORTANT</b>: Workfront uses the schedule of a user only when the Calculate Resource Availability Using setting is set to The User's Schedule. For information about how the Calculate Resource Availability Using setting affects which schedule is used for Resource Management, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the users. This ensures that timesheets generate automatically for the users.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>The list of timesheet profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and group-level timesheet profiles.</li>
       <li><p>As a group administrator, you can see system-level timesheet profiles, as well as those associated with the groups that you manage.</p></li>
       <li><p>As a user with a Planner license and access to edit users, you can see only system-level timesheet profiles.</p></li>
       </ul></li> 
       <li>If you are a group administrator, all of the users you are editing must be members of a group that you administer.</li> 
       </ul> </p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the users. This is the hour type that is used by default when the users log time.</li> 
       <li> <p><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the users can log time. A user can only see the hour types that are enabled at the project level as well as the user level.</p> 
       <p>For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</p> 
       </li> 
       <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
       <li> <p><b>Resource Pools</b>: Associate the users with resource pools.</p> <p><b>NOTE</b>:  Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.</p> 
       <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> </li> 
       <li><b>Cost Per Hour</b>: The amount of cost per hour for the user. </li> 
       <li><b>Billing Per Hour</b>: The amount of billing per hour for the user.</li> 
       <li><b>Custom Forms</b>: Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</li> 
       <li><b>Comment</b>: Enter a comment in the field provided. All users selected will receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates tab of the users' profile.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
-->

