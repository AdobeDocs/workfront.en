---
filename: calculate-hours-fte-for-users-roles-resource-planner
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
---



# Overview of calculating hours and FTE for users and roles in the *`Resource Planner`* {#overview-of-calculating-hours-and-fte-for-users-and-roles-in-the-resource-planner}

You can display the allocation and availability of your resources in the *`Resource Planner`* by Hours, FTE, or Cost.  
For more information about calculating Costs in the *`Resource Planner`*, see [Calculate costs in the Resource Planner](calculate-costs-resource-planner.md).


"FTE" stands for Full Time Equivalent. It is a measure of time that represents the amount of hours dedicated to real work during a day or week for a user or job role. 


The following sets of resource information are calculated differently in the *`Resource Planner`*:



*  The Available Hours or FTE values are calculated based on the way your System Administrator configures the Resource Management preferences in your system.  
  For more information about how the Available Hours and FTE values are calculated, see [Calculate Available Hours or FTE for users and job roles in the Resource Planner](#calculating-available-hours).  
  For more information about defining the Resource Management preferences for the *`Adobe Workfront`* system, see [Configure Resource Management preferences](configure-resource-mgmt-preferences.md).  

*  All other FTE values are calculated based on the System Default schedule.  
  For more information about how the all other values display in the *`Resource Planner`* when using FTE, see [Calculate all other hour and FTE values for users and job roles in the Resource Planner](#calculating-all-other-values).



It is important to understand what the FTE is for each of your users and their job roles to accurately manage your resources as you are assigning them to work.  



## Calculate Available Hours or FTE for users and job roles in the *`Resource Planner`* {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}




* [Calculate the Available Hours and FTE for a user in the Resource Planner](#user-availability) 
* [Calculate the Available Hours and FTE for a job role in the Resource Planner](#job-role-availability) 
* [Calculate the Available Hours and FTE for a user in the Resource Planner (Example)](#example) 




### Calculate the Available Hours and FTE for a user in the *`Resource Planner`* {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

The *`Workfront administrator`* determines how the available time for a user is calculated by selecting to use one of the following in the Resource Management area in&nbsp;Setup:



*  The Default Schedule of the system and the user's FTE. 
*  The user's schedule.&nbsp;


For more information, see [Configure Resource Management preferences](configure-resource-mgmt-preferences.md).


### Calculate the Available Hours and FTE for a job role in the *`Resource Planner`* {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

You first have to calculate the user availability, and then you can calculate the availability of each of their job roles. 


The availability of job roles in the *`Resource Planner`* takes into account the total availability of the user, and the `Percentage of FTE Availability` associated with each role of the user.  
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)  



For more information about associating a `Percentage of FTE Availability` value with a job role for a user, see [Edit a user's profile](edit-a-users-profile.md).


For example, if the value of Available Hours for a user is 40 and they can fulfill one Primary Role for 75% of that time, and one Other Role for 25% of that time, the *`Resource Planner`* shows that the `Available Hours` value for the Primary Role for one week is 30 hours, and that the `Available Hours` value for the Other Role is 10 hours. In this case, the FTE for the Primary Role is 0.75 and the FTE for the other role is 0.25. 


>[!NOTE]
>
>The total available time for the user is calculated by one of the two methods described in the [Calculate the Available Hours and FTE for a user in the Resource Planner](#user-availability) section in this article. 


When viewing the *`Resource Planner`* in the Role View, the availability of one job role is a total of the availability of all users who can fulfill that job role.  
For more information about availability of resources in the *`Resource Planner`*, see the [Resource Planner overview](get-started-resource-planner.md).


### Calculate the Available Hours and FTE for a user in the *`Resource Planner`* (Example) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

The following table illustrates how the Available Hours and Available FTE are calculated for the user in the *`Resource Planner`*, depending on which method is used by the system administrator for the FTE calculation in the Resource Management Preferences. 


For this example, we are using the following numbers: 



*  A system Default Schedule of 40 hours 
*  A user Schedule of 20 Hours 
*  A user FTE of 0.75. 





## Calculate all other hour and FTE values for users and job roles in the *`Resource Planner`* {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

In addition to the Available Hours or FTE, the following time information is also displayed in the *`Resource Planner`*: 



* Planned Hours
* Budgeted Hours
* Hour Variance
*  Net Hours  
  For more information about these values see [Overview of hours, FTE, and cost information in the Project and Role views of the Resource Planner](overview-of-planner-hour-fte-cost-information-in-role-project-views.md)  

*  Hour Difference  
  For more information about what this value represents see [Overview of hours, FTE, and cost information in the Project and Role views of the Resource Planner](overview-of-planner-hour-fte-cost-information-in-role-project-views.md).



You can display the same information in the *`Resource Planner`* as FTE or as hours. 


*`Workfront`* uses the following formula to display all other values as FTE in the *`Resource Planner`*:




```
FTE = <span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span> Hours/ Default Schedule Hours
```




>[!NOTE]
>
>The schedule of the user is ignored when calculating the FTE for all values except for the Available (AVL) FTE values, in the *`Resource Planner`*. Only the Default Schedule is taken into account for the calculation. 


This calculation applies for the following values:



* Planned FTE (PLN)
* Budgeted FTE (BDG)
* FTE Variance (VAR)
* NET FTE
* FTE Difference (DIF) 


