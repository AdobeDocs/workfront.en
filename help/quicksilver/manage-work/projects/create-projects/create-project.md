---
product-area: projects
navigation-topic: create-projects
title: Create a project
description: A project is a large unit of work in Adobe Workfront. You can create projects from scratch, use a template, or convert issues or tasks to projects.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
---
# Create a project

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is linked from the UI from the Projects global nav section in classic. Do not change/ remove)</p>
-->

Projects represent a large amount of work that needs to be done in Adobe Workfront.

## Access requirements

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
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
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New plan: Standard</p>
        <p>or</p>
        <p>Current plan: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project, you automatically receive Manage permissions to the project.</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Ways to create projects

You can create a project in Workfront using one of the following methods:

* Create a project from scratch without using a template. This article describes how to create a project from scratch. 

* Copy an existing project.  
  For more information about copying project, see [Copy a project](../../../manage-work/projects/manage-projects/copy-project.md).

* Use a template.  
  For more information about using a template to create a new project, see [Create a project using a template](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Import a project from Microsoft Project.  
  For more information about importing a project from MS Project, see [Import a project from Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Import a project using kick-starts.

  As a Workfront administrator, you can import projects using a kick-start.

  For information about importing data using kick-starts in Workfront, see [Import data into Adobe Workfront using a Kick-Start template](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  For information about importing projects using kick-starts, see [Kick-Starts scenario: simple project and task import preparation](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Publish an initiative from a scenario in the Adobe Workfront Scenario Planner. The Scenario Planner requires an additional license. For information about the Workfront Scenario Planner, see [The Scenario Planner overview](../../../scenario-planner/scenario-planner-overview.md). For information about creating projects from publishing initiatives, see  [Update or create projects by publishing initiatives in the Scenario Planner](../../../scenario-planner/publish-scenarios-update-projects.md).

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

## Create a project from scratch

1. Do one of the following:

   * Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner. Click **Projects**, then expand **New Project**.
   * Go to a portfolio, then expand **New Project**.
   * Go to a program, then expand **New Project**.
   * If you are a group administrator, you can also create a project in the Projects section of a group you manage. For more information, see [Create and modify a group's projects](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![New Project menu](assets/new-project-dropdown-nwe-350x358.png)

1. Click **New Project** in the menu to create a project from scratch.
1. Type a name for your project. Press Enter to save the name.

   ![Enter a name for the project](assets/rename-untitled-project.png)

   The header of the project page displays a quick overview of the current health and progress of a project. The information in the project header changes as the project information is updated.

1. Click **Start Adding Tasks**.

   Or

   Click **New Task** to add tasks to the project and assign resources to them.

   For more information about adding tasks to a project, see [Create tasks in a project](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Edit the project details by clicking the **More** menu and then **Edit** ![](assets/qs-edit-icon.png) next to the name of the project.

   The **Edit Project** dialog box opens.

   For more information about editing a project, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

1. (Optional) After configuring the project settings and adding the tasks, you can change the status of the project to **Current**.

   This indicates that the project is now ready to start and users assigned to the tasks can now start working on them.

   For more information about project statuses, see [Access the list of system project statuses](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
