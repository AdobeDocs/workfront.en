---
content-type: release-notes
title: Adobe Workfront Planning Release Activity for the 25.1 Release
description: This is the release activity for the Adobe Workfront Planning product for the 2025 First Quarter.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: ef0b719c-6d2e-4d3e-9522-da6dbd71c248
---
# First Quarter 2025 release activity for Adobe Workfront Planning

<!--remove this important intro after the 25.1 release-->

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning, a new offering from Adobe Workfront. 
>
>You must purchase a Workfront Planning plan, in addition to a Workfront plan to be able to access and use Workfront Planning capabilities. 
>
>For a complete list of requirements to access Workfront Planning, see [Access overview](/help/quicksilver/planning/access/access-overview.md). 
>For an overview of Workfront Planning, see [Adobe Workfront Planning overview](/help/quicksilver/planning/general/planning-overview.md). 

This article describes the features that are releasing for Workfront Planning during the 2025 First Quarter release. 

<!--keep the sentence below for all future quarterly release pages-->
<!--remove the general activity mention after First Quarter 2025 is released-->

For a list of all features released for Adobe Workfront Planning after the general availability release on August 28, 2024, see [Adobe Workfront Planning release activity: article index](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Intelligent search when looking for a field type in Workfront Planning

>[!NOTE]
>
>Preview release: December 5, 2024; Production release for all customers: December 5, 2024

We have added intelligent search functionality when looking for a field type in Workfront Planning. You can now find field types when typing a keyword. For example, typing "Price" finds the Number and Currency field types. Prior to this enhancement, you could search only for the actual field type name.

For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).

## Custom color picker for color coded options of single- or multi-select fields

>[!NOTE]
>
>Preview release: December 5, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025)

Now, you can make custom color choices when creating or editing a single- or multi-select field. When you create or edit fields with color-coded options, clicking on the color icon opens a color picker box. You can choose from predefined colors or create custom ones using hex codes or a color spectrum.

For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).

## Import existing Workfront fields to Workfront Planning record types  

>[!NOTE]
>
>Preview release: November 27, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025)

Now, when you add fields to a record type, you have the option to import existing Workfront custom or native fields and associate them with the record type you selected. Importing existing fields creates a copy of the Workfront fields in Workfront Planning. The copied fields are independent of their original versions.   

Prior to this enhancement, you had to manually create all fields and associate them with record types.  

Calculated fields are not supported at this time.   

For information, see [Import fields from Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md) 

## Create record types, records, and fields by importing a CSV or Excel file 

>[!NOTE]
>
>Preview release: November 27, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025) 

You can now import new record types by importing a CSV or Excel file.  

The following information is imported: 

* The name of the sheet or the file is imported as the record type name.  

* The first row of every column is imported as a new field. You can have up to 500 fields in each imported sheet.

* Each row is imported as a new record. You can have up to 10,000 records in each sheet.

For more information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).  

## Avoid circular references in formulas

>[!NOTE]
>
>Preview release: November 27, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025) 

We have introduced a warning message when editing or creating a formula field that might create a circular reference to itself or shared fields. You cannot save a formula field that either refers to itself or to items that are referenced in its calculation.  

For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).  

## Add Connection view pages to a record's page to display connected records in a table view

>[!NOTE]
>
>Preview release: November 27, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025) 

You can add pages to a record's details area to display connected records in a table view. You can add one page per connected record.  

The added pages are read-only. 

For information, see [Manage the record page layout](/help/quicksilver/planning/records/manage-the-record-page.md).  

## New Workfront and Planning tabs in the Submitted section of the Requests area

>[!NOTE]
>
>Preview release: November 27, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025) 

You can now find Workfront Planning requests in the Submitted section of the Requests area of Workfront. The Submitted section now displays the following tabs: 

* Workfront: Displays requests submitted in Workfront.
* Planning: Displays requests submitted using a Workfront Planning request form. 

You must use a link to the request form to be able to add requests to a Workfront Planning record type. Submitting a Workfront Planning request from Workfront's Requests area will be available at a later date.  

Your organization must purchase a Workfront Planning package before the Planning tab is available to you in the Requests area.  

For information, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md).   

## Additional field types are now supported in request forms

>[!NOTE]
>
>Preview release: November 27, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025) 

You can now add the following field types to a record type request form in Workfront Planning: 

* People 
* Workfront connections   

Prior to this enhancement, these types of fields could not be added to request forms in Workfront Planning. 

For information, see Create and manage a request form in Adobe Workfront Planning (/help/quicksilver/planning/requests/create-request-form.md). 

