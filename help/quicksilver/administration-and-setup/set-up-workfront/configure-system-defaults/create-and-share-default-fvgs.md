---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Create, edit, and share default filters, views, and groupings
description: You can create default filters, views, and groupings, then make them available to users in your organization.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
---
# Create, edit, and share default filters, views, and groupings

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

You can create default filters, views, and groupings, then make them available to users in your organization.

When you create default filters, views, and groupings as described in this section, users who you share them with are able to leverage them when viewing their lists. Users can create their own filters, views, and groupings based on those you create, but they cannot directly change those you create.

## Access requirements

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
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Create default filters, views, or groupings

1. Click the **Main Menu** ![](assets/main-menu-icon.png), then click **Setup**. 

1. Do any of the following, depending on whether you are creating or editing a filter, view, or grouping:

   * Click **Interface** > **Filters**.
   
   * Click **Interface >** **Views**.
   
   * Click **Interface** > **Groupings**.

1. If you're creating a filter, view, or grouping, click **New Filter**, **New View**, or **New Grouping,** then select the object type you want to associate the new filter, view, or grouping with.

   Or

   If you're editing an existing filter, view, or grouping, select it, then click **Edit**.

1. Configure the filter, view, or grouping.

   For information about available options, see one of the following articles:

   * [Filters overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) 
   * [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md) 
   * [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Click the **Save** option near the lower-left corner.

You can make the filter, view, or grouping available to users in your system. For more information about sharing filters, views or groupings with other users, see the section [Make filters, views, or groupings available to users](#make-filters-views-or-groupings-available-to-users) in this article.

## Make filters, views, or groupings available to users {#make-filters-views-or-groupings-available-to-users}

These steps explain how to make filters, views, and groupings available from the Interface area in Setup. You can also do this in the List Controls area in Setup. For more information, see [Edit list controls: filters, views, and groupings](../../../administration-and-setup/manage-workfront/configure-reports/edit-list-controls-filters-views-groupings.md).

1. Click the **Main Menu** ![](assets/main-menu-icon.png), then click **Setup**.

1. Click **Interface**, then click one of the following: **Filters**, **Views**, or **Groupings**.

1. Select the filter, view, or grouping that you want to make available to users, then click **Share** to open the Filter Access, View Access, or Grouping Access form.
1. (Conditional) To make the filter, view, or grouping available to all users in the system, click the **Gear** drop-down menu ![](assets/gear-menu-for-sharing-items.png), then click **Make this visible system-wide**. All users in the system can now see the filter, view, or grouping.

   Or

   Begin typing the name of specific users, teams, roles, groups, or companies to share the filter, view, or grouping with, then click the name when it appears in the drop-down list.

   For more information about sharing, see [Overview of sharing permissions on objects](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Click **Save**.

   Users that you specified can now see the default filter, view, or grouping when viewing the object type that you associated it with.

## Delete filters, views, and groupings

>[!NOTE]
>
>You can hide the options All, Standard, and Nothing after selecting different defaults (see Step 5), but they can't be deleted. You can delete any other option being used as a default, but you have to select a different default first.

1. Click the **Main Menu** ![](assets/main-menu-icon.png), then click **Setup**.

1. Do any of the following, depending on whether you are deleting a filter, view, or grouping:

   * Click **Interface** > **Filters**
   
   * Click **Interface** > **Views**
   
   * Click **Interface** > **Groupings**

1. Select one or more items in the list, then click **Delete**.
1. See one of the following sections for detailed information about configuring a filter, view, or grouping.

   * [Filters overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) 
   * [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md) 
   * [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
