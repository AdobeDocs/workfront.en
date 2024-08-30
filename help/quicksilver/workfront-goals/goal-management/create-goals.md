---
product-previous: workfront-goals
navigation-topic: goal-management
title: Create goals in Adobe Workfront Goals
description: Whether you are a CEO, a manager, or an individual contributor, you can create goals in Adobe Workfront Goals to align your work with your goals and the goals that outline the strategy of your organization.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
---
# Create goals in Adobe Workfront Goals

Whether you are a CEO, a manager, or an individual contributor, you can create goals in Adobe Workfront Goals to align your work with your goals and the goals that outline the strategy of your organization.

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
<p>View or higher permissions to the goal to view it</p>
<p>Manage permissions to the goal to edit it</p>
<p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
</td>
</tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

## Guidelines for creating goals

Before starting with Workfront Goals, we recommend that you read about our best practice recommendations and guidelines for managing goals effectively. For more information about guidelines for creating and managing goals, see [Adobe Workfront Goals overview](../../workfront-goals/goal-management/wf-goals-overview.md).

## Create goals

This article describes how you create a strategic goal in Workfront Goals. For information about creating a business case goal, see [Create Business Case goals](../../manage-work/projects/define-a-business-case/create-business-case-goals.md). 

You can create a strategic goal in one of the following ways:

* [Create a goal from scratch](#create-a-goal-from-scratch) 
* [Copy an existing goal](#copy-an-existing-goal) 
* [Convert a result or activity to a goal](#convert-a-result-or-activity-to-a-goal)

### Create a goal from scratch {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![](assets/add-goal-box-350x235.png)

   >[!TIP]
   >
   >You can add a goal from any section in Workfront Goals. The process for creating a goal is identical regardless of the section you choose to add the goal from.

1. Start typing what you want to achieve in the **Goal** field. This is the name of the goal and a required field. 
1. Select a time period when the goal should be executed in the **Period** drop-down menu. This is a pre-filled field. The default is the current quarter.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a **Start date** and an **End date** for your goal, if you clicked **Define custom dates**.

   >[!TIP]
   >
   >* You can create a goal with dates in any time period, including up to 2 years in the past. 
   >* When defining custom dates, they are constrained by the initial date you selected. So if you select quarter and then custom dates, you can't go beyond that quarter.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same timeframes for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your over-arching strategy.

1. (Optional) Click your name in the **Owner** field, if you want to indicate someone else as the owner of the goal. By default, you are the owner of goals you create. 
1. Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. (Optional) Enter a **Description** for the goal. This field is optional. 
1. Click **Save**.

   The status of the new goal is Draft.

   >[!IMPORTANT]
   >
   >You must associate a goal with a progress indicator to activate it and start working on it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >
   >* Add a Result
   >
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

-->

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper right corner, then click **Goals**. 

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   The goal list displays.
1. Click **New goal**.  

   The New goal box displays.  

   ![](assets/new-goal-box-unshimmed.png)

1. Enter information in the following fields:
    * **Goal name**: Enter a name for the goal. This is a required field.
    * **Period**: Select a predefined quarter or year from the **Period** drop-down field
   
      Or

      Select the **Enable custom dates** option, then select a **Start** and **End date** for the goal.  
   
      The previous, current, and following years and their respective quarters are listed as predefined options in the Period drop-down field.  
   
      The Period of the goal indicates the time frame when you expect the goal to complete.

    * **Goal owner**: Start typing the name of a user, a team, a group, or of your organization to indicate who is the owner of the goal. You are selected as the owner of the goal by default. 
    * **Description**: Enter additional information about the goal.
1. Click **Create goal**. 

   The new goal is listed in the Goal list and it has the status of **Draft**.
   
   You must associate a goal with a progress indicator to activate it and start working on it.
  
   Do at least one of the following to prepare a goal to be activated:
    * Add a Result
    
      For information about adding results, see [Add results to goals in Adobe Workfront Goals](../results-and-activities/add-results-to-goals.md).
    * Add an Activity 
    
      For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../results-and-activities/add-activities-to-goals.md).
    * Align another goal to it
    
      For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../goal-alignment/align-goals-by-connecting-them.md). 


### Copy an existing goal {#copy-an-existing-goal}

You can create a goal by copying an existing one.

For information about copying goals, see [Copy goals in Adobe Workfront Goals](../../workfront-goals/goal-management/copy-goals.md).

### Convert a result or activity to a goal {#convert-a-result-or-activity-to-a-goal}

You can create a goal by converting the result or the activity of an existing goal to a goal. The new goal becomes aligned to the original goal.

For information about converting results and activities to goals, see [Align goals by converting results and activities to goals](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

