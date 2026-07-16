---
content-type: release-notes
title: Third Quarter 2026 release activity for Adobe Workfront Planning
description: This is the release activity for the Adobe Workfront Planning product for the Third Quarter 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
---
# Third Quarter 2026 release activity for Adobe Workfront Planning

<!--
take the next sentence out when we start listing features
-->

<!--
There are no features released during the Third Quarter Release for 2026. When features are released for this quarter, we will document them in this article. 
-->

<!--keep the sentence below for all future quarterly release pages--> 

This article describes the features that are releasing for Workfront Planning during the Third  Quarter 2026 release.

For a list of all features released for Adobe Workfront Planning, see [Adobe Workfront Planning release activity: article index](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


## New license type fields for Access Levels 

>[!NOTE]
>
>Preview and production for all customers: July 16, 2026
>[!BADGE Off schedule]{type=Neutral}


We have made the following field changes in the Access Level box:

* We have renamed the License Type field in the Access Level box to Workflow License Type. There are no functionality changes with this relabeling.

    For information, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* For customers who also have purchased a Workfront Planning package, we have added a new Planning License Type field to illustrate a user's license to Workfront Planning. 
Customers who have purchased an equal number of Workflow and Planning licenses have the following license types available:

    * Planning Standard
    * Planning Contributor
    * None

>[!NOTE]
>
>You can assign users a mixed combination of licenses between Workflow and Planning, but users must have a paid Workflow license to have a Planning Standard license. 
>
>For example, a Planning Standard license cannot be assigned to a Workflow Contributor user. A user with a Workflow Light license can now be granted Standard license to Planning and thus manage workspaces and their content. Previously, they could only have view-only access to Planning data. 
>
>New customers can purchase Planning and Workflow licenses in different quantities and use them with any combination. In this scenario the Planning Contributor license type is not available.  

For information, see [Adobe Workfront Planning access overview](/help/quicksilver/planning/access/access-overview.md).  

## Automated access control for Workfront Planning in Snowflake

>[!IMPORTANT]
>
>Preview and Production for all customers: July 16, 2026
>[!BADGE Off schedule]{type=Neutral}


This release introduces automated, entitlement-driven access management for Workfront Planning data in Snowflake as part of Workfront Data Connect. 

It starts by extending secure view generation to Planning tables  establishing the required foundation for downstream access control and making entitlement-based grants possible. 

Building on this, reader account provisioning now checks TMS entitlements at creation time and automatically applies or withholds grants to the Planning database, ensuring correct.  

Prior to this enhancement, this was available only for Workfront. 

The update includes the following capabilities:  

* An automated daily job detects entitlement changes for existing customers 
* The new job grants, revokes, or preserves access based on entitlements 
* Full lifecycle coverage across provisioning, account creation, and ongoing entitlement changes. 

The [Workfront Data Connect data dictionary](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md) article will be updated after the release date.


## Set default permissions for records

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

Workspace managers can now set a default permission rule — Open or Restricted — for each record type, so newly created records are automatically protected without any manual steps.  

When you select Restricted, only the record creator and any specifically selected users, groups, teams, roles, or companies can edit the record, while everyone else retains view-only access.  

This rule applies automatically to new records, regardless of how the record is created (New record button, request forms, API, using a Fusion automation, or AI Assistant). Changes to the rule only affect records created going forward, never existing ones.  

Once a record is created, its permissions can still be updated independently without impacting the default rule for future records. 

For information, see [Set default permissions for records](/help/quicksilver/planning/access/set-default-record-permissions.md).  

## Swimlane grouping layout for the timeline view

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

Timeline views that are grouped now support a swimlane layout, with groups rendering as a frozen left header column instead of scrolling horizontal bands. This grouping type is additional to the current stacked grouping.  

Nested grouping levels show as indented sub-columns, and records within each lane stay sub-stacked and sorted. 

You can drag and drop records in the grouped view to smoothly update their information and dates.  

All users viewing the view can see the groupings applied.  

For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md). 


## Recently visited items in the global search box

>[!NOTE]
>
>Preview and Production for all customers: June 30, 2026
>[!BADGE Off schedule]{type=Neutral}