## Limit public sharing of request forms that contain certain field types

>[!NOTE]
>
>Preview release: November 27, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025)

You can no longer share a request form publicly if the form contains any of the following field types: 

* Formula 
* Workfront and AEM Assets connections
* Lookup fields 
* People 

 For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md). 


## Display records in the calendar view by week 

>[!NOTE]
>
>Preview release: November 26, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025)

You can now display records in the calendar view by week. Prior to this enhancement, you could display the calendar view only by month.  

 For information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

## Restore deleted records

>[!NOTE]
>
>Preview release: November 22, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025)

After records are deleted, they are now temporarily moved to a Recently deleted bin for 30 days. You can access the Recently deleted bin from the record type's page and it contains only records of a specific type. 

Workspace managers can restore records from the trash bin for up to 30 days after they were deleted. Connected records and their field information is also restored. 

Prior to this enhancement, deleted records could not be restored.

For more information, see [Restore deleted records](/help/quicksilver/planning/records/records-information.md).  

## Adobe AI Assistant available in the record details areas

>[!NOTE]
>
>Preview release: November 21, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025)

To make it easier for you to accomplish work, we've added the Adobe AI Assistant to a record's details preview or record's page. You can use the AI Assistant inside of a record page to update information about the record.

For information, see [Adobe Workfront Planning AI Assistant overview](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

## New experience when adding a thumbnail and a cover image to a record page

>[!NOTE]
>
>Preview release: November 20, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025)

When you open a record's preview or page and the record does not have a thumbnail or a cover image, you must now hover over the area above the record name in the header to see the options for adding a cover and a thumbnail image to the record. Prior to this enhancement, the empty placeholder images for the thumbnail and the cover displayed above the record name.

For more information, see the following articles:

* [Add a cover image to a record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
* [Add a thumbnail image to a record](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

## New display types for percentage-type fields in the table view

>[!NOTE]
>
>Preview release: November 7, 2024; Production for fast release: With the 24.12 release (December 12, 2024); Production for quarterly release: With the 25.1 release (January 2025)

To make numbers easier to read in the table view, you can now select from the following choices to change the how a Percentage-type field displays in the table view:

* Number
* Bar
* Circle

This display type is supported only in the table view.

Prior to this enhancement, you could display percentage values only as numbers.

For more information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).

## Connection fields are now supported in request forms 

>[!NOTE]
>
>Preview release: October 31, 2024; Production for fast release: With the 24.11 release (November 14, 2024); Production for quarterly release: With the 25.1 release (January 2025)

You can now add connected fields for Workfront Planning records to a record type request form. 

You cannot add connection look up fields, or connected fields for Workfront objects in the request form. 

Prior to this enhancement, these types of fields could not be added to request forms in Workfront Planning.  

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Connection warning when connecting records that are already linked to other records 

>[!NOTE]
>
>Preview release: October 31, 2024; Production for fast release: With the 24.11 release (November 14, 2024); Production for quarterly release: With the 25.1 release (January 2025)

When you try to connect records which are already connected elsewhere and which belong to a record type connected through a One to many or One to one connection type, you now receive a warning that the records are already connected. If you confirm that you want to move forward with your connection, the selected records are removed from the original record and added to the record you're currently editing.

For information about connection types, see [Connected record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## New information icon with the description of fields in the record's details page 

>[!NOTE]
>
>Preview release: October 30, 2024; Production for fast release: With the 24.11 release (November 14, 2024); Production for quarterly release: With the 25.1 release (January 2025)

We added an information icon to the right of the field names in a record page. Clicking the information icon displays the description of the field, when a description exists. Prior to this enhancement, the description of the field displayed when you hovered over the field name.

For information, see [Edit records](/help/quicksilver/planning/records/edit-records.md).

## New Workfront field type for Planning connections 

>[!NOTE]
>
>Preview release: October 24, 2024; Production for fast release: With the 24.11 release (November 14, 2024); Production for quarterly release: With the 25.1 release (January 2025)

To continue bridging Workfront objects to Workfront Planning records, we added a new field type in Workfront custom forms called Planning connection. By adding this field type on a Workfront custom form, and ultimately on a Workfront object, you can now do the following: 

* Display records connected to a Workfront object in the custom form.  

* Connect and disconnect Workfront Planning records form a Workfront object. 

You can add the new field to forms for all object types. However, you can edit the information in the field only from forms attached to the following Workfront objects that can be connected from Workfront Planning record types: Portfolio, Program, Project, Company, Group.  

Editing the Planning connection fields for Workfront objects in bulk is not yet available.  

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3435633/){target=_blank}
