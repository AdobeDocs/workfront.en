---
filename: remove-results-activities-from-goals
product: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Remove results, activities, and projects from goals in Adobe Workfront Goals
description: You can remove results, activities, and projects from goals if they are no longer relevant.
---

# Remove results, activities, and projects from goals in *Adobe Workfront Goals*

You can remove results, activities, and projects from goals if they are no longer relevant.

For information about creating goals, and adding results and activities to them, see the following articles:

* [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md) 
* [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
* [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md) 
* [Edit results and activities in Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Request</em> or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>You must purchase an additional license for the <em>Adobe Workfront Goals</em> to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Adobe Workfront Goals</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Goals or higher</p> <p>Note:  <p>If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader">Object permissions</td> 
    <td> 
     <div> 
      <p>Manage permissions to the goal</p> 
      <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Adobe Workfront Goals</a>. </p> 
     </div> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> 
    <div> 
     <p>Manage permissions to the goal</p> 
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Adobe Workfront Goals</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

You must have the following before you can start:

* A Layout Template that includes the Goals area in the Main&nbsp;Menu.
* A goal with results or activities.

## Considerations for removing results, activities, and disconnecting projects from goals

`<li>  <ul>   <li> <p>You can remove results and activities only from active goals that are in a current or future time period. </p> </li>  </ul> </li>`

* You can remove results and activities from a goal by deleting them. Deleted results and activities cannot be recovered. 
* You cannot delete a project from a goal, but you can disconnect it. By disconnecting the project from the goal the percent complete of the project no longer affects the progress of the goal.

  For information about how projects affect goal progress, see [Overview of connecting projects to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md). 

* You cannot remove or disconnect a result or an activity from a goal if they are the last progress indicator for the goal.

  ` `**Warning: **``You can delete a project from a goal, even if it is the last progress indicator on the goal.&nbsp;The goal remains Active, but it shows no progress.

## Delete results and activities from goals

Removing results and activities from goals is identical.

<ol> 
 <li value="1"> <p> <p>Click the <span class="bold">Main Menu icon </span><img src="assets/main-menu-icon.png"> in the upper-right corner of your screen, then click <span class="bold">Goals</span>.</p> <p>This opens the <em>Workfront Goals</em> area. </p> <p>The <em>Goal List</em> displays by default. </p> </p> </li> 
 <li value="2"> <p>Click the name of a goal you want to remove results and activities from. </p> <p>This opens the Goal Details panel on the right.</p> </li> 
 <li value="3">Click <span class="bold">Results</span> to remove results or <span class="bold">Activities</span> to remove activities. </li> 
 <li value="4"> <p>Click the <span class="bold">gear icon</span> <img src="assets/settings-gear-icon.png"> to the right of the result or activity name, then click <span class="bold">Delete</span> > <span class="bold">Yes, delete</span>. </p> <p> <img src="assets/delete-result-goal-details-350x108.png" style="width: 350;height: 108;"> </p> <p>The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result. </p> </li> 
</ol>

## Disconnect projects from goals

<ol> 
 <li value="1"> <p> <p>Click the <span class="bold">Main&nbsp;Menu</span> icon <img src="assets/main-menu-icon.png"> > <span class="bold">Goals</span> in the upper-right corner of your screen.</p> <p>This opens the <em>Workfront Goals</em> area. </p> <p>The <em>Goal List</em> displays by default. </p> </p> </li> 
 <li value="2"> <p>Click the name of a goal you want to remove results and activities from. </p> <p>This opens the Goal Details panel on the right.</p> </li> 
 <li value="3">Click the <span class="bold">right-pointing arrow</span> to the left of the Activities sections to expand it. </li> 
 <li value="4"> <p>Click the <span class="bold">gear icon</span> <img src="assets/settings-gear-icon.png"> to the right of the project name, then click <span class="bold">Disconnect</span>.</p> <p> <img src="assets/disconnect-project-goal-details-350x94.png" style="width: 350;height: 94;"> </p> <p>The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.</p> </li> 
</ol>