The global search box in Planning now remembers your most recent searches: the last 7 visited workspaces, record types, and views are surfaced in dedicated, clearly labeled sections so you can access them quickly without re-running a query.  

The recent results respect current permissions, and the list of most recent items is visually distinct from live search results. As before, you can access search from the Planning landing page or from any page by using a keyboard combination.  

For more information, see [Workspace overview](/help/quicksilver/planning/architecture/workspaces-overview.md).


## Support for currency Planning fields in Canvas Dashboards

>[!NOTE]
>
>Preview: June 25, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

You can now include currency Planning fields, in table, KPI, and chart reports in Canvas Dashboards.  

Prior to this enhancement, currency fields were not supported in Canvas Dashboards.  

For information, see [Use currency fields in Canvas Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md). 

## Row color controls interface improvement

>[!NOTE]
>
>Preview: June 22, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

We have updated the look and feel of the Row colors control in the table view. 

For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 

## Add default choices for select and People type fields 

>[!NOTE]
>
>Preview: June 18, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

When you create a single-, multi-select field or a People type field, you can now indicate a default value for these fields. The default values will always be applied when the field is visible on a record.  

You can change the default settings of the field after it is saved. You can replace the default values of the fields when working with records.  

For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md). 

## Interface improvements in the table view

>[!NOTE]
>
>Preview: June 11, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

We have updated the look and feel of the table view for the following areas in Workfront Planning: 

* All record type pages 

* All connected record type pages, except for Projects 

In addition to some navigation changes and design improvements, some improvements in this update include: 

* The addition of an aggregation row at the bottom of the table that summarizes number, currency, percentage, and some formula fields using the following aggregators: SUM, AVG, MAX, MIN.

* A simpler date format with fewer format types when adding a Date field. 

* Ability to select a time zone visible to all users, regardless of their profile's time zone, when adding a Date field. 

* Removal of row numbering for a cleaner look 

* Persistent row selection box, instead of visible only when hovering on the row 

* Persistent column separator lines for better readability 

* A simpler sorting experience when sorting from a column header  

For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).  


## GenStudio for Performance Marketing Brands can now be added to Planning request forms

>[!NOTE]
>
>Preview and Production for all customers: June 5, 2026
>Available only for Adobe Workfront Planning customers that also have Adobe GenStudio for Performance Marketing.
>[!BADGE Off schedule]{type=Neutral}


To allow you to add brands to your campaigns starting with submitting a request, it's now possible for you to add the Brands connected record field to a Planning request form. 

When a Planning record type is connected with the GenStudio Brands record type, you can add the Brands connected field to a Planning request form associated with the Planning record type.  

For information, see [Get started with the Adobe Workfront Planning and Adobe GenStudio for Performance Marketing integration](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).  


## New Sample workspaces tab added to the Planning landing page 

>[!NOTE]
>
>Preview: June 1, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026


We have added the Sample workspaces tab in the Planning landing area where you can view example of best-practice workspaces. The workspaces are not editable. Workspace managers can modify views in sample workspaces. The tab is visible for Standard and System Administrator users.  

We recommend that you view the sample workspaces as examples, and use the multi-workspace template bundle to create, edit, and share workspaces that result as a use of that template.  The template bundle contains the same workspaces as the Sample workspaces tab.   

For information, see [Workspaces overview](/help/quicksilver/planning/architecture/workspaces-overview.md). 

>[!NOTE]
>
>Creating workspaces from template bundles is only available for organizations on the Workflow Prime or Ultimate packages.

## Workfront Planning API version 2 

>[!NOTE]
>
>Available for all customers: May 28, 2026
>[!BADGE Off schedule]{type=Neutral}

Version 2 of Workfront Planning API is now available and it significantly expands the capabilities of Version 1.  

The following enhancements are included in Version 2: 

* Create, update, and delete workspaces, record types, and fields programmatically. 

* Fully manage records. 
* Improvements to URL structure, error handling, pagination, filtering, and permissions. 
* Includes partial updates via PATCH 
* Includes bulk record operations. 

Version 1 remains available, although we recommend that you switch to using Version 2.  

>[!NOTE]
>
>The Workfront Planning connector for Fusion has not been updated to API Version 2 and it will continue to use Version 1 until further notice.   

