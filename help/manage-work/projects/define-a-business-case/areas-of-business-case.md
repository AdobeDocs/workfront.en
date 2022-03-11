---
filename: areas-of-business-case
content-type: overview
navigation-topic: business-case-and-scorecards
title: Overview of the Areas of the Business Case
description: This article describes the areas of the Business Case of a project.
---

# Overview of the Areas of the Business Case

This article describes the areas of the Business Case of a project.

For information about creating a Business Case for a project, see [Create a Business Case for a project in Adobe Workfront](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Your `Adobe Workfront administrator` `or `group administrator`` must enable all the&nbsp;sections in the Business Case&nbsp;before they are visible on the project, except for the Project Info section.&nbsp;The Project Info section is enabled by default.

For more information about enabling the areas of the Business Case, see the "Business Cases" section in&nbsp; [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

The following are areas in the Business Case of a project:

* Project Info
* Goals
* Expenses
* Resource Budgeting
* Risks
* Scorecard
* Custom Forms
* Business Case Summary

## Project Info

The `Project Info` area of the Business Case is not configurable by the `Workfront administrator`. All projects have a Project Info area in the Business Case.&nbsp;

The Project Info section of the Business Case includes the basic information of a project, before the project has actually started.

Consider editing the following fields:

<ul> 
 <li><span class="bold">Description</span>: Specify a description for your project.</li> 
 <li> <p><span class="bold">Project Owner</span> </p> <p>By default, the user creating the project is also the Project Owner. You can edit this field and indicate another active user as the owner of the project. </p> </li> 
 <li> <p><span class="bold">Project Sponsor</span> </p> <p>Consider adding someone else than the Project Owner as the Sponsor of the project. The sponsor receives the approval of the Business Case.&nbsp;</p> </li> 
 <li> <p><span class="bold">Portfolio</span>: Specify a Portfolio for the project. You must create the Portfolio and place it in the status of <span class="bold">Active</span> before it is available to select in this drop-down menu.</p> <p>For more information about portfolios, see <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md" class="MCXref xref">Portfolio overview in Adobe Workfront</a>.<br></p> <p>For more information about creating Portfolios, see <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Create a portfolio</a>.</p> </li> 
 <li><span class="bold">Planned Benefit</span>: Estimate what the monetary benefit is planned to be for your organization when this project is completed. It can be any amount of currency and it must be a positive value. For example $10,000.</li> 
 <li> <p><span class="bold">Status</span>: By default, the Status for a project request is set to <span class="bold">Idea</span>.</p> <p>If you change the Status to anything other than&nbsp;Idea or&nbsp;Planning, the&nbsp;<span class="bold">Submit</span> button disappears from the Business Case Summary area, and you can no longer submit the Business Case for approval.&nbsp;</p> </li> 
 <li><span class="bold">Fixed Start Date</span>: Specify a date when you would like for the project to start.</li> 
 <li> <p><span class="bold">Fixed End Date</span>: Specify a date when you would like for the project to end.</p> <note type="note">
   The Fixed Start and End Date on the Business Case do not impact the Planned Start and Completion Dates of the project. These represent the dates requested by the&nbsp;project creator&nbsp;for when the project would ideally develop. Instead, the Planned Start and Planned Completion Dates of the project show the planned timeline for the project which is based on the tasks on the project.
  </note> </li> 
</ul>

## Goals

Goals define the objectives for the project. This area is enabled by default in the Business Case, but the `Workfront administrator` might choose to not display it. This field displays the goals in order of priority.

>[!TIP]
>
>You can create strategic goals for your organization that are not connected to a project's individual Business Case. You must have access to  `Adobe Workfront Goals` to be able to create strategic goals. You can then connect them with projects outside of their Business Cases. For information about creating goals using `Workfront Goals`, see [Adobe Workfront Goals overview](../../../workfront-goals/goal-management/wf-goals-overview.md).

Defining the goals is optional for the project to receive a Score&nbsp;in the Portfolio Optimizer. This section is the only optional section in the Business Case. All other sections of the Business Case must be completed before the project is scored in the Portfolio Optimizer.&nbsp;You can indicate a priority level for a goal as you create the goal.

For more information about&nbsp;goals, see&nbsp; [Create Business Case goals](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Expenses

Expenses represent the non-labor costs that might be incurred during the life of a project. This area is enabled by default in the Business Case, but the `Workfront administrator` might choose to not display it.&nbsp;

Any expenses that you enter on the Business Case are also entered&nbsp;on the Expenses tab&nbsp;of the project, as Planned Expenses.

Expenses affect the following fields on the project:

* Budgeted Cost
* Net Value

For more information about the Budgeted Costs and Net Values, see [Overview of Business Case financial fields](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

For more information about&nbsp;expenses, see&nbsp; [Manage project expenses](../../../manage-work/projects/project-finances/manage-project-expenses.md)&nbsp;.

Your `Workfront administrator` can set up custom Expense Types.

For more information about&nbsp;creating custom Expense Types, see [Create custom expense types](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).&nbsp;

## Resource Budgeting

You can perform the following actions in the Resource Budgeting area of the Business case:

* Associate Resource Pools with the project.
* Budget your resources at the project level.

The hours budgeted for the resources on the project display in the Resource Budgeting area of the Business Case, generating the Budgeted Labor Cost of the project. This area of the Business Case is enabled by default.

For more information about budgeting resources for the project in the Business Case, see [Budget resources in the Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

Consider the following when viewing the Resource Budgeting section of the Business Case:

<ul> 
 <li> <p>You can budget resource information here using the following tools:</p> 
  <ul> 
   <li> <p>The <span>Resource Planner</span></p> <p>For information, see <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md" class="MCXref xref">Budget resources in the Business Case using the Adobe Workfront Resource Planner</a>. </p> </li> The Scenario Planner , if your company has purchased an additional license for Adobe Scenario Planner For more information, see Budget resources in the Business Case using the Adobe Workfront Scenario Planner. This is available only in the new Adobe Workfront experience and requires an additional license. For information about the Workfront Scenario Planner, see The Adobe Workfront Scenario Planner overview. 
  </ul> </li> 
 <li>The information displayed here also displays in the system-level <span>Resource Planner</span> or Scenario Planner.&nbsp;<br></li> 
 <li> <p>After budgeting your resources, the Budgeted Labor Cost of the project displays in the Resource Budgeting area if the roles are associated with Cost per Hour rates.&nbsp;The Budgeted Labor&nbsp;Cost displays in the currency of the project. </p> <note type="important">
   The Budgeted Labor Cost is the cost associated with the roles on the project, and not with the users. The sum of all Budgeted Labor Costs for the users may or may not equal the Budgeted Labor Cost of the job role associated with the users.&nbsp;
   <br>
  </note> <p>For more information about Budgeted Labor Cost, see <a href="../../../manage-work/projects/define-a-business-case/business-case-finances.md" class="MCXref xref">Overview of Business Case financial fields </a>.</p> <p>For more information about creating job roles and associating Cost per Hour rates with them, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> </li> 
</ul>

## Risks

Risks are factors that might prevent a project from finishing on time or on budget. Defining these factors is important for the Portfolio Manager or Project Sponsor to make an educated decision on the approval of the project. This area is enabled by default in the Business Case, but the `Workfront administrator` might choose to not display it.

You can associate a potential cost with the risks you are defining in case they should occur. The cost of the risks on a project affect the Net Value of the project.&nbsp;

For more information about the project Net Value, see [Overview of Business Case financial fields](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

For more information about creating risks, see&nbsp; [Create and edit risks on projects](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

Your `Workfront administrator` can set up custom Risk Types.

For more information about creating and editing&nbsp;custom Risk Types, see [Edit and create risk types](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## Scorecard

Scorecards measure the Alignment of the project. This area is enabled by default in the Business Case, but the `Workfront administrator` might choose to not display it.

For more information about applying a scorecard to a project and generating an alignment score, see [Apply a scorecard to a project and generate an Alignment Score](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

To apply a scorecard, your `Workfront administrator` must create one. The `Scorecard` area of the Business Case does not display unless a scorecard is created.

For more information about&nbsp;creating a scorecard, see&nbsp; [Create a scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Custom Forms

You can attach Custom Forms to a project, when defining a Business Case. This area is not enabled by default in the Business Case. The `Workfront administrator` must enable it to&nbsp;display it in the Business Case.

For more information about enabling the areas of the Business Case, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

To apply a custom form, your `Workfront administrator` must first create a custom form.

For more information about&nbsp;creating a custom form, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)&nbsp;.

You can use custom forms to collect additional information that is not displayed in the other fields of the Business Case.

For more information about applying a custom form, see [Attach a Custom Form to a Business Case](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md). ``

## Business Case Summary

* [Overview of the Business Case Summary](#understanding-business-case-summary) 
* [Export the Business Case](#exporting-the-business-case)

### `Overview of the Business Case Summary`

You can see a summary of the main project finances and whether a project is aligned or not with a Scorecard in the Business Case Summary panel, in the upper-right corner of the Business Case .

You cannot edit the Business Case Summary. This is only a quick view of the state of&nbsp;the project as it relates to financial fields and the Scorecard.&nbsp;  
&nbsp;

The following fields display in the Business Case Summary:

* The Project Net Value
* The Project Budgeted Cost
* The Potential Risk Cost
* The Planned Benefit
* The Alignment Score

For more information about these fields, see [Overview of Business Case financial fields](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### `Export the Business Case`

You can export the Business Case to a PDF&nbsp;file, in case you need to print it or attach it to an email in a more condensed format.&nbsp;

For information, see [Export the Business Case of a project in Adobe Workfront](../../../manage-work/projects/define-a-business-case/export-business-case.md).

<!--
To export a Business Case: Go to the Business Case area of a project. In the Business Case Summary area, click Export. A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format. (Optional) You can attach the PDF file to an email, or print it.
-->

<!--
You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format. The file contains all areas of the Business Case in an easy to read format. For information about how to export the Business Case, see Export the Business Case of a project in Adobe Workfront
-->

