---
filename: configure-timeline-recalculations-projects
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configure timeline recalculations for projects
description: Recalculating timelines allows managers to see how forces outside of the project are impacting the project's timeline. A project's timeline refers to the planned and projected dates for the project.
---

# Configure timeline recalculations for projects

Recalculating timelines allows managers to see how forces outside of the project are impacting the project's timeline. A project's timeline refers to the planned and projected dates for the project.

As an *Adobe Workfront administrator*, you can manually recalculate timelines for all projects in the system. Project owners can also manually recalculate timelines for individual projects. For more information, see [Recalculate project timelines](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

This article describes how you, as a *Workfront administrator*, can determine how and when *Workfront* automatically calculates project timelines by configuring project preferences in the Setup area.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator access level</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure automatic recalculations

As an *Adobe Workfront administrator*, you can configure when&nbsp;*Workfront* automatically recalculates project timelines. *Workfront* can recalculate project timelines either every night or when the project scope changes, or both.

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">Main Menu</span> icon 
    <img src="assets/main-menu-icon.png"> in the upper-right corner of 
    <em>Workfront</em>, then click 
    <span class="bold">Setup</span>
    <img src="assets/gear-icon-settings.png">.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click the 
   <span class="bold">Main Menu</span> icon 
   <img src="assets/main-menu-icon.png"> in the upper-right corner of 
   <em>Workfront</em>, then click 
   <span class="bold">Setup</span>
   <img src="assets/gear-icon-settings.png">.
  </MadCap:conditionalText> </li> 
 <li value="2">Click <span class="bold">Project Preferences</span> > <span class="bold">Projects.</span></li> 
 <li value="3"> <p>In the <span class="bold">Timelines</span> section, enable or disable one or both of the settings below. By default, both settings are enabled. </p> 
  <ul> 
   <li> <p><span class="bold">Every night:</span> <em>Workfront</em>​​​ recalculates timelines at night only for projects where both of the following conditions are met:</p> 
    <ul> 
     <li>Have a status of Current</li> 
     <li> <p>Have had an update in the past three months</p> </li> 
    </ul> <p>In this case, <em>Workfront</em> recalculates the timeline for all projects that have an Update Type of Automatic or Automatic and On Change. </p> </li> 
   <li> <p><span class="bold">When a project's scope changes</span>: For information about what constitutes a project scope change, see <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>.</p> <p>In this case, <em>Workfront</em> recalculates the timeline for all projects that have an Update Type of Automatic and On&nbsp;Change or On Change Only.</p> </li> 
  </ul> <p>For information about project Update Types, see <a href="../../../manage-work/projects/planning-a-project/project-update-type-overview.md" class="MCXref xref">Project Update Type overview</a>. </p> </li> 
 <li value="4"> <p>Click <span class="bold">Save</span>.</p> <p>The timeline of all projects in the system recalculates automatically based on the Update Type of each project. </p> </li> 
</ol>

## Recalculate timelines for the entire&nbsp;*Workfront* instance

You can run the Recalculate Timeline diagnostic to manually recalculate all timelines in the *Workfront* system. This allows all Project Managers to see the influence of external changes immediately on both planned and projected dates. For more information, see [Use Diagnostics to trigger automated processes](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
