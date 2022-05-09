---
filename: how-workfront-calculates-finances
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: How Adobe Workfront calculates finances
description: "(NOTE: Alina: Keep this draft for a revamp of all definitions for financial fields in Workfront"
hidefromtoc: true
---

# How Adobe Workfront calculates finances

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;Alina: Keep this draft for a revamp of all definitions for financial fields in Workfront</p>
<p>-- <span class="wysiwyg-font-size-medium wysiwyg-color-pink">This article will replace the Support article here: https://support.workfront.com/hc/en-us/articles/217612358-How-Workfront-Calculates-Finances</span></p>
<p><span class="wysiwyg-font-size-medium wysiwyg-color-pink">-- This should be placed at the top of the Project Finances section.)</span> </p>
</div>
-->

## Understanding the Calculations of Adobe Workfront Project Finances

As the project manager, you can manually update some financial fields on projects. Other financial data is calculated automatically by Workfront.

Performance metrics are an example of financial data that is automatically calculated by Workfront.

Performance metrics show how your projects are performing at a given time.

You can measure how your project is performing, by referring to the following calculations:

* Schedule Performance Index (SPI). For more information about calculating SPI, see [Calculate Schedule Performance Index (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)
* Cost Performance Index (CPI). For more information about calculating CPI, see [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).
* Cost Schedule Performance Index (CSI). For more information about calculating CSI, see [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).
* Estimate at Completion (EAC). For more information about calculating EAC, see [Calculate Estimate At Completion (EAC)](../../../manage-work/projects/project-finances/calculate-eac.md).
* Performance Index Method (PMI). For more information about calculating PMI, see [Set the Performance Index Method (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

## Understanding the Fields Which Impact Financial Calculations

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Term</strong> </p> </td> 
   <td> <p><strong>Definition</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Actual Hours</p> </td> 
   <td> <p>The hours recorded against the task. For more information about logging time, see <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref" xrefformat="{para}">Log time</a>.</p> <p>Parent Task Actual Hours = Hours Logged on the Parent + All Hours Logged on the Children Tasks.</p> <p>Project Actual Hours = Hours Logged on the Project + All Hours Logged on All Tasks in the Project.</p> <p> For example, i f from the Updates tab for Task 1, you click ‘Log Time’ and enter 25 hours, the Actual Hours = 25. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Actual Labor Cost</p> </td> 
   <td> <p>The result of multiplying the actual hours by the rate of either the job role or the user, depending on how you decide to track your costs (either by job role or by user). </p> <p>For more information about tracking costs, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref" xrefformat="{para}">Track costs</a>.</p> <p> For example, i f the task is set up to have the Cost Type = User Hourly and the user’s cost per hour on their profile is $100.00, then if you record 5 actual hours, the Actual Labor Cost = $500.00. </p> <p> For more information about setting up the cost for individual tasks, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref" xrefformat="{para}">Track costs</a>.</p> <p> For more information about editing user profile preferences, including cost, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Planned Labor Cost</p> </td> 
   <td> <p>The result of multiplying the Planned Hours by either the job role or the user billing rate. </p> <p> For example, if the task is set up to have the Cost Type = User Hourly and the user’s cost per hour on their profile is $100.00, and if you set the task to take 5 Planned Hours to complete, the Planned Labor Cost = $500.00. </p> <p> For more information about setting up the cost for individual tasks, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref" xrefformat="{para}">Track costs</a>.</p> <p> For more information about editing user profile preferences, including cost, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>IncurredActualExpenseCost</p> </td> 
   <td> <p>The sum of the Actual Amount field for all expenses where the Actual Amount field &gt; 0 and Planned Amount &gt;0.</p> For more information about tracking expenses, see <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref" xrefformat="{para}">Manage project expenses </a>.<br><p>For example, if you create an expense for Task 1 and enter $600.00 in the Actual Amount field, the IncurredActualExpenseCost for this task is $600.00.</p><p><em><strong>IMPORTANT</strong> </em><em>If the values in either the Actual Amount or the Planned Amount fields for an expense are negative, the system will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, or if the Planned Amount is -$200.00 and the Actual Amount is $300.00, the system will ignore this entire expense record which means you would not include the Actual Amount in the IncurredActualExpenseCost calculation. </em></p></td> 
  </tr> 
  <tr> 
   <td> <p>IncurredPlannedExpenseCost </p> </td> 
   <td> <p>The sum of the Planned Amount field for all expenses where the Actual Amount field &gt; 0 and Planned Amount &gt;0.</p> <p> For example, i f you create an expense for Task 1 and enter $500.00 in the Planned Amount field and an amount &gt; 0 in the Actual Amount field (i.e. $600.00), the IncurredPlannedExpenseCost for this task is $500.00. </p> <p> <p>Tip:  If the values in either the Actual Amount or the Planned Amount fields for an expense are negative, the system will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, or if the Planned Amount is -$200.00 and the Actual Amount is $300.00, the system will ignore this entire expense record which means you would not include the Planned Amount in the IncurredPlannedExpenseCost calculation. </p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>NotIncurredPlannedExpense</p> </td> 
   <td> <p>The sum of the Planned Amount field for all expenses where the Actual Amount field = 0. </p> <p> For example, i f you create two expenses for Task 1 where for the first expense the value in the Planned Amount field is $500.00 and the value in the Actual Amount is $600.00 and for the second expense, the value in the Planned Amount field is $300.00 and the value of the Actual Amount field is $0.00, the value of the NotIncurredPlannedExpense for this task is $300.00. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Percent Complete</p> </td> 
   <td> <p>The value entered into the % Complete field for a task.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Planned Hours</p> </td> 
   <td> <p>The value entered into the Planned Hours field on the task.</p> </td> 
  </tr> 
  <tr> 
   <td>TotalBudgetedCostWorkPerformed</td> 
   <td> <p>The result of multiplying the budgeted cost of the work planned (budgeted cost) and the percent of the task that has been completed so far. </p> <p>TotalBudgetedCostWorkPerformed = Planned Hours * (Percent Complete/100)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Understanding Project Settings and How They Affect Project Finance Calculations

Your Workfront administrator sets up the default of how Estimate at Completion (EAC) should be calculated in the system, as well as whether Performance Index Method (PIM) should be hour-based or cost-based. The calculations for the performance metrics change according to how these defaults are set.

For more information about setting up project preferences in Workfront, including how to calculate the Estimate at Completion, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* "Calculating EAC"
* "Calculating EAC Based on the Performance Index Method"
* "Calculating CPI Using Hour-Based PIM"

### Calculating EAC

The Estimate at Completion (EAC) represents the projected total cost of your project or task when it completes.

The Workfront administrator can choose to calculate the EAC in one of the following two ways:

* [Calculate at Project Level](#calculate-at-project-level) 
* [Roll up from Tasks/ Subtasks](#roll-up-from-tasks-subtasks)

**Calculate at Project Level**

EAC for the parent task and project are determined by entering the actual hours/actual labor cost into the EAC Formulas. This calculation includes Actual Hours/ costs and expenses added directly to the parent task or project

**Roll up from Tasks/ Subtasks**

EAC for the parent task and project are determined by summing up the EAC for each child task. This calculation excludes Actual Hours/ costs and expenses added directly to the parent task or project

As a project manager, you can also change this preference at the project level, in the Finance tab of the project. For more information about editing the Finance sub-tab of a project, see [Manage information in the project Finance area](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Calculating EAC Based on the Performance Index Method

The Performance Index Method (PIM) for the project controls the method Workfront uses to calculate performance metrics such as [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) and [Calculate Estimate At Completion (EAC)](../../../manage-work/projects/project-finances/calculate-eac.md). Workfront allows you to choose hour-based or cost-based as the PIM of the project.

* [Calculating EAC Using Hour-Based PIM](#calculating-eac-using-hour-based-pim) 
* [Calculating EAC Using Cost-Based PIM](#calculating-eac-using-cost-based-pim)

In Workfront, the calculation for EAC depends on the selected Performance Index Method (PIM) of the project. For more information about calculating PIM, see [Set the Performance Index Method (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

**Calculating EAC Using Hour-Based PIM**

EAC = Total Planned Hours / CPI&#42;

&#42;If [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = Total Planned Hours + Actual Hours. <this occurs when hours have been captured, but project/task is at 0% complete>

### Calculating EAC Using Cost-Based PIM {#calculating-eac-using-cost-based-pim}

[Calculating EAC Using Cost-Based PIM for Labor Costs Only](#calculating-eac-using-cost-based-pim-for-labor-costs-only)

[Calculating EAC Using Cost-Based PIM for Total Costs](#calculating-eac-using-cost-based-pim-for-total-costs)

**Calculating EAC Using Cost-Based PIM for Labor Costs Only**

When you calculate the EAC using cost-based PIM for labor costs only, you are taking into account the labor cost only.

EAC(labor) = Planned Labor Cost / CPI

&#42;If [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC(labor) = Planned Labor Cost + Actual Labor Cost.

**Calculating EAC Using Cost-Based PIM for Total Costs**

When you calculate the EAC using cost-based PIM for total costs, you are taking into account the total cost.

EAC = EAC(labor) + Total Actual Expenses to Date + Remaining Planned Expenses + Project Fixed Costs&#42;

>[!TIP]
>
>&#42; Project Fixed Costs are ignored for task level EAC.

&nbsp;

### Calculating CPI Using Hour-Based PIM

If Actual Hours > 0 then CPI = TotalBudgetedCostWorkPerformed / Actual Hours

Otherwise, CPI = 1

TotalBudgetedCostWorkPerformed = Planned Hours &#42; (Percent Complete/100)

&nbsp;

# **Formulas**

## **PIM= Hour-based**

### **TotalBudgetedCostWorkPerformed**

**For a non parent task** :

TotalBudgetedCostWorkPerformed = Planned Hours &#42; (Percent Complete/100)

&nbsp;

**For a parent task:**

TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all direct child tasks.

&nbsp;

### **CPI**

* IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

****

### **EAC**

* IF * CPI <> 0 * THEN * EAC = Planned Hours / CPI

* ELSE * EAC = Planned Hours + Actual Hours

****

## **PIM =Cost-Based**

### **TotalBudgetedCostWorkPerformed**

**For a non parent task** :

TotalBudgetedCostWorkPerformed = Planned Labor Cost &#42; (Percent Complete/100)

&nbsp;

**For a parent task:**

TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all direct child tasks.

&nbsp;

### **CPI**

* IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

&nbsp;

### **EAC**

**EAC** = **EAC Labor** + **EAC Expense**

&nbsp;

For EAC Labor, we first need to determine CPI_Labor.

&nbsp;

**CPI_Labor** = IF Actual Labor Cost <> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost

ELSE CPI_Labor = 1

&nbsp;

**EAC Labor** = * IF * CPI_Labor <> 0 * THEN * EAC Labor = Planned Labor Cost / CPI_Labor

* ELSE * EAC Labor = Planned Labor Cost + Actual Labor Cost

****

**EAC Expense** = IncurredActualExpenseCost + NotIncurredPlannedExpense

&nbsp;

# **EAC Method: Calculate at Project Level**

## **PIM = Hour-Based**

### **Simple example: Project has no child tasks**

PIM = Hour-Based

EAC Method = Calculate at project level

&nbsp;

1. Create Project A with three tasks (no child tasks) all assigned to User 1 whose cost/hr is $100.00. 
1. Add planned/actual hours to each task and % Complete according to the table below:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <br> <p><strong>Task</strong> </p> </td> 
   <td> <br> <p><strong>Pln Hrs</strong> </p> </td> 
   <td> <br> <p><strong>Act Hrs</strong> </p> </td> 
   <td> <p><strong>% Complete</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> 5 hrs </p> </td> 
   <td> <p> 25 hrs </p> </td> 
   <td> <p> 20% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> 25 hrs </p> </td> 
   <td> <p> 30% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td> <p> 15 hrs </p> </td> 
   <td> <p> 25 hrs </p> </td> 
   <td> <p> 40% </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Recalculate Finance 
1. **CPI for Task 1** = .04 calculated as follows:

**CPI for Task 1** = * IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

**CPI for Task 1** = 1 / 25

**CPI for Task 1** = .04

&nbsp;

1. **EAC for Task 1** = 125 hrs calculated as follows:

**EAC for Task 1** = * IF * CPI <> 0 * THEN * EAC = Planned Hours / CPI

* ELSE * EAC = Planned Hours + Actual Hours

**EAC for Task 1** = 5 / .04

**EAC for Task 1** = 125 hrs

&nbsp;

1. CPI / EAC for Tasks 2 and 3 are:

Task 2 = .12 / 83.33 hrs

Task 3 = .24 / 62.5 hrs

&nbsp;

1. **CPI for Project** = .13 calculated as follows:

**CPI for Project** = * IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

**CPI for Project** = 10 / 75

**CPI for Project** = .13

&nbsp;

1. **EAC for Project** = 225 hrs calculated as follows:

**EAC for Project** = * IF * CPI <> 0 * THEN * EAC = Planned Hours / CPI

* ELSE * EAC = Planned Hours + Actual Hours

**EAC for Project** = 30 / .13333

**EAC for Project** = 225 hrs

****

### **Complicated Example: Project has child tasks**

PIM = Hour-Based

EAC Method = Calculate at project level

&nbsp;

1. Create Project A with six tasks where Task 3 is the parent of Tasks 4 and 5 and Task 1 is the parent of Tasks 2 and 3 as shown below:

&nbsp;

Task 1

Task 2

Task 3

Task 4

Task 5

Task 6

&nbsp;

1. Assign Tasks 2, 4, 5, and 6 to User 1 whose cost/hr rate is $100.00.

&nbsp;

1. Add planned/actual hours each task and % Complete according to the table below (Note: For Tasks 1 and 3, you are only adding actual hours):

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <br> <p><strong>Task</strong> </p> </td> 
   <td> <br> <p><strong>Pln Hrs</strong> </p> </td> 
   <td> <br> <p><strong>Act Hrs</strong> </p> </td> 
   <td> <p><strong>% Complete</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td>&nbsp;</td> 
   <td> <p> 10 hrs </p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> 5 hrs </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> 20% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td>&nbsp;</td> 
   <td> <p> 10 Hrs </p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 4 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> 40% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 5 </p> </td> 
   <td> <p> 15 hrs </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> 50% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 6 </p> </td> 
   <td> <p> 20 hrs </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> 60% </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Add 50 hours directly to the project (More>Hours>Log Hours). 
1. **CPI for Task 2** = .1 calculated as follows:

**CPI for Task 2** = * IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

**CPI for Task 2** = 1 / 10

**CPI for Task 2** = .1

&nbsp;

1. **EAC for Task 2** = 50 hrs calculated as follows:

**EAC for Task 2** = * IF * CPI <> 0 * THEN * EAC = Planned Hours / CPI

* ELSE * EAC = Planned Hours + Actual Hours

**EAC for Task 2** = 5 / .1

**EAC for Task 2** = 50 hrs

&nbsp;

1. The CPI / EAC for Tasks 4, 5, and 6 are as follows:

Task 4: .4 / 25 hrs

Task 5: .75 / 20 hrs

Task 6: 1.2 / 16.67 hrs

&nbsp;

1. **CPI for Task 3** = .38 calculated as follows:

**CPI for Task 3** = * IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

**CPI for Task 3** = 11.5 / 30

**CPI for Task 3** = .38

&nbsp;

1. **EAC for Task 3** = 65.22 hrs calculated as follows:

**EAC for Task 3** = * IF * CPI <> 0 * THEN * EAC = Planned Hours / CPI

* ELSE * EAC = Planned Hours + Actual Hours

**EAC for Task 3** = 25 / .383333

**EAC for Task 3** = 65.22 hrs

&nbsp;

1. **CPI for Task 1** = .25 calculated as follows:

**CPI for Task 1** = * IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

**CPI for Task 1** = 12.5 / 50

**CPI for Task 1** = .25

&nbsp;

1. **EAC for Task 1** = 120 hrs calculated as follows:

**EAC for Task 1** = * IF * CPI <> 0 * THEN * EAC = Planned Hours / CPI

* ELSE * EAC = Planned Hours + Actual Hours

**EAC for Task 1** = 30/ .25

**EAC for Task 1** = 120 hrs

&nbsp;

1. **CPI for Project** = .22 calculated as follows:

**CPI for Project** = * IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

**CPI for Project** = 24.5 / 110

**CPI for Project** = .22272

**CPI for Project** = .22

****

1. **EAC for Project** = 224.49 hrs calculated as follows:

**EAC for Project** = * IF * CPI <> 0 * THEN * EAC = Planned Hours / CPI

* ELSE * EAC = Planned Hours + Actual Hours

**EAC for Project** = 50 / .22272

**EAC for Project** = 224.49 hrs

****

## **PIM = Cost-Based**

### **Simple Example: Project has no child tasks**

PIM = Cost-Based

EAC Method = Calculate at project level

&nbsp;

1. Create Project A with three tasks (no child tasks) all assigned to User 1 whose cost/hr is $100.00. 
1. Add planned/actual hours to each task and % Complete according to the table below:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <br> <p><strong>Task</strong> </p> </td> 
   <td> <br> <p><strong>Pln Hrs</strong> </p> </td> 
   <td> <br> <p><strong>Pln Lbr Cost</strong> </p> </td> 
   <td> <br> <p><strong>Act Hrs</strong> </p> </td> 
   <td> <br> <p><strong>Act Lbr Cost</strong> </p> </td> 
   <td> <p><strong>% Complete</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> 5 hrs </p> </td> 
   <td> <p> $500.00 </p> </td> 
   <td> <p> 25 hrs </p> </td> 
   <td> <p> $2,500.00 </p> </td> 
   <td> <p> 20% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> 25 hrs </p> </td> 
   <td> <p> $2,500.00 </p> </td> 
   <td> <p> 30% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td> <p> 15 hrs </p> </td> 
   <td> <p> $1,500.00 </p> </td> 
   <td> <p> 25 hrs </p> </td> 
   <td> <p> $2,500.00 </p> </td> 
   <td> <p> 40% </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Add expenses to each task according to the table below:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Task</strong> </p> </td> 
   <td> <p><strong>Expense</strong> </p> </td> 
   <td> <p><strong>Planned Amount</strong> </p> </td> 
   <td> <p><strong>Actual Amount</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> Task 1 Exp 1 </p> </td> 
   <td> <p> $300.00 </p> </td> 
   <td> <p> $400.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> Task 1 Exp 2 </p> </td> 
   <td> <p> $500.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> Task 2 Exp </p> </td> 
   <td> <p> $200.00 </p> </td> 
   <td> <p> $100.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td> <p> Task 3 Exp </p> </td> 
   <td> <p> $800.00 </p> </td> 
   <td> <p> $700.00 </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Add two expenses to the project (i.e. not tied to a task) as follows:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Expense</strong> </p> </td> 
   <td> <p><strong>Planned Amount</strong> </p> </td> 
   <td> <p><strong>Actual Amount</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Project Exp 1 </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> $1,500.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 Exp 2 </p> </td> 
   <td> <p> $2,500.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Based on the above values, the Incurred/Not Incurred Costs are determined as follows:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Task</strong> </p> </td> 
   <td> <p><strong>Not Incurred Planned Expense</strong> </p> </td> 
   <td> <p><strong>Incurred Planned Expense</strong> </p> </td> 
   <td> <p><strong>Incurred Actual Expense</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> $500.00 </p> </td> 
   <td> <p> $300.00 </p> </td> 
   <td> <p> $400.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $200.00 </p> </td> 
   <td> <p> $100.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $800.00 </p> </td> 
   <td> <p> $700.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Project </p> </td> 
   <td> <p> $3,000.00 </p> </td> 
   <td> <p> $2,300.00 </p> </td> 
   <td> <p> $2,700.00 </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. From Project Actions, run Recalculate Finance 
1. **CPI for Task 1** = .14 
1. **CPI****for Task 1** = .14 calculated as follows:

**CPI****for Task 1** = * IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

&nbsp;

**CPI****for Task 1** = (100+300) / (2500+400)

**CPI****for Task 1** = 400 / 2900

**CPI****for Task 1** = .14

&nbsp;

1. **EAC****for Task 1** = $13,400.00

**CPI Labor****for Task 1** = IF Actual Labor Cost <> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost

ELSE CPI_Labor = 1

**CPI Labor****for Task 1** = 100/2500

**CPI Labor****for Task 1** = .04

&nbsp;

**EAC Labor****for Task 1** = * IF * CPI_Labor <> 0 * THEN * EAC Labor = Planned Labor Cost / CPI_Labor

* ELSE * EAC Labor = Planned Labor Cost + Actual Labor Cost

**EAC Labor****for Task 1** = 500.00/.04

**EAC Labor****for Task 1** = $12,500.00

&nbsp;

**EAC Expense****for Task 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense

**EAC Expense****for Task 1** = $400.00 + $500.00

**EAC Expense****for Task 1** = $900.00

&nbsp;

**EAC****for Task 1** = EAC Labor + EAC Expense

**EAC****for Task 1** = $12,500.00 + $900.00

**EAC****for Task 1** = $13,400.00

&nbsp;

1. Here are the CPI / EAC values for Task 2 and Task 3:

Task 2 = .19 / $8,433.33

Task 3 = .44 / $6,950.00

&nbsp;

1. **CPI for Project** = .32 calculated as follows:

**CPI****for Project** = * IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

**CPI****for Project** = (1000 + 2300) / (7500 + 2700)

**CPI****for Project** = 3300 / 10200

**CPI****for Project** = .32

&nbsp;

1. **EAC for Project** = $28,200.00 calculated as follows:

**CPI Labor****for Project** = IF Actual Labor Cost <> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost

ELSE CPI_Labor = 1

**CPI Labor****for Project** = 1000 / 7500

**CPI Labor****for Project** = .13333

**CPI Labor****for Project** = .13

&nbsp;

**EAC Labor****for Project** = * IF * CPI_Labor <> 0 * THEN * EAC Labor = Planned Labor Cost / CPI_Labor

* ELSE * EAC Labor = Planned Labor Cost + Actual Labor Cost

**EAC Labor****for Project** = 3000/ .13333

**EAC Labor****for Project** = $22,500.00

&nbsp;

**EAC Expense****Project** = IncurredActualExpenseCost + NotIncurredPlannedExpense

**EAC Expense****Project** = $3000.00 + 2,700.00

**EAC Expense****Project** = $5,700.00

&nbsp;

**EAC****Project** = EAC Labor + EAC Expense

**EAC****Project** = $22,500.00 + $5,700.00

**EAC****Project** = $28,200.00

****

### **Complicated Example: Project has child tasks**

PIM = Cost-Based

EAC Method = Calculate at project level

&nbsp;

1. Create Project A with six tasks where Task 3 is the parent of Tasks 4 and 5 and Task 1 is the parent of Tasks 2 and 3 as shown below:

&nbsp;

Task 1

Task 2

Task 3

Task 4

Task 5

Task 6

&nbsp;

1. Assign Tasks 2, 4, 5, and 6 to User 1 whose cost/hr rate is $100.00.

&nbsp;

1. Add planned/actual hours each task and % Complete according to the table below (Note: For Tasks 1 and 3, you are only adding actual hours):

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <br> <p><strong>Task</strong> </p> </td> 
   <td> <br> <p><strong>Pln Hrs</strong> </p> </td> 
   <td> <br> <p><strong>Pln Lbr Cost</strong> </p> </td> 
   <td> <br> <p><strong>Act Hrs</strong> </p> </td> 
   <td> <br> <p><strong>Act Lbr Cost</strong> </p> </td> 
   <td> <p><strong>% Complete</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> 5 hrs </p> </td> 
   <td> <p> $500.00 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> 20% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td> <p> 10 Hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 4 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> 40% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 5 </p> </td> 
   <td> <p> 15 hrs </p> </td> 
   <td> <p> $1,500.00 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> 50% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 6 </p> </td> 
   <td> <p> 20 hrs </p> </td> 
   <td> <p> $2,000.00 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> 60% </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Add 50 hours directly to the project (More>Hours>Log Hours) so that there is $5,000.00 of actual labor cost recorded directly to the project.

&nbsp;

1. Add expenses to each task according to the table below (I’ve added a blank row in between each task to make it easier to read):

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Task</strong> </p> </td> 
   <td> <p><strong>Expense</strong> </p> </td> 
   <td> <p><strong>Planned Amount</strong> </p> </td> 
   <td> <p><strong>Actual Amount</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> Task 1 Exp 1 </p> </td> 
   <td> <p> $300.00 </p> </td> 
   <td> <p> -$400.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> Task 1 Exp 2 </p> </td> 
   <td> <p> -$500.00 </p> </td> 
   <td> <p> $800.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> Task 1 Exp 3 </p> </td> 
   <td> <p> $400.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> Task 2 Exp 1 </p> </td> 
   <td> <p> $500.00 </p> </td> 
   <td> <p> $700.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> Task 2 Exp 2 </p> </td> 
   <td> <p> -$400.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> Task 2 Exp 3 </p> </td> 
   <td> <p> -$200.00 </p> </td> 
   <td> <p> $600.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> Task 2 Exp 4 </p> </td> 
   <td> <p> $700.00 </p> </td> 
   <td> <p> -$200.00 </p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td> <p> Task 3 Exp </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 4 </p> </td> 
   <td> <p> Task 4 Exp 1 </p> </td> 
   <td> <p> $800.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 4 </p> </td> 
   <td> <p> Task 4 Exp 2 </p> </td> 
   <td> <p> -$100.00 </p> </td> 
   <td> <p> $300.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 4 </p> </td> 
   <td> <p> Task 4 Exp 3 </p> </td> 
   <td> <p> -200.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 5 </p> </td> 
   <td> <p> Task 5 Exp 1 </p> </td> 
   <td> <p> $700.00 </p> </td> 
   <td> <p> $800.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 5 </p> </td> 
   <td> <p> Task 5 Exp 2 </p> </td> 
   <td> <p> -$100.00 </p> </td> 
   <td> <p> $300.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 5 </p> </td> 
   <td> <p> Task 5 Exp 3 </p> </td> 
   <td> <p> -$400.00 </p> </td> 
   <td> <p> -$200.00 </p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 6 </p> </td> 
   <td> <p> Task 6 Exp 1 </p> </td> 
   <td> <p> $600.00 </p> </td> 
   <td> <p> $700.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 6 </p> </td> 
   <td> <p> Task 6 Exp 2 </p> </td> 
   <td> <p> $500.00 </p> </td> 
   <td> <p> -$300.00 </p> </td> 
  </tr> 
 </tbody> 
</table>

****

1. Add two expenses to the project (i.e. not tied to a task) as follows:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Expense</strong> </p> </td> 
   <td> <p><strong>Planned Amount</strong> </p> </td> 
   <td> <p><strong>Actual Amount</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Project Exp 1 </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> $1,500.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 Exp 2 </p> </td> 
   <td> <p> $2,500.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Based on the above values, the Incurred/Not Incurred Costs are determined as follows:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Task</strong> </p> </td> 
   <td> <p><strong>Not Incurred Planned Expense</strong> </p> </td> 
   <td> <p><strong>Incurred Planned Expense</strong> </p> </td> 
   <td> <p><strong>Incurred Actual Expense</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> $400.00 </p> </td> 
   <td> <p> -$500.00 </p> </td> 
   <td> <p> $800.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> -$400.00 </p> </td> 
   <td> <p> $300.00 </p> </td> 
   <td> <p> $1,300.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 4 </p> </td> 
   <td> <p> $600.00 </p> </td> 
   <td> <p> -$100.00 </p> </td> 
   <td> <p> $300.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 5 </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $600.00 </p> </td> 
   <td> <p> $1,100.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 6 </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $600.00 </p> </td> 
   <td> <p> $700.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Project </p> </td> 
   <td> <p> $2,500.00 </p> </td> 
   <td> <p> $1000.00 </p> </td> 
   <td> <p> $1,500.00 </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

&nbsp;

1. From Project Actions, run Recalculate Finance 
1. **CPI** for Task 2 = .17 calculated as follows:

**CPI Task 2** = * IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

&nbsp;

**CPI****Task 2** = (100+300) / (1000+1300)

**CPI****Task 2** = 400 / 2300

**CPI****Task 2** = .17

&nbsp;

1. **EAC** for Task 2 = $5,900.00

**CPI Labor****Task 2** = IF Actual Labor Cost <> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost

ELSE CPI_Labor = 1

**CPI Labor****Task 2** = 100/1000

**CPI Labor****Task 2** = .1

&nbsp;

**EAC Labor****Task 2** = * IF * CPI_Labor <> 0 * THEN * EAC Labor = Planned Labor Cost / CPI_Labor

* ELSE * EAC Labor = Planned Labor Cost + Actual Labor Cost

**EAC Labor****Task 2** = 500.00/.1

**EAC Labor****Task 2** = $5,000.00

&nbsp;

**EAC Expense****Task 2** = IncurredActualExpenseCost + NotIncurredPlannedExpense

**EAC Expense****Task 2** = $1,300.00 + -$400.00

**EAC Expense****Task 2** = $900.00

&nbsp;

**EAC****Task 2** = EAC Labor + EAC Expense

**EAC****Task 2** = $5,000.00 + $900.00

**EAC****Task 2** = $5,900.00

&nbsp;

1. The CPI/EAC for Tasks 4, 5, and 6 are determined the same way so I’ll just provide those values below:

Task 4: .23 / $3,400.00

Task 5: .64 / $3,100.00

Task 6: 1.06 / $2,366.67

&nbsp;

1. CPI for Task 3 = .31 calculated as follows:

**CPI****Task 3** = * IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

&nbsp;

**CPI****Task 3** = (1,150 + 500) / (3000 + 2400)

**CPI****Task 3** = 1650 / 5400

**CPI****Task 3** = .31

&nbsp;

**EAC for Task 3** = $9,521.74 calculated as follows:

**CPI Labor****Task 3** = IF Actual Labor Cost <> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost

ELSE CPI_Labor = 1

**CPI Labor****Task 3** = 1150/3000

**CPI Labor****Task 3** = .383333

**CPI Labor****Task 3** = .38

****

**EAC Labor****Task 3** = * IF * CPI_Labor <> 0 * THEN * EAC Labor = Planned Labor Cost / CPI_Labor

* ELSE * EAC Labor = Planned Labor Cost + Actual Labor Cost

**EAC Labor****Task 3** = $2,500.00 / .383333

**EAC Labor****Task 3** = $6,521.74

&nbsp;

**EAC Expense****Task 3** = IncurredActualExpenseCost + NotIncurredPlannedExpense

**EAC Expense****Task 3** = $2,400.00 + $600.00

**EAC Expense****Task 3** = $3,000.00

&nbsp;

**EAC****Task 3** = EAC Labor + EAC Expense

**EAC****Task 3** = $6,521.74 + $3,000.00

**EAC****Task 3** = $9,521.74

&nbsp;

1. CPI for Task 1 = .16 calculated as follows:

**CPI****Task 1** = * IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

&nbsp;

**CPI****Task 1** = (1250 + 300) / (5000 + 4500)

**CPI****Task 1** = 1550 / 9500

**CPI****Task 1** = .16

&nbsp;

1. EAC for Task 1 is $17,100.00 calculated as follows:

**CPI Labor****Task 1** = IF Actual Labor Cost <> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost

ELSE CPI_Labor = 1

**CPI Labor****Task 1** = 1250 / 5000

**CPI Labor****Task 1** = .25

&nbsp;

**EAC Labor****Task 1** = * IF * CPI_Labor <> 0 * THEN * EAC Labor = Planned Labor Cost / CPI_Labor

* ELSE * EAC Labor = Planned Labor Cost + Actual Labor Cost

**EAC Labor****Task 1** = $3,000.00 / .25

**EAC Labor****Task 1** = $12,000.00

&nbsp;

**EAC Expense****Task 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense

**EAC Expense****Task 1** = $4500 + 600

**EAC Expense****Task 1** = $5,100.00

&nbsp;

**EAC****Task 1** = EAC Labor + EAC Expense

**EAC****Task 1** = $12,000.00 + 5,100.00

**EAC****Task 1** = $17,100.00

&nbsp;

1. CPI for Project is .25

**CPI****for Project** = * IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

&nbsp;

**CPI****for Project** = (2450 + 1900) / (11000 + 6700)

**CPI****for Project** = 4350 / 17700

**CPI****for Project** = .25

&nbsp;

1. **EAC for Project** = $32,248.98 calculated as follows:

**CPI Labor****for Project** = IF Actual Labor Cost <> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost

ELSE CPI_Labor = 1

**CPI Labor****for Project** = 2450 / 11000

**CPI Labor****for Project** = .22272

**CPI Labor****for Project** = .22

&nbsp;

**EAC Labor****for Project** = * IF * CPI_Labor <> 0 * THEN * EAC Labor = Planned Labor Cost / CPI_Labor

* ELSE * EAC Labor = Planned Labor Cost + Actual Labor Cost

**EAC Labor****for Project** = $5,000.00 / .22272

**EAC Labor****for Project** = $22,448.97959

**EAC Labor****for Project** = $22,448.98

&nbsp;

**EAC Expense****Project** = IncurredActualExpenseCost + NotIncurredPlannedExpense

**EAC Expense****Project** = $3,100.00 + $6,700.00

**EAC Expense****Project** = $9,800.00

&nbsp;

**EAC****Project** = EAC Labor + EAC Expense

**EAC****Project** = $22,448.98 + 9,800.00

**EAC****Project** = $32,248.98

&nbsp;

# **EAC Method: Roll up from tasks/subtasks**

## **PIM = Hour-Based**

### **Simple Example: Project has no child tasks**

PIM = Hour-Based

EAC Method = Roll up from tasks/subtasks

&nbsp;

1. Create Project A with three tasks (no child tasks) all assigned to User 1 whose cost/hr is $100.00. 
1. Add planned/actual hours to each task and % Complete according to the table below:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <br> <p><strong>Task</strong> </p> </td> 
   <td> <br> <p><strong>Pln Hrs</strong> </p> </td> 
   <td> <br> <p><strong>Act Hrs</strong> </p> </td> 
   <td> <p><strong>% Complete</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> 5 hrs </p> </td> 
   <td> <p> 25 hrs </p> </td> 
   <td> <p> 20% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> 25 hrs </p> </td> 
   <td> <p> 30% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td> <p> 15 hrs </p> </td> 
   <td> <p> 25 hrs </p> </td> 
   <td> <p> 40% </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Recalculate Finance 
1. **CPI for Task 1** = .04 calculated as follows:

**CPI for Task 1** = * IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

**CPI for Task 1** = 1 / 25

**CPI for Task 1** = .04

&nbsp;

1. **EAC for Task 1** = 125 hrs calculated as follows:

**EAC for Task 1** = * IF * CPI <> 0 * THEN * EAC = Planned Hours / CPI

* ELSE * EAC = Planned Hours + Actual Hours

**EAC for Task 1** = 5 / .04

**EAC for Task 1** = 125 hrs

&nbsp;

1. CPI / EAC for Tasks 2 and 3 are:

Task 2 = .12 / 83.33 hrs

Task 3 = .24 / 62.5 hrs

&nbsp;

1. **CPI for Project** = .13 calculated as follows:

**CPI for Project** = * IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

**CPI for Project** = 10 / 75

**CPI for Project** = .13

&nbsp;

1. **EAC for Project** = 270.83 hrs calculated as follows

**EAC for Project** = EAC Task 1 + EAC Task 2 + EAC Task 3

**EAC for Project** = 125 + 83.33 + 62.5

**EAC for Project** = 270.83 hrs

****

### **Complicated Example: Project has child tasks**

PIM = Hour-Based

EAC Method = Roll up from tasks/subtasks

&nbsp;

1. Create Project A with six tasks where Task 3 is the parent of Tasks 4 and 5 and Task 1 is the parent of Tasks 2 and 3 as shown below:

&nbsp;

Task 1

Task 2

Task 3

Task 4

Task 5

Task 6

&nbsp;

1. Assign Tasks 2, 4, 5, and 6 to User 1 whose cost/hr rate is $100.00.

&nbsp;

1. Add planned/actual hours each task and % Complete according to the table below (Note: For Tasks 1 and 3, you are only adding actual hours):

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <br> <p><strong>Task</strong> </p> </td> 
   <td> <br> <p><strong>Pln Hrs</strong> </p> </td> 
   <td> <br> <p><strong>Act Hrs</strong> </p> </td> 
   <td> <p><strong>% Complete</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td>&nbsp;</td> 
   <td> <p> 10 hrs </p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> 5 hrs </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> 20% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td>&nbsp;</td> 
   <td> <p> 10 Hrs </p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 4 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> 40% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 5 </p> </td> 
   <td> <p> 15 hrs </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> 50% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 6 </p> </td> 
   <td> <p> 20 hrs </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> 60% </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Add 50 hours directly to the project (More>Hours>Log Hours) so that there is $5,000.00 of actual labor cost recorded directly to the project.

&nbsp;

1. Run Recalculate Finance 
1. **CPI for Task 2** = .1 calculated as follows:

**CPI for Task 2** = * IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

**CPI for Task 2** = 1 / 10

**CPI for Task 2** = .1

&nbsp;

1. **EAC for Task 2** = 50 hrs calculated as follows:

**EAC for Task 2** = * IF * CPI <> 0 * THEN * EAC = Planned Hours / CPI

* ELSE * EAC = Planned Hours + Actual Hours

**EAC for Task 2** = 5 / .1

**EAC for Task 2** = 50 hrs

&nbsp;

1. CPI / EAC for Task 4, Task 5, and Task 6:

Task 4 = .4 / 25 hrs

Task 5 = .75 / 20 hrs

Task 6 = 1.2 / 16.67 hrs

&nbsp;

1. **CPI for Task 3** = .38

**CPI for Task 3** = * IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

**CPI for Task 3** = 11.5 / 30

**CPI for Task 3** = .38

&nbsp;

1. **EAC for Task 3** = EAC Task 4 + EAC Task 5

**EAC for Task 3** = 25 + 20

**EAC for Task 3** = 45 hrs

&nbsp;

1. **CPI for Task 1** = .25 calculated as follows:

**CPI for Task 1** = * IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

**CPI for Task 1** = 12.5 / 50

**CPI for Task 1** = .25

&nbsp;

1. **EAC for Task 1** = EAC Task 2 + EAC Task 3

**EAC for Task 1** = 50 + 45

**EAC for Task 1** = 95 hrs

&nbsp;

1. CPI for Project = .22 calculated as follows:

**CPI for Project** = * IF * Actual Hours > 0 * THEN * CPI = TotalBudgetedCostWorkPerformed / Actual Hours

* ELSE * CPI = 1

**CPI for Project** = 24.5 / 110

**CPI for Project** = .22272

**CPI for Project** = .22

&nbsp;

1. **EAC for project** = EAC Task 1 + EAC Task 6

**EAC for project** = 95 + 16.67

**EAC for project** = 111.67 hrs

****

&nbsp;

## **PIM = Cost-Based**

### **Simple Example: Project has no child tasks**

PIM = Cost-Based

EAC Method = Roll up from tasks/subtasks

&nbsp;

1. Create Project A with three tasks (no child tasks) all assigned to User 1 whose cost/hr is $100.00. 
1. Add planned/actual hours to each task and % Complete according to the table below:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <br> <p><strong>Task</strong> </p> </td> 
   <td> <br> <p><strong>Pln Hrs</strong> </p> </td> 
   <td> <br> <p><strong>Pln Lbr Cost</strong> </p> </td> 
   <td> <br> <p><strong>Act Hrs</strong> </p> </td> 
   <td> <br> <p><strong>Act Lbr Cost</strong> </p> </td> 
   <td> <p><strong>% Complete</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> 5 hrs </p> </td> 
   <td> <p> $500.00 </p> </td> 
   <td> <p> 25 hrs </p> </td> 
   <td> <p> $2,500.00 </p> </td> 
   <td> <p> 20% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> 25 hrs </p> </td> 
   <td> <p> $2,500.00 </p> </td> 
   <td> <p> 30% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td> <p> 15 hrs </p> </td> 
   <td> <p> $1,500.00 </p> </td> 
   <td> <p> 25 hrs </p> </td> 
   <td> <p> $2,500.00 </p> </td> 
   <td> <p> 40% </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Add expenses to each task according to the table below:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Task</strong> </p> </td> 
   <td> <p><strong>Expense</strong> </p> </td> 
   <td> <p><strong>Planned Amount</strong> </p> </td> 
   <td> <p><strong>Actual Amount</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> Task 1 Exp 1 </p> </td> 
   <td> <p> $300.00 </p> </td> 
   <td> <p> $400.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> Task 1 Exp 2 </p> </td> 
   <td> <p> $500.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> Task 2 Exp </p> </td> 
   <td> <p> $200.00 </p> </td> 
   <td> <p> $100.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td> <p> Task 3 Exp </p> </td> 
   <td> <p> $800.00 </p> </td> 
   <td> <p> $700.00 </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Add two expenses to the project (i.e. not tied to a task) as follows:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Expense</strong> </p> </td> 
   <td> <p><strong>Planned Amount</strong> </p> </td> 
   <td> <p><strong>Actual Amount</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Project Exp 1 </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> $1,500.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 Exp 2 </p> </td> 
   <td> <p> $2,500.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Based on the above values, the Incurred/Not Incurred Costs are determined as follows:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Task</strong> </p> </td> 
   <td> <p><strong>Not Incurred Planned Expense</strong> </p> </td> 
   <td> <p><strong>Incurred Planned Expense</strong> </p> </td> 
   <td> <p><strong>Incurred Actual Expense</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> $500.00 </p> </td> 
   <td> <p> $300.00 </p> </td> 
   <td> <p> $400.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $200.00 </p> </td> 
   <td> <p> $100.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $800.00 </p> </td> 
   <td> <p> $700.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Project </p> </td> 
   <td> <p> $3,000.00 </p> </td> 
   <td> <p> $2,300.00 </p> </td> 
   <td> <p> $2,700.00 </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. From Project Actions, run Recalculate Finance 
1. **CPI****for Task 1** = .14 calculated as follows:

**CPI****for Task 1** = * IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

&nbsp;

**CPI****for Task 1** = (100+300) / (2500+400)

**CPI****for Task 1** = 400 / 2900

**CPI****for Task 1** = .14

&nbsp;

1. **EAC****for Task 1** = $13,400.00

**CPI Labor****for Task 1** = IF Actual Labor Cost <> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost

ELSE CPI_Labor = 1

**CPI Labor****for Task 1** = 100/2500

**CPI Labor****for Task 1** = .04

&nbsp;

**EAC Labor****for Task 1** = * IF * CPI_Labor <> 0 * THEN * EAC Labor = Planned Labor Cost / CPI_Labor

* ELSE * EAC Labor = Planned Labor Cost + Actual Labor Cost

**EAC Labor****for Task 1** = 500.00/.04

**EAC Labor****for Task 1** = $12,500.00

&nbsp;

**EAC Expense****for Task 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense

**EAC Expense****for Task 1** = $400.00 + $500.00

**EAC Expense****for Task 1** = $900.00

&nbsp;

**EAC****for Task 1** = EAC Labor + EAC Expense

**EAC****for Task 1** = $12,500.00 + $900.00

**EAC****for Task 1** = $13,400.00

****

1. Here are the CPI / EAC values for Task 2 and Task 3:

Task 2 = .19 / $8,433.33

Task 3 = .44 / $6,950.00

&nbsp;

1. The CPI for the project = .32

**CPI****for Project** = * IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

**CPI****for Project** = (1000 + 2300) / (7500 + 2700)

**CPI****for Project** = 3300 / 10200

**CPI****for Project** = .32

&nbsp;

1. EAC for the project is $28,783.33

**EAC****for Project** = EAC Task 1 + EAC Task 2 + EAC Task 3

**EAC****for Project** = $13,400.00 + $8,433.33 + $6,950.00

**EAC****for Project** = $28,783.33

&nbsp;

&nbsp;

### **Complicated Example: Project has child tasks**

PIM = Cost-Based

EAC Method = Roll up from tasks/subtasks

&nbsp;

1. Create Project A with six tasks where Task 3 is the parent of Tasks 4 and 5 and Task 1 is the parent of Tasks 2 and 3 as shown below:

&nbsp;

Task 1

Task 2

Task 3

Task 4

Task 5

Task 6

&nbsp;

1. Assign Tasks 2, 4, 5, and 6 to User 1 whose cost/hr rate is $100.00.

&nbsp;

1. Add planned/actual hours each task and % Complete according to the table below (Note: For Tasks 1 and 3, you are only adding actual hours):

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <br> <p><strong>Task</strong> </p> </td> 
   <td> <br> <p><strong>Pln Hrs</strong> </p> </td> 
   <td> <br> <p><strong>Pln Lbr Cost</strong> </p> </td> 
   <td> <br> <p><strong>Act Hrs</strong> </p> </td> 
   <td> <br> <p><strong>Act Lbr Cost</strong> </p> </td> 
   <td> <p><strong>% Complete</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> 5 hrs </p> </td> 
   <td> <p> $500.00 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> 20% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td> <p> 10 Hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 4 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> 40% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 5 </p> </td> 
   <td> <p> 15 hrs </p> </td> 
   <td> <p> $1,500.00 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> 50% </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 6 </p> </td> 
   <td> <p> 20 hrs </p> </td> 
   <td> <p> $2,000.00 </p> </td> 
   <td> <p> 10 hrs </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> 60% </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Add 50 hours directly to the project (More>Hours>Log Hours) so that there is $5,000.00 of actual labor cost recorded directly to the project.

&nbsp;

1. Add expenses to each task according to the table below (I’ve added a blank row in between each task to make it easier to read):

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Task</strong> </p> </td> 
   <td> <p><strong>Expense</strong> </p> </td> 
   <td> <p><strong>Planned Amount</strong> </p> </td> 
   <td> <p><strong>Actual Amount</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> Task 1 Exp 1 </p> </td> 
   <td> <p> $300.00 </p> </td> 
   <td> <p> -$400.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> Task 1 Exp 2 </p> </td> 
   <td> <p> -$500.00 </p> </td> 
   <td> <p> $800.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> Task 1 Exp 3 </p> </td> 
   <td> <p> $400.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> Task 2 Exp 1 </p> </td> 
   <td> <p> $500.00 </p> </td> 
   <td> <p> $700.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> Task 2 Exp 2 </p> </td> 
   <td> <p> -$400.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> Task 2 Exp 3 </p> </td> 
   <td> <p> -$200.00 </p> </td> 
   <td> <p> $600.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> Task 2 Exp 4 </p> </td> 
   <td> <p> $700.00 </p> </td> 
   <td> <p> -$200.00 </p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td> <p> Task 3 Exp </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 4 </p> </td> 
   <td> <p> Task 4 Exp 1 </p> </td> 
   <td> <p> $800.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 4 </p> </td> 
   <td> <p> Task 4 Exp 2 </p> </td> 
   <td> <p> -$100.00 </p> </td> 
   <td> <p> $300.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 4 </p> </td> 
   <td> <p> Task 4 Exp 3 </p> </td> 
   <td> <p> -200.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 5 </p> </td> 
   <td> <p> Task 5 Exp 1 </p> </td> 
   <td> <p> $700.00 </p> </td> 
   <td> <p> $800.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 5 </p> </td> 
   <td> <p> Task 5 Exp 2 </p> </td> 
   <td> <p> -$100.00 </p> </td> 
   <td> <p> $300.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 5 </p> </td> 
   <td> <p> Task 5 Exp 3 </p> </td> 
   <td> <p> -$400.00 </p> </td> 
   <td> <p> -$200.00 </p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p> Task 6 </p> </td> 
   <td> <p> Task 6 Exp 1 </p> </td> 
   <td> <p> $600.00 </p> </td> 
   <td> <p> $700.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 6 </p> </td> 
   <td> <p> Task 6 Exp 2 </p> </td> 
   <td> <p> $500.00 </p> </td> 
   <td> <p> -$300.00 </p> </td> 
  </tr> 
 </tbody> 
</table>

****

1. Add two expenses to the project (i.e. not tied to a task) as follows:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Expense</strong> </p> </td> 
   <td> <p><strong>Planned Amount</strong> </p> </td> 
   <td> <p><strong>Actual Amount</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Project Exp 1 </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
   <td> <p> $1,500.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 Exp 2 </p> </td> 
   <td> <p> $2,500.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. Based on the above values, the Incurred/Not Incurred Costs are determined as follows:

&nbsp;

<table> 
 <tbody> 
  <tr> 
   <td> <p><strong>Task</strong> </p> </td> 
   <td> <p><strong>Not Incurred Planned Expense</strong> </p> </td> 
   <td> <p><strong>Incurred Planned Expense</strong> </p> </td> 
   <td> <p><strong>Incurred Actual Expense</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 1 </p> </td> 
   <td> <p> $400.00 </p> </td> 
   <td> <p> -$500.00 </p> </td> 
   <td> <p> $800.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 2 </p> </td> 
   <td> <p> -$400.00 </p> </td> 
   <td> <p> $300.00 </p> </td> 
   <td> <p> $1,300.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 3 </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $1,000.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 4 </p> </td> 
   <td> <p> $600.00 </p> </td> 
   <td> <p> -$100.00 </p> </td> 
   <td> <p> $300.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 5 </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $600.00 </p> </td> 
   <td> <p> $1,100.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Task 6 </p> </td> 
   <td> <p> $0.00 </p> </td> 
   <td> <p> $600.00 </p> </td> 
   <td> <p> $700.00 </p> </td> 
  </tr> 
  <tr> 
   <td> <p> Project </p> </td> 
   <td> <p> $2,500.00 </p> </td> 
   <td> <p> $1000.00 </p> </td> 
   <td> <p> $1,500.00 </p> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

1. From Project Actions, run Recalculate Finance 
1. **CPI****for Task 2** = .17 calculated as follows:

**CPI Task 2** = * IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

&nbsp;

**CPI****Task 2** = (100+300) / (1000+1300)

**CPI****Task 2** = 400 / 2300

**CPI****Task 2** = .17

&nbsp;

1. **EAC****for Task 2** = $5,900.00

**CPI Labor****Task 2** = IF Actual Labor Cost <> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost

ELSE CPI_Labor = 1

**CPI Labor****Task 2** = 100/1000

**CPI Labor****Task 2** = .1

&nbsp;

**EAC Labor****Task 2** = * IF * CPI_Labor <> 0 * THEN * EAC Labor = Planned Labor Cost / CPI_Labor

* ELSE * EAC Labor = Planned Labor Cost + Actual Labor Cost

**EAC Labor****Task 2** = 500.00/.1

**EAC Labor****Task 2** = $5,000.00

&nbsp;

**EAC Expense****Task 2** = IncurredActualExpenseCost + NotIncurredPlannedExpense

**EAC Expense****Task 2** = $1,300.00 + -$400.00

**EAC Expense****Task 2** = $900.00

&nbsp;

**EAC****Task 2** = EAC Labor + EAC Expense

**EAC****Task 2** = $5,000.00 + $900.00

**EAC****Task 2** = $5,900.00

&nbsp;

1. The CPI/EAC for Tasks 4, 5, and 6 are determined the same way so I’ll just provide those values below:

Task 4: .23 / $3,400.00

Task 5: .64 / $3,100.00

Task 6: 1.06 / $2,366.67

&nbsp;

1. **CPI for Task 3** = .31 calculated as follows:

**CPI****Task 3** = * IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

&nbsp;

**CPI****Task 3** = (1,150 + 500) / (3000 + 2400)

**CPI****Task 3** = 1650 / 5400

**CPI****Task 3** = .31

&nbsp;

1. **EAC for Task 3** = EAC Task 4 + EAC Task 5

**EAC for Task 3** $3,400.00 + $3,100.00

**EAC for Task 3** = $6,500.00

&nbsp;

1. **CPI for Task 1** = .16 calculated as follows:

**CPI****Task 1** = * IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

&nbsp;

**CPI****Task 1** = (1250 + 300) / (5000 + 4500)

**CPI****Task 1** = 1550 / 9500

**CPI****Task 1** = .16

&nbsp;

1. **EAC for Task 1** = EAC Task 2 + EAC Task 3

**EAC for Task 1** = 5900 + 6500

**EAC for Task 1** = $12,400.00

&nbsp;

1. Project CPI = .25 calculated as follows:

**CPI****for Project** = * IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN * CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)

* ELSE * CPI = CPI_Labor

&nbsp;

**CPI****for Project** = (2450 + 1900) / (11000 + 6700)

**CPI****for Project** = 4350 / 17700

**CPI****for Project** = .25

&nbsp;

1. **EAC for Project** = EAC Task 1 + EAC Task 6

**EAC for Project** = $12,400.00 + $2,366.67

**EAC for Project** = $14,766.67

**** 
