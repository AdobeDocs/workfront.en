---
title: Grant Access to Scenario Planner
description: As an Adobe Workfront administrator, you can use an access level to define a user's access to Scenario Planner.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
---
# Grant access to Scenario Planner

As an Adobe Workfront administrator, you can use an access level to define a user's access to Scenario Planner, as explained in [Access levels overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). 

In addition to access to Scenario Planner, a user with a non-System Administrator access level must also have access to financial data in order to see any financial information contained in a plan, such as budgets, costs, and job role rates. For more information, see [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Business or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher. For more information, see <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Licenses overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>You must purchase an additional license for the Adobe Workfront Scenario Planner to access functionality described in this article.</p> <p>For information about obtaining the Workfront Scenario Planner, see <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">Access needed to use the Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>View access or higher to the Scenario Planner</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> <p>View permissions or higher for a plan</p> <p>For information on requesting additional access to a plan, see <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">Request access to a plan in the Scenario Planner</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

+++

## Configure user access to Scenario Planner using a custom access level

1. Begin creating or editing the access level, as explained in [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Click the option to the right of **Scenario Planner** that you want to use for this access level.

   >[!NOTE]
   >
   >The Request or External license type do not allow View or Edit access to Scenario Planner.

1. (Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in [Configure access to Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), such as [Grant access to tasks](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) and [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. When you are finished, click **Save**.

## Access to Scenario Planner by license type

For information about what users in each access level can do with the Scenario Planner, see the section [Scenario Planner area](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) in the article [Functionality available for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Scenario Planner access by access level setting

The following information can help you understand how to use the Access level settings to control users' access to information in the Workfront Scenario Planner.

* [No access](#no-access) 
* [View access](#view-access) 
* [Edit access](#edit-access)

### No access {#no-access}

A user with no access to Scenario Planner can neither see the Scenarios icon in the Main Menu when it is added to their layout template, nor view plans and initiatives that are shared with them. If the link to a plan is shared with a user who has no access to Scenario Planner, the user cannot view or edit the plan.

### View access {#view-access}

Users with View access to Scenario Planner can do the following:

* See the Scenarios icon in the Main Menu ![](assets/esp-icon-in-main-menu.png), though the Plans area is empty unless the user clicks a plan link shared by another user. 
* View a plan when another user shares the link to it.

  This includes any job role information in the plan.

  It also includes job role rates and cost information on the plan if the recipient user also has access to financial data. For more information, see [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Edit access {#edit-access}

Users with Edit access to Scenario Planner can do the following:

* See the Scenarios icon in the Main Menu ![](assets/esp-icon-in-main-menu.png) and use it to access plan data.
* Create plans.
* View, edit, and delete plans that they create.
* View, edit, and delete other users' plans that they access using a shared link.

  This includes any job role information in a plan.

  It also includes job role rates and cost information on the plan if the recipient user has access to financial data. For more information, see [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
