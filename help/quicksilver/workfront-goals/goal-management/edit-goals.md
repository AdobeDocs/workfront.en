---
product-previous: workfront-goals
navigation-topic: goal-management
title: Edit goals in Adobe Workfront Goals
description: You can edit existing goals from any time period and in any status.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
---
# Edit goals in Adobe Workfront Goals

You can edit existing goals from any time period and in any status.

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

## Considerations about editing goals

* You cannot edit goals with a status of Closed. 
* You can edit goals from any time period.

  You can edit the following information for a past goal:

  * Name
  * Time period
  * Status

    >[!TIP]
    >
    >If the goal is Closed, reopening it recalculates the Progress percent complete. You cannot edit a closed goal.

  * Description
  * Results and activities

## Edit goals

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![](assets/more-icon.png), then click **Edit**.

   ![](assets/edit-goal-highlighted.png)

1. Update the name of the goal in the **Goal** field. 
1. Select a time period when the goal should be completed.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a start and an end date for your goal, if you clicked **Define custom dates**.

   
   <p>(NOTE: these fields don't yet have a name) </p>
   

   >[!CAUTION]
   >
   >You cannot create a goal with custom dates in the past.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same time frames for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your larger organization-wide strategy.

1. Click the **Owner** field and select a new owner for the goal, if you want to indicate someone else as the owner of the goal. 
1. (Conditional) Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. Update the **Description** of the goal, then click **Save**.

-->

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png), then click **Goals**.  
A list of goals displays.
1. Click a goal.  
   The goal page displays. 

   ![](assets/goal-page-unshimmed.png)

1. Do one of the following to edit information for the goal:
    * Click fields that display in the goal header to update them. Not all fields in the header are editable. 
    * Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Edit**. 
    * Click **Goal details** in the left panel and click the **Edit icon** ![](assets/edit-icon.png) in the upper-right corner, then click **Edit all**. Start updating fields in the Goal details section. 
    
      >[!IMPORTANT]
      >
      >Not all fields that display in the areas mentioned above can be edited. Workfront calculates some of the fields and they are read-only. 

1. (Conditional) Depending on what you selected in the previous step, update the following information about the goal:

   * Update the following information in the goal header, then press Enter to save your changes:
      * **Goal name**: Click the name of the goal and start typing a new name.
      * **Owner**: Click the name of the owner, and start typing the name of a user, team, group, or your company, then select it when it displays in the list. You can have only one owner for a goal. 
   * Update the following information in the Edit Goal box, then click **Save**: 
      * **Goal name**
      * **Period**: Click to update the time period for the goal  
         Or  
         Select **Enable custom dates** to specify dates for the goal's **Start** and **End dates**. 

         >[!TIP]
         >
         >Deselect **Enable custom dates** to return to the original time period for the goal. 

      * **Goal owner**
      * **Description**: Add or update information about the goal. 
   * Update or review information in the Goal details section. For more information, see [Update goals in the Goal details section in Adobe Workfront Goals](../goal-management/update-goals-in-goal-details-panel.md). 

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Optional)  Click **Progress Indicators** in the left panel to add results, activities, or projects to the goal. By adding progress indicators, you ensure you can track the goal's progress.
For more information, see the following articles: 
    * [Add activities to goals in Adobe Workfront Goals](../results-and-activities/add-activities-to-goals.md)
    * [Add results to goals in Adobe Workfront Goals](../results-and-activities/add-results-to-goals.md). 
    * [Add projects to goals in Adobe Workfront Goals](../results-and-activities/connect-projects-to-goals-overview.md).
    
</div>
