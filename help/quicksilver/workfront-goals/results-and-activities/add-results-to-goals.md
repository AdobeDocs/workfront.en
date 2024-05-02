---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Add results to goals in Adobe Workfront Goals
description: Results measure the progress of a goal. Without associating results, activities, or aligned goals to a goal, you cannot activate the goal and you cannot record progress on it.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
---
# Add results to goals in Adobe Workfront Goals

Results measure the progress of a goal. Without associating results, activities, or aligned goals to a goal, you cannot activate the goal and you cannot record progress on it.

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
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p>  </td>
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

You must have the following before you can start:

* A Layout Template that includes the Goals area in the Main Menu.
* An existing goal.

  For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>A goal cannot have more than a total of 1000 activities, results, projects, or aligned goals.

## Add a result to a goal

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![](assets/results-value-initial-target-boxes-350x49.png)

   Select from the following options:

   |Option|Value type|
   |---|---|
   | # |Number value |
   | % |Percentage value |
   |$, CN¥, DKK, KR, Mex$, R, R$, zł, £ , ¥ , &euro; , ₹, ฿, MYR, ₪  |Currency values |

   For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value.

   >[!TIP]
   >
   >The result Type is always Metric and cannot be edited.

1. In the Initial field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. 
1. In the Target field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.
1. Click **Save**.

   The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result.

-->

1. Click the Main Menu ![](assets/main-menu-icon.png), then **Goals**. 

1. From the **Goal List**, click the name of a goal to open the goal page.
1. Click **Progress indicators** in the left panel.
1. Expand the **New progress indicator** drop-down menu, then click **Create result**.

   The New result box opens. 

   ![](assets/new-result-box-unshimmed.png)
   
1. Enter a name for the result in the **Result name** field. This is a required field. 
1. (Optional) Remove your name from the **Result owner** field if you want to assign the result to another user. By default, you are the owner of an activity you create. 

   >[!NOTE]
   >
   >You cannot assign a team, group, or the company as a result owner.

1. In the **How do you want to measure your result?** area, specify the following information:
   * **Value type**: This indicates how you want to measure the progress on the result. You can measure progress numerically, with a percentage value, or using a currency amount. 
   
      Select a value type from the options listed in the following table:

      | Value type                                              | Description      |
      |---------------------------------------------------------|------------------|
      | Number                                                  | Number value     |
      | %                                                       | Percentage value |
      | CN¥,DKK,KR,Mex$, R, R$, zł, £ , ¥ , &euro; , ₹, ฿, MYR, ₪, $ | Currency values  |

   * **Initial Value**: The value that the result has in the beginning, before any progress on it has been recorded.
   * **Target Value**: The value that the result aims to achieve when it is considered completed. 
1. Click **Create result**.
   
   The result displays in the Progress indicators section of the goal page, unde the Result grouping.
   
   After you activate the goal, the progress of the goal automatically updates when you update the progress of a result. For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../goal-management/activate-goals.md). 
