---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Calculation Example - Calculate EAC as a Roll up from Tasks
description: This article gives an example of calculating the Estimate At Completio (EAC) of a project as a roll-up from all the tasks on the project in Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
---
# Calculation example - Calculate EAC as a roll up from tasks

## EAC method: roll up from tasks or subtasks

* [PIM= Hour-Based](#pim-hour-based) 
* [PIM= Cost-Based](#pim-cost-based)

### PIM= Hour-Based {#pim-hour-based}

* [Simple example: project has no children tasks](#simple-example-project-has-no-children-tasks) 
* [Complicated example: project has children tasks](#complicated-example-project-has-children-tasks)

#### Simple example: project has no children tasks {#simple-example-project-has-no-children-tasks}

PIM = Hour-Based

EAC Method = Roll up from tasks/ subtasks

1. Create Project A with three tasks (no child tasks) all assigned to User 1 whose cost/hr is $100.00. 
1. Add planned/ actual hours to each task and % Complete according to the table below:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Task</strong> </p> </th> 
   <th> <br> <p><strong>Pln Hrs</strong> </p> </th> 
   <th> <br> <p><strong>Act Hrs</strong> </p> </th> 
   <th> <p><strong>% Complete</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Task 1</p> </td> 
   <td> <p>5 hrs</p> </td> 
   <td> <p>25 hrs</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 2</p> </td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>25 hrs</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 3</p> </td> 
   <td> <p>15 hrs</p> </td> 
   <td> <p>25 hrs</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Recalculate Finance 
1. **CPI for Task 1** = .04 calculated as follows:  
   **CPI for Task 1** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours  
   &nbsp; &nbsp;&nbsp;*ELSE* CPI = 1  
   **CPI for Task 1** = 1 / 25  
   **CPI for Task 1** = .04

1. **EAC for Task 1** = 125 hrs calculated as follows:  
   **EAC for Task 1** = *IF* CPI <> 0 *THEN* EAC = Planned Hours/ CPI  
   &nbsp; &nbsp;&nbsp;*ELSE* 

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC for Task 1** = 5 / .04  
   **EAC for Task 1** = 125 hrs

1. CPI / EAC for Tasks 2 and 3 are:  
   Task &nbsp;2 = .12 / 83.33 &nbsp;hrs  
   Task 3 = .24 / 62.5 hrs

1. **CPI for Project** = .13 calculated as follows:  
   **CPI for Project** = *IF* Actual Hours > 0 *THEN* 

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   &nbsp; &nbsp;&nbsp;*ELSE* CPI = 1  
   **CPI for Project** = 10 / 75  
   **CPI for Project** = .13

1. **EAC for Project** = 270.83 hrs calculated as follows  
   **EAC for Project** = EAC Task 1 + EAC Task 2 + EAC Task 3  
   **EAC for Project** = 125 + 83.33 + 62.5  
   **EAC for Project** = 270.83 hrs

#### Complicated example: project has children tasks {#complicated-example-project-has-children-tasks}

PIM = Hour-Based

EAC Method = Roll up from tasks/ subtasks

1. Create Project A with six tasks where Task 3 is the parent of Tasks 4 and 5 and Task 1 is the parent of Tasks 2 and 3 as shown below:  
   Task 1  
   &nbsp; &nbsp;Task 2  
   &nbsp; &nbsp;Task 3  
   &nbsp; &nbsp; &nbsp; Task 4  
   &nbsp; &nbsp; &nbsp; Task 5  
   Task 6

1. Assign Tasks 2, 4, 5, and 6 to User 1 whose cost/hr rate is $100.00. 
1. Add planned/actual hours each task and % Complete according to the table below.

   >[!NOTE]
   >
   >For Tasks 1 and 3, you are only adding actual hours.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Task</strong> </p> </th> 
   <th> <br> <p><strong>Pln Hrs</strong> </p> </th> 
   <th> <br> <p><strong>Act Hrs</strong> </p> </th> 
   <th> <p><strong>% Complete</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Task 1</p> </td> 
   <td>&nbsp;</td> 
   <td> <p>10 hrs</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Task 2</p> </td> 
   <td> <p>5 hrs</p> </td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 3</p> </td> 
   <td>&nbsp;</td> 
   <td> <p>10 Hrs</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Task 4</p> </td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 5</p> </td> 
   <td> <p>15 hrs</p> </td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 6</p> </td> 
   <td> <p>20 hrs</p> </td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Add 50 hours directly to the project (More>Hours>Log Hours) so that there is $5,000.00 of actual labor cost recorded directly to the project. 
1. Run Recalculate Finance 
1. **CPI for Task 2** = .1 calculated as follows:  
   **CPI for Task 2** = *IF* Actual Hours > 0 *THEN* 

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   &nbsp; &nbsp;&nbsp;*ELSE* CPI = 1  
   **CPI for Task 2** = 1 / 10  
   **CPI for Task 2** = .1

1. **EAC for Task 2** = 50 hrs calculated as follows:  
   **EAC for Task 2** = *IF* CPI <> 0 *THEN* 

   ```
   EAC = Planned Hours / CPI
   ```

   &nbsp; &nbsp;&nbsp;*ELSE* EAC = Planned &nbsp;Hours + Actual &nbsp;Hours  
   **EAC for Task 2** = 5 / .1  
   **EAC for Task 2** = 50 hrs

1. CPI / EAC for Task 4, Task 5, and Task 6:  
   Task 4 = .4 / 25 hrs  
   Task 5 = .75 / 20 hrs  
   Task 6 = 1.2 / 16.67 hrs

1. **CPI for Task 3** = .38  
   **CPI for Task 3** = *IF* Actual Hours > 0 *THEN* 

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   &nbsp; &nbsp;&nbsp;*ELSE* CPI = 1  
   **CPI for Task 3** = 11.5 / 30  
   **CPI for Task 3** = .38

1. **EAC for Task 3** = EAC Task 4 + EAC Task 5  
   **EAC for Task 3** = 25 + 20  
   **EAC for Task 3** = 45 hrs

1. **CPI for Task 1** = .25 calculated as follows:  
   **CPI for Task 1** = *IF* Actual Hours > 0 *THEN* 

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   &nbsp; &nbsp;&nbsp;*ELSE* CPI = 1  
   **CPI for Task 1** = 12.5 / 50  
   **CPI for Task 1** = .25

1. **EAC for Task 1** = EAC Task 2 + EAC Task 3  
   **EAC for Task 1** = 50 + 45  
   **EAC for Task 1** = 95 hrs

1. CPI for Project = .22 calculated as follows:  
   **CPI for Project** = *IF* Actual Hours > 0 *THEN* 

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   &nbsp; &nbsp;&nbsp;*ELSE* CPI = 1  
   **CPI for Project** = 24.5 / 110  
   **CPI for Project** = .22272  
   **CPI for Project** = .22

1. **EAC for project** = EAC Task 1 + EAC Task 6  
   **EAC for project** = 95 + 16.67  
   **EAC for project** = 111.67 hrs

### PIM= Cost-Based {#pim-cost-based}

* [Simple example: project has no children tasks](#simple-example-project-has-no-children-tasks)

#### Simple example: project has no children tasks {#simple-example-project-has-no-children-tasks-1}

PIM = Cost-Based

EAC Method = Roll up from tasks/ subtasks

1. Create Project A with three tasks (no child tasks) all assigned to User 1 whose cost/ hr is $100.00. 
1. Add planned/ actual hours to each task and % Complete according to the table below:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Task</strong> </p> </th> 
   <th> <br> <p><strong>Pln Hrs</strong> </p> </th> 
   <th> <br> <p><strong>Pln Lbr Cost</strong> </p> </th> 
   <th> <br> <p><strong>Act Hrs</strong> </p> </th> 
   <th> <br> <p><strong>Act Lbr Cost</strong> </p> </th> 
   <th> <p><strong>% Complete</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Task 1</p> </td> 
   <td> <p>5 hrs</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>25 hrs</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 2</p> </td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>25 hrs</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 3</p> </td> 
   <td> <p>15 hrs</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>25 hrs</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Add expenses to each task according to the table below:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Task</strong> </p> </th> 
   <th> <p><strong>Expense</strong> </p> </th> 
   <th> <p><strong>Planned Amount</strong> </p> </th> 
   <th> <p><strong>Actual Amount</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Task 1</p> </td> 
   <td> <p>Task 1 Exp 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 1</p> </td> 
   <td> <p>Task 1 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 2</p> </td> 
   <td> <p>Task 2 Exp</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 3</p> </td> 
   <td> <p>Task 3 Exp</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Add two expenses to the project (i.e. not tied to a task) as follows:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Expense</strong> </p> </th> 
   <th> <p><strong>Planned Amount</strong> </p> </th> 
   <th> <p><strong>Actual Amount</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Project Exp 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 1 Exp 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Based on the above values, the Incurred/ Not Incurred Costs are determined as follows:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Task</strong> </p> </th> 
   <th> <p><strong>Not Incurred Planned Expense</strong> </p> </th> 
   <th> <p><strong>Incurred Planned Expense</strong> </p> </th> 
   <th> <p><strong>Incurred Actual Expense</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Task 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p>$2,700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. From Project Actions, run Recalculate Finance 
1. **CPI****for Task 1** = .14 calculated as follows:  
   **CPI****for Task 1** &nbsp;= *IF* Actual Labor Cost + IncurredActualExpenseCost &nbsp;<> 0 *THEN* 

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *&nbsp; &nbsp;ELSE* CPI = CPI_Labor  
   **CPI****for Task 1** &nbsp;= (100+300) / (2500+400)  
   **CPI****for Task 1** &nbsp;= 400 / 2900  
   **CPI****for Task 1** &nbsp;= .14

1. **EAC****for Task 1** = $13,400.00  
   **CPI Labor****for Task 1** = IF Actual Labor Cost <> 0 THEN 

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   &nbsp; &nbsp;ELSE CPI_Labor = 1  
   **CPI Labor****for Task 1** = 100/2500  
   **CPI Labor****for Task 1** = .04  
  
   **EAC Labor****for Task 1** = *IF* CPI_Labor <> 0 *THEN* 

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *&nbsp; &nbsp;ELSE* EAC &nbsp;Labor = Planned Labor Cost + Actual Labor Cost  
   **EAC Labor****for Task 1** = 500.00/.04  
   **EAC Labor****for Task 1** = $12,500.00  
  
   **EAC Expense****for Task 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense  
   **EAC Expense****for Task 1** = $400.00 + $500.00  
   **EAC Expense****for Task 1** = $900.00  
  
   **EAC****for Task 1** = EAC Labor + EAC Expense  
   **EAC****for Task 1** &nbsp;= $12,500.00 + $900.00  
   **EAC****for Task 1** &nbsp;= $13,400.00

1. Here are the CPI / EAC values for Task 2 and Task 3:  
   Task 2 = .19 / $8,433.33  
   Task 3 = .44 / $6,950.00****

1. The CPI for the project = .32  
   **CPI****for Project** = *IF* Actual Labor Cost + IncurredActualExpenseCost &nbsp;<> 0 *THEN* 

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *&nbsp; &nbsp;ELSE* CPI = CPI_Labor  
   **CPI****for Project** = (1000 + 2300) / (7500 + 2700)  
   **CPI****for Project** = 3300 / 10200  
   **CPI****for Project** = .32

1. EAC for the project is $28,783.33  
   **EAC****for Project** = EAC Task 1 + EAC Task 2 + EAC Task 3  
   **EAC****for Project** = $13,400.00 + $8,433.33 + $6,950.00  
   **EAC****for Project** = $28,783.33
