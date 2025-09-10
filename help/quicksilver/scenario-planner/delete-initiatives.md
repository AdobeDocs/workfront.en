---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Delete Initiatives in the Scenario Planner
description: You can delete initiatives on a plan that you created or on a plan that someone shared with you. You cannot recover initiatives that you deleted.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
---
# Delete initiatives in the [!DNL Scenario Planner]

You can delete initiatives on a plan that you created or on a plan that someone shared with you. You cannot recover initiatives that you deleted.

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] package</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTE</b></p>
<p>Speak with your Workfront representative if you have a different Workfront package.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license</p> </td> 
   <td> <p>[!UICONTROL Light] or higher</p> 
   <p>[!UICONTROL Review] or higher</p> </td> 
  </tr> 
    <tr> 
   <td>Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> </td> 
  </tr> 
 </tbody> 
</table>

For more information about access to the Scenario Planner, see [Access needed to use the [!DNL Scenario Planner]]( ../scenario-planner/access-needed-to-use-sp.md).

For information about Workfront access requirements, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
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

*For information, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Delete initiatives

Consider the following when deleting initiatives:

* Deleting an initiative removes the required amount of job roles and the cost information associated with the initiative from the plan.
* Deleting an initiative that was created by importing a project does not delete the project associated with the initiative.
* Deleting an initiative that has been published to a project at least once results in the following:

   * The initiative is deleted from the scenario but the [!DNL Scenario Planner] area remains in the [!UICONTROL Project Details] section. 
   * If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed.

     For information about publishing initiatives to projects, see [Update or create projects by publishing initiatives in the [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

     For information about creating initiatives by importing projects, see [Import projects to plans in the [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

You can delete one initiative at a time, or you can delete multiple initiatives in bulk.

* [Delete one initiative](#delete-one-initiative) 
* [Delete initiatives in bulk](#delete-initiatives-in-bulk)

### Delete one initiative {#delete-one-initiative}

{{step1-to-scenario-planner}}

   A list of plans displays. 

1. Click the name of a plan to open it, then locate the initiative you want to delete.
1. Do one of the following:

   * Click the **[!UICONTROL More menu]** ![More menu](assets/more-menu.png) to the right of the initiative name, then click **[!UICONTROL Delete]** > **[!UICONTROL Yes, delete it]**.

   * Select the box to the left of the initiative, then click **[!UICONTROL Delete]** on the floating menu that appears at the bottom of the plan, then click **[!UICONTROL Yes, delete it]**.

   The initiative and its job role and cost information are deleted from the plan.

1. Click **[!UICONTROL Save Plan]** to save your changes.

### Delete initiatives in bulk {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

  A list of plans displays. 

1. Click the name of a plan to open it, then locate the initiative you want to delete.
1. Select the boxes to the left of the initiatives that you want to delete, then click **[!UICONTROL Delete]** from the menu that appears at the bottom of the plan, then click **[!UICONTROL Yes, delete them]**.

   ![Manage initiative menu](assets/bottom-manage-initiative-menu-350x45.png)

   The initiatives and their job role and cost information are deleted from the plan.

1. Click **[!UICONTROL Save Plan]** to save your changes.
