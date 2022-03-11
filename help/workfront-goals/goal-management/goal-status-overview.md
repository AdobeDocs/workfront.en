---
filename: goal-status-overview
content-type: overview;reference
product: workfront-goals
navigation-topic: goal-management
title: Goal status overview in Adobe Workfront Goals
description: Your organization must have the following to use the functionality described in this article:
---

# Goal status overview in `Adobe Workfront Goals`

Your organization must have the following to use the functionality described in this article:

* A `Pro` or higher [ `Adobe Workfront` plan](https://www.workfront.com/plans). 
* An `Adobe Workfront Goals` license in addition to a `Workfront` license.

  Contact your `Workfront` account manager to learn about a `Workfront Goals` license.

  `Workfront Goals` is available only in `the new Adobe Workfront experience`.

For additional information about access to `Workfront Goals`, see Requirements to use Adobe Workfront Goals.
Goal statuses indicate whether a goal is active and currently recording progress, or if it is inactive, drafted, or already achieved.

## Consideration when updating goal statuses in `Workfront Goals`

<ul> 
 <li> <p>You can update the status of goals you created or that were shared with you. </p> </li> 
 <li> <p>Some restrictions exist and sometimes you cannot change the status of a goal to another status, according to the following rules: </p> 
  <table> 
   <col> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>From/ To</td> 
     <td>Draft</td> 
     <td>Active</td> 
     <td>Inactive</td> 
     <td>Closed</td> 
    </tr> 
    <tr> 
     <td>Draft</td> 
     <td>- </td> 
     <td>Yes</td> 
     <td>No</td> 
     <td>No</td> 
    </tr> 
    <tr> 
     <td>Active</td> 
     <td>No</td> 
     <td>-</td> 
     <td>Yes</td> 
     <td>Yes</td> 
    </tr> 
    <tr> 
     <td>Inactive</td> 
     <td>No</td> 
     <td>Yes</td> 
     <td>-</td> 
     <td>No</td> 
    </tr> 
    <tr> 
     <td>Closed </td> 
     <td>No</td> 
     <td>Yes</td> 
     <td>No</td> 
     <td>- </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li> <p>Opening a closed goal also updates the goal's progress. </p> </li> 
 <li> <p>Certain actions you perform on a goal also update its status.&nbsp;For information about how you can update goal statuses, see the following articles:</p> </li> 
 <ul style="list-style-type: circle;"> 
  <li><a href="../../workfront-goals/goal-management/create-goals.md" class="MCXref xref" xrefformat="{para}">Create goals in Adobe Workfront Goals</a> </li> 
  <li><a href="../../workfront-goals/goal-management/activate-goals.md" class="MCXref xref" xrefformat="{para}">Activate goals in Adobe Workfront Goals</a> </li> 
  <li><a href="../../workfront-goals/goal-management/delete-and-deactivate-goals.md" class="MCXref xref" xrefformat="{para}">Delete and deactivate goals in Adobe Workfront Goals</a> </li> 
  <li><a href="../../workfront-goals/goal-management/close-and-reopen-goals.md" class="MCXref xref" xrefformat="{para}">Close and reopen goals in Adobe Workfront Goals</a> </li> 
 </ul> 
</ul>

## Overview of goal statuses in  `Workfront Goals`

For information about creating `Workfront Goals` goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

Goals can have one of the following statuses in `Workfront Goals`:

* [Draft](#draft) 
* [Active](#active) 
* [Inactive](#inactive) 
* [Closed](#closed)

### Draft

* This is the default status for a newly created goal. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md). 
* `Workfront Goals` does not record progress on a drafted goal. 
* You cannot check in on a drafted goal. 
* You cannot close or deactivate drafted goals because they lack progress information.
* Drafted goals do not contribute to the progress calculation of other goals, and they are not taken into account in graphs. 
* Drafted goals display in the following areas of `Workfront Goals`:

  * `Goal List`
  * `Check-in` section (only as an aligned goal)
  * `Goal Alignment section` (only as an aligned goal)
  * `Pulse` section

>[!IMPORTANT]
>
>After you change the status of a goal to any other status, the goal can never be placed in a Draft status again.

### Active

* You can activate a drafted goal only when you associate it with a result, an activity, or align another goal to it. Activating the goal changes its status to Active. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md). 
* `Workfront Goals` records progress on active goals. 
* Active goals contribute to the progress calculation of other goals, and they are taken into account in graphs. 
* Active goals display in the following areas of `Workfront Goals`:

  * `Goal List`
  * `Check-in` section
  * `Goal Alignment section`
  * `Pulse` section
  * The progress of active goals displays in graphs

* You can re-activate a Closed or Inactive goal.

### Inactive

* You can deactivate an active goal when the owner stopped working on it temporarily or permanently. You can keep it for historical information. This updates the status of the goal to Inactive.

  For information about deactivating goals, see the "Deactivate goals" section in the article [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md). 

* You cannot deactivate a drafted or closed goal. 
* You can reactivate an inactive goal and continue to work on it. 
* `Workfront Goals` does not calculate progress on inactive goals. 
* You cannot check in on an inactive goal. 
* Inactive goals do not contribute to the progress calculation of other goals, and they are not taken into account in graphs. 
* Inactive goals have a progress history because they were once active, unlike drafted goals. 
* Inactive goals display in the following areas of `Workfront Goals`:

  * `Goal List`
  * `Goal Alignment section` (only as aligned goals)
  * `Pulse`

### Closed

<ul> 
 <li> <p>You can close a goal when you want to indicate that you have achieved it or that you are no longer working on it nor will you do so in the future. For information about closing goals, see <a href="../../workfront-goals/goal-management/close-and-reopen-goals.md" class="MCXref xref" xrefformat="{para}">Close and reopen goals in Adobe Workfront Goals</a>.</p> <note type="tip">
   If you plan on later working on a goal that is not yet achieved, we recommend you change the status to Inactive instead of Closed. 
  </note> </li> 
 <li>You cannot close goals that have never been activated, like drafted goals. </li> 
 <li>You can reopen a closed goal and continue working on it. </li> 
 <li><span>Workfront Goals</span> stops recording progress on closed goals.</li> 
 <li>You cannot check in on closed goals. </li> 
 <li>Closed goals display in the following area of <span>Workfront Goals</span>:
  <ul>
   <li><span>Goal List</span></li>
   <li><span>Check-in</span> section (only as aligned goals)</li>
   <li><span>Goal Alignment section</span> (only as aligned goals)</li>
   <li><span>Pulse</span></li>
   <li>Information from closed goals is also taken into account in the Graphs section. </li>
  </ul></li> 
</ul>

