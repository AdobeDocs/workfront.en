---
filename: assign-work-in-workload-balancer-by-drag-and-drop
product-area: resource-management
navigation-topic: the-workload-balancer
title: Assign work in the Adobe Workfront Workload Balancer by dragging and dropping
description: You can assign work items using the Adobe Workfront Workload Balancer by dragging and dropping work items to the correct users.
---

# Assign work in the *Adobe Workfront* *Workload Balancer* by dragging and dropping

You can assign work items using the *Adobe Workfront* *Workload Balancer* by dragging and dropping work items to the correct users.

For general information about assigning work to users using the *Workload Balancer*, see [Overview of assigning work in the Adobe Workfront Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to&nbsp;the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Assign an item by dragging and dropping

You can assign an item from the Unassigned Work area to a user, or you can reassign an already assigned item to another user in the Assigned Work area.

<ol> 
 <li value="1"> <p>Go to the <em>Workload Balancer</em> where you want to assign work.</p> <p>You can assign work to users using the <em>Workload Balancer</em> in the Resourcing area, at the project, or at the team level. For more information about where the <em>Workload Balancer</em> is located in&nbsp;<em>Workfront</em>, see <a href="../../resource-mgmt/workload-balancer/locate-workload-balancer.md" class="MCXref xref">Locate the&nbsp;Workload Balancer</a>.</p> </li> 
 <li value="2"> <p>(Optional) Go to the <span class="bold">Unassigned Work</span> area and apply a filter to view work items</p> <p>Or</p> <p>Go to the <span class="bold">Assigned Work</span> area and expand the name of a user to view the work items assigned to them, if you want to reassign their items.</p> <note type="important">
   <span>You cannot view or assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise,</span> you can assign issues from a list or at the issue level. For information, see 
   <a href="../../manage-work/issues/manage-issues/assign-issues.md" class="MCXref xref">Assign issues</a>.
  </note> </li> 
 <li value="3"> <p>Click the bar of a work item that indicates either the planned or the projected timeline and drag it over the name of a user in the <span class="bold">Assigned</span> area.</p> <p>The user you hover over to drop the work item to is highlighted.</p> <note type="tip">
   The Planned Hours for the user you're hovering over update in real time with the number of daily Planned Hours from the work item, to indicate what the impact of adding a new item might be to their overall allocation.
  </note> <p> <img src="assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png" style="width: 350;height: 152;"> </p> </li> 
 <li value="4"> <p>When you are ready, drop the selected work item in the same line as the user's name in the Assigned Area. The item is assigned and the allocated Planned Hours are updated for the user with the new hours from the work item.</p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>If you enabled Group by Project in the Settings area, the assigned task displays under the corresponding project. If the setting is disabled, the assigned task displays in the user area. </p> 
   <p>The item displays according to the <em>Workload Balancer</em> criteria for sorting work items.&nbsp;For more information, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p> 
  </div> </li> 
 <li value="5"> <p>(Optional) Click the bar of a work item under the name of a user in the Assigned Work area and drag it then drop it over the Unassigned area to unassign it. The item is unassigned from the user, but it might still be assigned to a job role in which case it displays in the Unassigned Work area. If the item is assigned to another user, it remains in the Assigned Work area under the name of the user who is still assigned. </p> </li> 
 <li value="6"> <p>(Optional) Click the <span class="bold">Show allocations icon</span> <img src="assets/show-allocations-icon-small.png">, then click the <span class="bold">More menu</span> <img src="assets/qs-more-menu.png"> > <span class="bold">Edit allocations</span>.</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the <em>Workload Balancer</em>, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> <p>For information about removing assignments from a work item using the <em>Workload Balancer</em>, see <a href="../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md" class="MCXref xref">Unassign work in the Adobe Workfront Workload Balancer</a>. </p> </li> 
</ol>

&nbsp;
