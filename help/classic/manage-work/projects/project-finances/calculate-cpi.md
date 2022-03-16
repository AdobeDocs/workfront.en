---
filename: calculate-cpi
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculate Cost Performance Index (CPI)
description: The Cost Performance Index (CPI) describes the relationship at the project or task level between the planned cost and actual cost. Project Managers review this metric to identify tasks or projects currently tracking under or over cost at a given point. Cost can be measured in hours or dollars, depending on your Performance Index Method (PIM). For more information about setting the Performance Index Method, see Set the Performance Index Method (PIM).
---

# Calculate Cost Performance Index (CPI)

The Cost Performance Index (CPI) describes the relationship at the project or task level between the planned cost and actual cost. Project Managers review this metric to identify tasks or projects currently tracking under or over cost at a given point. Cost can be measured in hours or dollars, depending on your Performance Index Method (PIM). For more information about setting the Performance Index Method, see [Set the Performance Index Method (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

Only organizations that require time entry can use CPI. Furthermore, cost-based PIM values are accurate only in organizations that have defined cost rates for task assignees (job roles or users).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Projects and Financial&nbsp;Data</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project with permissions to View Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Overview of the Cost Performance Index (CPI)

* [The CPI value](#understanding-the-cpi-value) 
* [How CPI is calculated](#understanding-how-cpi-is-calculated)

### The CPI value

Project managers understand that a CPI value of 1 means the project is exactly on budget. Values greater than 1 indicate a project is under budget (fewer hours or expenses have been recorded than originally planned), and values less than 1 mean a project is over budget (more hours or expenses have been recorded than originally planned). The further from 1, the greater deviation from the plan.

| `CPI Value`  | `Indication on Budget`  |
|---|---|
| 1 |On plan or budget |
| > 1 (greater than 1) |Under budget |
| < 1 (less than 1) |Over budget |

### How CPI is calculated

In Adobe Workfront, the calculation for CPI depends on the Performance Index Method selected for the project. For more information about setting the Performance Index Method, see [Set the Performance Index Method (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [CPI calculations when using Hour-based PIM](#cpi-calculations-when-using-hour-based-pim) 
* [CPI Calculations when using Cost-based PIM](#cpi-calculations-when-using-cost-based-pim)

#### `CPI calculations when using Hour-based PIM`

If 

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

Otherwise 

```
CPI = 1
```

* `For a non-parent task:`

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* `For a parent task:`   
  Total Budgeted Cost Work Performed = the sum of the Total Budgeted Cost Work Performed field for all direct child tasks.

* `For a project:`   
  Total Budgeted Cost Work Performed = the sum of the Total Budgeted Cost Work Performed field for all top level tasks (parents and standalone tasks).

For information about the total Budgeted Cost Work Performed (BCWP), see [Calculate Budgeted Cost Work Performed (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### `CPI Calculations when using Cost-based PIM`

<!--
CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses)
-->

If 

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```

<![CDATA[ ]]>

Otherwise 

```
CPI = 1<![CDATA[ 
]]>
```

The fields in this calculation are described below:

* Total Actual Cost = Actual (logged) Hours &#42; Hourly Rate of assignees 
* Incurred Actual Expense Cost = the same as Actual Cost 
* Incurred Expense is the expense on which Actual Cost>0 
* Planned Cost of Incurred Expenses= Total of Planned Cost of all incurred expenses 
* Planned Cost of Work Performed is calculated by the following formula:

  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100<![CDATA[
					]]>
  ```

The Total Budgeted Cost Work Performed is calculated for the following:<![CDATA[		]]>

* <![CDATA[			]]> `For a non-parent task:`

  ```
  Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
  ```

* `For a parent task:`   
  Total Budgeted Cost Work Performed = the sum of the Total Budgeted Cost Work Performed field for all direct child tasks.

* `For a project:`   
  Total Budgeted Cost Work Performed = the sum of the Total Budgeted Cost Work Performed field for all top level tasks.

## Locate CPI in a project or task

You can display the CPI of a project or a task in a project or task list or report. In addition, you can view it at the project or task level.

1. Go to the project or task where you want to view the CPI.
1. Select the Project Details tab or the Task Details tab, depending on whether you are viewing CPI for a project or task. 
1. Click `Finance`.

   The CPI displays in the `CPI/ SPI/ CSI` field.

