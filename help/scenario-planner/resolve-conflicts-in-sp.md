---
filename: resolve-conflicts-in-sp
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Resolve initiative conflicts in the Adobe Workfront Scenario Planner
description: When initiatives conflict with one another they are competing for the same resources. The resources you have available for a scenario are not enough to cover all of the resources required by all initiatives in the scenario.
---

# Resolve initiative conflicts in the *Adobe Workfront Scenario Planner*

When initiatives conflict with one another they are competing for the same resources. The resources you have available for a scenario are not enough to cover all of the resources required by all initiatives in the scenario.

This can happen in any of the following cases:

* The number of job roles required for the initiative is larger than the number of roles budgeted for the plan. 
* The costs of the initiative is larger than the budget amount available for the plan.

## Access requirements

You must have the following:

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
   <td> <p>You must purchase an additional license for the <em>Adobe Workfront Scenario Planner</em> to access functionality described in this article.</p> <p>For information about obtaining the <em>Workfront Scenario Planner</em>, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Adobe Workfront Scenario Planner</a>. </p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td><span class="bold">Access level configurations*</span> </td> 
    <td> <p>Edit or higher to the <em>Scenario Planner</em></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td><span class="bold">Access level configurations*</span> </td> 
   <td> <p>Edit or higher to the <em>Scenario Planner</em></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
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

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Resolve conflicts overview

* A conflict is also understood as an overallocation of the job roles or the budget of a scenario. 
* When&nbsp;*Workfront* detects a conflict, the bar corresponding to the conflicting month during the initiative's duration displays in red. This can happen in any of the following cases:

  * The number of job roles required monthly for an initiative is larger than the number of roles budgeted for the plan after all previous initiatives have used the resources budgeted for the plan.
  * The monthly costs of the initiative are larger than the budget available for the plan after all previous initiatives have used the plan's budget to cover their costs.

` `**Tip: **`` By default, the *Scenario Planner* assumes that you have budgeted for 0 job roles and $0 or the equivalent of $0 in your system's currency for a scenario, unless you specified otherwise. The number of job roles indicates the number of FTEs (Full Time Equivalents) `or hours` budgeted for the job role .

For all calculations in the *Scenario Planner*, *Workfront* uses the following value: 1 FTE = 8 Hours.

For information about updating the available roles for a plan and a budget see [Create and edit plans in the Adobe Workfront Scenario Planner](../scenario-planner/create-and-edit-plans.md).

* You can resolve a conflict by doing one of the following:

  * Adding the missing required resources automatically from the initiatives on the scenario. This article describes how to resolve conflicts using this option. 
  * Adjusting the job role and budget resources for the scenario, by editing the plan. For more information, see [Create and edit plans in the Adobe Workfront Scenario Planner](../scenario-planner/create-and-edit-plans.md).

## Resolve conflicts between initiatives

