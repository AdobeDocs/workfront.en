---
title: Adobe Maestro release activity
description: Adobe Maestro is currently available to select Workfront customers. Review this article often to learn about the features recently released for Adobe Maestro. 
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
---
# Adobe Maestro release activity 

>[!IMPORTANT]
>
>The information in this article refers to Adobe Maestro which is a new offering from Adobe Workfront. 
>
>Currently, Adobe Maestro is part of a beta program which is open to a limited number of customers. You must be a Workfront customer to use Maestro capabilities. 
>
>Contact your account representative for more information about joining the beta program for Maestro.
>
>For information, see [Adobe Maestro overview](../maestro/maestro-overview.md).

This article lists the features that have been released after the launch of the Maestro closed beta program, on May 22, 2023. 

The released features are listed in the order of their release, with the most recent first. Customers who are participating in the Maestro closed beta program can access all features in their Production environments. 

>[!IMPORTANT]
>
>Between May 2023 and December 2023, all features in this article were released to both the Preview and Production environment. The Maestro capabilities have temporarily been removed from the Preview and Sandbox environments since January 2024. All features released after this date are currently available in Production. 

This article lists the features and patches that have been released after the launch of the Maestro closed beta program, on May 22, 2023. 

The features are released weekly and are listed in the order of their release, with the most recent first. Customers who are participating in the Maestro closed beta program can access all features in their Preview and Production environments.

>[!IMPORTANT]
>
>The documentation referenced in the sections below will be available some time after the features are released to Production. 

## Week of January 15, 2024

### Maestro capabilities are removed from the Preview and Sandbox environments 

Preview and sandbox: January 11, 2024

The Maestro area and all Maestro capabilities have been temporarily removed from the Preview and Sandbox environments. Maestro will be added to these environments at a later date which we will communicate in the release activity notes.  

### Maestro permissions for workspaces and views

Production: January 11, 2024

Preview: To be determined

You can now share a workspace or a view with users and groups. You can set their permissions to different levels, depending on what information they need to view or edit. 

When you share a workspace, users have permissions to the record types, records, and fields in that space.

When you share a workspace, users don't receive sharing permissions to the views associated with the record types of the workspace. You must grant separate permissions to views. 

The following are the permissions levels for Maestro workspaces:  

* View: Users can view workspaces that are shared with them. They can also view record types, and records from the shared workspace. 

* Contribute: Users can create, edit, or delete records in the workspace that is shared with them.  They cannot create or edit record types or workspaces that are shared with them.  

* Manage: Users can create, edit, and delete workspaces, record types, records, and fields in workspaces that are shared with them.   

The following are the permissions levels for record views:

* View: Users can select the view from the View drop-down menu of a record type page.
* Manage: Users can edit, share, and delete the view. 

For more information, see [Access overview](/help/quicksilver/maestro/access/access-overview.md) and [Overview of sharing permissions in Adobe Maestro](../maestro/access/sharing-permissions-overview.md).

### New Formula field type

Production: January 11, 2024

Preview: To be determined 

You can now add a Formula-type field to a record type.  

Formula fields generate a new value using existing values from other fields in a record type and a function that indicates how the existing values should be calculated. 

You cannot use lookup fields from linked record types in a formula calculation. This functionality will be available at a later date.   

For information, see [Formula fields overview](/help/quicksilver/maestro/fields/formula-fields.md).  

### Undo/ Redo actions when managing records in the table view

Production: January 11, 2024

Preview: To be determined

You can now undo or redo your changes when performing the following actions in the table view:  

* Copy/ paste data 
* Edit record 
* Add record 
* Delete record 

You can use the following keystrokes to undo or redo actions: 

* Undo: CTRL/ CMD + Z 
* Redo: CTRL/ CMD + Shift+Z 

For more information, see the following articles:  

* [Edit records](/help/quicksilver/maestro/records/edit-records.md) 

* [Delete  records](/help/quicksilver/maestro/records/delete-records.md) 

* [Create records](/help/quicksilver/maestro/records/create-records.md) 

## Week of December 25, 2023

### Search in timeline view   

Preview and Production: December 27, 2023 

