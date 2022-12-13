---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Delete initiatives in the Scenario Planner
description: You can delete initiatives on a plan that you created or on a plan that someone shared with you. You cannot recover initiatives that you deleted.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
---
# Delete initiatives in the [!DNL Scenario Planner]

You can delete initiatives on a plan that you created or on a plan that someone shared with you. You cannot recover initiatives that you deleted.

## Access requirements

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] or higher</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> license*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>You must purchase an additional license for the [!DNL Adobe Workfront Scenario Planner] to access functionality described in this article. </p> <p>For information about obtaining the [!DNL Workfront Scenario Planner], see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!UICONTROL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>[!UICONTROL Edit] access or higher to the [!DNL Scenario Planner]</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png), then click [!UICONTROL Scenarios].

   A list of plans displays. 

1. Click the name of a plan to open it, then locate the initiative you want to delete.
1. Do one of the following:

   * Click the **[!UICONTROL More menu]** ![](assets/more-menu.png) to the right of the initiative name, then click **[!UICONTROL Delete]** > **[!UICONTROL Yes, delete it]**.

   * Select the box to the left of the initiative, then click **[!UICONTROL Delete]** on the floating menu that appears at the bottom of the plan, then click **[!UICONTROL Yes, delete it]**.

   The initiative and its job role and cost information are deleted from the plan.

1. Click **[!UICONTROL Save Plan]** to save your changes.

### Delete initiatives in bulk {#delete-initiatives-in-bulk}

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png), then click [!UICONTROL Scenarios].

   A list of plans displays. 

1. Click the name of a plan to open it, then locate the initiative you want to delete.
1. Select the boxes to the left of the initiatives that you want to delete, then click **[!UICONTROL Delete]** from the menu that appears at the bottom of the plan, then click **[!UICONTROL Yes, delete them]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   The initiatives and their job role and cost information are deleted from the plan.

1. Click **[!UICONTROL Save Plan]** to save your changes.
