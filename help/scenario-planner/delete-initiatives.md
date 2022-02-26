---
filename: delete-initiatives
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Delete initiatives in the Adobe Workfront Scenario Planner
description: You can delete initiatives on a plan that you created or on a plan that someone shared with you. You cannot recover initiatives that you deleted.
---

# Delete initiatives in the *Adobe Workfront Scenario Planner*

You can delete initiatives on a plan that you created or on a plan that someone shared with you. You cannot recover initiatives that you deleted.

## Access requirements

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><em>Adobe Workfront</em><b> plan*</b> </p> </td> 
   <td><em>Business</em> or higher</td> 
  </tr> 
  <tr> 
   <td> <p><em>Adobe Workfront</em><b> license*</b> </p> </td> 
   <td> <p><em>Review</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>You must purchase an additional license for the <em>Adobe Workfront Scenario Planner</em> to access functionality described in this article. </p> <p>For information about obtaining the <em>Workfront Scenario Planner</em>, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Adobe Workfront Scenario Planner</a>. </p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td><span class="bold">Access level configurations*</span> </td> 
    <td> <p>Edit access or higher to the <em>Scenario Planner</em></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td><span class="bold">Access level configurations*</span> </td> 
   <td> <p>Edit access or higher to the <em>Scenario Planner</em></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td> <p><span class="bold">Object permissions</span> </p> </td> 
    <td> <p>Manage permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the Adobe Workfront Scenario Planner</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td> <p><span class="bold">Object permissions</span> </p> </td> 
   <td> <p>Manage permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the Adobe Workfront Scenario Planner</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Delete initiatives

Consider the following when deleting initiatives:

* Deleting an initiative removes the required amount of job roles and the cost information associated with the initiative from the plan.
* Deleting an initiative that was created by importing a project does not delete the project associated with the initiative.
* `Deleting an initiative that has been published to a project at least once results in the following:`

  * `The initiative is deleted from the scenario but the *Scenario Planner* area remains in the Project Details section.` 
  * If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed.

    For information about publishing initiatives to projects, see [Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner](../scenario-planner/publish-scenarios-update-projects.md).

    For information about creating initiatives by importing projects, see [Import projects to plans in the Adobe Workfront Scenario Planner](../scenario-planner/import-projects-to-plans.md) .

You can delete one initiative at a time, `or you can delete multiple initiatives in bulk.`

* [Delete one initiative](#delete) 
* [Delete initiatives in bulk](#delete3)

### Delete one initiative

<ol> 
 <li value="1"> <p> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png">, then click&nbsp;<em>Scenarios</em>.</p> </p> <p>A list of plans displays. </p> </li> 
 <li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li> 
 <li value="3"> <p>Do one of the following:</p> 
  <ul> 
   <li> <p>Click the <span class="bold">More menu </span><img src="assets/more-menu.png"> to the right of the initiative name, then click <span class="bold">Delete</span> > <span class="bold">Yes, delete it</span>. </p> </li> 
  </ul> 
  <ul> 
   <li> <p>Select the box to the left of the initiative, then click <span class="bold">Delete</span> on the floating menu that appears at the bottom of the plan, then click <span class="bold">Yes, delete it</span>. </p> </li> 
  </ul> <p>The initiative and its job role and cost information are deleted from the plan.</p> </li> 
 <li value="4">Click <span class="bold">Save Plan</span> to save your changes. </li> 
</ol>

### Delete initiatives in bulk

<ol> 
 <li value="1"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png">, then click&nbsp;<em>Scenarios</em>.</p> <p>A list of plans displays. </p> </li> 
 <li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li> 
 <li value="3"> <p>Select the boxes to the left of the initiatives that you want to delete, then click <span class="bold">Delete</span> from the menu that appears at the bottom of the plan, then click <span class="bold">Yes, delete them</span>. </p> <p> <img src="assets/bottom-manage-initiative-menu-350x45.png" style="width: 350;height: 45;"> </p> <p>The initiatives and their job role and cost information are deleted from the plan.</p> </li> 
 <li value="4">Click <span class="bold">Save Plan</span> to save your changes. </li> 
</ol>

