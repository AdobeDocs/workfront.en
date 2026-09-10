---
title: Customize the Main Menu Using a Layout Template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: As an Adobe Workfront administrator or a group administrator, you can use a layout template to configure the options users see when they open the Main Menu in Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
TQID: https://experienceleague.adobe.com/g6y6RsDNuEDBGZBrZXxhyFZ2-z1EUr5yflGDQQ7AhdQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
  - id: d3382524-5489-431b-bde9-271ab257bc37
    internal-label: Workfront Scenario Planner
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
  - id: fceb5125-bb41-419a-b0db-31958cb42f6c
    internal-label: Workfront Goals
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Customize the Main Menu using a layout template

<!--Audited: 01/2024-->

As an Adobe Workfront administrator or a group administrator, you can use a layout template to configure the options users see when they open the Main Menu in Workfront.

>[!NOTE]
>
>The Main Menu options that users see depend on their license type and what settings are configured in their access level. Some users who will use this layout template may not see all the options you choose here. For more information see [How access levels and permissions work together](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) and [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).
>
>You might see different options in the Main Menu after your organization has been onboarded on the Adobe Workfront Unified Experience. For information, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md). 

For information about creating layout templates, see [Create and manage layout templates](../use-layout-templates/create-and-manage-layout-templates.md). 

For information about layout templates for groups, see [Create and modify a group's layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

After configuring a layout template, you must assign it to users for changes you made to be visible to others. For information about assigning a layout template to users, see [Assign users to a layout template](../use-layout-templates/assign-users-to-layout-template.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p>
       <p>Adding custom applications to the Main Menu is only available for organizations licensed for Adobe App Builder.</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td> <p>To perform these steps at the system level, you need the System Administrator access level.</p>
        <p>To perform them for a group, you must be a manager of that group.</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Customize the Main Menu

1. Begin working on a layout template, as described in [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Click **Set Main Menu** in the upper-right corner of the template.

   The Main Menu box opens and you can see the areas that currently display in the Main Menu for the template, as well as the items that are available to add. The following are all the possible items that you can add:
   * Home

     >[!TIP]
     >
     >By default, the Home icon in the Main Menu displays the My Updates area for Review-license users (in the current license plan), unless they have a layout template associated with their profile that includes the My Updates area in the Main Menu, in addition to the Home area.
  
   * Priorities
   * Portfolios
   * Programs
   * Projects
   * Reports
   * Dashboards
   * Calendars
   * Resourcing
   * Scenarios

     >[!NOTE]
     >
     >The Scenario Planner requires an additional license. For information about the Workfront Scenario Planner, see [The Scenario Planner overview](../../../scenario-planner/scenario-planner-overview.md).

   * Teams
   * Users

     >[!NOTE]
     >
     >Only users with a Plan license (in the current license model), or the users with a Standard license (in the new license model) can see the Users area ![Users icon](assets/users-icon-in-main-menu.png) in the Main Menu.

   * Requests
   * Timesheets
   * Documents
   * Templates
   * Goals

     >[!NOTE]
     >
     >Goals require an additional license. For information about Workfront Goals, see [Adobe Workfront Goals overview](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * My Updates
   * Boards
   * Blueprints
   * Planning

     >[!NOTE]
     >
     >Planning requires an additional license. For information about Workfront Planning, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
   
   * Custom Application

      >[!NOTE]
      >
      > Custom applications must be created separately before they become available as Main Menu options. For more information, see [Create a custom application for Workfront with Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

In the Preview environment:

1. Do any of the following for the **Native** items:

   * Hide ![Hide icon](assets/remove-icon---x-in-circle.png) items that you don't want to display on the Main Menu.
   * Show ![Show icon](assets/add-icon-plus-in-circle.png) items that you do want to display on the Main Menu.
   * Drag ![Drag icon](assets/move-icon---dots.png) items to change their display order on the Main Menu.

1. Do any of the following for the **System** items:

   * Hide ![Hide icon](assets/remove-icon---x-in-circle.png) items that you don't want to display on the Main Menu.
   * Show ![Show icon](assets/add-icon-plus-in-circle.png) items that you do want to display on the Main Menu.

   >[!NOTE]
   >
   >You can't change the order of system items. These items always display at the bottom of the Main Menu when they are active.

1. Click **Done**.

   You can also click **Cancel** at any time if you want to discard your changes.

1. Continue customizing the layout template. You can click **Apply** at any time to save your progress.

   Or

   If you are finished customizing, click **Save and Close**.

For more information about layout templates, see [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
