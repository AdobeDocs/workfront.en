---
filename: how-workfront-calculates-finances
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: How Adobe Workfront calculates finances
description: How Adobe Workfront calculates finances
hidefromtoc: true
---

# How Adobe Workfront calculates finances

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This should be moved to Project Finances when it's been improved)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(drafted articles because info moved to the glossary and to the Project&nbsp;Finances Overview article)</p>
-->

You can track your finances with a number of fields that capture budget, cost, and revenue in&nbsp;Adobe Workfront.

The following table contains some of the most common financial fields or references you might encounter when reviewing Workfront documentation or speaking with other customers.

For more information, also see the following articles:

* [Glossary of Adobe Workfront terminology](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md) 
* [Project finances](../../../manage-work/projects/project-finances/project-finances-overview.md) 
* [Project finances overview](../../../manage-work/projects/project-finances/project-finances-overview-1.md) 
* [Manage information in the project Finance area](../../../manage-work/projects/project-finances/manage-project-finance-area.md) 
* [Manage task finances in the Task Details tab](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

<table cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Term</strong> </p> </th> 
   <th> <p><strong>Definition</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Actual Hours</p> </td> 
    <td> <p>The hours recorded against the task (via Log Hours button).</p> <p><code>For parent tasks = children Actual Hours + Actual Hours on the parent task. For projects = Actual Hours logged on the project +Actual Hours logged on standalone or children tasks in the project</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> If from the Updates tab for Task 1, you click ‘Log Time’ and enter 25 hours, the Actual Hours = 25. </p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Actual Labor Cost</p> </td> 
    <td> <p>The result of multiplying the actual hours by the rate. </p> <br> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If the task is set up such that the Cost Type = ‘User Hourly’ (Task Details&gt;Finance) and the user’s cost/hr on their profile is $100.00/hr, then if you record 5 actual hours, the Actual Labor Cost = $500.00. </p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>(Incurred)&nbsp;Actual Expense Cost</p> </td> 
    <td> <p>The sum of the Actual Amount field for all expenses where the Actual Amount field &gt; 0.</p> <br> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> If you create an expense for Task 1 and enter $600.00 in the Actual Amount field, the Incurred Actual Expense Cost for this task is $600.00. </p> <br> <p>Important: If the value in the Actual Amount field for an expense is negative, the system will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations. </p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>(Incurred) Planned Expense Cost </p> </td> 
    <td> <p>The sum of the Planned Amount field for all expenses where the Actual Amount field &gt; 0.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> If you create an expense for Task 1 and enter $500.00 in the Planned Amount field and an amount &gt; 0 in the Actual Amount field (i.e. $600.00), the Incurred Planned Expense Cost for this task is $500.00. </p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>(Not Incurred) Planned Expense</p> </td> 
    <td> <p>The sum of the Planned Amount field for all expenses where the Actual Amount field = 0.</p> <br> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> If you create two expenses for Task 1 where for the first expense the value in the Planned Amount field is $500.00 and the value in the Actual Amount is $600.00 and for the second expense, the value in the Planned Amount field is $300.00 and the value of the Actual Amount field is $0.00, the value of the Not Incurred Planned Expense for this task is $300.00. </p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Percent Complete</p> </td> 
    <td> <p>The value entered into the Percent Complete field for a task.</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Planned Hours</p> </td> 
    <td> <p>The value entered into the Planned Hours field on the task (i.e. 10 Hours)</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Planned Labor Cost</p> </td> 
    <td> <p>The result of multiplying the planned hours by the rate. </p> <br> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> If the task is set up such that the Cost Type = ‘User Hourly’ (Task Details&gt;Finance) and the user’s cost/hr on their profile is $100.00/hr, then if you record 10 planned hours, the Planned Labor Cost = $1,000.00. </p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Total Budgeted Cost Work Performed</td> 
    <td> <p>The result of multiplying the budgeted cost of the work planned (Budgeted Cost) and the percent of the task that has been completed so far.</p> <p>For a non-parent task:<br><code>TotalBudgetedCostWorkPerformed = Planned Hours * (Percent Complete/100)</code><br>For a parent task:<br><code>TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all direct child tasks</code><br>For a project:<br><code>TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all top-level tasks (parents and standalone tasks)</code> </p> </td> 
   </tr>
  --> 
  <tr> 
   <td>EAC</td> 
   <td> <p>Estimate at Completion which represents the projected total cost of your project or task when it completes.</p> <p>For information, see <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calculate Estimate At Completion (EAC)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>CPI</td> 
   <td> <p>Cost Performance Index describes the relationship at the project or task level between the planned cost and actual cost.</p> <p>For information, see <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calculate Cost Performance Index (CPI)</a></p> </td> 
  </tr> 
  <tr> 
   <td>CSI</td> 
   <td> <p>Cost Schedule Performance Index is an automatic calculation which combines the Cost Performance Index (CPI) and Schedule Performance Index (SPI) into one general metric that balances cost and schedule. </p> <p>For information, see <a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calculate Cost Schedule Performance Index (CSI)</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>PIM</td> 
   <td> <p>The Performance Index Method (PIM) for the project controls the method Workfront uses to calculate project performance metrics such as Cost Performance Index (CPI), Cost Schedule Performance Index (CSI), Schedule Performance Index (SPI), and Estimate At Completion (EAC).</p> <p>For information, see <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Set the Performance Index Method (PIM)</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Differences between the two EAC methods</h2>
<p>(NOTE: drafted and replaced this with links from the table and in the intro. Will replace the article with another table with ALL the financial field - work in progress - backlog!) </p>
<p>There are two methods for calculating EAC:</p>
<ul>
<li><a href="#calculate-eac-at-project-level" class="MCXref xref">Calculate EAC at project level</a> </li>
<li><a href="#caculate-eac-as-a-roll-up-from-tasks" class="MCXref xref">Caculate EAC as a roll up from tasks</a> </li>
</ul>
<h3 id="calculate-eac-at-project-level"><a name="Calculat"></a>Calculate EAC at project level</h3>
<ul>
<li> EAC for the parent task and project are determined by entering the actual hours/actual labor cost into the EAC Formulas </li>
<li><em> Includes </em> Actual Hours/ Costs and expenses added directly to the parent task or project </li>
</ul>
<h3 id="caculate-eac-as-a-roll-up-from-tasks"><a name="Caculate"></a>Caculate EAC as a roll up from tasks</h3>
<ul>
<li> EAC for the parent task and project are determined by summing up the EAC for each <em> direct </em> child task </li>
<li><em> Excludes </em> Actual Hours and expenses added directly to the parent task or project </li>
</ul>
<h2><a name="Formulas"></a>Formulas</h2>
<ul>
<li><a href="#PIM-Hour-Based" class="MCXref xref">How Adobe Workfront calculates finances </a> </li>
<li><a href="#PIM-Cost-Based" class="MCXref xref">How Adobe Workfront calculates finances </a> </li>
</ul>
<h3><a name="PIM-Hour-Based_section-1"></a>PIM= Hour-Based</h3>
<h4><strong>TotalBudgetedCostWorkPerformed</strong> </h4>
<ul>
<li><strong>For a non-parent task</strong>: <code>TotalBudgetedCostWorkPerformed = Planned Hours * (Percent Complete/100)</code></li>
<li><strong>For a parent task:</strong> <code>TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all single children tasks</code></li>
<li> <p><strong>For a project:</strong> <code>TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all top-level tasks</code> </p> <note type="note">
This includes only first level parents, not secondary level parents, etc.
</note> </li>
</ul>
<h4><strong>CPI</strong> </h4>
<p><em> IF </em> Actual Hours > 0 <em> THEN </em><![CDATA[
]]><code>CPI = TotalBudgetedCostWorkPerformed / Actual Hours </code><![CDATA[    ]]></p>
<p><em> ELSE </em> CPI = 1 </p>
<p><strong>EAC</strong> </p>
<p><em> IF </em> CPI <> 0 <em> THEN </em> EAC = Planned Hours / CPI </p>
<p><em> ELSE </em> EAC = Planned Hours + Actual Hours </p>
<h3><a name="PIM-Cost-Based_section-1"></a>PIM= Cost-Based</h3>
<h4><strong>TotalBudgetedCostWorkPerformed</strong> </h4>
<p><strong>For a non parent task</strong> : <code>TotalBudgetedCostWorkPerformed = Planned Labor Cost * (Percent Complete/100)</code></p>
<p><strong>For a parent task:</strong> <code>TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all direct child tasks</code></p>
<p><strong>For a project:</strong> <code>TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all top-level tasks</code></p>
<h4><strong>CPI</strong> </h4>
<p><em> IF </em> Actual Labor Cost + IncurredActualExpenseCost <> 0 <em> THEN </em><![CDATA[
]]><code> CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)</code><![CDATA[
]]></p>
<p><em> ELSE </em> CPI = CPI_Labor </p>
<h4><strong>EAC</strong> </h4>
<p><strong>EAC</strong> = <strong>EAC Labor</strong> + <strong>EAC Expense</strong><strong></strong> </p>
<p> For EAC Labor, we first need to determine CPI_Labor. </p>
<p><strong>CPI_Labor</strong> = IF Actual Labor Cost <> 0 THEN <code>CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost</code><![CDATA[
]]></p>
<p> ELSE CPI_Labor = 1 <strong></strong> </p>
<p><strong>EAC Labor</strong> = <em> IF </em> CPI_Labor <> 0 <em> THEN </em><![CDATA[
]]><code>EAC Labor = Planned Labor Cost / CPI_Labor </code></p>
<p><em> ELSE </em><![CDATA[
]]><code>EAC Labor = Planned Labor Cost + Actual Labor Cost </code></p>
<p><strong>EAC Expense</strong><![CDATA[
]]><code>= IncurredActualExpenseCost + NotIncurredPlannedExpense</code><![CDATA[
]]></p>
</div>
-->

