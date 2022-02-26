---
filename: copy-initiatives
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copy initiatives in the Adobe Workfront Scenario Planner
description: You can create initiatives by copying existing ones. You can copy initiatives on a plan that you create or on a plan that someone shares with you.
---

# Copy initiatives in the *Adobe Workfront Scenario Planner*

You can create initiatives by copying existing ones. You can copy initiatives on a plan that you create or on a plan that someone shares with you.

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
   <td> <p><em>Adobe Workfront</em><b> license</b>*</p> </td> 
   <td> <p><em>Review</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>You must purchase an additional license for the <em>Adobe Workfront Scenario Planner</em> to access functionality described in this article.</p> <p>For information about obtaining the <em>Workfront Scenario Planner</em>, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Adobe Workfront Scenario Planner</a>. </p> </td> 
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

## Copy initiatives

Consider the following when copying initiatives:

* Copying an initiative places the copy on the same plan as the original initiative. 
* Copying an initiative copies and adds the following information from the original initiative to the new initiative:

  * Duration
  * Job roles
  * People and Fixed Costs
  * Planned Benefit

* Copying an initiative can modify the following information for the plan, if the information exists on the original initiative:

  * Required amount of job roles 
  * Costs
  * Plan Utilization
  * Job role utilization
  * Net Value

* Copying an initiative that was created by importing a project or has been published to a project at least once has the following implications:

  * It does not duplicate the project associated with the initiative.
  * It does not connect the copied initiative to the project. 
  * It does not modify the Scenario Planner section on the project, for projects that have been published at least once.

    For information about publishing initiatives to projects, see [Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner](../scenario-planner/publish-scenarios-update-projects.md).

    For information about creating initiatives by importing projects, see [Import projects to plans in the Adobe Workfront Scenario Planner](../scenario-planner/import-projects-to-plans.md) .

## Copy initiatives

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png">, then click&nbsp;<em>Scenarios</em>.<p>A list of plans displays. </p></li> 
 <li value="2">Click the name of a plan to open it, then locate the initiatives you want to copy.</li> 
 <li value="3"> <p>Select the box to the left of the initiative or initiatives that you want to copy, then click <span class="bold">Copy</span> from the menu that appears at the bottom of the plan.</p> <p> <img src="assets/bottom-manage-initiative-menu-350x45.png" style="width: 350;height: 45;"> </p> <p><em>Workfront</em> copies the initiatives immediately and places them underneath the last selected initiative. </p> <p>The name of the copied initiative is <i>Copy of <Name of original initiative></i>.</p> <note type="note"> 
   <span>Depending on where you insert the new initiatives, the numbers of existing initiatives may change. </span>
  </note> </li> 
 <li value="4"> <p>Update the name of the copied initiative. </p> <note type="tip">
   We recommend that you always update the name of the initiative to avoid confusion in case you want to copy them again. 
  </note> </li> 
 <li value="5"> <p>(Optional) Update the priority of your newly created initiatives. </p> <p>For information about prioritizing initiatives, see <a href="../scenario-planner/prioritize-initiatives.md" class="MCXref xref">Update initiative priorities in the Adobe Workfront Scenario Planner</a>. </p> </li> 
 <li value="6">Click <span class="bold">Save Plan</span> to save your changes. </li> 
</ol>

