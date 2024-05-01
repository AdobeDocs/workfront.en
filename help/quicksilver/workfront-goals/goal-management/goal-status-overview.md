---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Goal status overview in Adobe Workfront Goals
description: Goal statuses indicate whether a goal is active and currently recording progress, or if it is inactive, drafted, or already achieved.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
---
# Goal status overview in Adobe Workfront Goals

Your organization must have the following to use the functionality described in this article:

* For the new plan and license structure:

  * An Ultimate plan 
    
    Or
    
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. For information, see [Adobe Workfront plan](https://www.workfront.com/plans). 
    
* For the current plan and license structure: 

  * A Pro or higher 
  * An Adobe Workfront Goals license in addition to a Workfront license.

Contact your Workfront account manager to learn about a Workfront Goals license.

Goal statuses indicate whether a goal is active and currently recording progress, or if it is inactive, drafted, or already achieved.

## Consideration when updating goal statuses in Workfront Goals

* You cannot manually update the status of goals you created or that were shared with you. The status of goals updates depending on the actions you take on the goal. For example, activating a goal changes the Draft status to Active. 
* Some restrictions exist and sometimes you cannot change the status of a goal to another status, according to the following rules: 

  | From/ To |Draft |Active |Inactive |Closed |
  |---|---|---|---|---|
  | Draft |-  |Yes |No |No |
  | Active |No |- |Yes |Yes |
  | Inactive |No |Yes |- |No |
  | Closed  |No |Yes |No |-  |

* Opening a closed goal also updates the goal's progress. 
* Certain actions you perform on a goal also update its status.&nbsp;For information about how you can update goal statuses, see the following articles:

   * [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md) 
   * [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md) 
   * [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md) 
   * [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Overview of goal statuses in&nbsp;Workfront Goals

For information about creating Workfront Goals goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

Goals can have one of the following statuses in Workfront Goals:

* [Draft](#draft) 
* [Active](#active) 
* [Inactive](#inactive) 
* [Closed](#closed)

### Draft {#draft}

* This is the default status for a newly created goal. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md). 
* Workfront Goals does not record progress on a drafted goal. 
* You cannot update the progress of a drafted goal. 
* You cannot close or deactivate drafted goals because they lack progress information.
* Drafted goals do not contribute to the progress calculation of other goals, and they are not taken into account in graphs. 
* Drafted goals display in the following areas of Workfront Goals:

   * Goal List
   * Goal Alignment section (only as an aligned goal)
 

>[!IMPORTANT]
>
>After you change the status of a goal to any other status, the goal can never be placed in a Draft status again.

### Active {#active}

* You can activate a drafted goal only when you associate it with a result, an activity, or align another goal to it. Activating the goal changes its status to Active. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md). 
* Workfront Goals records progress on active goals. 
* Active goals contribute to the progress calculation of other goals, and they are taken into account in graphs. 
* Active goals display in the following areas of Workfront Goals:

   * Goal List
   * Goal Alignment section
   * The progress of active goals displays in graphs

* You can re-activate a Closed or Inactive goal.

### Inactive {#inactive}

* You can deactivate an active goal when the owner stopped working on it temporarily or permanently. You can keep it for historical information. This updates the status of the goal to Inactive.

  For information about deactivating goals, see the "Deactivate goals" section in the article [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md). 

* You cannot deactivate a drafted or closed goal. 
* You can reactivate an inactive goal and continue to work on it. 
* Workfront Goals does not calculate progress on inactive goals. 
* You cannot update the progress of an inactive goal. 
* Inactive goals do not contribute to the progress calculation of other goals, and they are not taken into account in graphs. 
* Inactive goals have a progress history because they were once active, unlike drafted goals. 
* Inactive goals display in the following areas of Workfront Goals:

   * Goal List
   * Goal Alignment section (only as aligned goals)

### Closed {#closed}

* You can close a goal when you want to indicate that you have achieved it or that you are no longer working on it nor will you do so in the future. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md).

  >[!TIP]
  >
  >If you plan on later working on a goal that is not yet achieved, we recommend you change the status to Inactive instead of Closed.

* You cannot close goals that have never been activated, like drafted goals. 
* You can reopen a closed goal and continue working on it. 
* Workfront Goals stops recording progress on closed goals.
* You cannot update the progress of a closed goal. 
* Closed goals display in the following area of Workfront Goals:

   * Goal List
   * Goal Alignment section (only as aligned goals)
   * Information from closed goals is also taken into account in the Graphs section.
