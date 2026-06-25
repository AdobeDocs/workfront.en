---
product-area: projects
navigation-topic: create-projects
title: Create a project
description: A project is a large unit of work in Adobe Workfront. You can create projects from scratch, use a template, or convert issues or tasks to projects.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ftDbs1BguO-wdhSEzFe318xKOV86cbfBbyHkm0FPmqM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
  - id: d3382524-5489-431b-bde9-271ab257bc37
    internal-label: Workfront Scenario Planner
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Create a project

<!--remove Preview and Production references-->

<!-- Audited: 110/2025 -->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Projects represent a large amount of work that needs to be done in Adobe Workfront.

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
   <td> <p>Standard</p>
        <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project, you automatically receive Manage permissions to the project.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project, you automatically receive Manage permissions to the project.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->


## Ways to create projects

You can create a project in Workfront using one of the following methods:

* Create a project from scratch without using a template. This article describes how to create a project from scratch. 

* Copy an existing project.  
  For more information about copying a project, see [Copy a project](../../../manage-work/projects/manage-projects/copy-project.md).

* Use a template.  
  For more information about using a template to create a new project, see [Create a project using a template](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Import a project from Microsoft Project.  
  For more information about importing a project from MS Project, see [Import a project from Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Import a project using kick-starts.

  As a Workfront administrator, you can import projects using a kick-start.

  For information about importing data using kick-starts in Workfront, see [Import data into Adobe Workfront using a Kick-Start template](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  For information about importing projects using kick-starts, see [Kick-Starts scenario: simple project and task import preparation](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Publish an initiative from a scenario in the Adobe Workfront Scenario Planner. 

  For information about the Workfront Scenario Planner, see [The Scenario Planner overview](../../../scenario-planner/scenario-planner-overview.md). 
  
  For information about creating projects from publishing initiatives, see  [Update or create projects by publishing initiatives in the Scenario Planner](../../../scenario-planner/publish-scenarios-update-projects.md).

* Add projects as you connect them from a record type in Workfront Planning. 

  For information about access to Workfront Planning, see [Access overview](/help/quicksilver/planning/access/access-overview.md).

  For information about creating projects by adding them to records, see the section "Create projects when connecting them with records from Workfront Planning" in the article [Create Workfront objects from Workfront Planning as you connect them to records](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md).

* Add projects using Workfront Planning automations. 

  For information, see [Create objects using Adobe Workfront Planning record automations](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md). 

   You must have a new Workfront license and an additional Workfront Planning package for Workfront Planning.

   For information about access to Workfront Planning, see [Access overview](/help/quicksilver/planning/access/access-overview.md).

## Prerequisites

Before you begin, you must ensure that:

* Your system or group administrator enabled the "Allow users to create projects without using a template" preference in the Setup area. 
  
  For more information, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## New project default settings

When you create a project, Workfront applies a set of default settings to it. For example, the Status, Group, and Schedule Mode are preset when you create a project.

Consider the following:

* As a Workfront administrator or a group administrator, you can configure the default settings for a new project when configuring Project Preferences for your entire Workfront instance or for a group.
* Workfront applies the settings of the group, if there are any, before it applies those set by the Workfront administrator. 
* The default status of a new project corresponds with the status defined by your Workfront administrator in the main Project Preferences area or by a group administrator (or Workfront administrator) in the Project Preferences area for a group. 

  >[!NOTE]
  >
  >We recommend that the default status for a new project is Planning. As you are making changes to the new project, this ensures that notifications are not sent to the users assigned to the project.
  >
  >For more information about setting up the default status and other default settings for a new project, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) or [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

* The following scenarios exist for how Workfront defines the Group and Status of a new project:

  * If you create a project from scratch, the Group of the project is your Home Group. 
  
    The Status of the project is the default status in the Project Preferences of your Home Group, if there is one, or of your Workfront instance. You can change the default status when creating the project to any status available for the Group of the project. 

  * If you create a project using a template, the settings from the template take precedence over the settings established by the Workfront or group administrator.
    
    The Group of the new project is the Group of the template. If the template is not associated with a Group, then the Group of the project is the Home Group of the user who creates the project.

    The default status of a new project created from a template corresponds with the status defined by your Workfront administrator in the main Project Preferences area or by a group administrator (or Workfront administrator) in the Project Preferences area for the group. You can change the default status when creating a project from a template, to any of the statuses of the Group of the project which is either the Group of the template, or the Home Group of the user who creates the project. 

  * If you create a project by converting an issue, the group of a new project is the Group of the issue's existing project. If the user converting the issue does not have access to the issue's project or if the issue's project does not have a Group, the Group of the new project is the Home Group of the user converting the issue. 
    
    The new project's statuses match the group statuses of the group associated with the project, which is either the Group of the original project or the Home Group of the user converting the issue. 

    If you are using a template when you're creating the project by converting the issue, refer to the second scenario above to understand which Group and which Status Workfront applies to the new project. 

* Where documents are stored for a project and for its children objects (tasks and issues) depends on what your Workfront administrator chooses as the default for Storage Preferences in the System Preferences area of Setup. Depending on where you store documents in your Workfront instance, you can create the following types of projects:

  * Legacy Workfront storage projects
  * Adobe cloud storage projects.

  For more information, see [Enable Adobe cloud storage for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md). 

  >[!TIP]
  >
  > Your Workfront instance might not have both types of document storage.

* When you create an Adobe cloud storage project, a document folder with the same name of the project is created in the **Documents** section of the project. After you add tasks to the project, folders with the task's name are added to the **Documents** section of each task. 

For more information, see [Document management overview for projects and related objects](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).

## Create a project from scratch

>[!NOTE]
>
>If you are creating a project using a template, we recommend that you also see the article [Create a project using a template](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Do one of the following:

   * Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Projects** and expand **New Project**.
   * Go to a portfolio, then expand **New Project**.
   * Go to a program, then expand **New Project**.
   * If you are a group administrator, you can also create a project in the Projects section of a group you manage. For more information, see [Create and modify a group's projects](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![New Project menu](assets/new-project-drop-down-with-legacy-storage-option.png)

1. (Conditional) Depending on which document storage your organization is using, click one of the following:

    * **New project**, when the Workfront administrator chooses either **Adobe cloud storage**, or **Legacy Workfront**, and they did or did not select the **Allow user to select storage provider** setting. 
    * **New project (Legacy storage)**, when the Workfront administrator chooses either **Adobe cloud storage**, or **Legacy Workfront**, and they also selected the **Allow user to select storage provider** setting. 

      This option displays only when the **Allow user to select storage provider** setting is selected in the Setup area.

      For more information, see [Enable Adobe cloud storage for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md). 

      >[!NOTE]
      >
      >* When you create an Adobe cloud storage project from a legacy Workfront storage portfolio or program, the portfolio or program are also converted to Adobe cloud storage objects. All other legacy Workfront storage projects under the same portfolio or program remain unchanged. 
      >* Your Workfront instance might not have both types of document storage.

      A project is created and its default name follows the following patterns, depending on which storage Workfront uses for documents: 

      * `Untitled Project` for a legacy Workfront storage project.

        A legacy Workfront storage project displays a **Legacy Workfront storage** icon ![Legacy-storage project icon](assets/legacy-storage-project-icon.png) next to its name. 

      * `Untitled Project - < Month day, year hour.minute.second >` for an Adobe cloud storage project

        >[!IMPORTANT]
        >
        >Projects using Adobe cloud storage must have unique names.    


1. In the project's header, update the name of the project. Press Enter to save the name.

   ![Enter a name for the project](assets/rename-untitled-project.png)

   The header of the project page displays a quick overview of the current health and progress of a project. The information in the project header changes as the project information is updated.

1. Click **Start Adding Tasks**.

   Or

   Click **New Task** to add tasks to the project and assign resources to them.

   For more information about adding tasks to a project, see [Create tasks in a project](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Edit the project details by clicking the **More** menu to the right of the project name, in the header, then **Edit** ![Edit icon](assets/qs-edit-icon.png) next to the name of the project.

   The **Edit Project** box opens.

1. Add information about the project. 

   For more information about editing a project, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

    >[!TIP]
    >
    >The Status of the project should be Planning, or another status that is not Current. This allows you to make changes to the project without generating notifications to the project participants. 

1. Click **Save** to save your changes.

1. (Optional) After configuring the project settings and adding the tasks, you can change the status of the project to **Current** in the project header.

   This indicates that the project is now ready to start and users assigned to the tasks can now start working on them.

   For more information about project statuses, see [Access the list of system project statuses](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