You can now search for a keyword to quickly find a record in the timeline view. You can use keywords and special characters from any fields that are visible on the screen to find a record. For information, see [Manage the timeline view](../maestro/views/manage-the-timeline-view.md). 

## Week of December 18, 2023

### Add comments on records from the Details page

Preview and Production for all customers: December 18, 2023 

>[!NOTE]
>
>The following capabilities will be available in Production with the January 2024 release: 
>
>* Search for comments 
>
>* Copy and paste images 
>
>* Drag and drop images 
>
>For more information, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

You can now collaborate with others on individual records by adding comments or replying to others while viewing a record in the Details page.   

The commenting experience for Maestro records matches the new commenting experience for Workfront objects.   

For more information, see [Manage record comments](/help/quicksilver/maestro/records/manage-record-comments.md).  

### Maestro connector (beta) for Adobe Workfront Fusion

Production: December 21, 2023

>[!IMPORTANT]
>
>Your organization must purchase Adobe Workfront Fusion to be able to build connections with Maestro.
>
>For information, see [Adobe Workfront Fusion overview](/help/quicksilver/workfront-fusion/get-started/workfront-fusion-overview.md).

Now, you can use Adobe Workfront Fusion to connect to Maestro. With the new Adobe Maestro Fusion connection, you can:  

* Create, read, update, and delete records 

* Get a list of records by record type 

* Delete or get a list of record types 

* Search records 

* Make an API call 

* Trigger a scenario when a change is made in Maestro 

For more information, see [Adobe Maestro modules](/help/quicksilver/workfront-fusion/apps-and-their-modules/maestro-modules.md).

## Week of December 11, 2023

### Update the primary field in a table view of a record type

Preview and Production: December 14, 2023 

You can now choose the field you want to display in the first column of a Maestro table view. This field is now called a primary field.  

Prior to this enhancement, the Name field of a record always displayed in the first column of the table view and it could not be placed in another position.

With this improvement, notice the following: 

* The Name column or field is still the first column of a table, by default.  

* You can choose any field of the following types to be a primary field and replace the Name field in the first column: 

    * Single-line text 

    * Number 

    * Formula

* The primary field of a table view is always frozen and cannot be moved, unless you set another field as a primary field.  

* You can change the primary field from a non-primary column header.  

* All table views of a record type have the same primary field you select. 

For more information, see [Manage table view](/help/quicksilver/maestro/views/manage-the-table-view.md).  


### Connect Maestro records with Adobe Experience Manager Assets 

Preview release: December 14, 2023 

Production release: December 21, 2023 

>[!IMPORTANT]
>
>Your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console to be able to connect Maestro records to Adobe Experience Manager Assets.
>
>If you have questions about onboarding to the Adobe Admin Console, see the [Adobe Unified Experience FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).


You can now establish a connection between Maestro record types and Adobe Experience Manager Assets.  

After you establish the connection, the following functionality is available with this update:  

* You can link Experience Manager assets and folders to a Maestro record from a specific repository in Experience Manager Assets to which they have access. You can connect asset fields to Maestro fields in this process. 

* Maestro users can view the name of the connected assets, as well as the values of the connected fields in Maestro

<!--removed per PM, for now: 
* An Experience Manager Assets record type is automatically created in Maestro after you establish the connection. Connected assets are visible in the Maestro table and timeline views of this new record type.  
-->

* You can click the asset name in the table view of the Maestro record from the connected record field, and view a pop-up window with the asset thumbnail and several key fields. From the pop-up window, you can navigate to the asset viewer in Experience Manager and view all the details about it.

For more information, see [Connect record types](/help/quicksilver/maestro/architecture/connect-record-types.md).  

## Week of December 4, 2023

### Copy and paste information from one field to another in the Maestro table view for People-type and linked record fields

Preview and Production: December 5, 2023

You can now copy and paste information from one field to another field of the same type in a Maestro record type table view. This functionality is now supported for the following types of fields: 

* People
* Linked record fields

Consider the following:  

* Copying and pasting field values from one field to another is supported for fields that display multiple values. 

* You cannot copy information from another source, other than a Maestro field of the same type as the field you paste the information in. 

* You cannot copy and paste field values for fields that display in the Details area of a record.  

For more information, see [Edit records](../maestro/records/edit-records.md). 

