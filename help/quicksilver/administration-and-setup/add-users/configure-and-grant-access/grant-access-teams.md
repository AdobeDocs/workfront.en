---
title: Grant Access to Teams
description: As an Adobe Workfront administrator, you can use an access level to define a user's access to teams in Workfront
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
---
# Grant access to teams

As an Adobe Workfront administrator, you can use an access level to define a user's access to teams in Workfront, as explained in [Access levels overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## Configure users' access to edit users using a custom access level

1. Begin creating or editing the access level, as explained in [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Click the gear icon ![](assets/gear-icon-settings.png) on the **View** or **Edit** button to the right of Teams, then select the abilities you want to grant under **Fine-tune your settings**.

   * **View**: If you are configuring how users with any license can view teams, change any of the following options:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">View teams associated with my groups</td>
         <td>
          <p><b>Enabled</b>: When users look for teams in a Team type-ahead field, the users can see the teams associated with their groups whether or not they are team members. </p>
          <p><b>Disabled</b>: When users look for teams in a Team type-ahead field, the users can see the teams associated with their groups only where they are team members</p><p>This option is enabled by default.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">View all teams</td>
         <td><p>When this option is enabled and users look for teams in a Team type-ahead field, the users can see and select any team.</p><p>This option is enabled by default. </p></td>
        </tr>
       </tbody>
      </table>

   * **Edit**: If you are configuring how users with a Plan license and Work license can manage teams, change any of the following options:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Create</td>
         <td><p>Allows users with a Plan license or Work license to create teams.</p><p>This option is enabled by default.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Delete</td>
         <td><p> Allows users with a Plan license to delete the teams that they have access to edit (unavailable for users with a Work license).</p><p>This option is enabled by default.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Edit teams in groups I manage (Group Admins only)</td>
         <td><p>Allows Plan license users who are designated as group administrators to edit teams associated with the groups they manage.</p><p>This option is enabled by default.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Edit teams I'm on</td>
         <td><p>Allows users Plan license or Work license to edit teams where they are a member.</p><p>This option is disabled by default.</p></td>
        </tr>
        <tr>
         <td role="rowheader">View teams associated with my groups</td>
         <td>
         <p><b>Enabled</b> When users look for teams in a Team type-ahead field, the users can see the teams associated with their groups whether or not they are team members. </p>
         <p><b>Disabled</b>: When users look for teams in a Team type-ahead field, the users can see the teams associated with their groups only where they are team members</p><p>This option is enabled by default.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">View all teams</td>
         <td><p>When this option is enabled and users look for teams in a Team type-ahead field, the users can see and select any team.</p><p>This option is enabled by default. </p></td>
        </tr>
       </tbody>
      </table>

1. Click the X to close the **Fine-tune your settings** box.
1. (Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in [Configure access to Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), such as [Grant access to tasks](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) and [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. When you are finished, click **Save**.

>[!NOTE]
>
>* The following are true, regardless of access level settings:
>
>   * Team owners can always view and edit their teams
>   * Users always have access to view the teams they're on
>
>* The configuration of any option available for both View and Edit (such as "View teams associated with my groups") is retained if you decide to select View instead of Edit or Edit instead of View in an access level.
>

## Access to teams by license type

For information about what users in each access level can do with issues, see the section [Teams](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) in the article [Functionality available for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
