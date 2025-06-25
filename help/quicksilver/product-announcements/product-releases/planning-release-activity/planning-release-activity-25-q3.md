---
content-type: release-notes
title: Third Quarter 2025 release activity for Adobe Workfront Planning
description: This is the release activity for the Adobe Workfront Planning product for the Third Quarter 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 6761f5af-2501-4487-8114-2751f1e4fe69
---
# Third Quarter 2025 release activity for Adobe Workfront Planning

This article describes the features that are releasing for Workfront Planning during the Third Quarter 2025 release. 

<!--keep the sentence below for all future quarterly release pages-->

For a list of all features released for Adobe Workfront Planning, see [Adobe Workfront Planning release activity: article index](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


## Expand and collapse all groupings in the table view

>[!NOTE]
>
>* Preview: June 26, 2025 
>* Production for everyone: July 17, 2025 

You can now collapse and expand the groupings in a table view using the following areas: 

* The Grouping box, accessible from the toolbar of the table view 

* A grouping's header, by right-clicking it 

You can collapse or expand either one grouping or all groupings at the same time. 

Prior to this enhancement, you could only collapse or expand one grouping at a time, from each grouping header. 

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## New aggregating functionality for formula fields

>[!NOTE]
>
>* Preview: June 26, 2025
>* Production for everyone: July 17, 2025 

Now, when you connect record types and bring in a formula field as a lookup, you can apply the aggregate functions (SUM, AVERAGE, MIN, MAX, etc) depending on the formula field's format. For example, if the formula field is numeric, you can use functions like SUM or AVG; if the formula field is formatted as text, aggregate functions like SUM will not apply.  

Previously, when connecting record types and bringing in lookup fields from the connected records, you could apply aggregate functions only to regular fields, but not to formula fields. 

For information, see [Formula field overview](/help/quicksilver/planning/fields/formula-fields.md). 

## Custom quarters availability for the Workfront Planning timeline view 

>[!NOTE]
>
>* Preview: June 12, 2025
>* Production fast release: July 17, 2025 
>* Production for all customers:  July 17, 2025

With this update, when you configure custom quarters in the Project Preferences area of Setup, the custom quarters are available for the Timeline view in Workfront Planning.  

Prior to this update, the custom quarters were only available for Workfront's reporting capabilities.  

With this improvement, customers who have purchased Workfront Planning will view an updated experience for defining custom quarters. This update includes the following improvements:  

Gaps and overlaps between the quarters are no longer accepted.  

You can set up to 100 custom quarters. Prior to this update you could set up only 8 custom quarters 

There are no changes in the custom quarter experience for customers who have not purchased Workfront Planning.  

For more information, see [Enable custom quarters for projects](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md). 

## Calculate all dependent formulas at the same time 

>[!NOTE]
>
>* Preview: June 12, 2025
>* Production fast release: June 12, 2025 
>* Production for all customers:  June 12, 2025

We have introduced an improvement that updates all formula fields dependent upon each other at the same time after a referenced field is updated manually. Formula fields that are 2, 3, or 4 fields away from the field whose value is manually changed and that reference each other will now automatically update at the same time.  

Prior to this improvement, only the directly dependent formula fields were updated when the value of a references field was manually updated.  

For information, see [Formula fields overview](/help/quicksilver/planning/fields/formula-fields.md).

## New expressions added to formula fields 

>[!NOTE]
>
>* Preview: June 6, 2025
>* Production fast release: June 6, 2025 
>* Production for all customers:  June 6, 2025

We have added the following expressions to formula fields: 
 
* ARRAYCONTAINS  

* SORTASCARRAY  

* SORTDESCARRAY  

Prior to this enhancement, these expressions were supported only in Workfront calculated custom fields.  

For information, see [Formula fields overview](/help/quicksilver/planning/fields/formula-fields.md).

## Filters, columns and additional fields added to the Planning tab in the Requests area 

>[!NOTE]
>
>* Preview: May 29, 2025
>* Production fast release: June 12, 2025 
>* Production for all customers:  July 17, 2025

We have added the following functionality to a list of requests in the Planning tab of the Requests area: 

* Entered by column to indicate the person who added a request
* Filters to limit the number of requests you view on the Planning tab. You can filter the list by the following items:

    * the Workspace the request form originated from
    * the record type associated with the request form
    * the Entry Date of the request
    * the name of the request form 
    * the Status of the requests
    * the name of the person who entered the request. 

* Columns control to view or hide fields (or columns) in the Planning requests list. 

For information, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md).

## New experience when breaking down records in Compact mode in the timeline view 

>[!NOTE]
>
>* Preview: May 22, 2025
>* Production fast release: June 12, 2025 
>* Production for all customers:  July 17, 2025

We have changed the experience when breaking down records in the timeline view and you have the Compact view applied. 
With the new update, when you define your breakdown objects while you display the timeline in the Compact mode,  you are prompted to switch the view to Standard after you finish configuring the breakdown conditions. 

Prior to this enhancement, defining the breakdown conditions was not possible when displaying the timeline view in Compact mode. 

With this upgrade, the Standard option is the default choice. Prior to this, the Compact mode was the default.

