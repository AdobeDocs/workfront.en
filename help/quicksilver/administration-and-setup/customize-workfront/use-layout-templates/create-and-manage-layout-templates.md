---
title: Create and manage layout templates
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: As a Workfront administrator or a group administrator, you can create and modify layout templates to customize layout elements in Workfront for your users.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
---
# Create and manage layout templates

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

As an Adobe Workfront administrator or a group administrator, you can create and modify layout templates to customize the following layout elements in Workfront for your users:

* Main Menu
* Left navigation panel
* Home area 
* Views, filters, and groupings people use with lists and reports.
* On-screen terminology
* Project, task, and issue headers

After you create or modify a layout template, you can assign it to individual users, teams, groups, or job roles.

Every user's default Workfront layout depends on their access level and license type. For example, some users might not see some areas in the Main Menu. For more information, see [About the default Adobe Workfront layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

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
   <td><p>New: Standard</p>
   Or
   <p>Current: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>To perform these steps at the system level, you need the System Administrator access level.</p>
<p>To perform them for a group, you must be a manager of that group.</p> <p><b>NOTE</b>:</p> <p>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. 

For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Considerations for creating and managing layout templates

* Users can customize a few areas of their own layout. When you change a layout template, your changes merge with any customizations they have made, without overwriting or resetting them. This is also true if you assign users to a new layout template.
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
* Group administrators and users with a Plan license who can edit other users can add system-level and group-level layout templates to the users they can manage when editing their profile.
* Group administrators cannot assign layout templates to job roles or teams.

For more information about layout templates, see [Layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## Create or modify a layout template

{{step-1-to-setup}}

1. In the left panel, click **Interface** > **Layout Templates**.

1. Click **New Layout Template**.

   Or

   Click the name of the layout template you want to modify.

1. If you are creating a new layout template, type a **Layout template name** and (optional) a **Description** for it.

1. Customize areas of the user interface, as described in the following articles:

   * [Customize the Main Menu using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) 
   * [Customize the left panel using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md) 
   * [Customize pinned pages using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md) 
   * [Customize the Details view using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md) 
   * [Customize Home and Summary using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md) 
   * [Customize the landing page using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md) 
   * [Customize Filters, Views, and Groupings using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md) 
   * [Customize user interface terminology using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Continue to test your layout template and make it available to users, as described in the articles below:

   * [Testing a new layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md) 
   * [Grant administrative access for a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md) 
   * [Assign users to a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>You can also create a layout template by copying it and changing the copy. For more information, see [Copy a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