For information about linked fields, see [Connect record types](../maestro/architecture/connect-record-types.md). 

## Week of November 27, 2023

### Copy and paste information from one field to another in the Maestro table view

Preview and Production: November 28, 2023

You can now copy and paste information from one field to another field of the same type in a Maestro record type table view.  

Consider the following:  

* You cannot copy information from another source, other than a Maestro field of the same type as the field you paste the information in. 

* You cannot copy and paste field values for fields that display in the Details area of a record.  

* You cannot copy and paste field values for the following field types:  

    * People 

    * System fields 

    * Linked fields created as a result of connecting records  

For more information, see [Edit records](../maestro/records/edit-records.md). 

## Week of November 6, 2023

### Grouping for the table view

Preview and Production: November 7, 2023

You can now group records in the table view of a record type page. You can group by three unique fields in the Maestro interface <!--checking into this for now: and by four fields when using the API-->.  

For more information, see [Manage the table view](../maestro/views/manage-the-table-view.md). 

## Week of October 30, 2023

### New field types for user and date fields to capture who created or last modified a record or on what date 

Preview and Production: October 30, 2023

We have introduced the following field types for Maestro records:  

* Created by 

* Created date 

* Last modified by 

* Last modified date 

The field values of the fields created from these field types are read-only and capture the name of the user who created or last modified a record, or the date when the record was created or last modified. 

For more information, see [Create fields](../maestro/fields/create-fields.md).

### Navigate to Workfront objects from a Maestro record

Preview and Production: October 31, 2023

You can now open the Workfront object pages from the following areas in Maestro: 

* The read-only linked Workfront object record table view

* The read-only Workfront object record Details page 

For more information, see [Connect records](../maestro/records/connect-records.md). 

### Improved navigation in the table view

Preview and Production: November 2, 2023

We have improved the navigation in the table view of a record type page.  

The following are some of the improvements: 

* Use the tab key on your keyboard to navigate the table's columns and rows 

* Add a new record from any column position. Prior to this improvement you could add a record only from the first column. 

* Use the Shift + Enter keyboard combination to add a new record (or row) in the table.  

For more information, see [Create records](../maestro/records/connect-records.md). 

## Week of October 16, 2023

### New People field type 

Preview and Production: October 16, 2023

You can now add a People-type field to Maestro record types. You can use People-type fields to associate existing users with a record. For information, see [Create fields](../maestro/fields/create-fields.md). 

### Rich Text- format for Paragraph fields

Preview and Production: October 16, 2023

We have added Rich Text format controls for Paragraph-type fields. You can format your paragraph fields using Rich Text either in the Table view of a record type, or in the Details page of a record. For more information, see [Edit records](../maestro/records/edit-records.md). 


### Record and grouping color-coding for the Timeline view 

Preview and Production: October 19, 2023

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

Preview and Production: October 9, 2023

You can now search for a keyword to quickly find a record in the table view. You can use keywords and special characters from any fields that are visible on the screen to find a record. For information, see [Manage the table view](../maestro/views/manage-the-table-view.md). 

## Week of September 18, 2023

### Reorder rows

Preview and Production: September 20, 2023

You can now reorder one or several rows (or records) in the Table view of a record type page. For information, see [Manage the table view](../maestro/views/manage-the-table-view.md). 

## Week of September 4, 2023

### Connect Maestro records with Workfront companies and groups

Preview and Production: September 5, 2023  

You can now connect a Maestro record with Workfront companies and groups. You must first create a connection between a Maestro record type and the Workfront companies and groups object types. Then, you can connect a single Maestro record of the selected record type to individual Workfront companies and groups.  

Consider the following:  

* You must create a connection between Maestro record types and the Workfront Company and Group object types for each Workspace.  

* You cannot connect taxonomy record types with Workfront object types. 

* You can connect multiple Maestro records to the same Workfront company or group, and multiple companies or groups to the same Maestro record.  

* You cannot edit companies or groups in Maestro. All company or group changes performed in Workfront are visible in Maestro, when reviewing the Maestro linked records.  

    For more information, see the following articles:

    * [Connect record types](../maestro/architecture/connect-record-types.md)
    * [Connect records](../maestro/records/connect-records.md)

### URL support for single-line text fields 

Preview and Production: September 7, 2023 

