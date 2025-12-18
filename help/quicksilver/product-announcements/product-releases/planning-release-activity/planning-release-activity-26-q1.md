---
content-type: release-notes
title: First Quarter 2026 release activity for Adobe Workfront Planning
description: This is the release activity for the Adobe Workfront Planning product for the First Quarter 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog

---
# First Quarter 2026 release activity for Adobe Workfront Planning

This article describes the features that are releasing for Workfront Planning during the First Quarter 2026 release.

<!--keep the sentence below for all future quarterly release pages-->

For a list of all features released for Adobe Workfront Planning, see [Adobe Workfront Planning release activity: article index](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Share views in the Projects Connected records page

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026  
>Production for everyone: January 15, 2026  

To make it easier to ensure to see the information you need, we've added the ability to share views to the Projects Connected records page. Now, you can share views with other users, teams, or groups.

For information, see [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

## Current user wildcard now available in project connection view filters

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026  
>Production for everyone: January 15, 2026 

To make it easier to filter for project connections that apply to you, we've created a current user wildcard. Now, when filtering, you can select "Me (logged in user)." The filter will then apply to the user who is viewing the request list. 

This can be convenient when adding a filter to a view that multiple users will use. Each user will see filter results that apply to them.

The wildcard is available in fields where the value is a user.

For more information on configuring project connection views, including filters, see [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

<!--

## Create record type hierarchies in workspaces

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production all: January 15, 2026 

You can now define flexible but structured hierarchies between record or object types.  

Hierarchies are connections between record types. You can have up to 4 record and object types connected in one hierarchy, and you can have multiple hierarchies in one workspace. The first record type in the hierarchy is a parent, and all the other record or object types are its children objects.  

You can use hierarchies to organize work in a way that reflects how your teams actually plan, operate, and deliver and to visualize how strategy flows into execution. 

Consider the following when building hierarchies: 

* You can have multiple hierarchies in a workspace 
* You can connect only Planning record types from one workspace and Workfront projects in a hierarchy.  
* A record type or a project can only have one parent in the same workspace. 
* A record type can be the parent in multiple hierarchies 
* Connectable record types cannot be used in hierarchies in other workspaces than their own. 
* Global record types can be used in hierarchies only in the workspaces that they were created in or have been added to.  

When you create hierarchies between record types, they generate breadcrumbs for records that belong to those record types. 

For more information, see [Hierarchy and breadcrumb overview](help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

<!--

## New unified breadcrumbs added to records' pages

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

We have added breadcrumbs to a record's page to reflect its spot in a hierarchy. After you create hierarchies, you can see a record's breadcrumb at the top of its page, indicating what other parent or children objects are connected to it. Hierarchies are consistent across Workfront and Planning.  

For example, you can view a project's Planning hierarchy when it's connected to Planning record types in its Planning breadcrumb, and its Workfront hierarchy when it's connected to Workfront object types, like Portfolios or Programs, in Workfront.  

For information, see [Hierarchy and breadcrumb overview](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

## Workspace main page improvements 

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

We have made the following improvements to the Workspaces main page in Workfront Planning:  

* A faster, more dynamic scrolling experience. This is especially visible if your organization has a large number of workspaces and for system administrators.  

* We added a search box which now allows you to search for a specific workspace by name.  

* The **Other workspaces** tab has been renamed to **All workspaces** and it includes all workspaces you have at least permissions to View, including the ones you created.  

For information, see [Edit workspaces](/help/quicksilver/planning/architecture/edit-workspaces.md).

<!--

## Improvements to connected records pages

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

To give you more flexibility when working with connected records pages, we have enhanced the functionality of views in this area of Workfront Planning. The following are improvements in the connected records pages of a record that are coming with this release:

* You can now add a timeline and a calendar view to a record's connected records page.
* You can now share views from a connected records page. The views shared from these pages are visible system-wide by all users you share them with in any other area of Workfront Planning. All views shared in any other areas of Planning are also visible in the connected records page for the same users they are shared with.
* We have added a restriction to only allow one connected records page per each record or object type. Prior to this enhancement, you could add multiple pages for the same record or object type. Now, you can use multiple views for the same record type in one connected records page.
* We have added a **New row** link at the bottom of a table view and a **Connect records** button in the upper-right area of the connected records page. Prior to this enhancement, the **New row** link and the **Connect records** button existed only on a project connected page. 

For information, see [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

-->

## Adding the Brand connection field to Products and Personas by default in the GenStudio workspace  

>[!NOTE]
>
>Preview: December 11, 2025
>Production fast release: December 11, 2025
>Production for everyone: December 11, 2025

The connection field with the GenStudio for Performance Marketing Brand is now added by default to the Products and Personas record types in the GenStudio workspace of Workfront Planning.  

Your organization must have both Workfront Planning and Adobe GenStudio for Performance Marketing. 

Prior to this enhancement, you could add the Brand connection field only manually to any record type, including Products and Personas. You can still manually connect the Brand GenStudio record type to other record types in Workfront Planning.  

For information, see [Get started with the Adobe Workfront Planning and Adobe GenStudio for Performance Marketing integration](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

## Restrict removing GenStudio for Performance Marketing users' permissions from Planning 

>[!NOTE]
>
>Preview: December 11, 2025
>Production fast release: December 11, 2025
>Production for everyone: December 11, 2025

We have added a guardrail that prevents you from removing the permissions of GenStudio for Performance Marketing users from Workfront Planning objects. With this improvement, you can no longer remove GenStudio users from the GenStudio workspace in Planning, nor can you disable Inherited permissions for record types in the GenStudio workspace, if those permissions include GenStudio users. Prior to this improvement, when you removed these users from the GenStudio workspace in Planning, they would lose permissions to record types in GenStudio as well. 

Your organization must have both Workfront Planning and Adobe GenStudio for Performance Marketing. 

For information, see [Get started with the Adobe Workfront Planning and Aobe GenStudio for Performance Marketing integration](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).


## Removed public sharing of views on a global record type in a secondary workspace


>[!NOTE]
>
>Preview: December 3, 2025
>Production fast release: December 4, 2025
>Production for everyone: January 15, 2026


We have removed the Public sharing tab when sharing a view for a global record in a secondary workspace. You cannot share a view publicly from a global record type added to another workspace from an existing global record type. You can share a global record type view publicly from its original workspace.

For information, see [Share views](/help/quicksilver/planning/access/share-views.md).


## Connect GenStudio for Performance Marketing Brands with Workfront Planning record types

>[!NOTE]
>
>Preview: November 13, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  November 13, 2025

You can now connect Workfront Planning record types with Brands from Adobe GenStudio for Performance Marketing. Your organization must have both Workfront Planning and Adobe GenStudio for Performance Marketing.  

For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).


## New field search box in the Filters, Fields, and Row colors icons in Planning views

>[!NOTE]
>
>Preview: November 6, 2025 
>Production fast release: December 11, 2025 
>Production for everyone:  January 15, 2026 

You can now search for a specific field when building a view element in a record type view. We have added search boxes when you build a filter, sort, grouping, or when you configure your fields or row colors. Prior to this enhancement, you could simply scroll through the list of available fields.  

This improvement is available in all record type views.  

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).


## Global record types and the ability to  add them as existing record types to other workspaces

>[!NOTE]
>
>Preview: October 16, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  January 15, 2026 

 When implementing Workfront Planning for a multi-team organization with common workflows, you might need to define a cohesive structure and metadata for key record types (like Campaigns or Deliverables) that can be added to each team's workspaces to capture and manage their work.   

 Also, you might need each team's work to roll up to a central level.   

 In such a workflow, you can ensure that teams capture their work consistently while unlocking cross-team visibility, without the need to add everyone in the organization to every workspace. You can use global record types to achieve this.  

 You can now designate a record type to be global and use it cross multiple workspaces. Users can use the same field structure and connections that are already configured in a central workspace.    

For more information, see the following articles:   

* [Cross-workspace record type overview](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)  

* [Configure record type cross-workspace capabilities](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)  

* [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## New limit for connection fields for one record type

>[!NOTE]
>
>Preview: October 16, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  January 15, 2026 

We have introduced a limit of 30 connection fields for each record type.

NOTE: If your organization currently has more than 30 connection fields for one record type, you can keep the additional fields that exceed the limit of 30. However, you cannot add more connection fields to those record types that exceed the limit. Going forward, the new limit of 30 connection fields will be enforced.

For more information, see [Connected Record Types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Set user-friendly values for select-type field choices

>[!NOTE]
>
>Preview: October 16, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  January 15, 2026 

When adding  field choices to a single- or multi-select field, Workfront will now assign unique user-friendly values to each choice. Prior to this improvement, Workfront generated an alpha-numeric ID that was difficult to understand and use in API calls and other integrations.  

Consider the following with this improvement:  

* The new values will be added to new field choices. Existing field choices will keep their alpha-numeric IDs. 

* Choice values are unique for one field but can be repeated between different fields.  

* Renaming a choice does not update its original value. 

* Choice values display in lowercase and are separated by underscores in the case of multi-word choices. If you use a label already used as another choice name for the same field, Workfront adds a sequential number to the value. 

For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).






