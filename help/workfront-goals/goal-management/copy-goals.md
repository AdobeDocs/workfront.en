---
filename: copy-goals
product: workfront-goals
navigation-topic: goal-management
title: Copy goals in Adobe Workfront Goals
description: You can copy goals in Adobe Workfront Goals to create a goal. Some of the original goal information transfers to the new goal.
---

# Copy goals in *Adobe Workfront Goals*

You can copy goals in&nbsp;*Adobe Workfront Goals* to create a goal. Some of the original goal information transfers to the new goal.

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

## Considerations for copying goals

`You must have access to Edit Goals in your access level before you can copy goals. For information about granting access to Goals, see` ` [Grant access to Adobe Workfront Goals](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)`.

Some of the reasons you might want to copy an existing goal are:

* At the end of a time period (quarter or year), when you want to recreate the same goal for the next period.
* At the end of a time period, when the goal cannot be completed, and you want to work on it for another time period.
* When multiple team members have similar goals and you might need to create one for each one of them.

>[!TIP]
>
>You can copy a goal in any status. For information about goal statuses, see [Goal status overview in Adobe Workfront Goals](../../workfront-goals/goal-management/goal-status-overview.md).

Consider the following when copying goals:

<ul> 
 <li>All information about the goal, except the goal&nbsp;Period when it is in the past, is also copied to the new goal. </li> 
 <li> <p>You can select to copy the results of an existing goal. The name of the results transfer to the new goal, but the current progress of the results on the existing goal does not copy to the new goal. The copied results are assigned to the same owner, by default. </p> <note type="note">
   If the original owner was deleted or deactivated from&nbsp;
   <em>Workfront</em>, the new result is assigned to the logged in user.
  </note> </li> 
 <li>You cannot copy the activities of a goal when you copy the goal. </li> 
</ul>

## Copy goals

<ol> 
 <li value="1"> <p>Go to a goal and click it to open the Goal Details panel. </p> <p>For information about accessing an individual goal, see the "Access individual goals" section in <a href="../../workfront-goals/goal-management/access-goals-in-wf-goals.md" class="MCXref xref">Access and open goals in Adobe Workfront Goals </a>.</p> <p>This opens the Goal Details panel.</p> </li> 
 <li value="2">Click the <span><span class="bold">More icon</span> <img src="assets/more-icon.png">, </span>then click <span class="bold">Copy</span>. </li> 
 <li value="3"> <p>Update any of the following information for the copied goal:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">New Goal</td> 
     <td>The name of the new goal. The default is the name of the original goal. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Period</td> 
     <td>The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click <span class="bold">Define custom dates</span> to indicate a custom time period. By default, the Period is always the current quarter.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Owner</td> 
     <td>The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Description</td> 
     <td>Additional information about the goal. </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4"> <p>(Conditional) Select <span class="bold">Copy results</span> if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal. </p> 
  <div class="tips" data-mc-autonum="<b>Tips: </b>">
   <span class="autonumber"><span><b>Tips: </b></span></span> 
   <ul> 
    <li>The progress of the original result does not transfer to the copied goal. </li> 
    <li>If the original owner was deleted or deactivated from&nbsp;<em>Workfront</em>, the new result is assigned to the logged in user.</li> 
   </ul> 
  </div> </li> 
 <li value="5"> <p>Click <span class="bold">Save</span>. </p> <p>The copied goal is saved with a status of Draft and displays in the Goal Details panel. </p> <note type="important"> 
   <p>If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. </p> 
   <p>Do at least one of the following to be able to activate a goal: </p> 
   <ul> 
    <li> <p>Add a Result</p> <p>For information about adding results, see <a href="../../workfront-goals/results-and-activities/add-results-to-goals.md" class="MCXref xref">Add results to goals in Adobe Workfront Goals</a>.</p> </li> 
    <li> <p>Add an Activity</p> <p>For information about adding activities, see <a href="../../workfront-goals/results-and-activities/add-activities-to-goals.md" class="MCXref xref">Add activities to goals in&nbsp;Adobe Workfront Goals</a>. </p> </li> 
    <li> <p>Align another goal to it</p> <p>For information about aligning goals, see <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Align goals by connecting them in Adobe Workfront Goals</a>.</p> </li> 
   </ul> 
  </note> </li> 
 <li value="6">Click&nbsp;<span class="bold">Activate</span>. The goal status updates to Active. </li> 
 <li value="7"> <p>Click the <span class="bold">X</span> icon in the upper-right of the Goal Details panel to close it. </p> <p>The new goal displays in the following sections:</p> 
  <ul> 
   <li><em>Goal List</em> </li> 
   <li><em>Check-in</em> (after it is activated)</li> 
   <li><em>Goal Alignment section</em> (after it is activated) </li> 
   <li><em>Pulse</em> </li> 
  </ul> </li> 
 <li value="8">(Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:
  <ol>
   <li value="1"><p>Go to the original goal in the <em>Goal List</em>, <em>Check-in</em> page, or <em>Pulse</em> section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see <a href="../../workfront-goals/goal-management/manage-goal-comments.md" class="MCXref xref">Manage goal comments in Adobe Workfront Goals</a>.</p></li>
   <li value="2">Close the original goal, to preserve the progress in its original time period. For information about closing goals, see <a href="../../workfront-goals/goal-management/close-and-reopen-goals.md" class="MCXref xref">Close and reopen goals in Adobe Workfront Goals</a>. </li>
   <li value="3"><p> Update the <span>the <span class="bold">Initial</span> value</span> of the new Result to match the <span class="bold">End At</span> value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.</p></li>
  </ol></li> 
</ol>

