---
filename: configure-resource-mgmt-preferences
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configure Resource Management preferences
description: As an Adobe Workfront administrator you can configure the Resource Management Preferences for your system.
---

# Configure Resource Management preferences

As an Adobe Workfront administrator you can configure the Resource Management Preferences for your system.

The Resource Management preferences determine how user availability or capacity and FTE are calculated for the Workfront resource scheduling and planning tools.

For information about planning and scheduling resources in Workfront, see [Get started with Resource Management](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
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
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure Resource Management preferences

>[!NOTE]
>
>Because this is a global setting, this selection affects all the calculations for the entire system, for all users, in all the resource management tools, and for all Resource Pools.

1. Click **Setup** near the upper-right corner of Workfront on the Global Navigation Bar.
1. Click **Resource Management**. 
1. Select one of the following methods to calculate the availability of users in Workfront:

   * **The Default Schedule**: Workfront uses the Default Schedule of the system and the individual FTE of the user to calculate the Available Hours of the user in resource management tools.   
     For more information about schedules, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

     For more information about the value of the user FTE, see&nbsp; [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>Workfront calculates the Available Hours of a user differently depending on which environment you choose. The following formulas are used to calculate user availability or capacity when the Workfront administrator chooses The Default Schedule: </p>   
     <ul>   
     <li><p>In the Production environment:</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p></li>   
     <li class="preview"><p>In the Preview environment:</p><p><code>User Available Hours = (Default Schedule Hours - Exceptions) *&nbsp;FTE - Time off hours</code></p></li>   
     </ul>   
     </div>   
     -->

     The Available Hours for the user are calculated by the following formula:

     ```   
     User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value
     ```

     ``` ```**Example: **``````For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.

     If the user has 1 hour of Time off one day during the week, their Available Hours will be calculated as follows:

     ```   
     User Daily Available Hours = (40-1) * 0.5 = 19.5 hours
     ```

   * **The User's Schedule**: Workfront uses the user's schedule as well as the Default Schedule of the system to calculate the Available FTE value of the user in resource management tools. The Available Hours are calculated according only to the user's schedule. The value of the FTE of the user is ignored. This is the default setting.

     >[!NOTE]
     >
     >If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.

     The Available FTE for the user is calculated by the following formula:

     ```   
     User Available FTE = (Hours from the Schedule of the User - Time off hours) / Default Schedule Hours
     ```

     ``` ```**Example: **``````For example, if the Default Schedule is 40 hours a week and the schedule of the user is 30 hours a week,&nbsp;the FTE of the user is 0.75.&nbsp;

     If the user has 2 hours of Time off one day, their Weekly Available FTE will be calculated as follows:

     ```   
     User Weekly Available FTE = (30-2) / 40 = 0.70
     ```

1. Click **Save**.

