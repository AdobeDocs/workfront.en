---
filename: assign-work-in-workload-balancer-manually
product-area: resource-management
navigation-topic: the-workload-balancer
title: Assign work manually using the Adobe Workfront Workload Balancer
description: You can manually assign work items to users using the Adobe Workfront Workload Balancer.
---

# Assign work manually using the `Adobe Workfront` `Workload Balancer`

You can manually assign work items to users using the `Adobe Workfront` `Workload Balancer`.

For general information about assigning work to users using the `Workload Balancer`, see [Overview of assigning work in the Adobe Workfront Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to&nbsp;the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Manually assign work in the `Workload Balancer`

You can assign work items that have not yet been assigned to a user or reassign items that have been assigned to users in the `Workload Balancer`.

<ol> 
 <li value="1"> <p>Go to the <span>Workload Balancer</span> where you want to assign work.</p> <p>You can assign work to users using the <span>Workload Balancer</span> in the Resourcing area, at the project, or at the team level. For more information about where the <span>Workload Balancer</span> is located in&nbsp;<span>Workfront</span>, see <a href="../../resource-mgmt/workload-balancer/locate-workload-balancer.md" class="MCXref xref">Locate the&nbsp;Workload Balancer</a>.</p> </li> 
 <li value="2"> <p>(Optional) Go to the <span class="bold">Unassigned Work</span> area and apply a filter to view work items</p> <p>Or</p> <p>Go to the <span class="bold">Assigned Work</span> area and expand the name of a user to view the work items assigned to them, if you want to reassign their items.</p> <note type="important">
   <span>You cannot view or assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise,</span> you can assign issues from a list or at the issue level. For information, see 
   <a href="../../manage-work/issues/manage-issues/assign-issues.md" class="MCXref xref">Assign issues</a>.
  </note> </li> 
 <li value="3"> <p>Click the <span class="bold">More menu</span> <img src="assets/qs-more-menu.png"> on the bar of a work item, then click <span class="bold">Assign this to</span>. </p> <p> <img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"> </p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p><span>You can also use the following shortcuts to assign tasks or issues:</span> </p> 
   <ul> 
    <li><span>In Windows: CTRL+click the task or issue bar.</span> </li> 
    <li><span>In&nbsp;Mac: CMD+click the task or issue bar.</span> </li> 
   </ul> 
  </div> </li> 
 <li value="4"> <p>Start typing the name of a user, job role, or team that you want to assign to the item in the <span class="bold">Search people, role or teams</span> field, select it when it displays in the list, then click&nbsp;<span class="bold">Save</span>. </p> <p> <img src="assets/assignments-box-wb.png"> </p> <p>This assigns or reassigns the work item to the specified assignees.</p> <p>If you assign an item to just a team or a job role, the item displays only in the Unassigned Work area. You must assign work items to users in order to display them in the Assigned Work area of the <span>Workload Balancer</span>.</p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>You can assign multiple users or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams.</span></p> 
   <p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span> </p> 
   <ul> 
    <li> <p><span>Reassign the work item to active resources.</span> </p> </li> 
    <li> <p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team.</span> </p> </li> 
   </ul> 
  </div> </li> 
 <li value="5"> <p>(Optional) Click the <span class="bold">Show allocations icon</span> <img src="assets/show-allocations-icon-small.png">, then click the <span class="bold">More menu</span> <img src="assets/qs-more-menu.png"> > <span class="bold">Edit allocations</span>.</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the <span>Workload Balancer</span>, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> <p>For information about removing assignments from a work item using the <span>Workload Balancer</span>, see <a href="../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md" class="MCXref xref">Unassign work in the Adobe Workfront Workload Balancer</a>. </p> <p>&nbsp;</p> </li> 
</ol>

