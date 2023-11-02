---
title: Adobe Maestro release activity
description: Use Maestro to create custom objects, fields, and workspaces.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
---
# Adobe Maestro release activity 

>[!IMPORTANT]
>
>The information in this article refers to Adobe Maestro which is a new offering from Adobe. 
>
>Currently, Adobe Maestro is part of a beta program which is open to a limited number of customers. 
>
>Contact your account representative for more information about joining the beta program for Maestro.
>
>For information, see [Adobe Maestro overview](../maestro/maestro-overview.md).

This article lists the features that have been released after the launch of the Maestro closed beta program, on May 22, 2023. 

The released features are listed in the order of their release, with the most recent first. Customers who are participating in the Maestro closed beta program can access all features in their Preview and Production environments. 

>[!IMPORTANT]
>
>The documentation referenced in the sections below will be available some time after the features are released to Production. 

This section lists the features and patches that have been released after the launch of the Maestro closed beta program, on May 22, 2023. 

The features are released weekly and are listed in the order of their release, with the most recent first. Customers who are participating in the Maestro closed beta program can access all features in their Preview and Production environments.

## Week of October 30, 2023

### New field types for user and date fields to capture who created or last modified a record or on what date 

Preview and production: October 30, 2023

We have introduced the following field types for Maestro records:  

* Created by 

* Created date 

* Last modified by 

* Last modified date 

The field values of the fields created from these field types are read-only and capture the name of the user who created or last modified a record, or the date when the record was created or last modified. 

For more information, see [Create fields](../maestro/architecture-and-fields/create-fields.md).

### Navigate to Workfront objects from a Maestro record

Preview and production: October 31, 2023

You can now open the Workfront object pages from the following areas in Maestro: 

* The read-only linked Workfront object record table view

* The read-only Workfront object record Details page 

For more information, see [Connect records](../maestro/records/connect-records.md). 

### Improved navigation in the table view

Preview and production: November 2, 2023

We have improved the navigation in the table view of a record type page.  

The following are some of the improvements: 

* Use the tab key on your keyboard to navigate the table's columns and rows 

* Add a new record from any column position. Prior to this improvement you could add a record only from the first column. 

* Use the Shift + Enter keyboard combination to add a new record (or row) in the table.  

For more information, see [Create records](../maestro/records/connect-records.md). 

## Week of October 16, 2023

### New People field type 

Preview and production: October 16, 2023

You can now add a People-type field to Maestro record types. You can use People-type fields to associate existing users with a record. For information, see [Create fields](../maestro/architecture-and-fields/create-fields.md). 


### Rich Text- format for Paragraph fields

Preview and production: October 16, 2023

We have added Rich Text format controls for Paragraph-type fields. You can format your paragraph fields using Rich Text either in the Table view of a record type, or in the Details page of a record. For more information, see [Edit records](../maestro/records/edit-records.md). 


### Record and grouping color-coding for the Timeline view 

Preview and production: October 19, 2023

You can now color-code the record bars and the groupings in the Timeline view.  

The following are options for the colors you can choose to display for record bars and groupings in the Timeline view: 

* Groupings can match the following colors:  

    * Gray (the default) 

    * The color of the field that you group by 

* Bars can match the following colors: 

    * The color of the record type 

    * The color of a field that you select 

    * The color of the grouping 

    * No color (the default) 

When matching colors to a certain field, you can select only fields with color-coded options.  

For more information, see [Manage the timeline view](../maestro/views/manage-the-timeline-view.md). 

## Week of October 9, 2023

### Search in table view  

Preview and production: October 9, 2023

You can now search for a keyword to quickly find a record in the table view. You can use keywords and special characters in any fields that are visible on the screen to find a record. For information, see [Manage the table view](../maestro/views/manage-the-table-view.md). 

## Week of September 18, 2023

### Reorder rows

Preview and production: September 20, 2023

You can now reorder one or several rows (or records) in the Table view of a record type page. For information, see [Manage the table view](../maestro/views/manage-the-table-view.md). 

## Week of September 4, 2023

### Connect Maestro records with Workfront companies and groups

Preview and production: September 5, 2023  

You can now connect a Maestro record with Workfront companies and groups. You must first create a connection between a Maestro record type and the Workfront companies and groups object types. Then, you can connect a single Maestro record of the selected record type to individual Workfront companies and groups.  

Consider the following:  

* You must create a connection between Maestro record types and the Workfront Company and Group object types for each Workspace.  

* You cannot connect taxonomy record types with Workfront object types. 

* You can connect multiple Maestro records to the same Workfront company or group, and multiple companies or groups to the same Maestro record.  

* You cannot edit companies or groups in Maestro. All company or group changes performed in Workfront are visible in Maestro, when reviewing the Maestro linked records.  

    For more information, see the following articles:

    * [Connect record types](../maestro/architecture-and-fields/connect-record-types.md)
    * [Connect records](../maestro/records/connect-records.md)

### URL support for single-line text fields 

Preview and production: September 7, 2023 

