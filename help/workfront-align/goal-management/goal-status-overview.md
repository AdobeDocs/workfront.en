---
filename: goal-status-overview
content-type: overview;reference
product: workfront-goals
navigation-topic: goal-management
---




# Goal status overview in `Workfront Align` {#goal-status-overview-in-workfront-align}


Your company must have a `Workfront Align` license in addition to a `Workfront` license to use this functionality. Contact your `Workfront` account manager to learn about a `Workfront Align` license. 


`Workfront Align` is available only in `the new Workfront experience`. 


For additional information about access to `Workfront Align`, see [Access needed to use Workfront Align](access-needed-for-wf-align.md).
Goal statuses indicate whether a goal is active and currently recording progress, or if it is inactive, drafted, or already achieved. 



## Consideration when updating goal statuses in `Workfront Align` {#consideration-when-updating-goal-statuses-in-workfront-align}

You can update the status of any `Workfront Align` goal, regardless of who created it or who the owner is. 


However, some restrictions exist and sometimes you cannot change the status of a goal to another status, according to the following rules: 

Certain actions you perform on a goal also update its status.&nbsp;For information about how you can update goal statuses, see the following articles:



* [Create goals in Workfront Align](create-goals.md) 
* [Activate goals in Workfront Align](activate-goals.md) 
* [Delete and deactivate goals in Workfront Align](delete-and-deactivate-goals.md) 
* [Close and reopen goals in Workfront Align](close-and-reopen-goals.md) 




## Overview of goal statuses in  `Workfront Align` {#overview-of-goal-statuses-in-workfront-align}

For information about creating `Workfront Align` goals, see [Create goals in Workfront Align](create-goals.md). 


For information about activating goals, see [Activate goals in Workfront Align](activate-goals.md). 


Goals can have one of the following statuses in `Workfront Align`:



* [Draft](#draft) 
* [Active](#active) 
* [Inactive](#inactive) 
* [Closed](#closed) 




### Draft {#draft}




* This is the default status for a newly created goal. For information about creating goals, see [Create goals in Workfront Align](create-goals.md). 
* `Workfront Align` does not record progress on a drafted goal. 
* You cannot check in on a drafted goal. 
* You cannot close or deactivate drafted goals because they lack progress information.
* Drafted goals do not contribute to the progress calculation of other goals, and they are not taken into account in graphs. 
* Drafted goals display in the following areas of `Workfront Align`:
    
    
    * `Goal List`
    * `Check-in` section (only as an aligned goal)
    * `Goal Alignment section` (only as an aligned goal)
    * `Pulse` section
    
    





>[!IMPORTANT] {type="important"}
>
>After you change the status of a goal to any other status, the goal can never be placed in a Draft status again. 




### Active {#active}




* You can activate a drafted goal only when you associate it with a result, an activity, or align another goal to it. Activating the goal changes its status to Active. For information about activating goals, see [Activate goals in Workfront Align](activate-goals.md). 
*  `Workfront Align` records progress on active goals. 
* Active goals contribute to the progress calculation of other goals, and they are taken into account in graphs. 
* Active goals display in the following areas of `Workfront Align`:
    
    
    * `Goal List`
    * `Check-in` section
    * `Goal Alignment section`
    * `Pulse` section
    * The progress of active goals displays in graphs
    
    

* You can re-activate a Closed or Inactive goal. 




### Inactive {#inactive}




*  You can deactivate an active goal when the owner stopped working on it temporarily or permanently. You can keep it for historical information. This updates the status of the goal to Inactive. 


  For information about deactivating goals, see the "Deactivate goals" section in the article [Delete and deactivate goals in Workfront Align](delete-and-deactivate-goals.md). 

* You cannot deactivate a drafted or closed goal. 
* You can reactivate an inactive goal and continue to work on it. 
* `Workfront Align` does not calculate progress on inactive goals. 
* You cannot check in on an inactive goal. 
* Inactive goals do not contribute to the progress calculation of other goals, and they are not taken into account in graphs. 
* Inactive goals have a progress history because they were once active, unlike drafted goals. 
* Inactive goals display in the following areas of `Workfront Align`:
    
    
    * `Goal List`
    * `Goal Alignment section` (only as aligned goals)
    * `Pulse` 
    
    





### Closed {#closed}




*  You can close a goal when you want to indicate that you have achieved it or that you are no longer working on it nor will you do so in the future. For information about closing goals, see [Close and reopen goals in Workfront Align](close-and-reopen-goals.md).


  >[!TIP] {type="tip"}
  >
  >If you plan on later working on a goal that is not yet achieved, we recommend you change the status to Inactive instead of Closed. 



* You cannot close goals that have never been activated, like drafted goals. 
* You can reopen a closed goal and continue working on it. 
* `Workfront Align` stops recording progress on closed goals.
* You cannot check in on closed goals. 
* Closed goals display in the following area of `Workfront Align`:
    
    
    * `Goal List`
    * `Check-in` section (only as aligned goals)
    * `Goal Alignment section` (only as aligned goals)
    * `Pulse`
    * Information from closed goals is also taken into account in the Graphs section. 
    
    



