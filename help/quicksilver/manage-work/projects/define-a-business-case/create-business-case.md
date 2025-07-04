---
navigation-topic: business-case-and-scorecards
title: Create a Business Case for a project
description: You can use the Business Case to request a project and define the purpose, the budget, and the potential benefit for the project. The Portfolio Manager or Project Sponsor uses the information from the Business Case to analyze and prioritize the project before they approve it.
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
---
# Create a Business Case for a project

<!--Audited: 6/2025-->

You can use the Business Case to request a project and define the purpose, the budget, and the potential benefit for the project. The Portfolio Manager or Project Sponsor uses the information from the Business Case to analyze and prioritize the project before they approve it.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
   <p>Current: Prime or higher</p> 
   <p>Legacy: Pro or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> 
   <p>Current: Standard </p> 
   <p>Legacy: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configurations</p></td> 
   <td> <p>Edit access to Projects, Financial Data, and Resource Management</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage or higher permissions on the project</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

 +++

## Prerequisites

Consider the following when requesting a project through a Business Case:

* Your Adobe Workfront administrator or group administrator must enable the sections of the Business Case before they appear on your project.  
  For information about enabling the sections in the Business Case at the system level, see the article [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  For information about the areas of the Business Case, see the article [Overview of the Areas of the Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* You must complete all areas of the Business Case except for the Goals area if you want your project to receive a Score in the Portfolio Optimizer. Completing the Goals area is optional. The project receives a Score in the Portfolio Optimizer, even if this area is not completed.

  For information about working with Scorecards and with the Portfolio Optimizer, see the article [Apply a scorecard to a project and generate an Alignment Score](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

## Create a Business Case

{{step1-to-projects}}

1. Click&nbsp;**New Project**, then select **Request Project** from the drop-down that appears. The project is created and the **Idea** status is assigned by default.

   >[!CAUTION]
   >
   >If the Idea status has been deleted in your Workfront instance, the project is placed in the default status for new projects as defined in the Project Preferences area. For information about setting up project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Enter a name in the project title field. 
1. (Optional) Click the **More** icon ![More icon](assets/qs-more-icon-on-an-object.png), then **Attach Template** to create the Work Breakdown Structure of your project.

   Or

   Start adding tasks to the project manually. 

1. (Conditional) If you selected to attach a template, continue attaching the template to the project.
1. In the left panel, click **Business Case**. 
1. (Optional) To edit the **Project Info** section, click **Edit Project Info**.&nbsp;

   For more information about editing the **Project Info** section fields, see the section [Project Info](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) in the article [Overview of the Areas of the Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Optional) To edit the **Goals** section, click **Edit Goals**.

   For more information about editing the **Goals** section of the Business Case, see the section [Goals](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) in the article [Overview of the Areas of the Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Optional) To edit the **Expenses** section, click **Edit Expenses**.

   For more information about editing the **Expenses** section of the Business Case, see the section [Expenses](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) in the article [Overview of the Areas of the Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Optional) Click **Edit Resource Budgeting** to budget your resources and obtain the Budgeted Labor Cost associated with the job roles on the project. For more information, see [Budget resources in the Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   >[!TIP]
   >
   >The information displayed here is the same as the information displayed in the system-level resource budgeting tools.

1. (Optional)&nbsp;Click **Edit Risks** to add potential risks to this project. For information about adding risks to the Business Case, see the [Risks](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks) section in the article [Overview of the Areas of the Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md). 
1. (Optional) Select a **Scorecard** in the **Add a Scorecard to this Project** drop-down menu.

   Scorecards must be created before they can be attached to projects.

   For more information about scorecards, see the article [Apply a scorecard to a project and generate an Alignment Score](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. (Optional) Select a **Custom Form** in the **Custom Forms** drop-down menu.

   Custom Forms must be created before they can be attached to projects.

   For more information about Custom Forms, see the article [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click&nbsp;**Submit**. The project status is changed to **Requested** and it is submitted to have the Business Case approved.
 
   For more information about approving a Business Case, see the article [Approve a Business Case](../../../manage-work/projects/define-a-business-case/approve-business-case.md).


>[!TIP]
>
> After completing the Business Case, you can export a copy of it to a .pdf file.&nbsp;For more information about exporting the Business Case to a .pdf file, see [Export the Business Case of a project](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md).


