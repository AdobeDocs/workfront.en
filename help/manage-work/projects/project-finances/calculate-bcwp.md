---
filename: calculate-bcwp
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculate Budgeted Cost of Work Performed (BCWP)
description: Also known as the Earned Value, the Budgeted Cost of Work Performed (BCWP) is a project performance metric that represents the amount of the task that has actually completed at the time when this metric is calculated.
---

# Calculate Budgeted Cost of Work Performed (BCWP)

## Overview of Budgeted Cost of Work Performed (BCWP)

Also known as the Earned Value, the Budgeted Cost of Work Performed (BCWP) is a project performance metric that represents the amount of the task that has actually completed at the time when this metric is calculated.

*Adobe Workfront* calculates the Budgeted Cost of Work Performed (BCWP) for both projects and tasks.

Consider the following when reviewing the values for the BCWP on a task or project:

* *Workfront* calculates the BCWP for a task based on your configuration for the Performance Index Method (PMI) of the project.

  You can configure your project to calculate the PMI using hours or cost and the BCWP is also calculated using the same values.

  For information about configuring how the BCWP is calculated, see the section [Configure how BCWP is calculated](#configur) in this article.

* *Workfront* calculates the BCWP for a project by adding all the BCWP values from all the parent tasks and individual tasks on the project.

  The values from children tasks are not added to the BCWP of the project.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Configure how BCWP is calculated

You can configure whether the BCWP is calculated in hours or costs by configuring how the Performance Index Method (PIM) of the project is calculated.

<ol> 
 <li value="1"> <p> </p> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Go to a project and expand 
     <span class="bold">Project Details</span> in the left panel.
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Go to a project and expand 
    <span class="bold">Project Details</span> in the left panel.
   </MadCap:conditionalText> </p> </li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In the <span class="bold">Finance</span> area, locate the <span class="bold">Performance Index Method</span> field and double click to edit it. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In the <span class="bold">Finance</span> area, locate the <span class="bold">Performance Index Method</span> field and double click to edit it. </p> <p> <img src="assets/pim-options-hour-cost-based-350x144.png" style="width: 350;height: 144;"> </p> </li> 
 <li value="3"> <p>Select from the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Hour-Based</td> 
     <td><em>Workfront</em> calculates the BCWP using the Planned Hours of the tasks.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Cost-Based</td> 
     <td><em>Workfront</em> calculates the BCWP using the Planned Cost of the tasks.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click&nbsp;<span class="bold">Save Changes</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click&nbsp;<span class="bold">Save Changes</span>.</p> <p>The BCWP of the tasks on the project is calculated using hours or costs.</p> </li> 
</ol>

## Calculate BCWP

*Workfront* calculates the Budgeted Cost of Work Performed (BCWP) for a task or project using the following formulas:

* 

  ```
  Task BCWP = Actual Percent Complete x Task Budget
  ```

* 

  ```
  Project BCWP = SUM(BCWP values of all parent and individual tasks)
  ```

The following values are used in these calculation:

| Actual Percent Complete |This is the actual percent complete of the task as it appears in *Workfront*. |
|---|---|
| Task Budget |This is the value for the Planned Hours or Planned Cost of the task. |

For example, if the actual percent complete of the task is 25% and the Task Budget or the Planned Cost is $10,000, then the BCWP for the task is:

```
BCWP = 25% x $10,000 = $2,500
```

## Locate the BCWP for a project or a task

You can view the value of the Budgeted Cost of Work Performed in a report or list, by adding the BCWP column to your view.

<ol> 
 <li value="1">Go to a list of tasks or projects.</li> 
 <li value="2">Expand the <span class="bold">View</span> menu and select <span class="bold">New View</span> or <span class="bold">Customize View</span>.</li> 
 <li value="3">Click <span class="bold">Add Column</span>.</li> 
 <li value="4"> <p>In the <span class="bold">Show in this column:</span> field start typing <span class="bold">BCWP</span> and click to select it when it displays in the list.</p> <p> <img src="assets/bcwp-project-view.png"> </p> </li> 
 <li value="5">Click <span class="bold">Save View</span>.</li> 
 <li value="6">The BCWP field displays in the view.</li> 
</ol>

