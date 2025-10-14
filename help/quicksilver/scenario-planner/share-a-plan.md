---
product-area: enterprise-scenario-planner-product-area
keywords: plan,permissions,share,initiatives,scenarios,scenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Share a Plan in the Scenario Planner
description: You can share a plan that you created in the Adobe Workfront Scenario Planner with other users.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
---
# Share a plan in the [!DNL Scenario Planner]

<!--Audited: 07/2024-->

You can share a plan in the [!DNL Adobe Workfront Scenario Planner] with other users, so they can collaborate on the same work that you do. 

>[!TIP]
>
>If you send a link to a plan to others, you must also share the plan with them for them to be able to view it.

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

For more information about access to the Scenario Planner, see [Access needed to use the [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

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
</table>-->

## Prerequisites

* The users given permissions to the plan must have access to the [!DNL Scenario Planner] area in their Access Levels, as granted by your [!DNL Workfront] administrator, in order to receive permissions to a plan.

  For example, [!UICONTROL Requestors] cannot view, create, or edit plans. You should keep this in mind when sharing a plan with a user who has a Requestor license. 

 <!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

For more information about access to the [!DNL Scenario Planner] for various license types, see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Considerations about plan sharing

* All users, including system administrators, have access only to plans that they created. 
* You can share a single plan, or you can share multiple plans, in bulk.
* You cannot view plans that you did not create or that are not shared with you.
* You can only share a plan with other users. You cannot share plans with groups, teams, or companies.
* You must first save a plan before you can share it.
* You can share a URL to a plan with another user. If the user does not have permissions to at least view the plan, they can request access to the plan from another user when they receive the URL. For information about requesting access to a plan, see [Request access to a plan in the [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md). 
* When sharing multiple plans that have already been shared with others, the users you share with do not replace but are added to the existing users on each plan you selected.

## Plan permission options

The following table lists the permissions that you can grant when sharing a plan. For more information about the access users get based on their license, see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Actions</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Manage]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL View]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>View plan </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>View initiatives </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>View scenarios</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>View job roles</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>View cost and budget information*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Manage cost and budget information*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Create initiatives</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Create scenarios</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Delete initiatives, or scenarios</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Copy scenarios</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Publish scenarios**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*You must have access to Financial Data to be able to view or manage financial information on plans, even if you have manage permissions to plans. For information about access to financial data, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**You must have access to create and permissions to manage projects to be able to publish scenarios.

For information about project access level, see [Grant access to projects](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

For information about project permissions, see [Share a project in [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

## Share plans

{{step1-to-scenario-planner}}

1. Click the name of a plan to open it

   Or

   Select several plans to share them in bulk. 

   >[!TIP]
   >
   >You can share a plan by clicking the avatars of users with whom the plan is shared in the upper-right corner of the plan header. 

1. (Conditional) If you opened a plan, click the **[!UICONTROL More]** icon ![More icon](assets/more-icon.png) to the right of the [!UICONTROL Plan] name, then click **[!UICONTROL Share]**

   Or

   If you selected several plans to share them in bulk, click the **[!UICONTROL Share]** icon ![](assets/share-icon-26x26.png) at the top of the list of plans to open the [!UICONTROL Plan] access box.

   >[!TIP]
   >
   >* Users that have permissions to all the plans you select display in the [!UICONTROL Plan] access box. 
   >* Any additional users are added to and do not replace the existing users on all the plans selected. 

1. In the **[!UICONTROL Give plan access to]** field, start typing the name of the users that you want to share the plan with, then select them when they appear in the list. 
1. From the permissions drop-down menu to the right of the user name, select the level of permission you want to grant them to the plan. 
1. Select from the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL View]</td> 
      <td>Users you share the plan with will have permissions to view the plan. They cannot edit information on the plan, add initiatives, scenarios, or publish scenarios. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Manage]</td> 
      <td> <p>Users you share the plan with have permissions to manage the plan, which includes edit information, add initiatives, scenarios, and publish the plan. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >You can delete a plan only when you created it. You cannot delete plans that are shared with you.

1. Click **[!UICONTROL Save]**.

   The plan is now shared with the users you specified.

   You can view users that have permissions to the plan in the Shared with me column in a list of plans or in the upper-right corner of the plan header.

   >[!TIP]
   >
   >You can view plans that are shared with you by applying the [!UICONTROL Shared with me] filter in a list of plans.


