---
product-area: templates
navigation-topic: templates-navigation-topic
title: Create a project template
description: You can create and delete templates from the Templates area. When building a new template, you can enter the information for all of the tasks and for your future project settings. This information will then transfer to any project that you create from the template.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/JqR-bwIq1AVMOMz3aTWIKoiPep1VQ6IaONbbuDJ1AiA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Create a project template

<!-- Audited: 10/2025 -->

<!--remove all instances of new/ old experience and redo the steps when the toggle is removed-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->

You can create and delete templates from the Templates area. When building a new template, you can enter the information for all of the tasks and for your future project settings. This information will then transfer to any project that you create from the template.

>[!NOTE]
>
>A template and its tasks do not have actual dates, but rather an indication of which day (from when the future project might start) a task might start and on which day the task might need to complete. When using templates to create the future projects, the projects will receive actual dates. For information, see [Create a project](../create-projects/create-project.md).


You can create a new template in the following ways:

* From scratch, as described in this article.
* From existing projects, by saving a project as a template.

  For more information about creating templates from existing projects, see [Save a project as a template](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* By copying it from another template.

  For more information about copying an existing template, see [Copy a project template](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* By importing Blueprints. You must be a Workfront administrator to import Blueprints. For information, see [Configure a blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard </p><p>Plan</p> <p>You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:
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
   <td> <p>New: Standard </p><p>Or </p><p>Current: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Create a template

{{step1-to-templates}}

1. Click **New Template**.

1. (Conditional) Depending on which document storage your organization is using, click one of the following:

    * **New Template**, when the Workfront administrator chooses either **Adobe cloud storage**, or **Legacy Workfront**, and they did or did not select the **Allow user to select storage provider** setting. 
    * **New Template (Legacy storage)**, when the Workfront administrator chooses either **Adobe cloud storage**, or **Legacy Workfront**, and they also selected the **Allow user to select storage provider** setting. 

      This option displays only when the **Allow user to select storage provider** setting is selected in the Setup area.

      For more information, see [Enable Adobe cloud storage for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md). 

      A template is created and its default name follows the following patterns, depending on which storage Workfront uses for documents: 

      * **Untitled Template** for a Worfront-storage template.

        A legacy Workfront storage template displays a **Legacy Workfront storage** icon ![Legacy-storage project icon](assets/legacy-storage-project-icon.png) next to its name. 

      * **Untitled Template - < Month day, year hour.minute.second >** for an Adobe cloud storage template

        >[!IMPORTANT]
        >
        >Templates using Adobe storage must have unique names. 

   ![New template](assets/create-template-nwe-2022-350x102.png)

1. Specify a name for the new template in the template header, then press **Enter.**
1. Click the **Template Tasks** section in the left panel. 
1. Click **Start Adding Template Tasks** to add tasks inline

   Or

   Click **New Template Task** to start adding tasks to your template in the **New Template Task** box.

   The **Create Template Task** box opens when you click **New Template Task**.

   ![New experience for New Template Task](assets/new-template-task-box-unshimmed.png)

1. (Conditional) Update information in the following areas in the **Create Template Task** box:

   * Template Task Name
   * Overview
   * Assignments
   * Finance
   * Custom Forms
   * Documents
   * Settings 

   Updating information for a template task is similar to editing template tasks. 
   
   For more information, see [Edit template tasks](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-template-task.md).

   >[!NOTE]
   >
   >You cannot add recurring tasks to a template.

1. Click **Create template task**.

1. (Optional) After adding the template tasks, in the **Template Tasks** section, click the **Gantt chart**  icon ![Gantt icon](assets/gantt-icon.png) in the upper-right corner of the task list to see a visual representation of the template's task list.

   >[!TIP]
   >
   >You cannot edit tasks directly from a template task Gantt chart.

1. To add information to your new template, click the **More** menu ![More icon](assets/more-icon.png) to the right of the template name in the header, then click **Edit**.

   For information about editing a template, see [Edit project templates](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

   >[!NOTE]
   >
   >A project template's association with a group (or lack of a group) affects how project, task, and issue preferences determine certain settings in the template. 
   >
   >For more information, see the section "How preferences apply to templates and template tasks" in the article [Create and modify a group's project templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

1. Click **Save**.
1. (Optional) Add the following items to the template

   * Documents
   * Risks
   * Approval processes
   * Billing Rates
   * Expenses
   * Queue Details
   * Topic Groups and Queue Topics

1. (Optional) Add the following items to the tasks in the template:

   * Documents
   * Expenses
   * Approvals

   For information, see the section "Add more items to a template" in the article [Edit project templates](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).




