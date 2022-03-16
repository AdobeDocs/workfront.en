---
filename: copy-goals
product: workfront-goals
navigation-topic: goal-management
title: Copy goals in Adobe Workfront Goals
description: You can copy goals in Adobe Workfront Goals to create a goal. Some of the original goal information transfers to the new goal.
---

# Copy goals in Adobe Workfront Goals

You can copy goals in&nbsp;Adobe Workfront Goals to create a goal. Some of the original goal information transfers to the new goal.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Adobe Workfront Goals</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Goals or higher</p> <p>Note:  <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> Object permissions Manage permissions to the goal For information about sharing goals, see Share a goal in Adobe Workfront Goals. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

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

* All information about the goal, except the goal&nbsp;Period when it is in the past, is also copied to the new goal. 
* You can select to copy the results of an existing goal. The name of the results transfer to the new goal, but the current progress of the results on the existing goal does not copy to the new goal. The copied results are assigned to the same owner, by default.

  >[!NOTE]
  >
  >If the original owner was deleted or deactivated from&nbsp;Workfront, the new result is assigned to the logged in user.

* You cannot copy the activities of a goal when you copy the goal.

## Copy goals

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the ` `More icon` ![](assets/more-icon.png),`then click `Copy`. 

1. Update any of the following information for the copied goal:

   | New Goal |The name of the new goal. The default is the name of the original goal.  |
   |---|---|
   | Period |The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click `Define custom dates` to indicate a custom time period. By default, the Period is always the current quarter. |
   | Owner |The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal.  |
   | Description |Additional information about the goal.  |

1. (Conditional) Select `Copy results` if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal. 

   ` `**Tips: **``

  * The progress of the original result does not transfer to the copied goal. 
  * If the original owner was deleted or deactivated from&nbsp;Workfront, the new result is assigned to the logged in user.

1. Click `Save`.

   The copied goal is saved with a status of Draft and displays in the Goal Details panel.

   >[!IMPORTANT]
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
   >
   >
   >Do at least one of the following to be able to activate a goal: 
   >
   >  
   >  
   >  * Add a Result
   >  
   >  
   >    For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >  
   >  * Add an Activity
   >  
   >  
   >    For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >  
   >  * Align another goal to it
   >  
   >  
   >    For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).
   >  
   >  
   >

1. Click  `Activate`. The goal status updates to Active. 
1. Click the `X` icon in the upper-right of the Goal Details panel to close it.

   The new goal displays in the following sections:

  * Goal List 
  * Check-in (after it is activated)
  * Goal Alignment section (after it is activated) 
  * Pulse

1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:

  1. Go to the original goal in the Goal List, Check-in page, or Pulse section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
  1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
  1. Update the `the `Initial` value` of the new Result to match the `End At` value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.