For better visibility when working with links in the Table view, we have added support for URLs in single-line text fields. Using URLs to other websites or external drives when updating a single-line text field, now identifies them as links and allows you to click them from the table. Prior to this enhancement, links displayed as text.  

## Week of August 28, 2023

### Field visibility menu for the Table View toolbar

Preview and production: August 31, 2023

To display the right information on a given set of records, especially if you intend to share the view with others who must see some but not all fields of a record type, you can now select which fields (or columns) to display and which to hide in the Table view.  

You can hide or show individual fields from each header of the field columns, or you can manage all fields of the record type from a setting in the table view toolbar.  

For more information, see [Manage the table view](../maestro/views/manage-the-table-view.md). 

## Week of August 21, 2023

### Connect Maestro records to programs and portfolios 

Preview and production: August 24, 2023

You can now connect a Maestro record with Workfront programs and portfolios. You must create a connection between a Maestro record type and a program or portfolio which creates a connected field. Then, you can connect any Maestro records from all other record types within the same workspace to specific programs and portfolios which creates a read-only Workfront Program or Workfront Portfolio record type in the same workspace. Consider the following:

* Workfront connector record types are unique for each workspace. 
* You can connect multiple Maestro records to the same Workfront program or portfolio, and multiple programs and portfolios to the same Maestro record. 
* You cannot edit programs and portfolios in Maestro. All program and portfolio changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

### New sorting functionality for the table view

Preview and production: August 24, 2023

You can now sort records in the table view of a record type page. 
The following capabilities are now available: 

* Sorting at the table-level, where you can sort by multiple fields at the same time. 
* Sorting at the column or field-level, where you can sort by an individual field at a time.

### Improvements to the timeline view: new look-and-feel for groupings and the Compact/ Standard view switch

Preview and production: August 24, 2023

We have introduced the following improvements to the timeline view: 

* You can now display the timeline view in the following modes:

    * Standard: Displays records in separate lines.
    * Compact: Display the records whose dates don't intersect on the same line. 

* We have changed the look-and-feel of the grouping lines in the timeline view to display above the timeline of the records they contain. Prior to this improvement, the grouping lines displayed across the entire length of the timeline.

## Week of August 14, 2023

### Reorder columns in the table view

You can now reorder columns in the Maestro table view. Consider the following when reordering columns: 

* The Name field is always the first field in the table view of a record type page 

* You cannot move the Name field to another position 

* The Name field is frozen and is not part of the horizontal scroll. 

### Horizontal scroll for timeline view

You can now scroll horizontally in the timeline view of a record type. 

## Week of August 7, 2023

### Import record types from an Excel file 

Preview and production: August 10, 2023

You can now import an Excel file to create record types in a workspace. The sheets of the file become the record types, and the columns of the file become their respective fields.  

### Improved experience for connecting record types and projects 

Preview and production: August 10, 2023

We have improved the way that you connect record types, including connecting to Workfront projects. As part of this improvement, we made the following changes when adding a field for a record type from the table view:  

* Removed the Relationship-type field from the "New field" tab.  

* Add a "New connection" tab where you can directly select the record or object type you want to connect to, eliminating the need for a Relationship-type field. 

## Week of July 10, 2023

### Update the appearance of a record type

Preview and production: July 13, 2023

You can now select a custom icon for a record type, and a custom color for the record type icon.  

### New Checkbox field type

Preview and production: July 13, 2023 

You can now add a Checkbox field type to Maestro record types. You can use a Checkbox-type field to add a single checkbox option to a record. You can use this field to indicate a specific attribute or status for that particular record. For example, you can use it as a flag for tracking completion, approval, or any other binary attribute for each record.  

## Week of June 26, 2023

### Quick activation of the contextual menu in a table

Preview and production: June 28, 2023
 
We have enabled the ability to activate the contextual menu by right-clicking anywhere in a record row, when viewing the records in the table view or a record type. You can now quickly view, delete, or copy a link to the record's Details page when you access the contextual menu from anywhere in the table view of a record type. Prior to this enhancement, the contextual menu was accessible only from the More menu in the Name column of a record.  

## Week of June 19, 2023

### Record field names are unique

We have introduced a requirement now that the field names of a Maestro record type should have unique names. Fields that belong to different record types do not have to have unique names.  

## Week of June 5, 2023

### Connect Maestro records with Workfront projects

Preview and production: June 5, 2023

You can now connect a Maestro record with Workfront projects. You must create a connector Maestro record type to establish the connection between Maestro records and Workfront projects. Then, you can connect any Maestro records from all other record types to the connector record using the Relationship field. Consider the following:

* You must have a connector record type for Workfront for each Workspace. 
* You can connect multiple Maestro records to the same Workfront project, and multiple projects to the same Maestro record. 
* You cannot edit projects in Maestro. All project changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

## Week of May 29, 2023

### Two-date requirement for creating a Timeline view

Preview and production: May 31, 2023  

You must have at least two date fields associated with a record type to create a Timeline view.
