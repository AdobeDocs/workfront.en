---
filename: select-project-update-type
product-area: projects
navigation-topic: manage-projects
title: Select the project Update Type
description: By selecting an Update Type for a project, you can control how frequently the changes you make to the timeline of the project are saved on the parent tasks or the project.
---

# Select the project Update Type

By selecting an Update Type for a project, you can control how frequently the changes you make to the timeline of the project are saved on the parent tasks or the project.

When the project timeline is updated, it is recalculated based on changes made to the project, its tasks, or changes made to another project that the timeline is dependent on.

For example, the following changes to the tasks on the project trigger an update to the timeline &nbsp;of the project:

* Update the dates of tasks
* Change predecessor relationships of tasks
* Change parent-child relationships, adding or removing assignments in addition to changing the task constraint or duration type.

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
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Update a project's Update&nbsp;Type

When the tasks update, their parent objects (parent tasks or the project) update at the time indicated by the Update Type.&nbsp; To specify an Update Type for your project:

<ol> 
 <li value="1">Go to the project whose Update Type you want to specify.</li> 
 <li value="2"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the More menu 
    <img src="assets/more-icon.png"> next to the name of the project, then click 
    <b>Edit</b> 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the More menu 
   <img src="assets/more-icon.png"> next to the name of the project, then click 
   <b>Edit</b> 
  </MadCap:conditionalText>.</li> 
 <li value="3"> <p>Click <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
     <span class="bold">Project</span> 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
    <span class="bold">Project</span> 
   </MadCap:conditionalText><span class="bold">Settings</span>.<br></p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/update-type-field-on-project-edit-box-nwe-350x378.png" style="width: 350;height: 378;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/update-type-field-on-project-edit-box-nwe-350x378.png" style="width: 350;height: 378;"> </p> </li> 
 <li value="4"> <p>In the <span class="bold">Update Type</span> field, select whether you want <em>Workfront</em> to calculate the timeline of the project automatically daily, when there is a change, or if you want the project manager to calculate it manually. </p> <p>Select from the options in the list below.&nbsp;</p> <note type="important">
   If the timeline of a project is longer than 15 years, 
   <em>Workfront</em> does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual. 
  </note> 
  <ul> 
   <li> <p><span class="bold">Automatic and On Change:</span>&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp; <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li> 
   <li><span class="bold">Change Only:</span>&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.</li> 
   <li> <p><span class="bold">Automatic Only:</span>&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
      A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
    </note> </li> 
   <li><span class="bold">Manual Only:</span>&nbsp;The project timeline is updated only&nbsp;when you select the option to <span class="bold">Recalculate Timelines</span>, as described in the section "Manual Recalculation" in&nbsp;the article <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li> 
  </ul> </li> 
 <li value="5"> <p>Click <span class="bold">Save</span>.</p> </li> 
</ol>

