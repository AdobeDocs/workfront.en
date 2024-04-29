---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Remove progress indicators from goals in Adobe Workfront Goals
description: You can remove results, activities, and projects from goals in Adobe Workfront Goals, when they are no longer relevant. 
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
---
# Remove progress indicators from goals in Adobe Workfront Goals

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

You can remove results, activities, and projects from goals if they are no longer relevant.

For information about creating goals, and adding results and activities to them, see the following articles:

* [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md) 
* [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
* [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md) 
* [Edit results and activities in Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

Goals can also be aligned to parent goals, becoming children goals. Children goals are also progress indicators of the parent goals.

You can remove the alignment between goals by removing the connection between them. For information, see [Remove goal alignment in Adobe Workfront Goals](../goal-alignment/remove-goal-alignment.md).

## Access requirements

You must have the following:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront plan</td>
 <td>
 <p>Any</p>
 
 </td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
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
 <td role="rowheader">Access level</td>
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

## Prerequisites

You must have a goal associated with results, activities, or projects. 

## Considerations for removing results, activities, and disconnecting projects from goals

* You can remove results and activities only from active goals. 
* You can remove results and activities from a goal by deleting them. Deleted results and activities cannot be recovered. 
* When you remove the result or activity from a goal, the progress of the removed result or the activity affects the overall progress of the goal. 
* You cannot delete a project from a goal, but you can disconnect it from the goal. By disconnecting the project from the goal the percent complete of the project no longer affects the progress of the goal.

  For information about how projects affect goal progress, see [Add projects to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md). 

* You cannot remove a result or an activity from a goal, and you cannot disconnect a child goal or a project, if they are the last progress indicator for the goal. 
* If a project is deleted from the Projects area and it is the last progress indicator of a goal, the goal becomes Inactive.

## Delete results and activities from goals

You remove results and activities from a goal by deleting them. Deleting results and activities from a goal is identical. 

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   This opens the Workfront Goals area and the Goal List displays by default.

1. Click the name of a goal you want to remove results and activities from.

   This opens the goal page. 

1. Click **Progress indicators** in the left panel.

1. Select a result or activity, then click the **Delete** icon ![](assets/delete-icon.png) at the top of the list. 

1. Click **Delete** to confirm the deletion. The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.


## Remove projects from goals

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. Click the **Main Menu** icon  in the upper-right corner, then click **Goals**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   This opens the Workfront Goals area and the Goal List displays by default.

1. Click the name of a goal you want to remove results and activities from.

   This opens the goal page. 
1. Click **Progress indicators** in the left panel.
1. Select a project, then click the **Disconnect** icon ![](assets/disconnect-icon.png) at the top of the list.
1. Click **Disconnect** to confirm. 

   The project is no longer connected to the goal. The percent complete of the goal updates to exclude the disconnected project. 

