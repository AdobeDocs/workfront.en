---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Delete plans in the Scenario Planner
description: You can delete plans that you created. You cannot delete plans that are shared with you.
feature: Workfront Scenario Planner
---

# Delete plans in the Scenario Planner

You can delete plans that you created. You cannot delete plans that are shared with you.

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront<b> plan*</b> </p> </td> 
   <td>Business or higher</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront<b> license*</b> </p> </td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>You must purchase an additional license for the Adobe Workfront Scenario Planner to access functionality described in this article.</p> <p>For information about obtaining the Workfront Scenario Planner, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access or higher to the Scenario Planner</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Manage permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the Scenario Planner</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Delete plans

>[!IMPORTANT]
>
>You cannot recover deleted plans.

You can delete a plan or you can delete one scenario in a plan.

* [Delete plans](#delete-plans) 
* [Delete scenarios](#delete-scenarios)

### Delete plans

>[!IMPORTANT]
>
>Consider the following when deleting plans:
>
>* All information related to the plan is also deleted. This includes all the scenarios and initiatives associated with the plan including information about job roles and costs. This information cannot be recovered.
>* If the plan contains a published scenario, the projects linked to the deleted initiatives are preserved and the Scenario Planner area remains in the Project&nbsp;Details section. 
>
>  For information about publishing initiatives to projects, see [Update or create projects by publishing initiatives in the Scenario Planner](../scenario-planner/publish-scenarios-update-projects.md).

To delete a plan:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png), then click&nbsp;Scenarios.

   A list of plans displays. 

1. Click the name of a plan to open it.
1. Click the **More menu** ![](assets/more-menu.png) to the right of the plan name, then click **Delete** > **Yes, delete it**.

   The plan is deleted and you return to the list of plans.

### Delete scenarios {#delete-scenarios}

>[!IMPORTANT]
>
>Consider the following when deleting a scenario:&nbsp;
>
>* Deleting a scenario deletes all initiatives and their information from the scenario. If they are copied to other scenarios, the initiatives remain on the other scenarios. 
>* When deleting a scenario, the subsequent scenario takes on the number of the deleted scenario and the counting order is preserved.&nbsp;For example, if you delete Scenario 4, Scenario 5 becomes Scenario 4. 
>* If some initiatives on the scenario are published, the project linked to the initiative is preserved and the Scenario Planner area remains on the linked projects 
>* If the published initiatives exist on another scenario, they remain on that scenario, including their link to the project. Publishing those initiatives from the other scenarios updates the linked projects with new information from those scenarios. 
>
>  For information about publishing initiatives to projects, see [Update or create projects by publishing initiatives in the Scenario Planner](../scenario-planner/publish-scenarios-update-projects.md).

To delete a scenario:

1. Go to the plan for which you want to delete a scenario.

   By default, the Initial scenario displays.

1. Click **Compare scenarios**.
1. From the upper-right corner of the scenario card, click the **More** menu ![](assets/more-menu.png), then click **Delete**.

   The scenario is deleted.

1. Click **Save plan** to save your changes.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete initiatives</h2>
<p>(NOTE: moved this section to its own article about deleting initiatives)&nbsp;</p> <note type="important">
<p>Consider the following when deleting initiatives:</p>
<ul>
<li>Deleting an initiative deletes the job roles and cost information from the initiative.</li>
<li><span>When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project&nbsp;Details section.</span> </li>
<li> <p>If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. </p> <p>For information about publishing initiatives to projects, see <a href="../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Scenario Planner</a>.</p> </li>
</ul>
</note>
<p>To delete an initiative:</p>
<ol>
<li value="1"> <p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png">, then click&nbsp;Scenarios.</p> </p> <p>A list of plans displays. </p> </li>
<li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/more-menu.png"> to the right of the initiative name, then click <strong>Delete</strong> > <strong>Yes, delete it</strong>. </p> <p>The initiative is deleted. </p> </li>
<li value="4">Click <strong>Save Plan</strong> to save your changes. </li>
</ol>
</div>
-->

&nbsp;
