---
filename: how-workfront-calculates-finances
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
---




# How `Workfront` calculates finances  {#how-workfront-calculates-finances}



## Definition of terms {#definition-of-terms}


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="0"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><b>Term</b> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p><b>Definition</b> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Actual Hours</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The hours recorded against the task (via Log Hours button).</p> <p><code>For parent tasks = children Actual Hours + Actual Hours on the parent task. For projects = Actual Hours logged on the project +Actual Hours logged on standalone or children tasks in the project</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> If from the Updates tab for Task 1, you click ‘Log Time’ and enter 25 hours, the Actual Hours = 25. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Actual Labor Cost</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The result of multiplying the actual hours by the rate. </p> <br> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If the task is set up such that the Cost Type = ‘User Hourly’ (Task Details&gt;Finance) and the user’s cost/hr on their profile is $100.00/hr, then if you record 5 actual hours, the Actual Labor Cost = $500.00. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>IncurredActualExpenseCost</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The sum of the Actual Amount field for all expenses where the Actual Amount field &gt; 0.</p> <br> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> If you create an expense for Task 1 and enter $600.00 in the Actual Amount field, the Incurred Actual Expense Cost for this task is $600.00. </p> <br> <p>Important: If the value in the Actual Amount field for an expense is negative, the system will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>IncurredPlannedExpenseCost </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The sum of the Planned Amount field for all expenses where the Actual Amount field &gt; 0.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> If you create an expense for Task 1 and enter $500.00 in the Planned Amount field and an amount &gt; 0 in the Actual Amount field (i.e. $600.00), the Incurred Planned Expense Cost for this task is $500.00. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>NotIncurredPlannedExpense</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The sum of the Planned Amount field for all expenses where the Actual Amount field = 0.</p> <br> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> If you create two expenses for Task 1 where for the first expense the value in the Planned Amount field is $500.00 and the value in the Actual Amount is $600.00 and for the second expense, the value in the Planned Amount field is $300.00 and the value of the Actual Amount field is $0.00, the value of the Not Incurred Planned Expense for this task is $300.00. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Percent Complete</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The value entered into the Percent Complete field for a task.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Planned Hours</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The value entered into the Planned Hours field on the task (i.e. 10 Hours)</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Planned Labor Cost</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The result of multiplying the planned hours by the rate. </p> <br> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span> If the task is set up such that the Cost Type = ‘User Hourly’ (Task Details&gt;Finance) and the user’s cost/hr on their profile is $100.00/hr, then if you record 10 planned hours, the Planned Labor Cost = $1,000.00. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> TotalBudgetedCostWorkPerformed</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>The result of multiplying the budgeted cost of the work planned (Budgeted Cost) and the percent of the task that has been completed so far.</p> <p>For a non-parent task:<br><code>TotalBudgetedCostWorkPerformed = Planned Hours * (Percent Complete/100)</code><br>For a parent task:<br><code>TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all direct child tasks</code><br>For a project:<br><code>TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all top-level tasks (parents and standalone tasks)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>



## Differences between the two EAC methods {#differences-between-the-two-eac-methods}

There are two methods for calculating EAC:



* [Calculate EAC at project level](#calculat) 
* [Caculate EAC as a roll up from tasks](#caculate) 




### Calculate EAC at project level {#calculate-eac-at-project-level}




*  EAC for the parent task and project are determined by entering the actual hours/actual labor cost into the EAC Formulas 
* * Includes * Actual Hours/ Costs and expenses added directly to the parent task or project 




### Caculate EAC as a roll up from tasks {#caculate-eac-as-a-roll-up-from-tasks}




*  EAC for the parent task and project are determined by summing up the EAC for each * direct * child task 
* * Excludes * Actual Hours and expenses added directly to the parent task or project 




## Formulas {#formulas}




* [How Workfront calculates finances](#pim-hour-based) 
* [How Workfront calculates finances](#pim-cost-based) 




### PIM= Hour-Based {#pim-hour-based}



#### **TotalBudgetedCostWorkPerformed**  {#totalbudgetedcostworkperformed}




* **For a non-parent task** : 

  ```
  TotalBudgetedCostWorkPerformed = Planned Hours * (Percent Complete/100)
  ```

  <![CDATA[ ]]>

* **For a parent task: **<![CDATA[			]]>

  ```
  TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all single children tasks
  ```

  <![CDATA[ ]]>

*  **For a project: **

  ```
  TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all top-level tasks
  ```




  >[!NOTE]
  >
  >This includes only first level parents, not secondary level parents, etc.







#### **CPI**  {#cpi}

* IF * Actual Hours > 0 * THEN *<![CDATA[			]]>

```
CPI = TotalBudgetedCostWorkPerformed / Actual Hours
```

<![CDATA[ ]]>


* ELSE * CPI = 1 


**EAC** 


* IF * CPI <> 0 * THEN * EAC = Planned Hours / CPI 


* ELSE * EAC = Planned Hours + Actual Hours 


### PIM= Cost-Based {#pim-cost-based}



#### **TotalBudgetedCostWorkPerformed**  {#totalbudgetedcostworkperformed-1}

**For a non parent task** : 

```
TotalBudgetedCostWorkPerformed = Planned Labor Cost * (Percent Complete/100)
```

<![CDATA[ ]]>


**For a parent task: **<![CDATA[		]]>

```
TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all direct child tasks
```




**For a project: **

```
TotalBudgetedCostWorkPerformed = the sum of the TotalBudgetedCostWorkPerformed field for all top-level tasks
```

** **


#### **CPI**  {#cpi-1}

* IF * Actual Labor Cost + IncurredActualExpenseCost <> 0 * THEN *<![CDATA[			]]>

```
CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
```

<![CDATA[ ]]>


* ELSE * CPI = CPI_Labor 


#### **EAC**  {#eac}

**EAC** = **EAC Labor** + **EAC Expense**** **


For EAC Labor, we first need to determine CPI_Labor. 


**CPI_Labor** = IF Actual Labor Cost <> 0 THEN 

```
CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
```

<![CDATA[ ]]>


ELSE CPI_Labor = 1 ** **


**EAC Labor** = * IF * CPI_Labor <> 0 * THEN *<![CDATA[			]]>

```
EAC Labor = Planned Labor Cost / CPI_Labor
```




* ELSE *<![CDATA[			]]>

```
EAC Labor = Planned Labor Cost + Actual Labor Cost
```




**EAC Expense**<![CDATA[			]]>

```
= IncurredActualExpenseCost + NotIncurredPlannedExpense
```

<![CDATA[ ]]>