For information, see [Adobe Workfront Planning API basics](/help/quicksilver/planning/general/planning-api-basics.md).  

For Workfront Planning API specifications, see the [Workfront Planning API](https://developer.adobe.com/wf-planning/) developer documentation. 

## Grant permissions to records

>[!NOTE]
>
>Preview: May 28, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026


You can now adjust individual record permissions to control who can manage them within a record type. 

By default, users inherit record permissions from the workspace and record type. You can now override inherited permissions on specific records to grant View or Manage access to a subset of users. Permission overrides can be applied to individual records or updated in bulk across multiple records.

<!-- 
Laurel asked for this to be replaced with the above: 

Users inherit record permissions from the workspace and record type by default. To give only select users with record type permissions Manage permissions to only certain records, you can disable inherited permissions on select records and grant only those users Manage access to those records. You can adjust permissions for one record, or for multiple records at the same time, in bulk.

You can give users the following permissions levels: 

* View 
* Manage 
-->

>[!NOTE]
>
>* A user's record-level permissions cannot exceed their record type permissions. For example, a user with View access to a record type cannot be granted Manage access to individual records of that type.
>* You cannot remove a user's permissions from a record at this time. Any user with at least View access to the record type can view all records of that type.

For information, see [Share records](/help/quicksilver/planning/access/share-records.md).

## Streamlined global record type addition  

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

To reduce clicks and help you quickly find the record types you need, we've enhanced the experience for adding records to make it faster and more intuitive when you add global record types to another workspace.  

When you choose to add a record from existing record types, you'll now immediately see a list of all available Global Record Types.  

You can select and add one or multiple global record types at the same time directly from this screen.  

For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).  

## Planning Designer now available in Beta for all Workfront Planning customers

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 
>[!BADGE In Beta]{type=Neutral}

You can now use the Adobe Planning Designer powered by AI to configure your workspaces and data structures with ease. The Planning Designer supports everything from creating and configuring workspaces to defining fields and formulas, managing records, reviewing change history and building custom views.  

Whether used directly or through the AI Assistant, the Planning Designer provides a flexible, powerful environment for building and maintaining structured, connected information. 

A Workfront administrator can manage the availability of the Planning Designer from the System Preferences area in Setup.   

For information, see [Get started with the Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).


## Synchronize metadata from Planning to AEM Assets
 
>[!NOTE]
>
>Preview and Production for everyone: May 28, 2026
>Available only for Adobe Workfront Planning customers that also have Adobe GenStudio for Performance Marketing and Adobe Experience Manager.
>[!BADGE Off schedule]{type=Neutral} 

To improve data integrity, we've released seamless metadata synchronization between  GenStudio for Performance Marketing record types and AEM Assets when AEM Assets are linked to GenStudio record types in Workfront Planning. 

The following GenStudio for Performance Marketing record types can be connected to AEM Assets: Campaign, Product, Persona, Region, and Channel. 

Information added to a GenStudio record type in Workfront Planning displays in a separate Campaign tab of an AEM Asset in AEM. Information about Product, Persona, Region, and Channel for that campaign also displays on that tab, in read-only mode. 

With this release key metadata is consistent across both platforms and reflects updates in near real-time, reducing manual reconciliation. 

For information, see [Manage the GenStudio workspace in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).

## Synchronize Metadata from Planning to AEM Content Fragments  

>[!NOTE]
>
>Preview and Production for everyone: May 28, 2026
>Available only for Adobe Workfront Planning customers that also have Adobe GenStudio for Performance Marketing and Adobe Experience Manager.
>[!BADGE Off schedule]{type=Neutral}

To improve data integrity, we've released seamless metadata synchronization between Planning record types in the GenStudio workspace and AEM Content Fragments when Content Fragments are linked to GenStudio for Performance Marketing campaigns.  

GenStudio campaign information now displays in the Metadata tab of a Content Fragment in AEM.  Information about Product, Persona, Region, and Channel for that campaign also displays on that tab, in read-only mode. 

With this release key metadata is consistent across both platforms and reflects updates in near real-time, reducing manual reconciliation. 

For information, see [Manage the GenStudio workspace in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).


## List view updates 

