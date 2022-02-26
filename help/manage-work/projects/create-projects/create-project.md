---
filename: create-project
product-area: projects
navigation-topic: create-projects
title: Create a project
description: Projects represent a large amount of work that needs to be done in Adobe Workfront.
---

# Create a project

Projects represent a large amount of work that needs to be done in *Adobe Workfront*.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Workfront</em>plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## New project default settings

When you create a project, *Workfront* applies a set of default settings to it. For example, the Status, Group, or Schedule Mode are preset when you create the project.

Consider the following:

* As a *Workfront administrator* `or a *group administrator*`, you can configure the default settings for a new project when configuring Project Preferences.
* *Workfront* applies the settings of the group, if there are any, before it applies those set by the *Workfront administrator*. 
* If you create a project using a template, the settings from the template take precedence over the settings established by the *Workfront* or *group administrator*.

>[!NOTE]
>
>We recommend that the default status for a new project is Planning. As you are making changes to the new project, this ensures that notifications do not trigger to the users assigned to the project.

For more information about setting up the default status and other default settings for a new project, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Ways to create projects

You can create a project in *Workfront* by using one of the following methods:

* Create a project from scratch. This article describes how to create a project from scratch. 
* Copy an existing project.  
  For more information about copying project, see [Copy a project](../../../manage-work/projects/manage-projects/copy-project.md).

* Use a template.  
  For more information about using a template to create a new project, see [Create a project using a template](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Import a project from Microsoft Project.  
  For more information about importing a project from MS Project, see [Import a project from Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Import a project using kick-starts.

  As a *Workfront administrator*, you can import projects using a kick-start.

  For information about importing data using kick-starts in *Workfront*, see [Import data into Adobe Workfront via a Kick-Start template](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md) .

  For information about importing projects using kick-starts, see [Kick-Starts scenario: simple project and task import preparation](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md) .

* Publish an initiative from a scenario in the *Adobe Workfront Scenario Planner*. This is available only in *the new Adobe Workfront experience* and requires an additional license. For information about the *Workfront Scenario Planner*, see [The Adobe Workfront Scenario Planner overview](../../../scenario-planner/scenario-planner-overview.md). For information about creating projects from publishing initiatives, see 

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  <a href="../../../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner</a>
  </MadCap:conditionalText>
  -->

  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  <a href="../../../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner</a></MadCap:conditionalText>` .

## Create a project from scratch

<ol> 
 <li value="1"> <p>Do one of the following:</p> 
  <ul> 
   <li> <p> <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       Click the 
       <span class="bold">Main Menu</span> 
       <img src="assets/main-menu-icon.png">, click 
       <span class="bold">Projects</span>, then expand 
       <span class="bold">New Project</span>. 
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Click the 
      <span class="bold">Main Menu</span> 
      <img src="assets/main-menu-icon.png">, click 
      <span class="bold">Projects</span>, then expand 
      <span class="bold">New Project</span>. 
     </MadCap:conditionalText></p> </li> 
   <li> <p> <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       Go to a portfolio, then expand 
       <span class="bold">New Project</span>.
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Go to a portfolio, then expand 
      <span class="bold">New Project</span>.
     </MadCap:conditionalText></p> <note type="tip">
     When you create a project using a template from a portfolio, the Portfolio field of the new project updates to display the portfolio you chose to create the project from. This overwrites the Portfolio field on the template, if it is specified. 
    </note> </li> 
   <li> <p> <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       Go to a program, then expand 
       <span class="bold">New Project</span>.
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Go to a program, then expand 
      <span class="bold">New Project</span>.
     </MadCap:conditionalText></p> <note type="tip">
     When you create a project using a template from a program, the Program field of the new projects updates to display the Program you chose to create the project from. The Portfolio field of the template updates to display the portfolio of the program you chose to create the project from. This overwrites the Program and Portfolio fields on the template, if they are specified. 
    </note> </li> <draft-comment>
    <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>If you are a <em>group administrator</em>, you can also create a project in the Projects section of a group you manage. For more information, see<a href="view-manage-projects-groups-area.md" class="MCXref xref"> View and create projects from the Groups area in the new Adobe Workfront experience</a>.</p> <note type="tip">
      When you create a project using a template from a group, the group you create the project from displays in the Group field of the new project only when the Group field of the template is not specified. If the template Group field is specified, the Group field of the new project is that of the template. 
     </note> </li>
   </draft-comment>
   <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>If you are a <em>group administrator</em>, you can also create a project in the Projects section of a group you manage. For more information, see<a href="view-manage-projects-groups-area.md" class="MCXref xref"> View and create projects from the Groups area in the new Adobe Workfront experience</a>.</p> <note type="tip">
     When you create a project using a template from a group, the group you create the project from displays in the Group field of the new project only when the Group field of the template is not specified. If the template Group field is specified, the Group field of the new project is that of the template. 
    </note> </li> 
  </ul> <p> <draft-comment>
    <img src="assets/new-project-dropdown-nwe-350x358.png" style="width: 350;height: 358;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/new-project-dropdown-nwe-350x358.png" style="width: 350;height: 358;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="2">Click <span class="bold">New Project</span> if you want to create a project from scratch.</li> 
 <li value="3"> <p>Enter a name for your project. Press Enter to save the name.</p> <p> <draft-comment>
    <img src="assets/untitled-project-rename-new-project-nwe-350x127.png" style="width: 350;height: 127;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/untitled-project-rename-new-project-nwe-350x127.png" style="width: 350;height: 127;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The header of the project page displays a quick overview of the current health and progress of a project. The information in the project header changes as the project information is updated.</p> </li> 
 <li value="4"> <p>Click <span class="bold">Start Adding</span> <span class="bold">Tasks</span>.</p> <p>Or</p> <p>Click <span class="bold">New Task</span> to add tasks to the project and assign resources to them. <br>For more information about adding tasks to a project, see <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p> </li> 
 <li value="5"> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Edit the project details, by clicking the
     <span class="bold"> More menu</span> and then 
     <span class="bold">Edit</span> 
     <img src="assets/qs-edit-icon.png"> next to the name of the project.
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Edit the project details, by clicking the
    <span class="bold"> More menu</span> and then 
    <span class="bold">Edit</span> 
    <img src="assets/qs-edit-icon.png"> next to the name of the project.
   </MadCap:conditionalText></p> <p>The <span class="bold">Edit Project</span> dialog box opens.<br></p> <p>For more information about editing a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li> 
 <li value="6"> <p>(Optional) After configuring the project settings and add the tasks, you can change the status of the project to <span class="bold">Current</span>. </p> <p>This indicates that the project is now ready to start and users assigned to the tasks can now start working on them.<br></p> <p>For more information about project statuses, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref">Access the list of system project statuses</a>.</p> </li> 
</ol>

