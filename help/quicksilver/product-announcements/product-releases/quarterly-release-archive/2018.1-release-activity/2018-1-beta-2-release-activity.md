---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 2 release activity
description: This page describes all changes most recently available in the Preview environment with the 2018.1 Beta 2 release. The functionality on this page was made available in the Preview environment on December 14, 2017. It will be made available in the Production environment in March, 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
---
# 2018.1 Beta 2 release activity

This page describes all changes most recently available in the Preview environment with the 2018.1 Beta 2 release. The functionality on this page was made available in the Preview environment on December 14, 2017. It will be made available in&nbsp;the Production environment in March, 2018.

>[!IMPORTANT]
>
>&nbsp;Functionality described on this page is subject to change prior to availability in the Production environment.

For a list of all changes made in 2018.1, see&nbsp; [2018.1 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

The 2018.1 Beta 2 release contains enhancements for both for Workfront administrators and other users:

**For Administrators**

* [Group Administration for Users and Layout Templates](#group-administration-for-users-and-layout-templates)

**For All Users**

* [System-Wide Widescreen Display](#system-wide-widescreen-display) 
* [Resize Timeline Snapshot on the Gantt Chart](#resize-timeline-snapshot-on-the-gantt-chart) 
* [Interactive Resource Planner in the Business Case](#interactive-resource-planner-in-the-business-case) 
* [Visualization in the Resource Planner - User Allocation Chart](#visualization-in-the-resource-planner-user-allocation-chart) 
* [Improvements in the Home Area](#improvements-in-the-home-area) 
* [New proofing viewer Improvements](#new-proofing-viewer-improvements)&nbsp;

## Group Administration for Users and Layout Templates {#group-administration-for-users-and-layout-templates}

You can now designate group administrators in Workfront.&nbsp;The Group Owner field has been renamed to group administrator, and users who are designated as group administrators have additional permissions to manage users and layout templates for the groups they manage.

* [User Management by group administrator](#user-management-by-group-administrator) 
* [Layout Template Management by group administrators](#layout-template-management-by-group-administrators)

### User Management by group administrator {#user-management-by-group-administrator}

We are introducing the new concept of **group administrator**. To support this, the **Group Owner** field has been renamed to **group administrator** and the users who are designated as group administrators have additional permissions to manage users and the groups.

In addition to the permissions that the Group Owner previously had to manage users, the group administrator now has the following additional access when managing users within the groups where they are set as a group administrator:

* Log in as another user who belongs to a group they manage.
* Reset the password for another user who belongs to a group they manage.
* Create Layout Templates administered by their group.&nbsp;

Prior to this change, only the Workfront administrator could perform these functions.

For more information about group administrators, see the "Understanding group administrators" section in [Create a group](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Layout Template Management by group administrators {#layout-template-management-by-group-administrators}

We are introducing the new concept of **Group with Administration Access** which you can associate with a Layout Template.

The user designated as a group administrator on this group has access to manage that Layout Template and create new Layout Templates where the groups they manage are the administrative groups of the templates.&nbsp;

Prior to this change, only the Workfront administrator could create Layout Templates.

For more information about creating Layout Templates, see see "Creating and Managing Layout Templates."

## System-Wide Widescreen Display {#system-wide-widescreen-display}

When you display any page in Workfront, the entire browser window is now filled automatically and it adjusts to your screen size.

Prior to this change, only the pages associated with the following objects were displayed in widescreen:

* Projects
* Tasks
* Issues
* Reports
* Dashboards
* Calendars

## Resize Timeline Snapshot on the Gantt Chart {#resize-timeline-snapshot-on-the-gantt-chart}

You can now expand the timeline snapshot to show the entire project in the Gantt chart.

Prior to this enhancement, you could select a specific point on the timeline snapshot to navigate to it in the Gantt chart.

For more information about configuring how information displays on the Gantt chart, see [Configure how information displays on the Gantt Chart](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Interactive Resource Planner in the Business Case {#interactive-resource-planner-in-the-business-case}

As a Resource Manager, you can now add Resource Pools in the Resource Budgeting section of the Business Case. You can also budget your project resources using the project-level Resource Planner. Budgeting your resources for a project generates the Budgeted Labor Cost of the project.

Prior to this change, you could view Resource Budgeting information in the Business Case if the project had been budgeted for resources in the global Resource Planner.

For more information about completing budgeting project resources in the Business Case, see [Budget resources in the Business Case](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

## Visualization in the Resource Planner - User Allocation Chart {#visualization-in-the-resource-planner-user-allocation-chart}

You can now display the overall Planned Allocation of all users against their availability in a chart in the Resource Planner. The chart is available when you select **View by User** in the Resource Planner.

The chart displays the following information:

* Availability % with no overallocation for all users
* Overallocation % for all users
* Underutilization % for all users
* There is an overallocation for at least one user during this time period

Prior to this change, you could view the allocation and availability of individual users only in table format.

For more information about the user allocation chart in the Resource Planner, see [Resource Planner overview](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Improvements in the Home Area {#improvements-in-the-home-area}

Various improvements are now available in the Home area, including:

* Look and feel improvements

   * The right panel is now larger, allowing more space for task and issue information.
   * Overdue items are now shown in a lighter shade of red when selected in the left panel.
   * You can now more easily see the relationship between the left panel and the right panel. The selected document in the left panel points to the right panel.

* Default fields are displayed for selected items.&nbsp;

  For more information about the default fields, see "Creating and Managing Layout Templates."

* After you click "Work On It" on a request, the fields associated with the issue are displayed in the right panel.

  For more information about working on requests from the Home area, see [Manage work and team requests in the Home area](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md) in [Manage work and team requests in the Home area](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md).

* Point to a user avatar on a work item in the left panel to view the name of the user.
* Expand the "Late" area in the left panel to view all late items (when this area is collapsed, only the first 5 items are displayed).
* After you mark an item as Complete, the item stays in the left panel until you select another item.  
  For information about showing completed items, see [Display items in the Work List in the Home area](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) in [Display items in the Work List in the Home area](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

For more information about using the new Home area, as well as information describing differences in functionality between My Work and Home, see [Use the Home area](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## New proofing viewer Improvements&nbsp; {#new-proofing-viewer-improvements}

* [Improved Layout and Design](#improved-layout-and-design) 
* [Search Comments by Comment Number](#search-comments-by-comment-number) 
* [Option to Edit Comment next to the Markup Indicator](#option-to-edit-comment-next-to-the-markup-indicator) 
* [Mark All Comments as Read](#mark-all-comments-as-read) 
* [Left Menu Improvements](#left-menu-improvements)

### Improved Layout and Design {#improved-layout-and-design}

The proofing viewer has an updated look and feel. The&nbsp; following areas of the proofing viewer were updated:

* Thumbnails area

  For more information about using the thumbnails area, see in&nbsp;.

* Comments area  
  For more information about the comments area, see&nbsp;.
* Left menu area

### Search Comments by Comment Number {#search-comments-by-comment-number}

Now when you search the comment list in the proofing viewer, you can enter the number of the comment in the search field. The comment list is then filtered to display the comment you searched for.&nbsp;

For more information, see in .

### Option to Edit Comment next to the Markup Indicator {#option-to-edit-comment-next-to-the-markup-indicator}

You can now more easily edit an existing comment. After clicking a comment indicator on the proof, an edit icon is displayed next to the balloon.&nbsp;

Prior to this change, you had to click the edit icon in the Comment area.&nbsp;&nbsp;

For more information, see .

### Mark All Comments as Read {#mark-all-comments-as-read}

When viewing a document in the proofing viewer, you can now mark all comments as Read.

### Left Menu Improvements {#left-menu-improvements}

The menu on the left side of the proofing viewer contains the following improvements:

* Updated look and feel
* Icon at the top of the menu to show or hide the menu

  ![proof_viewer_menu_hide.png](assets/proof-viewer-menu-hide.png)

* Mouse over the menu to automatically expand the menu to view labels in addition to icons. (Or enable the option to keep the menu always in the collapsed view.)
