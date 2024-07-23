---
product-area: projects
navigation-topic: update-work-in-a-project
title: Update Condition for tasks and issues
description: The Condition of a task or issue is a flag placed on it to indicate how it's going. This is different than the Status of the work item, which indicates the current stage of the development of the item.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
---
# Update Condition for tasks and issues

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

The Condition of a task or issue is a flag placed on it to indicate how it's going. This is different than the Status of the work item, which indicates the current stage of the development of the item.

You can set the Condition of a task or an issue either automatically or manually.

The Condition values that we refer to in this article are available in Workfront by default. Your Adobe Workfront administrator can create custom Conditions for your environment, as described in [Create or edit a custom condition](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md). 

## Access requirements {#access-requirements}

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   New:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>
   Current:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

You must be assigned to a task or an issue to be able to manually update its Condition. 

## Locate the Condition of tasks and issues

Conditions display as a flag associated with tasks or issues. They can also be associated with a number which can display in reports instead of the label. For more information about associating conditions with numbers, see [Create or edit a custom condition](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md). 

You can locate the Condition of tasks and issues in the following areas of Workfront:

* The Details page, after a Workfront or group administrator adds it to your layout template. For information, see [Customize the Details view using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md). 

* The header of a task or issue, after a Workfront or group administrator adds it to your layout template. For information, see [Customize object headers using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md). 

* The Summary panel, after a Workfront or group administrator adds it to your layout template. For information, see [Customize Home and Summary using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). 

* Reports and lists when you display the Condition field in a View or Grouping. 

     >[!NOTE]
     >
     >When the word "condition" displays in the Field Name field of a Journal Entry report, this indicates that the Condition of an item was updated. When the Condition field is tracked in Journal Entries reports, the New and Old Number Values display the number associated with the condition instead of its name. If a condition is originally not defined for a task or an issue and you later update it, the journal entry that captures the update will display the Old Number Value of the Condition field as -2,147,483,648.

## Automatically update the Condition by updating the status

When you are assigned a task or issue and you click **Work On It** , Start Task or Start Issue, or update its status, the Condition of the task or issue automatically changes to the default Condition associated with **Going Smoothly**.

For information about using a custom Condition as a default Condition, see the articles  [Set a custom condition as the default for tasks and issues](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) and [Set a custom condition as the default for projects](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

For information about changing the task status, see [Update task status](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

For information about changing the issue status, see [Update issue status](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

For information about setting the Work On It button to a Start Task or Start Issue button, see [Replace the Work On It button with a Start button](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Manually update the Condition

You must be assigned to a task or the issue or have Manage permissions to it to be able to set the Condition on it.

You can manually update the Condition of a task or issue in a task or issue report or list when  you display the Condition field in the view. 

>[!NOTE]
>
>You can ask your system or group administrator to add the Condition field to your Summary panel, or the task or issue header or Details pages. 
>
>For more information, see the following articles:
>
>* [Summary overview](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Customize Home and Summary using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

You can manually update the Condition of tasks and issues in various areas of Workfront. The following sections describe how you can manually update the Condition of tasks and issues. 

### Update the Condition of a task or issue in the task or issue header

1. (Conditional) If your Workfront or group administrator added the Condition field to the task or issue header of your layout template, click the **Condition** field in the header and select from the following options: 
     * Going Smoothly
     * Some Concerns
     * Major Roadblocks

     ![](assets/condition-in-task-header.png)
1. Click Enter to save the Condition. 

### Update the Condition of a task or issue in the task or issue Details section

1. (Conditional) If your Workfront or group administrator added the Condition field to the Details section of a task or issue in your layout template, click **Details** in the left panel, then click **Task Condition** or **Issue Condition** and select from the following options: 
     * Going Smoothly
     * Some Concerns
     * Major Roadblocks
1. Click **Save Changes**. The Condition of the task or issue is updated. 

### Update the Condition of a task or issue in a report or list

1. Go to a list of tasks or issues that you have Manage permissions to. Ensure the **Condition** field is visible in the list's view. 

1. Update the **Condition** of the issue or task inline, by double-clicking the existing condition and selecting a new value from the drop-down menu. 

     ![](assets/condition-drop-down-values-in-task-list.png)

     >[!NOTE]
     >
     >Conditions can be customized for your environment, so you may find more than three options for Condition in your environment. The names of the Conditions might be different than the ones listed above. For information about customizing Conditions in Workfront, see [Create or edit a custom condition](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).


1. Press **Enter** on your keyboard, or click outside the Condition field to save the new task or issue Condition. 

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


