---
filename: copy-goals
product: workfront-goals
navigation-topic: goal-management
---




# Copy goals in `Workfront Align` {#copy-goals-in-workfront-align}


Your company must have a `Workfront Align` license in addition to a `Workfront` license to use this functionality. Contact your `Workfront` account manager to learn about a `Workfront Align` license. 


`Workfront Align` is available only in `the new Workfront experience`. 


For additional information about access to `Workfront Align`, see [Access needed to use Workfront Align](access-needed-for-wf-align.md).


## Overview of copying goals {#overview-of-copying-goals}

Some of the reasons you might want to copy an existing goal are:



* At the end of a time period (quarter or year), when you want to recreate the same goal for the next period.
* At the end of a time period, when the goal cannot be completed, and you want to work on it for another time period.
* When multiple team members have similar goals and you might need to create one for each one of them. 




>[!TIP] {type="tip"}
>
>You can copy a goal in any status. For information about goal statuses, see [Goal status overview in Workfront Align](goal-status-overview.md).


Consider the following when copying goals:



* All information about the goal, except the goal&nbsp;Period when it is in the past, is also copied to the new goal. 
*  You can select to copy the results of an existing goal. The name of the results transfer to the new goal, but the current progress of the results on the existing goal does not copy to the new goal. The copied results are assigned to the same owner, by default. 


  >[!NOTE]
  >
  >If the original owner was deleted or deactivated from  `Workfront`, the new result is assigned to the logged in user.



* You cannot copy the activities of a goal when you copy the goal. 




## Copy goals {#copy-goals}




1.  Go to a goal and click it to open the Goal Details panel. 


   For information about accessing an individual goal, see the "Access individual goals" section in [Access goals in Workfront Align](access-goals-in-wf-align.md).


   This opens the Goal Details panel.

1. Click the **gear** icon ![](assets/setup-gear-icon.png) , then click **Copy**. 

1.  Update any of the following information for the copied goal:


1.  (Conditional) Select **Copy results** if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal. 

   ` `**Tips: **`` 
    
    
    * The progress of the original result does not transfer to the copied goal. 
    * If the original owner was deleted or deactivated from  `Workfront`, the new result is assigned to the logged in user.
    
    

1.  Click **Save**. 


   The copied goal is saved with a status of Draft and displays in the Goal Details panel. 


   >[!IMPORTANT] {type="important"}
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
   >
   >
   >You can do one or several of the following to enable activating a goal:
   >
   >    
   >    
   >    *  Add a Result
   >    
   >    
   >      For information about adding results, see [Add results to goals in Workfront Align](add-results-to-goals.md).
   >    
   >    *  Add an Activity
   >    
   >    
   >      For information about adding activities, see [Add activities to goals in Workfront Align](add-activities-to-goals.md). 
   >    
   >    *  Align another goal to it
   >    
   >    
   >      For information about aligning goals, see [Align goals by connecting them in Workfront Align](align-goals-by-connecting-them.md).
   >    
   >    
   >    




1. Click&nbsp;**Activate**. The goal status updates to Active. 
1.  Click the **X** icon in the upper-right of the Goal Details panel to close it. 


   The new goal displays in the following sections:

    
    
    * `Goal List` 
    * `Check-in` (after it is activated)
    * `Goal Alignment section` (after it is activated) 
    * `Pulse` 
    
    

1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:
    
    
    1. Go to the original goal in the `Goal List`, `Check-in` page, or `Pulse` section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Workfront Align](manage-goal-comments.md).
    1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Workfront Align](close-and-reopen-goals.md). 
    1. Update the **Starting At** value of the new Result to match the **End At** value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.
    
    


