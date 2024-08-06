---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Update initiative priorities in the Scenario Planner
description: Prioritizing initiatives is important because initiatives receive job roles and budget resources from the plan in the order they are listed on the plan.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
---
# Update initiative priorities in the [!DNL Scenario Planner]

Prioritizing initiatives is important because initiatives receive job roles and budget resources from the plan in the order they are listed on the plan.

You can prioritize initiatives on a plan that you created or on a plan that someone shared with you.

For information about creating plans, see [Create and edit plans in the [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

For information about creating initiatives, see [Create and edit initiatives in the [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <p>Current: [!UICONTROL Business] or higher</p>
   <p>New: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> 
   <p>For the current Workfront plans: </p>
   <p>You must purchase an additional license for the [!DNL Adobe Workfront Scenario Planner] to access functionality described in this article.</p> <p>For information about access and permissions for the [!DNL Workfront Scenario Planner], see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Update initiative priorities

When you change the priority of initiatives, you modify their listing order on the plan.

We recommend that you place more urgent initiatives at the top of a plan and the more fluid ones - that could be done any time and only if resources are available - at the bottom of the plan.

>[!NOTE]
>
>[!DNL Workfront] allocates plan resources to initiatives in the order they are listed on the plan. 
>
>For example, if the plan has 3 available Engineers and Initiative 1 and Initiative 2 each require 2 Engineers to complete and they are both scheduled for the same time frame, Workfront associates 2 Engineers with Initiative 1 and one remaining available Engineer with Initiative 2. In this case Initiative 2 shows as having a conflict, because it is missing one Engineer. Sometimes, changing the priority of your initiatives is the only way to avoid conflicts on a plan.

To update initiative priority:

{{step1-to-scenario-planner}}

   A list of plans displays.

1. Click the name of a plan to open it, then locate the initiatives you want to prioritize.
1. Click the box to the left of one or more of the initiatives' name and do one of the following:

   * Click the handle to the left of one of the selected initiatives' names, then drag it up or down in the list to change the initiative's priority.

     Workfront displays the number of selected initiatives.

     ![](assets/multi-select-initiative-number.png)

   * Click the **[!UICONTROL Prioritize]** box at the bottom of the plan, then choose from the following options:

      * **[!UICONTROL Top]**: Moves the selected initiatives to the top of the initiative list. The selected initiatives are listed first on the plan.
      * **[!UICONTROL Bottom]**: Moves the selected initiatives to the bottom of the initiative list. The selected initiatives are listed last on the plan.
      * **[!UICONTROL Select a number]**: Moves the selected initiatives after the initiative you indicate here.

        ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] immediately places the selected initiatives where you indicate and the numbers of all initiatives update accordingly.

1. Click **[!UICONTROL Save Plan]** to save your changes.