>[!NOTE]
>
>Preview: May 27, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026

Multiple field types on the list view have been updated to include keyboard navigation and other enhancements. 

Multi-, Single-select, and Assignee fields now offer keyboard navigation in the list view: 

* Use the up and down arrows on your keyboard to move through the list of people. 

* Press the space bar to select a person or to remove a selected person. 

On single and multi-select fields in the list view:  

* You can add new options directly from the editor when no results are found. Note that this feature may not be available on all lists. 

* The field interaction is now keyboard accessible. This includes navigation between the tags, search options, and list using the up and down arrows. Press the space bar to select an item or remove a selected item. 

Reference fields such as typeahead and external lookup fields, have received some interface enhancements. 

Also, where available, the experience of dragging and dropping columns has been improved visually. 

For more information, see [Manage the list view in Adobe Workfront Planning](/help/quicksilver/planning/views/manage-the-list-view.md). 

## Workfront reference fields are enabled as lookup fields for Planning connections

>[!NOTE]
>
>Preview: May 27, 2026 
>Production fast release: June 11, 2026  
>Production for everyone: July 16, 2026 

You can now add Workfront reference fields as lookup fields when connecting a Planning record type with a Workfront object type. 

For example, you can add the Portfolio, Program, Group or Company information from the Project object to a project connection field of a campaign in Planning.  

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 

## New filters for the timeline view breakdown feature 

>[!NOTE]
>
>Preview: May 27, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

You can now filter information in the timeline view based on criteria that match objects included in the breakdown of the records.  

Prior to this enhancement, you could only apply filters for the main records in the timeline view. 

For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md). 

## New indication that edited and deleted fields impact request forms 

>[!NOTE]
>
>Preview: May 27, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

We have added a reminder that record fields that you edit or delete might impact request forms that contain those fields. Now, you will have a chance to review the affected forms and ensure the changes you want to make to the fields will not impact existing information.  

For information, see [Edit field settings](/help/quicksilver/planning/fields/edit-fields.md). 

## Edit submitted Planning requests

>[!NOTE]
>
>Preview: May 27, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

You can now edit Planning requests after you submit them, before a record is created from the request. 

The following users can edit a submitted request: 

* The request creator 
* Workspace managers for the workspace where the request was submitted 
* System administrators 

Prior to this enhancement, you could not edit submitted requests. 

For more information, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md). 

## New preview window for AEM content fragments

>[!NOTE]
>
>Preview and Production for all customers: May 14, 2026
>[!BADGE Off schedule]{type=Neutral}

For better visibility when working with AEM content fragments that are connected to Workfront Planning records, we have added a preview window that displays information about the fragments in Workfront Planning.

This functionality was previously available for AEM assets and we have now added it to content fragments. 

For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).  

## Lookup fields now available for AEM content fragments in Workfront Planning

>[!NOTE]
>
>Preview and Production for all customers: May 14, 2026
>Available only for Adobe Workfront Planning customers that also have Adobe Experience Manager.
>[!BADGE Off schedule]{type=Neutral}

You can now add the following lookup fields when you connect a Planning record type to an AEM Content Fragment: 

* Created by 
* Created at 
* Modified by 
* Modified at 

Prior to this enhancement, lookup fields were only available for AEM assets and folders.  

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 



## Custom views for a record's Details page 

>[!NOTE]
>
>Preview: May 14, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

To allow for better flexibility of visualizing your information in a record's details page, we have introduced the ability to create custom views for this page.  

In addition to adding two already-built details page views that contain either all the records fields or just the fields visible in the table view, you can now create custom views for a record's details pages. The views you create are visible to everyone that can access the record.  

This update removes the **Show all fields** setting and replaces it with custom details views.  

For information, see [Manage the record page](/help/quicksilver/planning/records/manage-the-record-page.md).

## Add groupings to a Projects connected record page

>[!NOTE]
>
>Preview: May 14, 2026     
>Production fast: June 11, 2026 
>Production for everyone: July 16, 2026 

You can now group your information in the projects connected records page of a record in Workfront Planning. This capability did not exist in this area prior to this enhancement.

For information, see [Manage the list view](/help/quicksilver/planning/views/manage-the-list-view.md).

