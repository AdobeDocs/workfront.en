---
filename: share-a-plan
product-area: enterprise-scenario-planner-product-area
keywords: plan,permissions,share,initiatives,scenarios,scenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Share a plan in the Adobe Workfront Scenario Planner
description: You can share a plan that you created in the Adobe Workfront Scenario Planner with other users.
---

# Share a plan in the Adobe Workfront Scenario Planner

##  

You can share a plan that you created in the Adobe Workfront Scenario Planner with other users.

>[!TIP]
>
>If you send a link to a plan to others, you must also share the plan with them for them to be able to view it.

## Access requirements

You must have the following:

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront<b> plan*</b> </p> </td> 
   <td>Business or higher</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront<b> license*</b> </p> </td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>You must purchase an additional license for the Adobe Workfront Scenario Planner to access functionality described in this article.</p> <p>For information about obtaining the Workfront Scenario Planner, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Adobe Workfront Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access or higher to the Scenario Planner</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>You must be the creator of the plan. </p> <p>Plan creators have Manage permissions to the plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the Adobe Workfront Scenario Planner</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

* You must be the creator of the plan to be able to share it with another user and grant permissions for what that user can do with the plan.
* The users given the access to the plan must have access to the Scenario Planner area in their Access Levels, as granted by your Workfront administrator in order to receive permissions to a plan.

  For example, Requestors cannot view, create, or edit plans. You should keep this in mind when sharing a plan with a user who has a Requestor license.

For more information about access to the Scenario Planner for various license types, see [Grant access to Scenario Planner](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Considerations about plan sharing

* You can share a single plan, or you can share multiple plans, in bulk. 
* You cannot view plans that you did not create or that are not shared with you.
* You must be the creator of the plan 

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  or a plan must be shared with you
  </MadCap:conditionalText>
  -->

  to share it with other users. You cannot share plans that are shared with you. 
* You can only share a plan with other users. You cannot share plans with groups, teams, or companies. 
* You must first save a plan before you can share it. 
* You can share a URL to a plan with another user. If the user does not have permissions to at least view the plan, they can request access to the plan from the plan creator when they receive the URL.&nbsp;For information about requesting access to a plan, see [Request access to a plan in the Adobe Workfront Scenario Planner](../scenario-planner/request-access-to-plan.md). 
* When sharing multiple plans in bulk, they must all be plans that you created. If you select a plan that you created and a plan shared with you, the Share icon does not display on the list of plans.
* When sharing multiple plans that have already been shared with others, the users you share with do not replace but are added to the existing users on each plan you selected.

## Share plans

>[!TIP]
>
>You can share the plan by clicking the avatars of users with whom the plan is shared from the plan header.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Scenarios**.
1. Click the name of a plan to open it

   Or

   Select several plans to share them in bulk. 

1. (Conditional) If you opened a plan, click the **More** icon ![](assets/more-icon.png) to the right of the Plan name, then click Share

   Or

   If you selected several plans to share them in bulk, click the **Share** icon ![](assets/share-icon-26x26.png) at the top of the list of plans to open the Plan access box.

   >[!TIP]
   >
   >
   >   
   >   
   >   * Users that have permissions to all the plans you select display in the Plan access box. 
   >   * Any additional users are added to and do not replace the existing users on all the plans selected. 
   >   
   >

1. In the **Give plan access to** field, start typing the name of the users that you want to share the plan with, then select them when they appear in the list. 
1. From the permissions drop-down menu to the right of the user name, select the level of permission you want to grant them to the plan. 
1. Select from the following:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">View</td> 
      <td>Users you share the plan with will have permissions to view the plan.&nbsp;They cannot edit information on the plan, add initiatives, scenarios, or publish scenarios. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Manage</td> 
      <td> <p>Users you share the plan with have permissions to manage the plan, which includes edit information, add initiatives, scenarios, and publish the plan. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >You can delete a plan only when you created it. You cannot delete plans that are shared with you.

1. Click&nbsp;**Save**.

   The plan is now shared with the users you specified.

   You can view users that have permissions to the plan in the Shared with me column in a list of plans or in the upper-right corner of the plan header.

   >[!TIP]
   >
   >You can view plans that are shared with you by applying the Shared with me filter in a list of plans.

## Plan permission options

The following table lists the permissions that you can grant when sharing a plan. For more information about the access users get based on their license, see [Grant access to Scenario Planner](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Actions</strong> </p> </th> 
   <th> <p><strong>Manage</strong> </p> </th> 
   <th> <p><strong>View</strong> </p> </th> 
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
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Create initiatives</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Create scenarios</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Delete initiatives, or scenarios</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Copy scenarios</td> 
   <td>✓ </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Publish scenarios**</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

&#42;You must have access to financial data to be able to view or manage financial information on plans, even if you have manage permissions to plans. For information about access to financial data, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

&#42;&#42; You must have access to create and permissions to manage projects to be able to publish scenarios.

For information about project access level, see [Grant access to projects](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

For information about project permissions, see [Share a project in Adobe Workfront](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md). 
