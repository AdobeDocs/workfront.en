---
title: Grant Access to Resource Management
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: As an Adobe Workfront administrator, you can use an access level to define a user's access to Resource Management in Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
---
# Grant access to Resource Management

As an Adobe Workfront administrator, you can use an access level to define a user's access to Resource Management, as explained in [Access levels overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configure user access to Resource Management tools using a custom access level

1. Begin creating or editing the access level, as explained in [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Click the gear icon ![](assets/gear-icon-settings.png) on the **View** or **Edit** button to the right of Resource Management, then select the abilities you want to grant under **Fine-tune your settings**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Edit priorities and budget hours in the Planner</td> 
      <td> <p>Allows users with this license to do the following:</p> <p>Prioritize projects in the Resource Planner.</p> <p>Budget allocation for resources in the Resource Planning tools (the Resource Planner and the Resource Budgeting section in the Business Case of a project.)</p> <p>This option is enabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Manage Resource Pools</td> 
      <td> <p>Allows users with this license to create, edit, and delete Resource Pools. This option is disabled by default.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Update Planned Hours in the Workload Balancer</span> </td> 
      <td> <p>Allows users with this license to update the Planned Hours of work items when they update the user allocations in the Workload Balancer. The total number of allocated hours becomes the Planned Hours of the work items.</p> <p>This option is disabled by default.</p> <p> For more information, see <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in [Configure access to Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), such as [Grant access to tasks](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) and [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. When you are finished, click **Save**.

   After the access level is created, you can assign it to a user. For more information, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Access to Resource Management by license type

For information about what users in each access level can do with Resource Management, see the section [Resource Management](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) in the article [Functionality available for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Access to shared issues

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

When you share an object with another user, the recipient's rights to budget or view resource allocation on it are determined by a combination of 3 things:

* The recipient's access level setting for Resource Management
* The user's access to financial data, as explained in [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Any permissions to financial data that the sharer granted for the object

For information about permissions users can grant to financial data on an object when sharing the object, see [Share financial permissions on an object](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
