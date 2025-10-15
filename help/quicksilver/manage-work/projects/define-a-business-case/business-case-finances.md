---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Overview of Business Case financial fields
description: The Business Case sub-tab includes financial fields for the project. In order for some of the financial fields to have values, corresponding areas of the Business Case must be completed.
author: Becky
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
---
# Overview of Business Case financial fields

The Business Case sub-tab includes financial fields for the project.&nbsp;In order for some of the financial fields to have values, corresponding areas of the Business Case must be completed.&nbsp;&nbsp;

The following project financial fields display in the Business Case:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="col">Name of Field</th> 
   <th scope="col">Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aligned&nbsp;</td> 
   <td> <p>Displays the alignment of the project according to its scorecard. A high percentage value indicates that the project is well-aligned with the purpose and goals of the organization. <br>For more information about using scorecards, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Create a scorecard</a>.</p> <p>This field displays in the Business Case Summary area.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Budgeted Cost</td> 
   <td> <p>The total cost estimated to be associated with the project when the project launches.</p> <p>The Budgeted Cost for the project is calculated by the following formula:<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront uses the Budgeted Hours from the&nbsp;Resource Planner to calculate the Budgeted Labor Cost.<br>For more information about calculating Budgeted Cost, see <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calculate Budgeted Cost</a>.&nbsp;</p> <p>This field displays in the Business Case Summary area.</p> </td> 
  </tr> 
  <tr> 
   <td>Budgeted Expense Cost</td> 
   <td> <p>The budgeted cost of all the expenses on the project.&nbsp;</p> <p>This is calculated by the following formula:</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>For more information about calculating expenses, see <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Manage project expenses </a>.</p> <p>This field displays in the Expenses&nbsp;area.</p> </td> 
  </tr> 
  <tr> 
   <td>Budgeted Labor Cost</td> 
   <td> <p>The cost associated with the resources assigned to complete the work on the project.</p> <p>The Budgeted Labor Cost for the project is calculated by the following formula:<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>Workfront uses the Budgeted Hours from the&nbsp;Resource Planner to calculate the Budgeted Labor Cost.<br>For more information about calculating Budgeted Labor Cost, see <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>.</p> <p>This field displays in the Resource Budgeting area of the Business Case.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Expenses Planned Cost</td> 
   <td> <p>This is the same as Budgeted Expense Cost.&nbsp;</p> <p>Note:  The Expenses Planned Cost is different than the Planned Cost for the Project. The Expenses Planned Cost is calculated the Planned Amount of the expenses on the project, whereas the Planned Cost is calculated using the Planned Hours on the project.&nbsp;</p> <p>This field displays in the Expenses&nbsp;area, for each expense.</p> </td> 
  </tr> 
  <tr> 
   <td>Net Value</td> 
   <td> <p>This is the total expected value of the project after calculating its benefit and removing the costs.</p> <p>The Net Value for the project is calculated by the following formula:<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>For more information about calculating Net Value, see <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calculate Net Value</a>.<br></p> <p>This field displays in the Business Case Summary area.</p> </td> 
  </tr> 
  <tr> 
   <td>Planned Benefit</td> 
   <td>A manual estimate of the monetary benefit for your organization when this project is completed. It can be any amount of currency and it is specific to you and to each project you manage. The Planned Benefit cannot have a negative value. This field displays in the Business Case Summary area and it can be edited in the Project Info area of the Business Case. </td> 
  </tr> 
  <tr> 
   <td>Potential&nbsp;Cost of Risks</td> 
   <td> <p>This is the Potential Cost of all the risks on the project. </p> <p>This is calculated using the following formula:</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>For more information about risks on the project, see&nbsp;<a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Create and edit risks on projects</a>.</p> <p>This field displays in the Business Case Summary area.</p> </td> 
  </tr> 
  <tr> 
   <td>Potential Risk</td> 
   <td> <p>In the Business Case Summary, this is the amount of the cost of the all the risks if they should occur, based on their probability. For example, if a Risk has a Potential Cost of $100 and a Probability of occurring of 10%, the Potential&nbsp;Risk is $10. The Potential Risk in the Business Case Summary is calculated by the following formula:</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> for all risks. </p> </td> 
  </tr> 
  <tr> 
   <td>Risk Mitigation Cost</td> 
   <td> <p>The&nbsp;cost of the mitigation plan for the risks you are estimating might occur on the project.<br>For more information about risks on the project, see <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Create and edit risks on projects</a>.</p> <p>This field displays in the&nbsp;Risks area for each risk specified on the project.</p> </td> 
  </tr> 
  <tr> 
   <td>Potential Cost for one Risk</td> 
   <td> <p>The estimated financial cost when the risks defined on the project would actually occur, regardless of their probability.&nbsp;</p> <p>This is a manually updated field which displays on each risk in the Risks area of the Business Case.&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Risks Total Potential Cost</td> 
   <td> <p>This is the total estimated financial cost of all the risks defined on the project when they actually have occurred.&nbsp;</p> <p>This is calculated by the following formula:</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>It displays as a currency number next to the title of the Risks area of the Business Case.</p> </td> 
  </tr> 
 </tbody> 
</table>
