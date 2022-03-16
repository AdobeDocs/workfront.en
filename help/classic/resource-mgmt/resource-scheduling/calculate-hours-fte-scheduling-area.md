---
filename: calculate-hours-fte-scheduling-area
product-area: resource-management
navigation-topic: resource-scheduling
title: Configure how Workfront calculates resource hour and FTE availability for the Scheduling area
description: We are no longer developing the Resource Scheduling tools and they will soon be removed from Adobe Workfront. We recommend that you use the Workload Balancer for scheduling your resources.
---

# Configure how Workfront calculates resource hour and FTE&nbsp;availability for the Scheduling area

>[!NOTE]
>
>We are no longer developing the Resource Scheduling tools and they will soon be removed from Adobe Workfront. We recommend that you use the Workload Balancer for scheduling your resources. 
>
>For information about scheduling resources using the new Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
>
>For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

The Adobe Workfront administrator determines how Workfront calculates resource availability and user allocation at the system level (considering hours as well as FTE availability) when they configure Resource Management preferences.

They can select to use one of the following:

* The Default Schedule of the system and the user's FTE. 
* The user's schedule.&nbsp;

For more information, see [Configure Resource Management preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

This setting affects user availability in the following circumstances when scheduling resources:

* When allowing Workfront to automatically assign resources, as described in [Manually assign unassigned tasks and issues in the Scheduling areas](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).
* When displaying allocation indicators, as described in the section "Allocation indicators" in the article&nbsp; [Manage user allocations in the Scheduling areas](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

<!--
Access requirements You must have the following: Adobe Workfront plan* Any Adobe Workfront license* Plan Access level configurations* System administrator Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see Create or modify custom access levels. Object permissions For information on requesting additional access, see Request access to objects in Adobe Workfront. *To find out what plan, license type, or access you have, contact your Workfront administrator. Configure how Workfront calculates resource availability when scheduling resources Log in to Workfront as an administrator. Go to the Setup area in your Global Navigation Bar. Click Resource Management. Select to calculate the availability of users in Workfront using one of the following methods: The Default Schedule: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user when scheduling resources. The Schedule of the user is ignored. In this case: The Available Hours for a user when scheduling resources are calculated using the following formula: User Available Hours = Default Schedule Hours * User FTE value For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Scheduling area. For more information about schedules, including the Default Schedule, see Create a schedule. The Available FTE for the user when scheduling resources is the same as the user FTE specified in the user settings. For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner. For more information about the value of the user FTE as it displays in the user settings, see Edit a user's profile. The User's Schedule: The Schedule of the user is used to determine the availability of the user when scheduling resources. The value of the user FTE is ignored. In this case: The Available Hours in the Resource Planner are the same as the Hours from the Schedule of the user. For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the Resource Planner. The Available FTE in the Resource Planner is calculated by the following formula: User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in Workfront has 40 hours available to work, the user's FTE is 0.5. For more information about schedules, including the Default Schedule, see Create a schedule. Note: If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
-->

