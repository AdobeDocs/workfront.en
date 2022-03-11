---
filename: assign-work-in-workload-balancer
product-area: resource-management
navigation-topic: the-workload-balancer
title: Overview of assigning work in the Adobe Workfront Workload Balancer
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Overview of assigning work in the `Adobe Workfront` `Workload Balancer`

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

As a resource manager, you can use the `Adobe Workfront` `Workload Balancer` to view work items that have not yet been assigned to users as well as assign these items to them.

For general information about the `Workload Balancer`, see [Overview of the Workload Balancer](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

You can assign work items (tasks and issues) to users in other areas of `Workfront`. However, by using the `Workload Balancer` you can easily understand users' availability and clearly see all other items they are assigned to before assigning them more work.

For information about assigning work items in other areas of `Workfront`, see the following articles:

* [Assign tasks](../../manage-work/tasks/assign-tasks/assign-tasks.md) 
* [Assign issues](../../manage-work/issues/manage-issues/assign-issues.md)

## User availability in the `Workload Balancer`

You can assign work in the `Workload Balancer` to match the users' available time. To ensure that you assign the right amount of work and not overallocate the user, the total of the Planned Hours of the work items assigned to the user must match the user daily or weekly allocations.

You must understand how `Workfront` calculates the available time for a user. The `Workfront administrator` determines how the available time is calculated by selecting to use one of the following in the Resource Management area in&nbsp;Setup:

* The Default Schedule of the system and the user's FTE. 
* The user's schedule.&nbsp;

For more information, see [Configure Resource Management preferences](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Assign work in the `Workload Balancer`

You can assign work items that have not yet been assigned to a user or reassign items that have been assigned to users in the `Workload Balancer`.

You can assign work in the Workload Balancer in the following ways:

* One item at a time by manually assigning each item.

  For more information, see [Assign work manually using the Adobe Workfront Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

For information about unassigning work, see [Unassign work in the Adobe Workfront Workload Balancer](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

## Assignment areas in the `Workload Balancer`

You can assign work to users using the `Workload Balancer` in the Resourcing area, at the project, or at the team level. For more information about where the `Workload Balancer` is located in  `Workfront`, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

There are two areas in the `Workload Balancer` where you can view work items:

* `Unassigned Work`:&nbsp;displays items that are not assigned to users.
* `Assigned Work`: displays items that are assigned to users.

The following table describes which items display in each area based on their assignments:

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><span class="bold">Type of assignment</span> </td> 
   <td colspan="2"><span class="bold">Visible in the:</span> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>Unassigned Work </td> 
   <td>Assigned Work </td> 
  </tr> Unassigned item ✔ 
  <tr> 
   <td>Team</td> 
   <td>✔</td> 
   <td>&nbsp;</td> 
  </tr> Role ✔ 
  <tr> 
   <td>Role and Team</td> 
   <td>✔</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>User</td> 
   <td>&nbsp;</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>User and Team</td> 
   <td> <p>&nbsp;</p> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>User,&nbsp;Role, and Team</td> 
   <td>✔*</td> 
   <td>✔**</td> 
  </tr> User and Role ✔* ✔** 
 </tbody> 
</table>

&#42;When a work item is assigned to a user and a role, it displays in the Unassigned Work area only when the role is the Primary Assignee.

&#42;&#42;When a work item is assigned to a user and another entity, it displays in the Assigned Work area only when the user is the Primary Assignee.

For more information about the Unassigned and Assigned areas of the `Workload Balancer`, see [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Considerations for multiple assignments to job roles, teams, and users

Consider the following when assigning multiple resources to a work item:

* Users can have more than one job role associated with their profile. For information about associating users with job roles, see [Edit a user's profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Tasks or issues are usually first assigned to one or multiple job roles or to a team. When projects are ready to start, they might need to also be assigned to users.   
  If a task or an issue is assigned to one or multiple roles and then you also assign a user, `Adobe Workfront` decides which job role to associate with the additional user (if any)&nbsp;according to the following rules:

  * If there is only one job role assigned and it matches the user's Primary Role, then the task or issue is assigned only to the user fulfilling their&nbsp;Primary Role. 
  * If there are multiple roles assigned and at least one of the roles matches the user's secondary roles, then the task or issue is assigned to the user fulfilling one of their Other Roles — which `Workfront` selects at random if there are multiple matches — as well as any additional roles that are assigned.
  * If there is one or more job roles assigned and there are no matches to the user's roles, then the task or issue is assigned to both&nbsp;the role or roles as well as to the user.

* If a task or an issue is assigned to a team and you also assign a user, the task or issue remains assigned to both the team and the user.

<!--
Manually assign one item at a time Go to the Workload Balancer. Go to the Unassigned Work area and apply a filter to view work items Or Go to the Assigned Work area and expand the name of a user to view the work items assigned to them. Important: You cannot view and assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise, you can assign issues from a list or at the issue level. For information, see Assign issues. Click the More menu on the bar of a work item, then click Assign this to. Tip: You can also use the following shortcuts to assign tasks or issues: In Windows: CTRL+click the task or issue bar. In Mac: CMD+click the task or issue bar. Start typing the name of a user, job role, or team that you want to assign to the item in the Search people, role or teams field, select it when it displays in the list, then click Save. This assigns or reassigns the work item to the specified assignees. If you assign an item to just a team or a job role, the item displays only in the Unassigned Work area. You must assign work items to users in order to display them in the Assigned Work area of the Workload Balancer. Tip: You can assign multiple users or job roles, and you can assign only one team. You can assign only active users, job roles, and teams. If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following: Reassign the work item to active resources. Associate the users in a deactivated team with an active team and reassign the work item to the active team. (Optional) Click the Show allocations icon , then click the More menu > Edit allocations. Or Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item. For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations" section in the article Manage user allocations in the Workload Balancer. Assign an item by dragging and dropping You can assign an item from the Unassigned Work area to a user, or you can reassign an already assigned item to another user in the Assigned Work area. Go to the Workload Balancer. Go to the Unassigned Work area and apply a filter to view work items. Important: You cannot view and assign issues from the Unassigned Work area. Click the bar of a work item that indicates either the planned or the projected timeline and drag it over the name of a user in the Assigned area. The user you hover over to drop the work item to is highlighted. Tip: The Planned Hours for the user you're hovering over update in real time with the number of daily Planned Hours from the work item, to indicate what the impact of adding a new item might be to their overall allocation. When you are ready, drop the selected work item in the same line as the user's name in the Assigned Area. The item is assigned and the allocated Planned Hours are updated for the user with the new hours from the work item. Tip: If you enabled Group by Project in the Settings area, the assigned task displays under the corresponding project. If the setting is disabled, the assigned task displays in the user area. The item displays according to the Workload Balancer criteria for sorting work items. For more information, see Navigate the Workload Balancer. (Optional) Click the Show allocations icon , then click the More menu > Edit allocations. Or Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item. For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations" section in the article Manage user allocations in the Workload Balancer. Assign items in bulk
-->

<!--
Unassign work items in the Workload Balancer You can either unassign items from users and move them to the Unassigned Work area, or reassign them to other users. To unassign work items from users: In the Workload Balancer, go to the Assigned Work area and expand a user. Do one of the following: Find the item you want to unassign in a user's area, click it, drag and drop it in the Unassigned area or in another user's area. Click the More icon to the right of the name of a work item, click Assign this to , then remove the name of the entities assigned to the work item or enter another name and click Save. The item displays in the Unassigned Work area if it matches the filtering criteria for that area and it is not assigned to any users or it displays in the user area if it is assigned to that user. Tip: Unassigned issues do not display in the Unassigned area. For information about filtering information in the Workload Balancer, see Manage filters in the Workload Balancer.
-->

