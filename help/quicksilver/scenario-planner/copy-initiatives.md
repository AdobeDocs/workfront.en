---
filename: copy-initiatives
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copy initiatives in the Adobe Workfront Scenario Planner
description: You can create initiatives by copying existing ones. You can copy initiatives on a plan that you create or on a plan that someone shares with you.
---

# Copy initiatives in the Adobe Workfront Scenario Planner

You can create initiatives by copying existing ones. You can copy initiatives on a plan that you create or on a plan that someone shares with you.

## Access requirements

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront<b> plan*</b> </p> </td> 
   <td>Business or higher</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront<b> license</b>*</p> </td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>You must purchase an additional license for the Adobe Workfront Scenario Planner to access functionality described in this article.</p> <p>For information about obtaining the Workfront Scenario Planner, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Adobe Workfront Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access or higher to the Scenario Planner</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
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

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png), then click&nbsp;Scenarios.

   A list of plans displays. 

1. Click the name of a plan to open it, then locate the initiatives you want to copy.
1. Select the box to the left of the initiative or initiatives that you want to copy, then click **Copy** from the menu that appears at the bottom of the plan.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   Workfront copies the initiatives immediately and places them underneath the last selected initiative.

   The name of the copied initiative is *Copy of <Name of original initiative>*.

   >[!NOTE]
   >
   >```Depending on where you insert the new initiatives, the numbers of existing initiatives may change.```

1. Update the name of the copied initiative.

   >[!TIP]
   >
   >We recommend that you always update the name of the initiative to avoid confusion in case you want to copy them again.

1. (Optional) Update the priority of your newly created initiatives.

   For information about prioritizing initiatives, see [Update initiative priorities in the Adobe Workfront Scenario Planner](../scenario-planner/prioritize-initiatives.md). 

1. Click **Save Plan** to save your changes.

