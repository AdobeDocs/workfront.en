---
filename: import-project-from-ms-project
product-area: projects
navigation-topic: create-projects
title: Import a project from Microsoft Project
description: You can import projects from Microsoft Project into Adobe Workfront and manage all your projects in one application. Every time you import a project from Microsoft Project, a new project is created in Workfront.
---

# Import a project from Microsoft Project

You can import projects from Microsoft Project into *Adobe Workfront* and manage all your projects in one application. Every time you import a project from Microsoft Project, a new project is created in *Workfront*.

>[!IMPORTANT]
>
>Not all Microsoft Project fields are transferred to *Workfront*. 
>
>For more information about the compatibility of fields between *Workfront* and Microsoft Project, see [Map Microsoft Project fields to Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

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

## Create a project from a MS&nbsp;Project

You can create a project from the Projects area in the

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Main Menu
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu</MadCap:conditionalText>`, or from the Projects area of a portfolio or a program.

<ol> 
 <li value="1">Go to Microsoft Project and open a project that you want to import from in <em>Workfront</em>. </li> 
 <li value="2">Click <span class="bold">File</span>, then <span class="bold">Save As</span> to save the project as an .xml file. </li> 
 <li value="3">Log in to <em>Workfront</em>. </li> 
 <li value="4"> <p>Do one of the following:</p> 
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
     </MadCap:conditionalText> </p> </li> 
   <li> <p> <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       Go to a portfolio, then expand 
       <span class="bold">New Project</span>.
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Go to a portfolio, then expand 
      <span class="bold">New Project</span>.
     </MadCap:conditionalText> </p> </li> 
   <li> <p> <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       Go to a program, then expand 
       <span class="bold">New Project</span>.
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Go to a program, then expand 
      <span class="bold">New Project</span>.
     </MadCap:conditionalText> </p> </li> <draft-comment>
    <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>If you are a <em>group administrator</em>, you can also create a project in the Projects section of a group you manage. For more information, see<a href="view-manage-projects-groups-area.md" class="MCXref xref"> View and create projects from the Groups area in the new Adobe Workfront experience</a>.</p> </li>
   </draft-comment>
   <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>If you are a <em>group administrator</em>, you can also create a project in the Projects section of a group you manage. For more information, see<a href="view-manage-projects-groups-area.md" class="MCXref xref"> View and create projects from the Groups area in the new Adobe Workfront experience</a>.</p> </li> 
  </ul> </li> 
 <li value="5"> <p>Choose the <span class="bold">Import MS Project</span> option. </p> <p> <draft-comment>
    <img src="assets/new-project-dropdown-nwe-350x358.png" style="width: 350;height: 358;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/new-project-dropdown-nwe-350x358.png" style="width: 350;height: 358;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li> 
 <li value="6">Click <span class="bold">Select File</span>, then browse for the .xml file on your computer which you exported from Microsoft Project. </li> 
 <li value="7"> <p>Import the selected file.</p> <p><em>Workfront</em> begins the import process and creates a new project based on the file exported from Microsoft Project.<br></p> <p>After the import process is complete, you are directed to the new project page that displays a confirmation that the import has completed successfully.</p> <note type="note">
   <em>Workfront</em> has a 15-minute time limitation on file uploads. If the file upload takes longer than that, we recommend that you break out your project into smaller projects and import them separately. Once they have been imported into 
   <em>Workfront</em>, move the tasks from one project to the other project to combine them into one project. For information on moving tasks, see 
   <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Move tasks</a>.
  </note> </li> 
 <li value="8"> <p>(Optional) Continue editing the project in <em>Workfront</em>. For information about editing projects, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> <p>The status of a new project created from a template corresponds with the status defined by your <em>Workfront administrator</em> in the Project Preferences area or by a <em>group administrator</em> <span>in the Group Project Preferences area.</span> For information about configuring project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </li> 
</ol>

