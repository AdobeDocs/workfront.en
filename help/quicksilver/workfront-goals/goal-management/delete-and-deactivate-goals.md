---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Delete and deactivate goals in Adobe Workfront Goals
description: When you start working on a goal and it becomes irrelevant in your organization, we recommend deactivating it, instead of deleting it. Deactivating a goal keeps its historical information and gives you a chance to reactivate it at a later time. There are times, however, when deleting a goal might make sense, to keep your goal list accurate.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
---
# Delete and deactivate goals in Adobe Workfront Goals

When you start working on a goal and it becomes irrelevant in your organization, we recommend deactivating it, instead of deleting it. Deactivating a goal keeps its historical information and gives you a chance to reactivate it at a later time. There are times, however, when deleting a goal might make sense, to keep your goal list accurate.

## Access requirements

You must have the following:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Deactivate goals

You can deactivate a goal that is no longer relevant and that you might want to reactivate in the future.

* [Considerations when deactivating goals](#considerations-when-deactivating-goals) 
* [Deactivate goals](#deactivate-goals)

### Considerations when deactivating goals

Remember the following when deactivating goals:

* You can only deactivate goals in an Active status. For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

  >[!TIP]
  >
  >You cannot deactivate goals in a Draft status.

* Workfront stops calculating the progress of deactivated goals. 
* Inactive goals no longer display on or are taken into account in the Graphs section of Workfront Goals. For information about Workfront Goals graphs, see [Review graphs to understand goal progress trends in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

   <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* You can no longer make updates on deactivated goals. 
* You can edit information about the goal and its alignment. 
* You can reactivate a previously deactivated goal.

### Deactivate goals

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   The goal list displays.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The goal page opens.

   ![](assets/goal-page-unshimmed.png)

1. Click the **More** menu ![](assets/more-icon.png) to the right of the goal name, then click **Deactivate**. 

1. The goal is deactivated and its status becomes Inactive. 

## Delete goals

You can delete goals that are no longer or might never be relevant.

* [Considerations when deleting goals](#considerations-when-deleting-goals) 
* [Delete goals](#delete-goals)

### Considerations when deleting goals {#considerations-when-deleting-goals}

* You can delete goals in any status, including closed goals. 
* You cannot recover deleted goals. 
* Results and Manual progress bar activities attached to the goal are also deleted. 
* Projects associated with goals are not deleted, but their association with the goal is removed.

### Delete goals

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![](assets/more-icon.png), then click **Delete**.

   ![](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. Click the Main Menu icon ![](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   The goal list displays. 

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Click the name of a goal. This opens the goal page. 
1. Click the **More** menu ![](assets/more-icon.png) to the right of the goal name, then click **Delete Goal**, then **Delete**. 

   The goal and its activities and results are also deleted and cannot be recovered. Projects that were associated with the goal or children goals are not deleted. 


