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

Users inherit record permissions from the workspace and record type by default. To give only select users with record type permissions Manage permissions to only certain records, you can disable inherited permissions on select records and grant only those users Manage access to those records. You can adjust permissions for one record, or for multiple records at the same time, in bulk.

You can give users the following permissions levels: 

* View 
* Manage 

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