<ol> 
 <li value="1"> <p>Go to a plan for which you want to resolve conflicts.</p> <p>For information about creating plans, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Adobe Workfront Scenario Planner</a>.</p> <p>For information about creating initiatives, see <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Create and edit initiatives in the Adobe Workfront Scenario Planner</a>. </p> </li> 
 <li value="2"> <p>(Optional)&nbsp;From the <span class="bold">Initial scenario</span> drop-down menu, select the scenario you want to review. </p> <note type="tip">
   A plan may have several scenarios. When looking at the plan's conflicts,&nbsp;
   <em>Workfront</em> is referring to the resources currently available on the selected scenario and those required on that scenario's initiatives. For information about scenarios, see 
   <a href="../scenario-planner/create-and-compare-scenarios-for-a-plan.md" class="MCXref xref">Create and compare plan scenarios in the Adobe Workfront Scenario Planner</a>. 
  </note> </li> 
 <li value="3"> <p>Ensure that <span class="bold">Show conflicts</span> is enabled. It is enabled by default. </p> <p> <img src="assets/show-scenarios-toggle-on.png"> </p> <p>The first conflicting initiative displays the months that have conflicts in red and a warning icon displays next to the initiative name. </p> <p>The background of all initiatives starting with the first conflicting one displays in red on the plan's chart. </p> <p>When an initiative displays a conflict, it means that the number of job role for at least one specific role, the costs incurred, or both exceed the number of job roles or the budget defined for the plan for a specific month. </p> <p> <img src="assets/initiatives-on-plan-with-conflicts-350x126.png" style="width: 350;height: 126;"> </p> </li> 
 <li value="4"> <p>Do one of the following to understand more about the conflicts that might exist:</p> 
  <ul> 
   <li> <p>Hover over the warning icon next to the initiative name to understand whether you have a job role or a budget conflict. </p> <p> <img src="assets/budget-job-role-conflict-tooltip-on-warning-icon-350x109.png" style="width: 350;height: 109;"> </p> <p>Depending on whether you overallocated job roles or overestimated costs for your initiative you might see one of the following options when hovering over the warning icon:</p> 
    <ul> 
     <li> <p>Show job role conflict details</p> </li> 
     <li> <p>Show budget conflict details</p> </li> 
     <li> <p>Show job role and budget details</p> </li> 
    </ul> </li> 
  </ul> 
  <ul> 
   <li> <p>When viewing the plan by month, hover over a month in the plan's timeline to view the required resources for that month and whether the conflicts for the month are people or cost-related. </p> <p> <img src="assets/details-of-conflicts-on-monthly-plan-timeline-pop-up-350x178.png" style="width: 350;height: 178;"> </p> <p>Review the following monthly information at the plan-level: </p> 
    <ul> 
     <li> <p>The number of available, required, and overallocated job roles for the month for all initiatives planned for that month</p> </li> 
     <li> <p>The available, required, and overallocated costs for the month for all the initiatives planned for that month</p> <note type="tip">
       The Available costs are the scenario's budget for that month. 
      </note> </li> 
    </ul> </li> 
   <li> <p>Hover over an initiative's red bar for a month to display the additional information box about the conflict that occurs that month.&nbsp;</p> <p> <img src="assets/details-of-conflicts-on-initiative-timeline-pop-up-350x113.png" style="width: 350;height: 113;"> </p> <p>Review the following fields in the additional information box at the initiative's level:</p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">Month when the conflict occurs</td> 
       <td>Displays in the title of the additional information box.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">The initiative name</td> 
       <td>Displays in the title of the additional information box.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Job&nbsp;Roles</td> 
       <td> <p>The job roles associated with this initiative that are overallocated for the selected month. The following columns display information for each job role that is required for the selected month and that conflicts with the number of job roles available for that month:</p> 
        <ul> 
         <li> <p><span class="bold">Available</span>: The number of each job role available from the scenario for the selected month.</p> </li> 
         <li> <p><span class="bold">Required</span>: The number of each job role required for the initiative for the selected month.</p> </li> 
         <li> <p style="font-weight: normal;"><span class="bold">Overallocated: </span>The difference between the number required on the initiative and the number available from the scenario. </p> </li> 
        </ul> <note type="tip">
         Sometimes, the number of Available roles matches or is higher than the number of Required roles, but the 
         <em>Scenario Planner</em> still shows an overallocation.&nbsp;This means that there are higher-ranking initiatives that already used the job roles available on the plan for the same month. 
        </note> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Costs</td> 
       <td> <p>The costs of the initiative for the month selected. The following columns display information for the costs needed and the budget available of the selected month:</p> 
        <ul> 
         <li> <p><span class="bold">Available</span>: The budget available from the plan for the selected month .</p> </li> 
         <li> <p><span class="bold">Required</span>: The costs associated with this initiative for the selected month.</p> </li> 
         <li> <p style="font-weight: normal;"><span class="bold">Overallocated: </span>The difference between the costs of the initiative and the budget available from the plan. </p> </li> 
        </ul> <note type="tip">
         Sometimes, the Available costs match or are higher than the Required cost of the initiative for the selected month and the 
         <em>Scenario Planner</em> still shows an overallocation of cost.&nbsp;This means that there are higher-ranking initiatives that already use the available budget on the plan for the same month. 
        </note> </td> 
      </tr> 
     </tbody> 
    </table> </li> 
  </ul> </li> 
 <li value="5"> <p>Do one of the following to open the initiative details panel and view more information about where the conflicts occur and to resolve them:</p> 
  <ul> 
   <li> <p>Click the warning icon next to the initiative's name.</p> </li> 
   <li> <p>Click the bar of an initiative.</p> </li> 
   <li> <p>Click the <span class="bold">More</span> icon <img src="assets/more-icon.png"> to the right of the initiative’s name, then click <span class="bold">Edit</span>.</p> <p>The initiative details panel displays on the right. </p> <p>When you do not have enough people or budget available for your initiative, a red warning icon displays next to following sections: </p> </li> 
   <li> <p style="font-weight: bold;">Required Job&nbsp;Roles</p> </li> 
   <li> <p style="font-weight: bold;">Costs</p> </li> 
  </ul> </li> 
 <li value="6"> <p>(Conditional)&nbsp;For initiatives that have job role conflicts, go to the <span class="bold">Required Job&nbsp;Roles</span> section to view all job roles required for your initiative. Identify which job roles might be overallocated.&nbsp;Review the number of FTE <span>or hours</span> needed for each job role for each month of the initiative. The box with the FTE <span>or hours</span> number for months that have overallocations displays in a red outline. </p> <p> <img src="assets/details-panel-overallocated-roles-350x275.png" style="width: 350;height: 275;"> </p> </li> 
 <li value="7"> <p>(Optional) Click the right-pointing arrow next to the months in the initiative's timeline to view which additional months display job role conflicts. </p> <p> <img src="assets/right-arrow-initiative-months-inside-details-box-highlighted-350x145.png" style="width: 350;height: 145;"> </p> </li> 
 <li value="8"> <p>(Optional) Click&nbsp;<span class="bold">Show details </span>under the job role that displays a conflict to see where the conflicts appear and to highlight the conflicting months in the plan's chart area. Additional information displays for each job role.</p> <p>The following fields display for each job role:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Available</td> 
     <td> <p>The number of job roles available from the plan for each month. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Previously allocated</td> 
     <td>The number of job roles already allocated from the plan's budget to higher-ranking initiatives for a specific month. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Overallocated</td> 
     <td> <p>The difference between the number of required job roles on the initiative and the number available from the plan after higher-ranking initiatives also used some of the roles. <em>Workfront</em> calculates the number of Overallocated job roles using the following formula:</p> <p><code>Overallocated roles = (Roles Previously Allocated to higher initiatives + Required roles for current initiative) - Monthly available roles from the plan</code> </p> </td> 
    </tr> 
   </tbody> 
  </table> <note type="tip">
   On the plan's chart, the months where the job roles are allocated display the name and the number of roles needed for each initiative where they are needed. You must select the Month view to see the name of the job roles
  </note> <p> <img src="assets/conflicting-job-role-months-on-plan-after-clicking-show-details-350x158.png" style="width: 350;height: 158;"> </p> </li> 
 <li value="9"> <p>Do one of the following to resolve job role conflicts:</p> 
  <ul style="list-style-type: circle;"> 
   <li> <p>Manually adjust the number of job roles for each month of the initiative to a lower number.</p> </li> 
   <li> <p>Hover over the name of the job role and click the <span class="bold">delete icon </span> <img src="assets/delete.png"> to remove the job role from the initiative. </p> </li> 
   <li> <p>Select <span class="bold">Add roles to the scenario's available resources</span>, then click <span class="bold">Apply</span>. </p> <p>This adds the missing number of job role FTEs <span>or hours</span> to the scenario's Available field. </p> <note type="note">
     The roles you add to resolve the conflicts modify the Available job roles for the selected scenario and not for all the scenarios in the plan. 
    </note> <p>An upward-pointing green arrow <img src="assets/upward-green-arrow.png"> displays for the month in the timeline of the plan to indicate that more resources were added to the plan that month. You must select the Month view to see this indicator. </p> </li> 
   <li> <p>(Conditional) Close the details panel and give the initiative a higher priority to receive budget resources from the plan first, if possible. For information about updating initiative priority, see <a href="../scenario-planner/prioritize-initiatives.md" class="MCXref xref">Update initiative priorities in the Adobe Workfront Scenario Planner</a>.</p> </li> 
  </ul> </li> 
 <li value="10">(Optional) Click <span class="bold">Hide details</span> to close the additional details box, then click&nbsp;<span class="bold">Apply</span> to save the changes you make to job roles. </li> 
 <li value="11"> <p>(Conditional) For initiatives that have costs conflicts, go to the <span class="bold">Costs</span> section in the initiative details panel to review costs for every month of the initiative's duration. Identify which months might not have enough money in the plan's budget to cover the costs for the selected initiative. The box with the insufficient available budget displays in a red outline.</p> </li> 
 <li value="12"> <p>(Optional) Click the right-pointing arrow next to the months in the initiative's timeline to view additional months that have insufficient budget to cover the costs. </p> <p> <img src="assets/details-panel-insufficient-costs-350x239.png" style="width: 350;height: 239;"> </p> </li> 
 <li value="13"> <p>(Optional) Click&nbsp;<span class="bold">Show details</span> under the cost information to see where the conflict appears and to highlight the conflicting months on the plan's chart.&nbsp;The following additional fields display for each type of cost: </p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Available</td> 
     <td> <p>The costs available from the plan's Budget for each month. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Previously allocated</td> 
     <td>The amount of money already allocated from the plan's budget to higher-ranking initiatives. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Overallocated</td> 
     <td> <p>The monthly difference between the costs needed for the initiative and the amount of money available from the plan's budget after higher-ranking initiatives also used some of the available budget. <em>Workfront</em> calculates the number of Overallocated costs using the following formula:</p> <p><code>Overallocated costs = (Costs Previously Allocated to higher initiatives + Required costs for the current initiative) - Monthly available budget from the plan</code> </p> <p><em>Workfront</em> calculates the Required costs for the current initiative for each month using the following formula:</p> <p><code>Required initiative costs = Initiative Fixed Costs + Initiative People Costs</code> </p> </td> 
    </tr> 
   </tbody> 
  </table> <note type="tip">
   On the plan's chart, the months where the costs are insufficient display the name and the number of roles still needed for the initiative. You must select the Month view to view the cost amounts. 
  </note> <p> <img src="assets/conflicting-costs-months-on-plan-after-clicking-show-details-350x139.png" style="width: 350;height: 139;"> </p> <note type="note">
   If you disabled the Include people cost setting for the plan's Budget box when you created the plan, the People Costs line does not display for any initiative in any scenario. In this case, 
   <em>Workfront</em> does not take People Costs into calculations to determine cost conflicts. For information about creating a plan, see 
   <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Adobe Workfront Scenario Planner</a>. 
  </note> </li> 
 <li value="14"> <p>Do one of the following to resolve costs conflicts:</p> 
  <ul style="list-style-type: circle;"> 
   <li> <p>Manually adjust the number of Fixed Costs for each month of the initiative to a lower number.</p> </li> 
   <li> <p>In the <span class="bold">Required Job Roles</span> section, manually adjust the number of job roles for the month with a People Costs budget, if possible. This reduces the number of People Costs. </p> <note type="tip">
     You cannot manually adjust People Costs. 
    </note> </li> 
   <li> <p>Select <span class="bold">Add amount to the scenario's budget</span>, then click <span class="bold">Apply</span>. </p> <p>This adds the insufficient amount to the scenario's budget for the months where it was missing which also updates the overall scenario budget. </p> <note type="note">
     The amount you add to resolve the cost conflicts modify the Budget for the selected scenario and not for all the scenarios in the plan. 
    </note> </li> 
   <li> <p>(Conditional) Close the details panel and give the initiative a higher priority to receive budget resources from the plan first, if possible. For information about updating initiative priority, see <a href="../scenario-planner/prioritize-initiatives.md" class="MCXref xref">Update initiative priorities in the Adobe Workfront Scenario Planner</a>.</p> </li> 
  </ul> </li> 
 <li value="15"> <p>Click <span class="bold">Apply </span>when you make any changes to the Costs section. </p> </li> 
 <li value="16">Click <span class="bold">Save plan</span> to save your changes. </li> 
</ol>

&nbsp;
