---
filename: legacy-fte
product-area: resource-management
navigation-topic: legacy-resource-planning
title: Overview of FTE in the Legacy Resource Management tools
description: "FTE" stands for Full Time Equivalent. It is a measure of time that represents the amount of hours dedicated to real work during a day or week for a user.
---

# Overview of FTE in the Legacy&nbsp;Resource Management tools

>[!IMPORTANT]
>
>&nbsp;The information in this article refers to the functionality of Legacy Resource Planning. This functionality is currently deprecated and will be removed from Workfront.&nbsp;For information about the&nbsp;current&nbsp;functionality for managing resources in Workfront, see the&nbsp; [Resource Planning in Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md)&nbsp;section.&nbsp;For information about FTE in the current resource management tools, see [Overview of calculating hours and FTE for users and roles in the Resource Planner](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

"FTE" stands for Full Time Equivalent. It is a measure of time that represents the amount of hours dedicated to&nbsp;real work during a day or&nbsp;week for a user.&nbsp;

It is important to define your system FTE, as well as the FTE values for your users and their job roles&nbsp;to accurately manage your resources as you are assigning them to work.&nbsp;

For more information about how FTE is calculated in the Resource Planning tools, see [Overview of calculating hours and FTE for users and roles in the Resource Planner](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Overview of the system-level FTE {#overview-of-the-system-level-fte}

As a System Administrator, you can configure your system FTE. You&nbsp;can define the amount of hours in a day and the amount of days in a week that represents the amount of time dedicated to real work in your organization. This is configured in Project Preferences in Setup.

For more information about how to configure the amount of hours in a work day, and the amount of days in a work week, see the "Timeline Calculations" section in [Configure system-wide project preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

The&nbsp;number that you define in this configuration represents the FTE for your organization. This is what the timeline engine uses when calculating allocations for your projects. It is important that you define this number in accordance with the work schedule of most of your users.&nbsp;

The default FTE is 8 hours/day and 5 days/week, for a total of 40 hours/week.   
In other words, as a default:  
1 FTE = 40 hours/week and 1 FTE = 8 hours/day.&nbsp;

However, if in your organization most users work 7 hour days, then your weekly hours should be 35 (5 days a week at 7 hours per day).   
In this case, in your Workfront environment:  
1 FTE = 35 hours and 1 FTE = 7 hours/day.

## Overview of the FTE of a user

Each user in Workfront should be assigned an FTE value when they are created. This allows for an accurate representation of what full-time equivalent is allocated to the Primary Job role of the user in the Resource Budget Manager.

For more information about the Resource Budget Manager, see&nbsp; [Budget Legacy Resource Pools in the Resource Budget Manager](../../resource-mgmt/legacy-res-planning/budget-legacy-pools-in-budget-manager.md).

>[!NOTE]
>
>&nbsp;The FTE value for the user does not contribute to the correct user allocation represented&nbsp;in the Resource Grid. Only the amount of hours in a user's schedule contribute to the allocation of the user in the Resource Grid. For more information about the Resource Grid, see&nbsp; [Overview of the Resource Grid](../../resource-mgmt/legacy-res-planning/resource-grid-overview.md).

There is no default value for the FTE of a user, but we recommend that you define this when you create the user.&nbsp;

For more information about how to&nbsp;define the FTE value for an existing user, see&nbsp; [Edit a user's profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

We recommend that all users should have a value of 1 for their FTE. This would mean that they are working a full time schedule in their Primary Job Role, as understood by your system and as&nbsp;specified&nbsp;in Project Preferences.&nbsp;

However, some users might work a part time schedule, in which case, they should&nbsp;have a value of 0.5 or 0.75 for their FTE. This would mean that their Primary Job Role can be allocated to work only for 0.5 or 0.75 of a full time equivalent, as specified in Project Preferences.&nbsp;

For more information about defining your Project Preferences, see&nbsp; [Configure system-wide project preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

For more information about the system FTE and how to configure it, see&nbsp; [Overview of the system-level FTE](#overview-of-the-system-level-fte).

## Overview of the FTE of&nbsp;a job role

* [Assign FTE to a job role through the user's Primary Role](#assign-fte-to-a-job-role-through-the-user-s-primary-role) 
* [Assign FTE to a job role using the Resource Budget Manager](#assign-fte-to-a-job-role-using-the-resource-budget-manager)

### Assign FTE to a job role through the user's Primary Role {#assign-fte-to-a-job-role-through-the-user-s-primary-role}

The following are two&nbsp;of the pre-requisites of Resource Management:

* All users should have a value for their FTE.
* All users should be associated with one Primary Job Role.&nbsp;

For more information about associating a user with a job role, see [Edit a user's profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

When you associate a user with an FTE value and a primary job role, the job role is automatically associated with that FTE of the user in the Resource Management tools (Resource Budget Manager and Capacity Planner).&nbsp;

### Assign FTE to a job role using the Resource Budget Manager {#assign-fte-to-a-job-role-using-the-resource-budget-manager}

If you associate a user with multiple job roles, only their primary job role FTE&nbsp;appears in the Resource Budget Manager by default. If you want their secondary job roles to have FTE values in the Resource Management Tools (Resource Budget Manager and Capacity Planner), you will have to manually configure&nbsp;the allocation for each&nbsp;secondary role using the Resource Budget Manager.

For more information about how to allocate resources in the Resource Budget Manager, see [Budget Legacy Resource Pools in the Resource Budget Manager](../../resource-mgmt/legacy-res-planning/budget-legacy-pools-in-budget-manager.md).&nbsp;

When you manually configure the amount of the FTE for the job roles assigned as secondary roles to users in the Resource Budget Manager, then the Capacity Planner will show your manual value for the FTE for those job roles, in the respective Legacy Resource Pools.&nbsp;
