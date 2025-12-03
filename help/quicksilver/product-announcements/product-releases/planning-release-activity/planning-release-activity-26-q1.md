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

<!--## Removed public sharing of views on a global record type in a secondary workspace

Preview: December 3, 2025 (****LILIT IS CHECKING ON THIS*****)
Production fast release: WAITING ON LILIT
Production for everyone: January 15, 2026

We have removed the Public sharing tab when sharing a view for a global record in a secondary workspace. You cannot share a view publicly from a global record type added to another workspace from an existing global record type. You can share a global record type view publicly from its original workspace.

For information, see [Share views](/help/quicksilver/planning/access/share-views.md).
-->

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