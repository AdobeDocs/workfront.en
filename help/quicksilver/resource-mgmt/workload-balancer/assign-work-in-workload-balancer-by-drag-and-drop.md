---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Assign work in the Workload Balancer by dragging and dropping
description: Assign work in the Workload Balancer by dragging and dropping
author: Alina
feature: Resource Management
---

# Assign work in the Workload Balancer by dragging and dropping

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is just a NWE article)</p>
-->

You can assign work items using the Adobe Workfront Workload Balancer by dragging and dropping work items to the correct users.

For general information about assigning work to users using the Workload Balancer, see [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to&nbsp;the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Assign an item by dragging and dropping

You can assign an item from the Unassigned Work area to a user, or you can reassign an already assigned item to another user in the Assigned Work area.

1. Go to the Workload Balancer where you want to assign work.

   You can assign work to users using the Workload Balancer in the Resourcing area, at the project, or at the team level. For more information about where the Workload Balancer is located in&nbsp;Workfront, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Optional) Go to the **Unassigned Work** area and apply a filter to view work items

   Or

   Go to the **Assigned Work** area and expand the name of a user to view the work items assigned to them, if you want to reassign their items.

   >[!IMPORTANT]
   >
   >**You cannot view or assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise,** you can assign issues from a list or at the issue level. For information, see [Assign issues](../../manage-work/issues/manage-issues/assign-issues.md).

1. Click the bar of a work item that indicates either the planned or the projected timeline and drag it over the name of a user in the **Assigned** area.

   The user you hover over to drop the work item to is highlighted.

   >[!TIP]
   >
   >The Planned Hours for the user you're hovering over update in real time with the number of daily Planned Hours from the work item, to indicate what the impact of adding a new item might be to their overall allocation.

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. When you are ready, drop the selected work item in the same line as the user's name in the Assigned Area. The item is assigned and the allocated Planned Hours are updated for the user with the new hours from the work item.

   >[!TIP]
   >
   >If you enabled Group by Project in the Settings area, the assigned task displays under the corresponding project. If the setting is disabled, the assigned task displays in the user area. 
   >
   >
   >The item displays according to the Workload Balancer criteria for sorting work items.&nbsp;For more information, see [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. (Optional) Click the bar of a work item under the name of a user in the Assigned Work area and drag it then drop it over the Unassigned area to unassign it. The item is unassigned from the user, but it might still be assigned to a job role in which case it displays in the Unassigned Work area. If the item is assigned to another user, it remains in the Assigned Work area under the name of the user who is still assigned. 
1. (Optional) Click the **Show allocations icon** ![](assets/show-allocations-icon-small.png), then click the **More menu** ![](assets/qs-more-menu.png) > **Edit allocations**. 

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: make sure these are still called this, and that the icon has not changed)
   </MadCap:conditionalText>
   -->

   &nbsp;

   Or

   Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.

   For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   For information about removing assignments from a work item using the Workload Balancer, see [Unassign work in the Workload Balancer](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

&nbsp;
