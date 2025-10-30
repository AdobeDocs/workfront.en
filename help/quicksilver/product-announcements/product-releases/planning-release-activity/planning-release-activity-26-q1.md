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


<!--## New field search box in the Filters, Fields, and Row colors icons in Planning views

>[!NOTE]
>
>Preview: October 30, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  January 15, 2026 


You can now search for a specific field when building a view element in record type view. The new search boxes have been added when you build a filter, sort, grouping, or when you configure your fields or row colors. Prior to this enhancement, you could simply scroll through the list of available fields.
This improvement is available in all views.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).-->


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