---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configure Resource Management preferences
description: As an Adobe Workfront administrator you can configure the Resource Management Preferences for your system. These Resource Management preferences determine how user availability or capacity and FTE are calculated for the Workfront resource scheduling and planning tools.
author: Caroline
feature: System Setup and Administration
role: Admin
---

# Configure Resource Management preferences

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

As an Adobe Workfront administrator you can configure the Resource Management Preferences for your system. These Resource Management preferences determine how user availability or capacity and FTE are calculated for the Workfront resource scheduling and planning tools.

For information about planning and scheduling resources in Workfront, see [Get started with Resource Management](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Access requirements

You must have the following to perform the steps in this article:

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure Resource Management preferences

>[!NOTE]
>
>Because this is a global setting, this selection affects all the calculations for the entire system, for all users, in all the resource management tools, and for all Resource Pools.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Setup** ![](assets/gear-icon-settings.png).
1. Click **Resource Management**. 
1. Select one of the following methods to calculate the availability of users in Workfront:

   * **The Default Schedule**: Workfront uses the Default Schedule of the system and the individual FTE of the user to calculate the Available Hours of the user in resource management tools.   
     For more information about schedules, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

     For more information about the value of the user FTE, see  [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   
     Workfront calculates the Available Hours of a user using the following formula when the Workfront administrator chooses The Default Schedule:

     ```   
     User Available Hours = (Default Schedule Hours - Exceptions) * FTE - Time off hours
     ```

     **Example:**   
     For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.

     If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:

     ```   
     User Available Hours = (40 * 0.5) - 1 = 19 hours
     ```

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
        <div class="example" data-mc-autonum="<b>Example: </b>">      
        <span class="autonumber"><span><b>Example: </b></span></span>      
        <div>      
        <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
        <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
        <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code><br></p>      
        </div>      
        </div></li>      
        -->

   * **The User's Schedule**: Workfront uses the user's schedule as well as the Default Schedule of the system to calculate the Available FTE value of the user in resource management tools. The Available Hours are calculated according only to the user's schedule. The value of the FTE of the user is ignored. This is the default setting.

     >[!NOTE]
     >
     >If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.

     The Available FTE for the user is calculated by the following formula:

     ```   
     User Available FTE = (Hours from the Schedule of the User - Time off hours) / Default Schedule Hours
     ```

     **Example:** For example, if the Default Schedule is 40 hours a week and the schedule of the user is 30 hours a week, the FTE of the user is 0.75. 

     If the user has 2 hours of Time off one day, their Weekly Available FTE will be calculated as follows:

     ```   
     User Weekly Available FTE = (30-2) / 40 = 0.70
     ```

1. Click **Save**.

