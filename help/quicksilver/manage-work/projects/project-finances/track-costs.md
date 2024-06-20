---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Track costs
description: You can track costs for projects, tasks, and issues in Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
---
# Track costs

<!-- Audited: 02/2024 -->

You can track costs for projects, tasks, and issues in Adobe Workfront.

## How Workfront calculates costs

To track costs, you must associate users and job roles with hourly cost rates.

Hourly cost rates are amounts of costs per work unit associated with job roles or users. Multiplying the rates by the hours spent on work generates costs for your projects, tasks, or issues.

The following scenarios exist:

* If the Cost Type of your tasks is User Hourly, the user hourly rate calculates the task and project costs.

  For information about associating users with cost rates, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* If the Cost Type of your tasks is Role Hourly, the job role hourly rate calculates the task and project costs.

  For information about associating job roles with cost rates, see [Create and manage job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront calculates only Actual Cost for issues, and issues do not have a Cost Type. For more information, see the section [How Workfront tracks costs for issues](#how-workfront-tracks-costs-for-issues) in this article.

>[!TIP]
>
>You cannot override cost rates for projects. Once you establish the cost per hour rate on a user or job role, that rate calculates all costs in the system.

## Workfront cost performance indexes

Workfront calculates a number of cost performance indexes for projects so projects can be tracked for cost efficiency.  
For more information about calculating cost-performance indexes, see:

* [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) 
* [Calculate Cost Schedule Performance Index (CSI)](../../../manage-work/projects/project-finances/calculate-csi.md) 
* [Calculate Schedule Performance Index (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## How Workfront tracks costs for tasks and projects

The types of costs are calculated differently for tasks and for projects.

### How Workfront tracks costs {#how-workfront-tracks-costs}

You can track several types of costs for tasks and projects in Workfront. Overall costs are calculated by the following formula:

`Costs = Labor Costs + Expense Costs`

* **Labor Costs** are associated with the hours on tasks and projects and the Cost per Hour rates of the resources associated with tasks. Generally, Workfront calculates the following labor costs:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Planned Labor Costs</td> 
     <td> <p>They are calculated using the following formula:</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Budgeted Labor Costs</td> 
     <td> <p>They are calculated using the following formula:</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Actual Labor Costs</td> 
     <td> <p>They are calculated using the following formula:</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> </td> 
    </tr> 
   </tbody> 
  </table>

  For more information, see the [How Workfront calculates Planned, Budgeted, and Actual Costs](#how-workfront-calculates-planned-budgeted-and-actual-costs) section in this article. 

* **Expense Costs** are associated with expenses on projects and tasks.  
  When you create a project, you can set planned expenses for the entire project. Additionally, you can associate expenses with new or existing tasks. For information, see [Manage project expenses](../../../manage-work/projects/project-finances/manage-project-expenses.md). 

* **Fixed Costs** are defined as a fixed amount of cost for a project. This is part of the Planned Cost of the project, which represents the amount of money that you need to complete the project.

  >[!TIP]
  >
  >When attaching a template to a project, the Fixed Cost of a template is added to the Fixed Cost of the project. For information, see [Overview of attaching a template to a project](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### How Workfront calculates Planned, Budgeted, and Actual Costs {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront calculates the Planned Cost and the Actual Cost for each individual task in a project. Workfront uses these calculations for individual tasks to calculate the Planned Cost and the Actual Cost for the project.

#### Planned Cost {#planned-cost}

The Planned Cost of a project is the cost associated with the planned work (Planned Hours) on the project.

The Planned Cost of a project is calculated by the following formula:

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

For example, you have the following expenses on the Expenses tab of a task: a $100 Marketing expense and a $50 Administrative expense. In the Finance tab, you select the User Hourly cost type. A user is assigned to the task, and the user's hourly rate is $15. The user is assigned to work 5 hours on this task. In the Expenses tab of the project, you have a $100 Planned Cost for an expense called Consulting. You also have a $200 Fixed Cost for the project.

The Planned Cost of the project is calculated as follows:

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

The hourly rate in the formula considers any date effective changes of the rate.

#### Budgeted Cost {#budgeted-cost}

The Budgeted Cost of a project is the cost associated with the budgeted work (Budgeted Hours) on the project.

The Budgeted Cost of the project is the same as the Planned Cost of the project if the following two conditions are met:

* The Planned Hours of the tasks on the project match the Budgeted Hours (in the Resource Planner).
* The Billing Type of the tasks is Role Hourly.

The Budgeted Cost of the project is calculated using the formula below if the following conditions are met:

* The Planned Hours of the tasks on the project do not match the Budgeted Hours (in the Resource Planner).
* The Billing Type of the tasks is Role Hourly.

When the above conditions are met, Workfront calculates the Budgeted Cost of the project using the following formula: 

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### Actual Cost {#actual-cost}

The Actual Cost of a project is the cost associated with the actual work (Hours logged) on the project.

Actual Cost is calculated using the following formula:

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

For example, you have the following expenses on the Expenses tab of a task: a Marketing expense with an Actual Cost of $110, and an Administrative expense with an Actual Cost of $40. You select the Role Hourly cost type and assign the Consultant job role to the task. The consultant job role's rate is $15 per hour, and there are 6 hours logged on the task for the Consultant job role. There is a Consulting expense associated with the project (in the Expenses tab), with an Actual Cost of $100 and a user with a Cost per Hour rate of $20 in their user profile logs 10 hours on the project. You also have a $200 Fixed Cost for the project.

The Actual Cost of the project is calculated as follows:

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

The hourly rate in the formula considers any date effective changes of the rate.

>[!NOTE]
>
>The Actual Expense Cost of the project is calculated as follows:
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>These costs are not duplicated in the Actual Cost calculation. For example, if a Fixed Cost is part of the Actual Expense Cost of the project, it is not added separately to the Actual Cost.

>[!NOTE]
>
>When logging time on a project, the following scenarios exist when calculating Actual Labor Cost for the project:
>
>* By default, Workfront uses the Cost per Hour rate of the user to calculate Actual Labor Cost.
>* If the user logging the time is not associated with any cost, then Workfront uses the Cost per Hour rate of the user's Primary Role.
>* If your Workfront administrator enabled the **Assign Job Roles to hour entries manually** setting in the Timesheets & Hours Preferences area of Setup, and the user logging time on the project selects a different role to associate with this time, the Actual Cost of the project calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article [Configure timesheet and hour preferences](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

### How Workfront calculates Cost Types for tasks {#how-workfront-calculates-cost-types-for-tasks}

The Planned and Actual Cost of the tasks and their Labor Costs are determined by the Cost Type of each task.

You can configure the Cost Type for individual tasks within the project. Each cost type affects the Planned Cost and Actual Cost values.

For information about how to modify the Cost Type of a task, see [Update task Cost Type](../../../manage-work/tasks/task-information/update-task-cost-type.md). 

The following table describes the available task Cost Types in Workfront:

<table style="table-layout:auto">
 <col> 
 <col> 
<tbody> 
  <tr> 
   <td> <p><strong>Task Cost Type</strong> </p> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr>
  <tr> 
   <td> <p>User Hourly</p> </td> 
   <td> <p>This is the default Cost Type when you create a task.</p> <p><strong>Planned Cost</strong> is calculated by the following formula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Where the Planned Labor Cost is calculated by:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Note: <p>Consider the following impacts of using the User Hourly Cost Type and calculating Planned Cost:</p> 
     <ul> 
      <li>If you assign multiple resources to a task, Workfront adjusts calculations for Planned Cost based on the percentage of the task assigned to each resource.</li>
      <li>For date effective cost rates, the Planned Labor cost is the sum of the planned costs of each time period covered in the task.</li>
      <li>The value of the Planned Cost field can differ depending on whether you view the Planned Cost from the task itself or from the Utilization report.<br><strong>When viewing Planned Cost from the task itself:</strong> The Planned Cost field takes into consideration the Cost/Hr field set at the Job Role level (when the Cost/Hr field has not been set at the user level).<br><strong>When viewing Planned Cost from the Utilization report on the project:</strong> The Planned Cost field does not take into consideration the Cost/Hr field set at the Job Role level. Instead, if you want the Utilization report to take into consideration the Cost/Hr field set at the Job Role level, you must set the Cost Type on the task to Role Hourly. </li> 
     </ul> </p> <p><strong>Actual Cost</strong> is calculated by the following formula: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Where the Actual Labor Cost is calculated by:</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>For example, a user has a Cost per Hour rate of $20 in their profile. When they log 5 hours for a task, the Actual Labor Cost is $100 for that task. If the user does not have a Cost per Hour rate associated with them, the Actual Cost calculates based on the Cost per Hour rate of their Primary Job Role. If they do not have a job role or the Cost per Hour rate of their job role is not defined, then the Actual Cost of the task is zero. </p> <p>Note: Actual Costs are calculated based on the Cost per Hour rate for the user who is logging the time, regardless of who is assigned to the task. Also, the billing hourly rate in the formula considers any date effective changes of the rate.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Role Hourly</p> </td>
   <td> <p><strong>Planned Cost</strong> is calculated by the following formula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Where the Task Planned Labor Cost is calculated by:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Note: If you assign multiple resources to a task, Workfront adjusts calculations for Planned Hours based on the percentage of the task assigned to each resource. Also, the hourly rate in the formula considers any date effective changes of the rate.</p> <p><strong>Actual Cost</strong> is calculated by the following formula: </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Where the Task Actual Labor Cost is calculated by:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>For example, a task is assigned to a job role or a user with a job role for which the Cost per Hour rate is $20. When a user logs 5 hours for a task, the Actual Labor Cost is $100 for that task. If the user assigned to the task does not have a job role associated with them on the task, the Actual Cost calculates based on the Cost per Hour rate of their Primary Job Role. If they do not have a job role or the Cost per Hour rate of their job role is not defined, then the Actual Cost of the task is zero. </p> <p>Note: The Actual Hours of a Role Hourly task calculate based on the job roles of the users associated with the task, not on the roles associated with the user who is logging the time. Also, the billing hourly rate in the formula considers any date effective changes of the rate.</p> <p>If your Workfront administrator enabled the <strong>Assign Job Roles to hour entries manually</strong> setting in the Timesheets &amp; Hours Preferences area in Setup, and the user logging time on the task selects a different role to associate with this time, the Actual Cost of a Role Hourly task calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fixed Hourly</p> </td> 
   <td> <p><strong>Planned Cost</strong> is calculated by the following formula:</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Where the Task Labor Cost is calculated by:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>Actual Cost</strong> is calculated by the following formula: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Where the Actual Task Labor Cost is calculated by:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>This cost type does not take individual users or job roles into account.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>No Cost</p> </td> 
   <td> <p>This Cost Type does not affect costs. If a parent task has this Cost Type, subtasks with another Cost Type calculate according to their individual Cost Types, and the cost of the parent task is affected accordingly. </p> <p>When a user with No Access to Financial Data or a user with no financial permissions on a template creates a project from that template, this is the default Cost Type for the tasks on the project.</p> <p>For information about access to Financial Data, see the article <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> <p>For information about financial permissions on objects, see the article <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Share financial permissions on an object</a>.</p> <p>For information about creating projects from templates, see the article <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Create a project using a template</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## How Workfront tracks costs for issues {#how-workfront-tracks-costs-for-issues}

Issues do not have and do not affect the following types of costs on a project:

* Planned Cost
* Budgeted Cost

Issues, can, however, have an **Actual Cost**, which also affects the Actual Cost of the project.

The following table explains how Actual Cost is calculated for issues, depending on the type of assignment on the issue:

<table style="table-layout:auto"> 
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td> <p>User Assignment</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Actual Cost</strong> is calculated by the following formula:</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>The Cost per Hour rate of the user who is logging the time is taken into account here, regardless of who is assigned to the issue. </p> <p>If the user who logs the time does not have a Cost per Hour rate in their profile, the Cost per Hour rate of their Primary Job Role calculates the Actual Cost of the issue.</p> <p>If the user who is logging the time has no role in their profile or no rate associated with it, the Actual Hours are calculated using the Cost per Hour rate of the Primary Job Role of the Primary Assignee on the issue. If that role has no rate defined, the Actual Cost of the issue is zero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Role Assignment</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Actual Cost</strong> is calculated by the following formula:</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>The Cost per Hour rate of the user logging the time on the issue is taken into account here, regardless of what role is assigned to the issue. </p> <p>If the user logging the time does not have a Cost per Hour rate associated with them, the Cost per Hour rate of their Primary Role calculates the Actual Cost of the issue.</p><p>If the user who is logging the time has no role in their profile or no rate associated with it, the Actual Cost of the issue is zero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>No Assignment</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Actual Cost</strong> is calculated by the following formula:</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>If the user who logs the time does not have a Cost per Hour rate associated with their profile, the Cost per Hour rate of their Primary Job Role calculates the Actual Cost of the issue. </p> <p>If the user who is logging the time has no job role associated with their profile or their Primary Job Role does not have a Cost per Hour rate defined, the Actual Cost of the issue is zero. </p> </td> 
  </tr> 
 </tbody> 
</table>
