---
filename: customize-left-panel
title: Customize the left panel using a Layout Template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
title: Customize the left panel using a layout template
description: In a layout template, you can customize what users see in the left panel area throughout Adobe Workfront.
---

# Customize the left panel using a layout template

In a layout template, you can customize what users see in the left panel area throughout Adobe Workfront.

For example, you can determine which of the following items users see in the left panel when viewing a task:

![](assets/left-panel-adobe-branding-350x233.png)

>[!IMPORTANT]
>
>Changes made to order and visibility are reflected in the mobile app.

For information about layout templates for groups, see [Create and modify a group’s layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Customize the left panel for an area in Workfront:

1. Begin working on a layout template, as described in [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Click the down arrow ![](assets/dropdown-arrow.png) under `Customize what users see`, then click the left panel you want to customize.

   >[!NOTE]
   >
   >For information about the Home option in this drop-down list, see [Customize Home and Summary using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). For information about the Lists option, see [Customize Filters, Views, and Groupings using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. In the `Left panel` list, do any of the following to determine what will users see in the left panel for the option (Workfront area or object type) you have selected:

  * Show ![](assets/add-secondary-nav-item.png) or hide ![](assets/delete-secondary-nav-item.png) items. Any item without ![](assets/add-secondary-nav-item.png) or ![](assets/delete-secondary-nav-item.png) cannot be hidden.
  
  * Drag items ![](assets/move-icon---dots.png) to change their order on the left panel.

   | Option |When users click the following... |They see the left panel items you choose from the following: |
   |---|---|---|
   | Project |The name of a project |Tasks, Project Details, Business Case, Updates, Documents, Issues, Risks, Approvals, Baselines, Billing Rates, Billing Records, Expenses, Hours, Scheduling, People, Utilization, Queue Details, Routing Rules, Queue Topic, Topic Group, Metrics |
   | Task |The name of a task | Updates, Documents, Task Details, Subtask, Issues, Hours, Approvals, Expenses, Predecessors |
   | Issue |The name of an issue | Updates, Documents, Issue Details, Hours, Approvals |
   | Portfolio |The name of a portfolio |Projects, Programs, Portfolio Details, Portfolio Optimization, Documents, Updates |
   | Program |The name of a program |Projects, Program Details, Updates, Documents |

   >[!NOTE]
   >
   >The last 3 items in the `Customize what users see` drop-down list (Lists, Home and Summary, and Branding) are for configuring areas other than the left panel. For information about them, see these articles:
   >
   >  
   >  
   >  * [Customize Filters, Views, and Groupings using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md) 
   >  * [Customize Home and Summary using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md) 
   >  * [Brand Adobe Workfront using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md) 
   >  
   >

1. (Optional) If you want to add a left panel item that links to one of your organization's dashboards, click `Add custom section`, type a `Custom section title` for the item, then add the dashboard.

   Dashboard items appear at the bottom of the left panel. Users see the Custom section title you type next to the dashboard item when they hover over the left panel.

   >[!NOTE]
   >
   >Users can add custom dashboard items to their own left panel. When you add custom dashboard items in a layout template, your items merge with theirs, without overwriting or resetting them. This is also true if you assign users to a new layout template with custom dashboard items. For information about how users can customize the left panel, see [Create custom tabs or sections](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

   For information about dashboards, see [Dashboards](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Continue customizing the layout template.

   Or

   If you are finished customizing, click `Save`.

   >[!TIP]
   >
   >You can `Save` your progress at any time, then continue to modify the template later.

