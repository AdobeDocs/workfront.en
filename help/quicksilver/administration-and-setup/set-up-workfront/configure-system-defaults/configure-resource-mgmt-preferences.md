---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configure Resource Management Preferences
description: As an [!DNL Adobe Workfront] administrator, you can configure the Resource Management Preferences for your system. These Resource Management preferences determine how user availability or capacity and FTE are calculated for the [!DNL Workfront] resource scheduling and planning tools.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
---
# Configure [!UICONTROL Resource Management] preferences

<!-- Audited: 5/2025 -->

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

As an [!DNL Adobe Workfront] administrator, you can configure the [!UICONTROL Resource Management] Preferences for your system. These preferences determine how user hour or FTE availability or capacity are calculated for the [!DNL Workfront] resource scheduling and planning tools.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Information taken into account when calculating a user's capacity

When calculating a user's capacity, Workfront takes into account the following information:

* The number of scheduled hours, as defined in either the user's Schedule or the Workfront system's Default Schedule.
* Schedule Exceptions (depending on which Schedule is used, it can be the exceptions of the user's schedule, or those associated with the Workfront Default Schedule).
* The user's time off.
* The value of the Full Time Equivalent ([!UICONTROL FTE]) of the user or that of the [!DNL Workfront] system. The [!UICONTROL FTE] equals 1 when the user works full time, as defined in the schedule. 
* The value of [!UICONTROL Work Time] for the user, which refers to time that the user spends on project-related work. This does not include overhead time, like meetings and training. The [!UICONTROL Work Time] equals 1 when the user is available for work the entire time as indicated by the [!UICONTROL FTE] or the schedule, which means they don't spend any time on non-project-related work like meetings or trainings.


For information about planning and scheduling resources in [!DNL Workfront], see [Get started with Resource Management](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configure [!UICONTROL Resource Management] preferences

>[!NOTE]
>
>Because this is a global setting, this selection affects all the calculations for the entire system, for all users, in all the resource management tools.

{{step-1-to-setup}}

1. Click **[!UICONTROL Resource Management]**.
1. Select one of the following methods to calculate the availability of users in [!DNL Workfront]:

   * **The Default Schedule**: [!DNL Workfront] uses the Default Schedule of the system and the user's individual FTE to calculate the Available Hours of the user in resource management tools.

      For more information, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) and [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      When this option is selected, Workfront calculates the user's Available Hours using the following formula:
      
      
      `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`
      

      >[!INFO]
      >
      >For example, if the Default Schedule is 40 hours a week, the FTE in the user's profile is 0.5, the user has 1 hour of Time off one day, and the [!UICONTROL Work Time] in the user's profile is 0.5, and the user is available for actual project work for 9.5 hours a week.
      >
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >
      >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
      >
     
      <!--
      This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      -->
      
      
      
      <!--      
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
      <div class="example" data-mc-autonum="<b>Example: </b>">      
      <span class="autonumber"><span><b>Example: </b></span></span>      
      <div>      
      <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
      <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
      <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code></p>      
      </div>      
      </div></li>      
      -->

   * **The User's Schedule**: [!DNL Workfront] uses the user's schedule as well as the [!UICONTROL Default Schedule] of the system to calculate the Available [!UICONTROL FTE] value of the user in resource management tools. The Available Hours are calculated according only to the user's schedule, and the value of the [!UICONTROL FTE] of the user is ignored. This is the default setting.

      For more information, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) and [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >If the user is not associated with a schedule, the Available Hours for the user are calculated using only the [!UICONTROL Default Schedule].

      The Available hours for the user is calculated by the following formula:

      
      `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`
      

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      
      `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`
      

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week, the user's schedule is 30 hours a week, the user's [!UICONTROL Work Time] is 0.5, and the [!UICONTROL FTE] of the user is 0.35.
      >
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      >
      >
      >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`
      >
      
      <!--This used to be the calculation before we implemented the Work Time field: 
      

      The Available hours for the user are calculated by the following formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```  

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the schedule of the user is 30 hours a week, the [!UICONTROL FTE] of the user is 0.70.
      >  
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      > 
      >```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```
      -->
   
1. Click **[!UICONTROL Save]**.
