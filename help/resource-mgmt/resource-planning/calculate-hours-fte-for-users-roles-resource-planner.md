---
filename: calculate-hours-fte-for-users-roles-resource-planner
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Overview of calculating hours and FTE for users and roles in the Resource Planner
description: You can display the allocation and availability of your resources in the Resource Planner by Hours, FTE, or Cost. For more information about calculating Costs in the Resource Planner, see Calculate costs in the Resource Planner .
---

# Overview of calculating hours and FTE for users and roles in the *Resource Planner*

You can display the allocation and availability of your resources in the *Resource Planner* by Hours, FTE, or Cost.  
For more information about calculating Costs in the *Resource Planner*, see [Calculate costs in the Resource Planner](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

"FTE" stands for Full Time Equivalent. It is a measure of time that represents the amount of hours dedicated to real work during a day or week for a user or job role.

The following sets of resource information are calculated differently in the *Resource Planner*:

* The Available Hours or FTE values are calculated based on the way your System Administrator configures the Resource Management preferences in your system.  
  For more information about how the Available Hours and FTE values are calculated, see [Calculate Available Hours or FTE for users and job roles in the Resource Planner](#calculating-available-hours).  
  For more information about defining the Resource Management preferences for the *Adobe Workfront* system, see [Configure Resource Management preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).  

* All other FTE values are calculated based on the System Default schedule.  
  For more information about how the all other values display in the *Resource Planner* when using FTE, see [Calculate all other hour and FTE values for users and job roles in the Resource Planner](#calculating-all-other-values).

It is important to understand what the FTE is for each of your users and their job roles to accurately manage your resources as you are assigning them to work.

## Calculate Available Hours or FTE for users and job roles in the *Resource Planner*

* [Calculate the Available Hours and FTE for a user in the Resource Planner](#user-availability) 
* [Calculate the Available Hours and FTE for a job role in the Resource Planner](#job-role-availability) 
* [Calculate the Available Hours and FTE for a user in the Resource Planner (Example)](#example)

### Calculate the Available Hours and FTE for a user in the *Resource Planner*

The *Workfront administrator* determines how the available time for a user is calculated by selecting to use one of the following in the Resource Management area in&nbsp;Setup:

* The Default Schedule of the system and the user's FTE. 
* The user's schedule.&nbsp;

For more information, see [Configure Resource Management preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><![CDATA[
]]><br></p>
<p> <draft-comment>
<img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
</draft-comment><img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p>
<p> Based on how this setting is configured, the availability of the users in the <em>Resource Planner</em> (hours as well as FTE availability) is calculated by using the following methods: </p>
<ul>
<li><span class="bold">The Default Schedule</span>: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user in the <em>Resource Planner</em>. The Schedule of the user is ignored. In this case:
<ul>
<li> The <span class="bold">Available Hours</span> in the<span class="bold"> <em>Resource Planner</em></span> are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE value</code><br>For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the <em>Resource Planner</em>.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a></li>
<li style="font-weight: normal;"> The <span class="bold">Available FTE</span> for the user in the<span class="bold"> <em>Resource Planner</em></span> is the same as the user FTE specified in the user settings. <br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the <em>Resource Planner</em>. For more information about the value of the user FTE as it displays in the user settings, see <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><span class="bold">The User's Schedule</span>: The Schedule of the user is used to determine the availability of the user in the <em>Resource Planner</em>. The value of the user FTE is ignored. In this case:
<ul>
<li> The <span class="bold">Available Hours</span> in the<span class="bold"> <em>Resource Planner</em></span> are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the <em>Resource Planner</em>. </li>
<li> The <span class="bold">Available FTE</span> in the<span class="bold"> <em>Resource Planner</em></span> is calculated by the following formula:<br><em><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in <em>Workfront</em> has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul></li>
</ul> <note type="note">
If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note>
</div>
-->

<![CDATA[ ]]>

![](assets/nwe-resource-management-system-setting-user's-schedule-350x157.png)

Based on how this setting is configured, the availability of the users in the *Resource Planner* (hours as well as FTE availability) is calculated by using the following methods:

* `The Default Schedule`: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user in the *Resource Planner*. The Schedule of the user is ignored. In this case:

  * The `Available Hours` in the ` *Resource Planner*` are calculated using the following formula:

    ```  
    User Available Hours = Default Schedule Hours * User FTE value
    ```

    For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the *Resource Planner*.  
    For more information about schedules, including the Default Schedule, see [Create a schedule](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
  
  * The `Available FTE` for the user in the ` *Resource Planner*` is the same as the user FTE specified in the user settings.   
    For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the *Resource Planner*. For more information about the value of the user FTE as it displays in the user settings, see [Edit a user's profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* `The User's Schedule`: The Schedule of the user is used to determine the availability of the user in the *Resource Planner*. The value of the user FTE is ignored. In this case:

  * The `Available Hours` in the ` *Resource Planner*` are the same as the Hours from the Schedule of the user.  
    For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the *Resource Planner*. 
  
  * The `Available FTE` in the ` *Resource Planner*` is calculated by the following formula:  
    * 
  
    ```  
    User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours
    ```

    *For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in *Workfront* has 40 hours available to work, the user's FTE is 0.5.  
    For more information about schedules, including the Default Schedule, see [Create a schedule](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

>[!NOTE]
>
>If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.

### Calculate the Available Hours and FTE for a job role in the *Resource Planner*

You first have to calculate the user availability, and then you can calculate the availability of each of their job roles.

The availability of job roles in the *Resource Planner* takes into account the total availability of the user, and the `Percentage of FTE Availability` associated with each role of the user.  
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

For more information about associating a `Percentage of FTE Availability` value with a job role for a user, see [Edit a user's profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

For example, if the value of Available Hours for a user is 40 and they can fulfill one Primary Role for 75% of that time, and one Other Role for 25% of that time, the *Resource Planner* shows that the `Available Hours` value for the Primary Role for one week is 30 hours, and that the `Available Hours` value for the Other Role is 10 hours. In this case, the FTE for the Primary Role is 0.75 and the FTE for the other role is 0.25.

>[!NOTE]
>
>The total available time for the user is calculated by one of the two methods described in the [Calculate the Available Hours and FTE for a user in the Resource Planner](#user-availability) section in this article.

When viewing the *Resource Planner* in the Role View, the availability of one job role is a total of the availability of all users who can fulfill that job role.  
For more information about availability of resources in the *Resource Planner*, see the [Resource Planner overview](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Calculate the Available Hours and FTE for a user in the *Resource Planner* (Example)

The following table illustrates how the Available Hours and Available FTE are calculated for the user in the *Resource Planner*, depending on which method is used by the system administrator for the FTE calculation in the Resource Management Preferences.

For this example, we are using the following numbers:

* A system Default Schedule of 40 hours 
* A user Schedule of 20 Hours 
* A user FTE of 0.75.

| Method for FTE Calculation (System Setting) | `Hours from User's Schedule`  | `Hours from the Default Schedule`  | `User FTE field`  | `Available Hours in the *Resource Planner*`  | `Available FTE in the *Resource Planner*`  |
|---|---|---|---|---|---|
| `The Default Schedule`  |Ignored |40 |0.75 | `30` (calculated) | `0.75`  |
| `The User's Schedule`  |20 |40 |Ignored | `20`  | `0.5` (calculated) |

## Calculate all other hour and FTE values for users and job roles in the *Resource Planner*

In addition to the Available Hours or FTE, the following time information is also displayed in the *Resource Planner*:

* Planned Hours
* Budgeted Hours
* Hour Variance
* Net Hours  
  For more information about these values see [Overview of hours, FTE, and cost information in the Project and Role views of the Resource Planner](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)  

* Hour Difference  
  For more information about what this value represents see [Overview of hours, FTE, and cost information in the Project and Role views of the Resource Planner](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

You can display the same information in the *Resource Planner* as FTE or as hours.

*Workfront* uses the following formula to display all other values as FTE in the *Resource Planner*:

```
FTE = <em>Resource Planner</em> Hours/ Default Schedule Hours
```

>[!NOTE]
>
>The schedule of the user is ignored when calculating the FTE for all values except for the Available (AVL) FTE values, in the *Resource Planner*. Only the Default Schedule is taken into account for the calculation.

This calculation applies for the following values:

* Planned FTE (PLN)
* Budgeted FTE (BDG)
* FTE Variance (VAR)
* NET FTE
* FTE Difference (DIF)

