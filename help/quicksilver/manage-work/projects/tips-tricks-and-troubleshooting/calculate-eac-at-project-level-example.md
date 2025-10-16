---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Calculation Example - Calculate EAC at the Project Level
description: This article gives an example of calculating the Estimate At Completion (EAC) of a project at the project level in Adobe Workfront. 
author: Lisa
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
---
# Calculation example - calculate EAC at the Project Level

## EAC method: Calculate at the project level

* [PIM = Hour-Based](#pim-hour-based) 
* [PIM= Cost-Based](#pim-cost-based)

### PIM = Hour-Based {#pim-hour-based}

* [Simple example: project has no children tasks](#simple-example-project-has-no-children-tasks) 
* [Complicated example: project has children tasks](#complicated-example-project-has-children-tasks)

#### Simple example: project has no children tasks {#simple-example-project-has-no-children-tasks}

PIM = Hour-Based

EAC Method = Calculate at project level ****

1. Create Project A with three tasks (no child tasks) all assigned to User 1 whose cost/hr is $100.00. 
1. Add Planned and Actual hours to each task and % Complete according to the table below: 

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>Task</strong></p></th>
      <th><br><p><strong>Pln Hrs</strong></p></th>
      <th><br><p><strong>Act Hrs</strong></p></th>
      <th><p><strong>% Complete</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>Task 1</p></td>
      <td><p>5 hrs</p></td>
      <td><p>25 hrs</p></td>
      <td><p>20%</p></td>
     </tr>
     <tr>
      <td><p>Task 2</p></td>
      <td><p>10 hrs</p></td>
      <td><p>25 hrs</p></td>
      <td><p>30%</p></td>
     </tr>
     <tr>
      <td><p>Task 3</p></td>
      <td><p>15 hrs</p></td>
      <td><p>25 hrs</p></td>
      <td><p>40%</p></td>
     </tr>
    </tbody>
   </table>

1. Recalculate Finance on the project. 
1. **CPI for Task 1** = .04 calculated as follows:  
   **CPI for Task 1** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours  
   &nbsp; &nbsp;*ELSE* CPI = 1  
   **CPI for Task 1** = 1 / 25  
   **CPI for Task 1** = .04

1. **EAC for Task 1** = 125 hrs calculated as follows:  
   **EAC for Task 1** = *IF* CPI <> 0 *THEN* EAC = Planned Hours/CPI  
   &nbsp; &nbsp;&nbsp;*ELSE* EAC = Planned &nbsp;Hours + Actual &nbsp;Hours  
   **EAC for Task 1** = 5 / .04  
   **EAC for Task 1** = 125 hrs****

1. CPI / EAC for Tasks 2 and 3 are:  
   Task &nbsp;2 = .12 / 83.33 &nbsp;hrs  
   Task 3 = .24 / 62.5 hrs

1. **CPI for Project** = .13 calculated as follows:  
   **CPI for Project** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours  
   &nbsp; &nbsp;&nbsp;*ELSE* CPI = 1  
   **CPI for Project** = 10 / 75  
   **CPI for Project** = .13

1. **EAC for Project** = 225 hrs calculated as follows:  
   **EAC for Project** = *IF* CPI <> 0 *THEN* EAC = Planned Hours/CPI  
   &nbsp; &nbsp;&nbsp;*ELSE* EAC = Planned &nbsp;Hours + Actual &nbsp;Hours  
   **EAC for Project** = 30 / .13333  
   **EAC for Project** = 225 hrs

#### Complicated example: project has children tasks {#complicated-example-project-has-children-tasks}

PIM = Hour-Based

EAC Method = Calculate at project level

1. Create Project A with six tasks where Task 3 is the parent of Tasks 4 and 5 and Task 1 is the parent of Tasks 2 and 3 as shown below:  
   Task 1  
   &nbsp; &nbsp;Task 2  
   &nbsp; &nbsp;Task 3  
   &nbsp; &nbsp; &nbsp; Task 4  
   &nbsp; &nbsp; &nbsp; Task 5  
   Task 6

1. Assign Tasks 2, 4, 5, and 6 to User 1 whose cost/hr rate is $100.00. 
1. Add planned/ actual hours each task and % Complete according to the table below.

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

1. Add 50 hours directly to the project (More>Hours>Log Hours). 
1. **CPI for Task 2** = .1 calculated as follows:  
   **CPI for Task 2** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours  
   &nbsp; &nbsp;&nbsp;*ELSE* CPI = 1  
   **CPI for Task 2** = 1 / 10  
   **CPI for Task 2** = .1

1. **EAC for Task 2** = 50 hrs calculated as follows:  
   **EAC for Task 2** = *IF* CPI <> 0 *THEN* EAC = Planned Hours/CPI  
   &nbsp; &nbsp;&nbsp;*ELSE* EAC = Planned &nbsp;Hours + Actual &nbsp;Hours  
   **EAC for Task 2** = 5 / .1  
   **EAC for Task 2** = 50 hrs

1. The CPI / EAC for Tasks 4, 5, and 6 are as follows:  
   Task 4: .4 / 25 hrs  
   Task 5: .75 / 20 hrs  
   Task 6: 1.2 / 16.67 hrs

1. **CPI for Task 3** = .38 &nbsp;calculated as follows:  
   **CPI for Task 3** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours  
   &nbsp; &nbsp;&nbsp;*ELSE* CPI = 1  
   **CPI for Task 3** = 11.5 / 30  
   **CPI for Task 3** = .38

1. **EAC for Task 3** = 65.22 hrs calculated as follows:  
   **EAC for Task 3** = *IF* CPI <> 0 *THEN* EAC = Planned Hours/CPI  
   &nbsp; &nbsp;&nbsp;*ELSE* EAC = Planned &nbsp;Hours + Actual &nbsp;Hours  
   **EAC for Task 3** = &nbsp;25 / .383333  
   **EAC for Task 3** = 65.22 hrs

1. **CPI for Task 1** = .25 calculated as follows:  
   **CPI for Task 1** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours  
   &nbsp; &nbsp;&nbsp;*ELSE* CPI = 1  
   **CPI for Task 1** = 12.5 / 50  
   **CPI for Task 1** = .25

1. **EAC for Task 1** = 120 hrs calculated as follows:  
   **EAC for Task 1** = *IF* CPI <> 0 *THEN* EAC = Planned Hours / CPI  
   &nbsp; &nbsp;&nbsp;*ELSE* EAC = Planned &nbsp;Hours + Actual &nbsp;Hours  
   **EAC for Task 1** = &nbsp;30/ .25  
   **EAC for Task 1** = 120 hrs

1. **CPI for Project** = .22 calculated as follows:  
   **CPI for Project** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours  
   &nbsp; &nbsp;&nbsp;*ELSE* CPI = 1  
   **CPI for Project** = 24.5 / 110  
   **CPI for Project** = .22272  
   **CPI for Project** = .22

1. **EAC for Project** = 224.49 &nbsp;hrs calculated as follows:  
   **EAC for Project** = *IF* CPI <> 0 *THEN* EAC = Planned Hours/CPI  
   &nbsp; &nbsp;&nbsp;*ELSE* EAC = Planned &nbsp;Hours + Actual &nbsp;Hours  
   **EAC for Project** = &nbsp;50 / .22272  
   **EAC for Project** = 224.49 hrs

### PIM= Cost-Based {#pim-cost-based}

* [Simple example: project has no children tasks](#simple-example-project-has-no-children-tasks) 
* [Complicated example: project has children tasks](#complicated-example-project-has-children-tasks)

#### Simple example: project has no children tasks {#simple-example-project-has-no-children-tasks-1}

PIM = Cost-Based

EAC Method = Calculate at project level

1. Create Project A with three tasks (no child tasks) all assigned to User 1 whose cost/hr is $100.00. 
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
   <td> <p> $2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. From Project Actions, run Recalculate Finance 
1. **CPI for Task 1** = .14 
1. **CPI****for Task 1** = .14 calculated as follows:  
   **CPI** &nbsp;**for Task 1** = *IF* Actual Labor Cost + IncurredActualExpenseCost &nbsp;<> 0 *THEN* 

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *&nbsp; &nbsp; ELSE* CPI = CPI_Labor  
   **CPI****for Task 1** = (100+300) / (2500+400)  
   **CPI** &nbsp;**for Task 1** = 400 / 2900  
   **CPI** &nbsp;**for Task 1** &nbsp;= .14****

1. **EAC****for Task 1** = $13,400.00  
   **CPI Labor** &nbsp;**for Task 1** = IF Actual Labor Cost <> 0 THEN 

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

   &nbsp; &nbsp;ELSE CPI_Labor = 1  
   **CPI Labor** &nbsp;**for Task 1** = 100/2500  
   **CPI Labor** &nbsp;**for Task 1** = .04******EAC Labor****for Task 1** = *IF* CPI_Labor <> 0 *THEN* EAC Labor = Planned Labor Cost/CPI_Labor  
   *&nbsp; &nbsp; ELSE* EAC &nbsp;Labor = Planned Labor Cost + Actual Labor Cost  
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
   Task 3 = .44 / $6,950.00

1. **CPI for Project** = .32 calculated as follows:  
   **CPI****for Project** = *IF* Actual Labor Cost + IncurredActualExpenseCost &nbsp;<> 0 *THEN* 

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *&nbsp; &nbsp;ELSE* CPI = CPI_Labor  
   **CPI****for Project** = (1000 + 2300) / (7500 + 2700)  
   **CPI****for Project** = 3300 / 10200  
   **CPI****for Project** = .32

1. **EAC for Project** = $28,200.00 calculated as follows:  
   **CPI Labor****for Project** = IF Actual Labor Cost <> 0 THEN 

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

   &nbsp; &nbsp;ELSE CPI_Labor = 1  
   **CPI Labor****for Project** = 1000 / 7500  
   **CPI Labor****for Project** = .13333  
   **CPI Labor****for Project** = .13  
  
   **EAC Labor****for Project** = *IF* CPI_Labor <> 0 *THEN* 

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *&nbsp; &nbsp;ELSE* EAC &nbsp;Labor = Planned Labor Cost + Actual Labor Cost  
   **EAC Labor****for Project** = 3000/ .13333  
   **EAC Labor****for Project** = $22,500.00  
  
   **EAC Expense****Project** = 

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC Expense****Project** = $3000.00 + 2,700.00  
   **EAC Expense****Project** = $5,700.00  
  
   **EAC****Project** = EAC Labor + EAC Expense  
   **EAC****Project** &nbsp;= $22,500.00 + $5,700.00  
   **EAC****Project** &nbsp;= $28,200.00

#### Complicated example: project has children tasks {#complicated-example-project-has-children-tasks-1}

PIM = Cost-Based

EAC Method = Calculate at project level

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
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Task 2</p> </td> 
   <td> <p>5 hrs</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 3</p> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td> <p>10 Hrs</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Task 4</p> </td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 5</p> </td> 
   <td> <p>15 hrs</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 6</p> </td> 
   <td> <p>20 hrs</p> </td> 
   <td> <p>$2,000.00</p> </td> 
   <td> <p>10 hrs</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Add 50 hours directly to the project (More>Hours>Log Hours) so that there is $5,000.00 of actual labor cost recorded directly to the project. ****
1. Add expenses to each task according to the table below (I've added a blank row in between each task to make it easier to read):

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
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 1</p> </td> 
   <td> <p>Task 1 Exp 2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 1</p> </td> 
   <td> <p>Task 1 Exp 3</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Task 2</p> </td> 
   <td> <p>Task 2 Exp 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 2</p> </td> 
   <td> <p>Task 2 Exp 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 2</p> </td> 
   <td> <p>Task 2 Exp 3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>$600.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 2</p> </td> 
   <td> <p>Task 2 Exp 4</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Task 3</p> </td> 
   <td> <p>Task 3 Exp</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Task 4</p> </td> 
   <td> <p>Task 4 Exp 1</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 4</p> </td> 
   <td> <p>Task 4 Exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 4 </p> </td> 
   <td> <p>Task 4 Exp 3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Task 5</p> </td> 
   <td> <p>Task 5 Exp 1</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 5</p> </td> 
   <td> <p>Task 5 Exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 5</p> </td> 
   <td> <p>Task 5 Exp 3</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Task 6</p> </td> 
   <td> <p>Task 6 Exp 1</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 6</p> </td> 
   <td> <p>Task 6 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>-$300.0</p> </td> 
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
   <td> <p> $0.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Based on the above values, the Incurred/Not Incurred Costs are determined as follows:

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
   <td> <p>$400.00</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$1,300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 4</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 5</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$1,100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Task 6</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$1000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. From Project Actions, run Recalculate Finance 
1. **CPI** for Task 2 = .17 calculated as follows:  
   **CPI Task 2** = *IF* Actual Labor Cost + IncurredActualExpenseCost &nbsp;<> 0 *THEN* CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)  
   *&nbsp; &nbsp;ELSE* CPI = CPI_Labor  
   **CPI****Task 2** = (100+300) / (1000+1300)  
   **CPI****Task 2** &nbsp;= 400 / 2300  
   **CPI****Task 2** &nbsp;= .17

1. **EAC** for Task 2 = $5,900.00  
   **CPI Labor****Task 2** = IF Actual Labor Cost <> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost  
   &nbsp; &nbsp;ELSE CPI_Labor = 1  
   **CPI Labor****Task 2** = 100/1000  
   **CPI Labor****Task 2** = .1  
  
   **EAC Labor****Task 2** = *IF* CPI_Labor <> 0 *THEN* 

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *&nbsp; &nbsp;ELSE* EAC &nbsp;Labor = Planned Labor Cost + Actual Labor Cost  
   **EAC Labor****Task 2** = 500.00/.1  
   **EAC Labor****Task 2** = $5,000.00******EAC Expense****Task 2** = IncurredActualExpenseCost + NotIncurredPlannedExpense  
   **EAC Expense****Task 2** = $1,300.00 + -$400.00  
   **EAC Expense****Task 2** = $900.00  
  
   **EAC****Task 2** = EAC Labor + EAC Expense  
   **EAC****Task 2** &nbsp;= $5,000.00 + $900.00  
   **EAC****Task 2** &nbsp;= $5,900.00

1. The CPI/EAC for Tasks 4, 5, and 6 are determined the same way so I'll just provide those values below:  
   Task 4: .23 / $3,400.00  
   Task 5: .64 / $3,100.00  
   Task 6: 1.06 / $2,366.67

1. CPI for Task 3 = .31 calculated as follows:  
   **CPI****Task 3** = *IF* Actual Labor Cost + IncurredActualExpenseCost &nbsp;<> 0 *THEN* 

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *&nbsp; &nbsp;ELSE* CPI = CPI_Labor  
   **CPI****Task 3** &nbsp;= (1,150 + 500) / (3000 + 2400)  
   **CPI****Task 3** &nbsp;= &nbsp;1650 / 5400  
   **CPI****Task 3** &nbsp;= .31******EAC for Task 3** = $9,521.74 calculated as follows:  
   **CPI Labor****Task 3** = IF Actual Labor Cost <> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   &nbsp; &nbsp;ELSE CPI_Labor = 1  
   **CPI Labor****Task 3** = 1150/3000  
   **CPI Labor****Task 3** = .383333  
   **CPI Labor****Task 3** = .38  
  
   **EAC Labor****Task 3** = *IF* CPI_Labor <> 0 *THEN* 

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *&nbsp; &nbsp;ELSE* EAC &nbsp;Labor = Planned Labor Cost + Actual Labor Cost  
   **EAC Labor****Task 3** = $2,500.00 / .383333  
   **EAC Labor****Task 3** = $6,521.74  
  
   **EAC Expense****Task 3** = IncurredActualExpenseCost + NotIncurredPlannedExpense  
   **EAC Expense****Task 3** = $2,400.00 + $600.00  
   **EAC Expense****Task 3** = $3,000.00  
  
   **EAC****Task 3** = EAC Labor + EAC Expense  
   **EAC****Task 3** &nbsp;= $6,521.74 + $3,000.00  
   **EAC****Task 3** &nbsp;= $9,521.74

1. CPI for Task 1 = .16 calculated as follows:  
   **CPI****Task 1** = *IF* Actual Labor Cost + IncurredActualExpenseCost &nbsp;<> 0 *THEN* 

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *&nbsp; &nbsp;ELSE* CPI = CPI_Labor  
   **CPI****Task 1** &nbsp;= (1250 + 300) / (5000 + 4500)  
   **CPI****Task 1** &nbsp;= &nbsp;1550 / 9500=  
   **CPI****Task 1** &nbsp;= .16

1. EAC for Task 1 is $17,100.00 calculated as follows:  
   **CPI Labor****Task 1** = IF Actual Labor Cost <> 0 THEN 

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   &nbsp; &nbsp;ELSE CPI_Labor = 1  
   **CPI Labor****Task 1** = 1250 / 5000  
   **CPI Labor****Task 1** = .25  
  
   **EAC Labor****Task 1** = *IF* CPI_Labor <> 0 *THEN* EAC Labor = Planned Labor Cost / CPI_Labor  
   *&nbsp; &nbsp;ELSE* EAC &nbsp;Labor = Planned Labor Cost + Actual Labor Cost  
   **EAC Labor****Task 1** = $3,000.00 / .25  
   **EAC Labor****Task 1** = $12,000.00  
  
   **EAC Expense****Task 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense  
   **EAC Expense****Task 1** = $4500 + 600  
   **EAC Expense****Task 1** = $5,100.00  
  
   **EAC****Task 1** = EAC Labor + EAC Expense  
   **EAC****Task 1** &nbsp;= $12,000.00 + 5,100.00  
   **EAC****Task 1** &nbsp;= $17,100.00

1. CPI for Project is .25  
   **CPI****for Project** = *IF* Actual Labor Cost + IncurredActualExpenseCost &nbsp;<> 0 *THEN* 

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *&nbsp; &nbsp;ELSE* CPI = CPI_Labor  
  
   **CPI****for Project** = (2450 + 1900) / (11000 + 6700)  
   **CPI****for Project** = &nbsp;&nbsp;4350 / 17700  
   **CPI****for Project** = .25

1. **EAC for Project** = $32,248.98 calculated as follows:  
   **CPI Labor****for Project** = IF Actual Labor Cost <> 0 THEN 

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   &nbsp; &nbsp;ELSE CPI_Labor = 1  
   **CPI Labor****for Project** = 2450 / 11000  
   **CPI Labor****for Project** = .22272  
   **CPI Labor****for Project** = .22  
  
   **EAC Labor****for Project** = *IF* CPI_Labor <> 0 *THEN* 

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *&nbsp; &nbsp;ELSE* EAC &nbsp;Labor = Planned Labor Cost + Actual Labor Cost  
   **EAC Labor****for Project** = $5,000.00 / .22272  
   **EAC Labor****for Project** = $22,448.97959  
   **EAC Labor****for Project** = $22,448.98  
  
   **EAC Expense****Project** = IncurredActualExpenseCost + NotIncurredPlannedExpense  
   **EAC Expense****Project** = $3,100.00 + $6,700.00  
   **EAC Expense****Project** = $9,800.00  
  
   **EAC****Project** = EAC Labor + EAC Expense  
   **EAC****Project** &nbsp;= $22,448.98 + 9,800.00  
   **EAC****Project** &nbsp;= $32,248.98
