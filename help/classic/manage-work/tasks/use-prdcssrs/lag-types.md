---
filename: lag-types
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Overview of Lag Types
description: Lag is the amount of time that must pass after the completion of an enforced predecessor until the dependent task can begin (Positive Lag), or the amount of time that a dependent task could start before the predecessor starts (Negative Lag).
---

# Overview of Lag Types

Lag is the amount of time that must pass after the completion of an enforced predecessor until the dependent task can begin (Positive Lag), or the amount of time that a dependent task could start before the predecessor starts (Negative Lag).

The Planned, Projected and Estimated dates of the successor tasks are calculated taking into account the lag and Planned, Projected and Estimated Start (Completion) dates of the predecessor tasks.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Indicate Lag and Lag Types on tasks

You can indicate lag types on tasks when you define their predecessor relationships.

* [Indicate Lag Types in the Predecessors tab of a task](#lag-in-predecessors-tab) 
* [Indicate Lag Types in a task list](#add-lags-in-task-list)

### Indicate Lag Types in the Predecessors tab of a task

1. Go to a task for which you want to define the predecessor and the Lag Type. 
1. Select the **Predecessors** tab.

   Depending on your configuration, the **Predecessors** tab might be listed under the **More** drop-down menu.

1. (Optional) If you want to add a cross-project predecessor, click **Cross-Project Predecessors**.
1. Click **Add Predecessor**.

   ![add_predecessor_with_negative_lag__1_.png](assets/add-predecessor-with-negative-lag--1--350x311.png)

1. Start typing the name of the predecessor task, then select it when it appears in the list. 
1. Select the **Dependency Type**.

   For more information about predecessor Dependency Types, see [Overview of task dependency types](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Specify a **Lag** amount using a numeric value. You can specify negative numbers to indicate a negative lag. 
1. Select from the following options to identify the type of lag you would like to indicate for your predecessor:

   * **Days**
   * **Calendar Days**
   * **Percent**
   * **Day of the Week**
   * **Day of the Week (Non-Zero)**

     For more information about these Lag Types and how they are calculated, see the section [Lag Types overview](#understanding-lag-types) in this article.

1. Click **Save**.

### Indicate Lag Types in a task list

1. Go to a task list, and select the **Standard** View from the **View** drop-down menu.

1. Click inside the **Predecessors** column corresponding to the task for which you want to specify a predecessor and a lag amount. 
1. Enter the following with no spaces:

   * the number of the task you want to indicate as the predecessor of the task selected
   * the abbreviation for the dependency type you want to indicate between the tasks

     For more information about the abbreviations for Dependency Types, see [Overview of task dependency types](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
   
   * either a **+** for a positive lag or a **-** for a negative lag
   
   * the amount of the lag
   * the abbreviation for the Lag Type you want to use.

     For more information about the abbreviations for Lag Types, see the section [Lag Types overview](#understanding-lag-types) in this article.

   For example, to indicate that a task has a predecessor and a positive lag of 2 days, you would enter "1fs+2d" in the Predecessors column. 

1. Click Enter on your keyboard to save the changes to your task.

## Lag Types overview

An example of a task that would require a lag time might be sawing trees into lumber. If the freshly-cut wood must dry for a time before it can be cut, then there would be a lag time between cutting the trees and sawing them into lumber.

The following table illustrates the Lag Types and how to indicate the amount of time for each one: 

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Value</strong> </p> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Days (d)</p> </td> 
   <td> <p>The delay between two tasks linked by dependency is measured in working days. This is the default Lag Type. </p> <p>For example, if there is a finish-start dependency with a 2 working day lag and the predecessor task finishes on Friday, the dependent task starts on Wednesday. The weekend days do not count as part of the lag. </p> <p>Note: The maximum lag limit for days is 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Calendar Days (c)</p> </td> 
   <td> <p>The delay between two tasks is measured in calendar days, including holidays and weekends. </p> <p>Note: Although this lag type counts non-working days as part of the lag, a dependent task can never start on a non-working day. If this lag type makes the dependent task start on a non-working day, the Planned Start Date of the dependent task is scheduled for the following working day. </p> <p>For example, if there is a finish-start dependency with a 2 calendar day lag and the predecessor task finishes on Thursday, the dependent task starts on Monday instead of a Sunday. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Percent (p or pe)</p> </td> 
   <td> <p>The delay is expressed as a percentage of the estimated time to complete the predecessor task. </p> <p>For example, if there is a finish-start dependency with at 20% lag between on a 10 day predecessor task, the system will calculate how many days is 20% of the predecessors task duration and use that as the lag. In this case it would be 2 days after the task's completion. </p> <p>Note: The maximum lag limit for percent is 2000%.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Day of Week (w) </p> </td> 
   <td> <p>The delay between two tasks is measured by indicating the days of the week for the week that contains the Planned Completion Date of the predecessor.</p> <p>For this Lag Type, each day of the week is associated with a number:</p> 
    <ul> 
     <li>Sunday=1</li> 
     <li>Monday=2</li> 
     <li>Tuesday=3</li> 
     <li>Wednesday=4</li> 
     <li>Thursday=5</li> 
     <li>Friday=6</li> 
     <li>Saturday=7</li> 
    </ul> <p>If you want to indicate that the Planned Start Date of the successor should fall on a Tuesday of the current week, and the Tuesday is prior to the Planned Completion Date of the predecessor, you would code your successor with the following formula: </p> <p><em>4fs-3w</em> </p> <p>Note:  If the Tuesday passed for the week of the Planned Completion Date of the predecessor, then the Planned Start Date of the successor task is the first available working day of that week. </p> <p>If you want to indicate that the lag should fall on a Saturday of the current week, and the Saturday is after the Planned Completion Date of the predecessor, you would code your successor with the following formula:</p> <p><em>4fs+7w</em> </p> <p>If Saturday is a non-working day, the next available day after Saturday (to indicate positive lag) is selected as the Planned Start Date of the successor. </p> <p>To indicate past or future weeks, you can add a number in front of the day number for the lag type. </p> <p>For example, to indicate the Monday of 10 weeks ago, you can use this code to indicate the predecessor of your successor:</p> <p><code>4fs-102w</code> </p> <p>10 indicates 10 weeks ago, and 2 is the number assigned to Monday. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Day of Week Non Zero (k)</p> </td> 
   <td> <p>The delay between two tasks is measured identically to the Day of the Week lag type, except if the predecessor's time ends on the same day of the week specified. The lag time is then calculated to the adjacent week (+/-). </p> <p>In this case, the lag time can never be 0.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Negative Lag overview

You can use a negative Lag to indicate the need or ability for the task to begin before the predecessor task ending.

Consider the following rules when using negative lags:

* Negative Lag cannot force the Start/ Finish dates of a task to be before or after the Planned Start/ Finish dates of the project. These dates are specified in the Schedule From field on the project.

  In this case, consider the following:

   * Schedule the project From Completion Date. 
   * The last task on the project should use the Must Finish on Task Constraint. It is recommended to give the task a large enough duration in order to account for all tasks on the project. The remaining tasks work well with the As Soon As Possible constraint.

* Using a Finish-Start predecessor relationship with tasks might produce an error message.

  In this case, consider the following:

   * Set a Finish-Finish predecessor relationship between tasks.
   * The Duration of the successor task should equal or exceed the intended number of lag days between tasks.

