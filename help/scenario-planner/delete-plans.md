---
filename: delete-plans
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Delete plans in the Adobe Workfront Scenario Planner
description: You can delete plans that you created. You cannot delete plans that are shared with you.
---

# Delete plans in the `Adobe Workfront Scenario Planner`

You can delete plans that you created. You cannot delete plans that are shared with you.

## Access requirements

You must have the following:

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><span>Adobe Workfront</span><b> plan*</b> </p> </td> 
   <td><span>Business</span> or higher</td> 
  </tr> 
  <tr> 
   <td> <p><span>Adobe Workfront</span><b> license*</b> </p> </td> 
   <td> <p><span>Review</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>You must purchase an additional license for the <span>Adobe Workfront Scenario Planner</span> to access functionality described in this article.</p> <p>For information about obtaining the <span>Workfront Scenario Planner</span>, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Adobe Workfront Scenario Planner</a>. </p> </td> 
  </tr> Access level configurations* Edit access or higher to the Scenario Planner Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see Create or modify custom access levels. Object permissions Manage permissions to a plan For information on requesting additional access to a plan, see Request access to a plan in the Adobe Workfront Scenario Planner. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Delete plans

>[!IMPORTANT]
>
>You cannot recover deleted plans.

You can delete a plan or you can delete one scenario in a plan.

* [Delete plans](#delete3) 
* [Delete scenarios](#delete4)

### Delete plans

>[!IMPORTANT]
>
>Consider the following when deleting plans:
>
>* All information related to the plan is also deleted. This includes all the scenarios and initiatives associated with the plan including information about job roles and costs. This information cannot be recovered.
>* >
>  If the plan contains a published scenario, the projects linked to the deleted initiatives are preserved and the `Scenario Planner` area remains in the Project&nbsp;Details section. 
>
>  For information about publishing initiatives to projects, see [Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner](../scenario-planner/publish-scenarios-update-projects.md).
>

To delete a plan:

<ol> 
 <li value="1"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png">, then click&nbsp;<span>Scenarios</span>.</p> <p>A list of plans displays. </p> </li> 
 <li value="2">Click the name of a plan to open it.</li> 
 <li value="3"> <p>Click the <span class="bold">More menu</span> <img src="assets/more-menu.png"> to the right of the plan name, then click <span class="bold">Delete</span> > <span class="bold">Yes, delete it</span>.</p> <p>The plan is deleted and you return to the list of plans. </p> </li> 
</ol>

### Delete scenarios

>[!IMPORTANT]
>
>Consider the following when deleting a scenario:&nbsp;
>
>* Deleting a scenario deletes all initiatives and their information from the scenario. If they are copied to other scenarios, the initiatives remain on the other scenarios. 
>* When deleting a scenario, the subsequent scenario takes on the number of the deleted scenario and the counting order is preserved.&nbsp;For example, if you delete Scenario 4, Scenario 5 becomes Scenario 4. 
>* `If some initiatives on the scenario are published, the project linked to the initiative is preserved and the `Scenario Planner` area remains on the linked projects.` 
>* >
>  If the published initiatives exist on another scenario, they remain on that scenario, including their link to the project. Publishing those initiatives from the other scenarios updates the linked projects with new information from those scenarios. 
>
>  For information about publishing initiatives to projects, see [Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner](../scenario-planner/publish-scenarios-update-projects.md).
>

To delete a scenario:

<ol> 
 <li value="1"> <p>Go to the plan for which you want to delete a scenario. </p> <p>By default, the Initial scenario displays.</p> </li> 
 <li value="2">Click <span class="bold">Compare scenarios</span>.</li> 
 <li value="3"> <p>From the upper-right corner of the scenario card, click the <span class="bold">More</span> menu <img src="assets/more-menu.png">, then click <span class="bold">Delete</span>. </p> <p>The scenario is deleted.</p> </li> 
 <li value="4">Click <span class="bold">Save plan</span> to save your changes. </li> 
</ol>

<!--
Delete initiatives Important: Consider the following when deleting initiatives: Deleting an initiative deletes the job roles and cost information from the initiative. When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project Details section. If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. For information about publishing initiatives to projects, see Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner. To delete an initiative: Click the Main Menu icon , then click Scenarios. A list of plans displays. Click the name of a plan to open it, then locate the initiative you want to delete. Click the More menu to the right of the initiative name, then click Delete > Yes, delete it. The initiative is deleted. Click Save Plan to save your changes.
-->

&nbsp;