For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Update the timeline view settings to define the look and feel of the connected records' bars when using the Breakdown option 

>[!NOTE]
>
>* Preview: May 15, 2025
>* Production fast release: June 12, 2025 
>* Production for all customers:  July 17, 2025

You can now format the look and feel of the record bars in the timeline view for the records in the breakdown. You can update the following settings for the bars of these records: 

* Bar style  
* Color 

Prior to this enhancement, you could only format the bars of the main records as they display in the timeline view, and you could not format the bars of the connected records.  
 
For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).  

## Export the table view to a CSV or Excel file 

>[!NOTE]
>
>* Preview: May 15, 2025
>* Production fast release: June 12, 2025 
>* Production for all customers:  July 17, 2025

We have added a new capability to Workfront Planning where you can export information visible in the table view to a CSV or an Excel file.  

Consider the following when exporting information from the table view:  

* The information exported takes into account the filters, groupings, and sorts applied to the table view in Workfront Planning.
* Thumbnails and custom row colors are not supported in the exported file.  
* Only fields made visible in the Workfront interface are exported. Hidden fields are not exported.  

For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 

## Workfront Planning connected fields are now supported when importing records using a CSV or Excel file

>[!NOTE]
>
>* Preview: May 15, 2025
>* Production fast release: June 12, 2025 
>* Production for all customers:  July 17, 2025

You can now populate the values of connected fields when you add records to a record type using a CSV or Excel file.  Only connected Planning record fields are supported. Fields displaying connections to other applications are not supported. 

This change is supported when importing a CSV and Excel file to create both a record type and records for an existing record type. 

Prior to this enhancement, connection fields could not be populated when you imported records.  

For information, see the following articles:  

* [Create records by importing information from a CSV or Excel file](/help/quicksilver/planning/records/import-file-to-create-records.md).  

* [Create record types by importing information from a CSV or Excel file](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

## Inline editing in the Connected records page of a record

>[!NOTE]
>
>* Preview: April 30, 2025
>* Production fast release: May 15, 2025 
>* Production for all customers:  July 17, 2025

You can now edit records in the Connected records page of a record. With this update, we have introduced the following:   

* The name of the page has been changed from "Connection view" to "Connected records page".  
* Connected records displayed in this page are inline editable in the table view. Connected Workfront objects continue to display in a read-only table.  

Prior to this enhancement, the table of the Connection view page was read-only for record connections.  

For information, see [Manage the record page layout](/help/quicksilver/planning/records/manage-the-record-page.md).

## Planning area visible by default in the Main Menu for Standard-license  users 

>[!NOTE]
>
>* Preview: April 30, 2025
>* Production fast release: May 15, 2025 
>* Production for all customers:  July 17, 2025

Standard and System Administrator users can now find the Planning area in the Main Menu by default, without being assigned to a layout template that includes it. All other users must have a layout template that includes the Planning area assigned to them in order to access it.   

Prior to this enhancement, users with all license levels had to be assigned to layout template modified to include the Planning area in the Main Menu in order to access this area.   
 
>[!NOTE]
>
>This change will be visible for all new and existing users with a System Administrator and Standard license. 
>Existing users assigned to a layout template will continue to see everything according to the settings defined in the layout template.  

For information, see [Adobe Workfront Planning overview](/help/quicksilver/planning/access/access-overview.md).

## Row-level color formatting in the table view 

>[!NOTE]
>
>* Preview: April 30, 2025
>* Production fast release: May 15, 2025 
>* Production for all customers:  July 17, 2025

For better visibility of the important information of your records, we have introduced row-level color formatting for the table view. You can now choose a color for each row after you define conditions for each choice.  This is a new capability that did not exist before this update. 

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## New setting to truncate long record names in the Standard timeline view 

>[!NOTE]
>
>* Preview: April 23, 2025
>* Production fast release: May 15, 2025 
>* Production for all customers:  July 17, 2025

You can now enable a setting in the Bar style tab of the Settings box of a timeline view to truncate longer record names, when displaying them in the Standard view. The setting is disabled by default and can be enabled only when you display the timeline view in the Standard mode. As this setting is disabled, information on the record bars displays expanded, by default. Prior to this enhancement, information on the record bars was truncated by default.   

For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Sharing permissions for record types
 

>[!NOTE]
>
>* Preview: April 17, 2025
>* Production fast release: July 17, 2025
>* Production for all customers: July 17, 2025

To better control who can view or manage records in each record type and ensure that only authorized people can manage each record type's information based on their roles and responsibilities, we have introduced permissions at the record type level. 

Prior to this enhancement, you could share only workspaces with others and the permission they were granted to a workspace applied to all the record types in the workspace.  

We have introduced the following updates:  

* Workspace permissions are automatically shared with all record types in the workspace. 
* The level of permissions granted for the workspace displays as Inherited permissions for the record type.  
* You cannot share a record type with a higher permission level than users have on the workspace.
* You can disable the inherited permissions on the record type to make it read-only for all people in the workspace. After that,  you can add individual people, teams, groups, companies or roles and grant them Contribute permission to the record type.  

For more information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md).


