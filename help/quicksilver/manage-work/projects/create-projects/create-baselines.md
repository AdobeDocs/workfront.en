---
product-area: projects
navigation-topic: create-projects
title: Create project baselines
description: A baseline is a project snapshot that represents key pieces of information included in the initial project plan or at any given time during the life of the project.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
---
# Create project baselines

<!-- Audited: 12/2023 -->

A baseline is a project snapshot that represents key pieces of information included in the initial project plan or at any given time during the life of the project.

You can use baseline to compare those pieces of information from the current plan to the original plan or any other point in time, to identify problem tasks, scope creep, and other trends over time.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<!--
drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
    <td><p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations for working with baselines

* You can capture a snapshot of the progress on a project multiple times during the lifetime of the project, creating multiple baselines.
* You can view the information included in the baselines of a project by creating a baseline or by building a Baseline report.
* When you create a baseline, the task information is also captured on the baseline tasks of that baseline.
* You can view the information of the baseline tasks by building a Baseline Task report.

>[!IMPORTANT]
>
>A baseline takes a snapshot of the name, dates, and financial information of the project. The baseline does not include the values of custom fields on the project. For information about financial information included in the baseline, see [Project finances included in project baselines](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Create a baseline

You can create a baseline in the following ways:

* **Automatically**: Your Workfront administrator or a group administrator sets the project preference for Workfront to automatically create a baseline when a project becomes Current. When this setting is enabled, a baseline is created when the project status becomes Current. When this setting is not enabled, you must manually create baselines.

  For more information about configuring project preferences and setting up automatic baseline creation, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  >[!CAUTION]
  >
  >Enabling this setting automatically creates a baseline for a project every time a project's status changes to Current. The first created baseline is the default one. You must manually create all other baselines during the life of the project .

* **Manually**: You can create new baselines for the project as needed as the project progresses. You can then compare baselines to see how the project progressed over time.

To create a baseline:

1. Navigate to a project. 
1. In the left panel, click **Baselines**.

   Or

   Click **Show More**, then click **Baselines**.

   ![Baselines section on project](assets/baselines-section-on-project-with-header.png)

1. Click **New Baseline.**
1. Specify the name for the baseline.
1. (Optional) If this is the first baseline, you may want to choose it as the default.
1. Click **Save**.

   By default, the following information displays about the baseline you created:

   * Baseline name
   * Baseline Entry Date
   * Planned Start Date of the project when the baseline was created
   * Projected Start Date of the project when the baseline was created
   * Actual Duration of the project when the baseline was created
   * % Complete of the project when the baseline was created
   * Default Baseline indicator that shows whether a baseline is the Default baseline of the project

     >[!TIP]
     >
     >You cannot view information from any two baselines at the same time in the same view or report. You can only view information from a given baseline and the Default baseline in the same report. You can modify which baseline you consider to be the Default baseline any time during the life of the project.

1. (Optional) Click the **View** button, then create a new view or edit the current view to add fields to the view and compare additional information between baselines. For information, see [Create or edit views in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Create a Baseline or a Baseline Task report

To view baseline information, you can also create a Baseline or Baseline Task report. This allows you to display any number of fields about the baselines or baseline tasks to compare them in one view.

>[!TIP]
>
>You must create a baseline before you can create a Baseline or Baseline Task report.

For information about creating a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

We recommend that you add a Project Name grouping to your Baseline or Baseline Task report to make it easier to read.

For information about creating a grouping, see [Create groupings in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).