For better visibility when working with links in the Table view, we have added support for URLs in single-line text fields. Using URLs to other websites or external drives when updating a single-line text field, now identifies them as links and allows you to click them from the table. Prior to this enhancement, links displayed as text.  

## Week of August 28, 2023

### Field visibility menu for the Table View toolbar

Preview and Production: August 31, 2023

To display the right information on a given set of records, especially if you intend to share the view with others who must see some but not all fields of a record type, you can now select which fields (or columns) to display and which to hide in the Table view.  

You can hide or show individual fields from each header of the field columns, or you can manage all fields of the record type from a setting in the table view toolbar.  

For more information, see [Manage the table view](../maestro/views/manage-the-table-view.md). 

## Week of August 21, 2023

### Connect Maestro records to programs and portfolios 

Preview and Production: August 24, 2023

You can now connect a Maestro record with Workfront programs and portfolios. You must create a connection between a Maestro record type and a program or portfolio which creates a connected field. Then, you can connect any Maestro records from all other record types within the same workspace to specific programs and portfolios which creates a read-only Workfront Program or Workfront Portfolio record type in the same workspace. Consider the following:

* Workfront connector record types are unique for each workspace. 
* You can connect multiple Maestro records to the same Workfront program or portfolio, and multiple programs and portfolios to the same Maestro record. 
* You cannot edit programs and portfolios in Maestro. All program and portfolio changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

### New sorting functionality for the table view

Preview and Production: August 24, 2023

You can now sort records in the table view of a record type page. 
The following capabilities are now available: 

* Sorting at the table-level, where you can sort by multiple fields at the same time. 
* Sorting at the column or field-level, where you can sort by an individual field at a time.

### Improvements to the timeline view: new look-and-feel for groupings and the Compact/ Standard view switch

Preview and Production: August 24, 2023

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

Preview and Production: August 10, 2023

You can now import an Excel file to create record types in a workspace. The sheets of the file become the record types, and the columns of the file become their respective fields.  

### Improved experience for connecting record types and projects 

Preview and Production: August 10, 2023

We have improved the way that you connect record types, including connecting to Workfront projects. As part of this improvement, we made the following changes when adding a field for a record type from the table view:  

* Removed the Relationship-type field from the "New field" tab.  

* Add a "New connection" tab where you can directly select the record or object type you want to connect to, eliminating the need for a Relationship-type field. 

## Week of July 10, 2023

### Update the appearance of a record type

Preview and Production: July 13, 2023

You can now select a custom icon for a record type, and a custom color for the record type icon.  

### New Checkbox field type

Preview and Production: July 13, 2023 

You can now add a Checkbox field type to Maestro record types. You can use a Checkbox-type field to add a single checkbox option to a record. You can use this field to indicate a specific attribute or status for that particular record. For example, you can use it as a flag for tracking completion, approval, or any other binary attribute for each record.  

## Week of June 26, 2023

### Quick activation of the contextual menu in a table

Preview and Production: June 28, 2023
 
We have enabled the ability to activate the contextual menu by right-clicking anywhere in a record row, when viewing the records in the table view or a record type. You can now quickly view, delete, or copy a link to the record's Details page when you access the contextual menu from anywhere in the table view of a record type. Prior to this enhancement, the contextual menu was accessible only from the More menu in the Name column of a record.  

## Week of June 19, 2023

### Record field names are unique

We have introduced a requirement now that the field names of a Maestro record type should have unique names. Fields that belong to different record types do not have to have unique names.  

## Week of June 5, 2023

### Connect Maestro records with Workfront projects

Preview and Production: June 5, 2023

You can now connect a Maestro record with Workfront projects. You must create a connector Maestro record type to establish the connection between Maestro records and Workfront projects. Then, you can connect any Maestro records from all other record types to the connector record using the Relationship field. Consider the following:

* You must have a connector record type for Workfront for each Workspace. 
* You can connect multiple Maestro records to the same Workfront project, and multiple projects to the same Maestro record. 
* You cannot edit projects in Maestro. All project changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

## Week of May 29, 2023

### Two-date requirement for creating a Timeline view

Preview and Production: May 31, 2023  

You must have at least two date fields associated with a record type to create a Timeline view.
