---
filename: create-project-from-template
product-area: projects;templates
navigation-topic: create-projects
title: Create a project using a template
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Create a project using a template

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

You can use templates as a framework to create new projects. If you have projects that repeat often, using templates for the general timeline of the new project saves you from having to build the same projects repeatedly.

Templates provide you with a way to capture all of the repeatable processes, information, and settings associated with your projects. All of the information associated with a template is transferred to the project. This includes tasks, assignments, durations, documents, financial details, risks, and custom forms.

>[!TIP]
>
>The status of a new project created from a template corresponds with the status defined by your *Workfront administrator* in the main Project Preferences area or by a *group administrator* `(or *Workfront administrator*) in the Project Preferences area for a group.` For information about configuring project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) or [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

You have the following options for creating a project from a template:

* Create a project from a template in the Projects area
* Create a project from a template at the template level
* Attach a template to an existing project

  For information, see [Attach a template to a project](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">Create a project from a template in the Groups area</li>
  -->

* Create a project from a template in the Groups area

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Workfront</em> licenses overview*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects and to Templates</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Create a project from a template in the Projects area

You can create a project from the Projects area in the

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Main Menu
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu</MadCap:conditionalText>`, or from the Projects area of a portfolio or a program.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
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
</ul> <note type="note">
If you have the Milestone View applied to the list of projects, follow the steps in the following section:
<a href="https://one.workfront.com/s/document-item?bundleId=workfront-classic&topicId=Content%2FManage_work%2FProjects%2FCreate_projects%2Fcreate-project-from-template.html#Create" target="_blank">Create a project from a template</a>.
</note> <p> <img src="assets/new-project-dropdown-nwe-350x358.png" style="width: 350;height: 358;"> </p> </li>
<li value="2"> <p>Click the name of a template in the <span class="bold">Favorite templates</span> list</p> <p>Or</p> <p>Do the following:</p>
<ol>
<li value="1"> <p>Select <span class="bold">New Project from&nbsp;Template</span>.</p> </li>
<li value="2"> <p>In the <span class="bold">Search&nbsp;Templates</span> field, start typing the name of a template and click it when it displays in the list.</p> </li>
<li value="3"> <p>Review template details on the right.</p>
<div>
<p>The template details include the following:</p>
<ul>
<li> <p>Template duration</p> </li>
<li> <p>Template owner</p> </li>
<li> <p>The number of top-level tasks which includes the names of the top three tasks</p> </li>
<li> <p>The number of all tasks in the template</p> </li>
<li> <p>The names of the template custom forms</p> </li>
</ul>
</div> </li>
<li value="4">
<div>
<p>(Optional)&nbsp;Hover over the name of a template name and click the <span class="bold">Favorites</span> <span class="bold">icon</span><img src="assets/favorites-icon-small.png"> to mark it as a favorite for future use. </p>
<p>Or</p>
<p>Expand the <span class="bold">Favorite templates</span> list and select a template from the drop-down list. </p> <note type="tip">
You can have up to 40
<em>Workfront</em> items marked as favorites. This includes templates and other items.
</note>
</div> </li>
<li value="5"> <p>Click <span class="bold">Use template</span> when you have selected a template.</p> </li>
</ol> <p> <img src="assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png" style="width: 350;height: 279;"> </p> </li>
<li value="3"> <p>The <span class="bold">New Project</span> box opens.</p> <p> <img src="assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x285.png" style="width: 350;height: 285;"> </p> </li>
<li value="4"> <p>If a field is already populated in the template, the field is pre-populated in the <span class="bold">New Project</span> box. You can edit the pre-populated values to better match your project. For more information, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
<li value="5"> <p>Click <span class="bold">Create Project</span>.</p> <p>All details defined in the template associate automatically with the newly created project if you didn't change them in the previous step.</p> </li>
</ol>
</div>
-->

<ol> 
 <li value="1"> <p>Do one of the following:</p> 
  <ul> 
   <li> <p> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Click the 
      <span class="bold">Main Menu</span> 
      <img src="assets/main-menu-icon.png">, click 
      <span class="bold">Projects</span>, then expand 
      <span class="bold">New Project</span>. 
     </MadCap:conditionalText></p> </li> 
   <li> <p> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Go to a portfolio, then expand 
      <span class="bold">New Project</span>.
     </MadCap:conditionalText></p> <note type="tip">
     When you create a project using a template from a portfolio, the Portfolio field of the new project updates to display the portfolio you chose to create the project from. This overwrites the Portfolio field on the template, if it is specified. 
    </note> </li> 
   <li> <p> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Go to a program, then expand 
      <span class="bold">New Project</span>.
     </MadCap:conditionalText></p> <note type="tip">
     When you create a project using a template from a program, the Program field of the new projects updates to display the Program you chose to create the project from. The Portfolio field of the template updates to display the portfolio of the program you chose to create the project from. This overwrites the Program and Portfolio fields on the template, if they are specified. 
    </note> </li> 
   <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>If you are a <em>group administrator</em>, you can also create a project in the Projects section of a group you manage. For more information, see<a href="view-manage-projects-groups-area.md" class="MCXref xref"> View and create projects from the Groups area in the new Adobe Workfront experience</a>.</p> <note type="tip">
     When you create a project using a template from a group, the group you create the project from displays in the Group field of the new project only when the Group field of the template is not specified. If the template Group field is specified, the Group field of the new project is that of the template. 
    </note> </li> 
  </ul> <note type="note">
   If you have the Milestone View applied to the list of projects, follow the steps in the following section: 
   <a href="https://one.workfront.com/s/document-item?bundleId=workfront-classic&topicId=Content%2FManage_work%2FProjects%2FCreate_projects%2Fcreate-project-from-template.html#Create" target="_blank">Create a project from a template</a>.
  </note> <p> <img src="assets/new-project-dropdown-nwe-350x358.png" style="width: 350;height: 358;"> </p> </li> 
 <li value="2"> <p>Click the name of a template in the <span class="bold">Favorite templates</span> list</p> <p>Or</p> <p>Do the following:</p> 
  <ol> 
   <li value="1"> <p>Select <span class="bold">New Project from&nbsp;Template</span>.</p> </li> 
   <li value="2"> <p>In the <span class="bold">Search&nbsp;Templates</span> field, start typing the name of a template and click it when it displays in the list.</p> </li> 
   <li value="3"> <p>Review template details on the right.</p> 
    <div> 
     <p>The template details include the following:</p> 
     <ul> 
      <li> <p>Template duration</p> </li> 
      <li> <p>Template owner</p> </li> 
      <li> <p>The number of top-level tasks which includes the names of the top three tasks</p> </li> 
      <li> <p>The number of all tasks in the template</p> </li> 
      <li> <p>The names of the template custom forms</p> </li> 
     </ul> 
    </div> </li> 
   <li value="4"> 
    <div> 
     <p>(Optional)&nbsp;Hover over the name of a template name and click the <span class="bold">Favorites</span> <span class="bold">icon</span><img src="assets/favorites-icon-small.png"> to mark it as a favorite for future use. </p> 
     <p>Or</p> 
     <p>Expand the <span class="bold">Favorite templates</span> list and select a template from the drop-down list. </p> <note type="tip">
      You can have up to 40 
      <em>Workfront</em> items marked as favorites. This includes templates and other items.
     </note> 
    </div> </li> 
   <li value="5"> <p>Click <span class="bold">Use template</span> when you have selected a template.</p> </li> 
  </ol> <p> <img src="assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png" style="width: 350;height: 279;"> </p> </li> 
 <li value="3"> <p>The <span class="bold">New Project</span> box opens.</p> <p> <img src="assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x285.png" style="width: 350;height: 285;"> </p> </li> 
 <li value="4"> <p>If a field is already populated in the template, the field is pre-populated in the <span class="bold">New Project</span> box. You can edit the pre-populated values to better match your project. For more information, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li> 
 <li value="5"> <p>Click <span class="bold">Create Project</span>.</p> <p>All details defined in the template associate automatically with the newly created project if you didn't change them in the previous step.</p> </li> 
</ol>

## Create a project from a template in the Templates area

Instead of starting in the Projects area, you can create a project from a template by starting with the template.

&nbsp;

<!--
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<ol>
<li value="1">From the <span class="bold">Main Menu</span>, click <span class="bold">Templates</span>.</li>
<li value="2">Click the name of a template you want to use.</li>
<li value="3"> <p>Click the <span class="bold">More</span> menu <img src="assets/more-icon.png">, then click <span class="bold">Create Project.</span></p> <draft-comment>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/create-project-from-template-template-level-nwe-350x179.png" style="width: 350;height: 179;"> </p>
</draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/create-project-from-template-template-level-nwe-350x179.png" style="width: 350;height: 179;"> </p> <draft-comment>
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/project-sharing-on-template-nwe-2022-350x172.png" alt="Create project from template" style="width: 350;height: 172;"> </p>
</draft-comment><p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/project-sharing-on-template-nwe-2022-350x172.png" alt="Create project from template" style="width: 350;height: 172;"> </p> <p>The <span class="bold">New Project</span> box opens.</p> </li>
<li value="4"> <p>Specify a name for the project, then review each section and make any necessary changes.</p> <p> <img src="assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x285.png" style="width: 350;height: 285;"> </p> <p>If a field is already populated in the template, the field is pre-populated in the <span class="bold">New Project</span> box. You can edit the pre-populated values to better match your project. For more information, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
<li value="5"> <p>Click <span class="bold">Create Project.</span></p> <p>All details defined in the template associate automatically with the newly created project if you didn't change them in the previous step.</p> </li>
</ol>
</div>
-->

<ol> 
 <li value="1">From the <span class="bold">Main Menu</span>, click <span class="bold">Templates</span>.</li> 
 <li value="2">Click the name of a template you want to use.</li> 
 <li value="3"> <p>Click the <span class="bold">More</span> menu <img src="assets/more-icon.png">, then click <span class="bold">Create Project.</span></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/create-project-from-template-template-level-nwe-350x179.png" style="width: 350;height: 179;"> </p> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/project-sharing-on-template-nwe-2022-350x172.png" alt="Create project from template" style="width: 350;height: 172;"> </p> <p>The <span class="bold">New Project</span> box opens.</p> </li> 
 <li value="4"> <p>Specify a name for the project, then review each section and make any necessary changes.</p> <p> <img src="assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x285.png" style="width: 350;height: 285;"> </p> <p>If a field is already populated in the template, the field is pre-populated in the <span class="bold">New Project</span> box. You can edit the pre-populated values to better match your project. For more information, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li> 
 <li value="5"> <p>Click <span class="bold">Create Project.</span></p> <p>All details defined in the template associate automatically with the newly created project if you didn't change them in the previous step.</p> </li> 
</ol>

