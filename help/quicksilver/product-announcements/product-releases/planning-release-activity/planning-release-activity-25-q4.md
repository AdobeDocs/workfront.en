---
content-type: release-notes
title: Fourth Quarter 2025 release activity for Adobe Workfront Planning
description: This is the release activity for the Adobe Workfront Planning product for the Fourth Quarter 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 4e1761f9-bf73-4355-925a-9136f2787a3f
---
# Fourth Quarter 2025 release activity for Adobe Workfront Planning

This article describes the features that are releasing for Workfront Planning during the Fourth Quarter 2025 release. 

<!--keep the sentence below for all future quarterly release pages-->

For a list of all features released for Adobe Workfront Planning, see [Adobe Workfront Planning release activity: article index](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

<!--## Unified request form list now available

>[!NOTE]
>
>* Preview: September 4, 2025
>* Production fast release: September 11, 2025
>* Production all: October 16, 2025

To make it easier to find the request form you're looking for in Workfront Planning, we've created a unified list for request forms. Now, all request forms that you have access to can be found in a single list, regardless of the object they were created for. Clicking on a form in this list brings you to the request form's page, where you can edit, preview, or publish and unpublish the form.

Previously, request forms were located only on the object for which they were created.

For more information on request forms, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md). -->

## Resize records in the calendar monthly view

>[!NOTE]
>
>* Preview: September 4, 2025
>* Production fast release: October 15, 2025
>* Production all: October 16, 2025

In the calendar view of a record type page, you can now click, drag and drop a record's left or right margins to modify its duration.

Moving a record's margins also modifies its start and end dates immediately.

An outline appears to guide you to the new location before the event is resized.

Resizing records in the calendar view is available only when displaying the view by month.

For more information, see [Edit records](/help/quicksilver/planning/records/edit-records.md).

## Create records in the calendar view

>[!NOTE]
>
>* Preview: September 4, 2025
>* Production fast release: October 15, 2025
>* Production for all customers: October 16, 2025

You can now create records in the calendar view of a record type by double-clicking anywhere on the calendar.

You can select the date range of your record or open the record's page to edit all its details.

Prior to this enhancement, to add a record from the calendar view, you could only add new records by using the New record button.

For information, see [Create records](/help/quicksilver/planning/records/create-records.md).

## Resize records in the timeline view

>[!NOTE]
>
>* Preview: September 4, 2025
>* Production fast release: October 15, 2025
>* Production for all customers: October 16, 2025

In the timeline view of a record type page, you can now click, drag and drop a record's left or right margins to modify its duration.

Moving a record's margins also modifies its start and end dates immediately.

An outline appears to guide you to the new location before the event is resized.

>[!NOTE]
>
>Resizing records in the timeline view is available when displaying the view yearly, quarterly, or monthly.


For more information, see [Edit records](/help/quicksilver/planning/records/edit-records.md).

## Control how many records display in the Calendar view

>[!NOTE]
>
>* Preview: September 4, 2025
>* Production fast release: October 15, 2025
>* Production for all customers: October 16, 2025

We have added the Row height setting in the Calendar view toolbar of a record page. You can now choose how many records display in a calendar cell by selecting one of the following options for the row height of the view:  

* Short 
* Standard 
* Medium 
* Tall 
* Fit to content 

The setting is available only when the calendar view displays by month. The setting is not available when the calendar displays by week.  

For more information, including limits for each option, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md).  


## Add new choice to select-type fields in the table view

>[!NOTE]
>
>* Preview: September 4, 2025
>* Production fast release: October 15, 2025
>* Production for all customers: October 16, 2025

You can now add a new choice to a single- or multi-select field as you update the field value in the table view. For example, when the single-select field of Status has three choices and you want to have a fourth choice, you can add it as you edit the Status field of a record in the table view.

Prior to this enhancement, you could add new choices only by editing the field.

>[!NOTE]
>
>This functionality is available only when you update field values in the table view.


For information, see [Edit records](/help/quicksilver/planning/records/edit-records.md).

## New combined Status column in unified Request list 

>[!NOTE]
>
>* Preview: August 28, 2025
>* Production fast release: September 11, 2025
>* Production for all customers: October 16, 2025

To simplify the unified request experience, the Status column now displalys both Request Status and Approval Status, whichever applies to a given request.

For more information on creating requests see:

* For Workfront: [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* For Workfront Planning: [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md)

## New limits for formula fields

>[!NOTE]
>
>* Preview: August 28, 2025
>* Production fast release: September 11, 2025
>* Production for all customers: October 16, 2025

We have placed the following limits on formula fields:

* There is a limit of 20 formula fields per record type
* There is a limit of 50,000 characters for a formula expression

For more information, see [Formula field overview](/help/quicksilver/planning/fields/formula-fields.md).

## Show error when formula values cannot be resolved

>[!NOTE]
>
>* Preview: August 28, 2025
>* Production fast release: September 11, 2025
>* Production for all customers: October 16, 2025

To indicate that there is a problem resolving a formula field, the field will now display as "#ERROR!" in one of the following cases:

* When a field used in a formula is deleted.

* When a field used in an aggregated lookup field displays as #ERROR!.

* When a formula value cannot be displayed in the selected format.

For information, see [Formula fields overview](/help/quicksilver/planning/fields/formula-fields.md).

## New expressions added to formula fields in Planning  

>[!NOTE]
>
>Preview: August 7, 2025
>Production for all customers:August, 2025
>[!BADGE Off schedule]{type=Neutral}

We have added new expressions with the following usage to formula fields in Workfront Planning and to calculated custom fields in Workfront:

* **REMOVEACCENTS(string)**: Removes diacritical marks from all accented characters in the input string.
* **REPLACEPATTERN (string, pattern, replacement string)**: Replaces the matches of the given pattern with the replacement string. 
* **PASCAL(string)**: Converts the input string to PascalCase by capitalizing the first letter of each word and removing all spaces.

For more information, see [Overview of calculated data expressions](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Adding Maximize and Minimize buttons to the formula field creation window

>[!NOTE]
>
>Preview: July 31, 2025
>Production for all customers: July 31, 2025
>[!BADGE Off schedule]{type=Neutral}

We have added a Maximize button to enlarge the Formula field when creating or editing the field in a record table view. Additionally, we added a Minimize button in the new enlarged window to revert to the field creation box.

For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).

## The Connected records page is now available in a record's preview area 

>[!NOTE]
>
>* Preview: July 31, 2025
>* Production fast release: August 14, 2025
>* Production for all customers: October 16, 2025

We have now made the experience in the connected records page in the preview box match that of the page in the full page of a record's Details area.

Prior to this enhancement, viewing connected records in a connected records page was only possible in the full page of a record's Details area.

For information, see [Manage the record page layout](/help/quicksilver/planning/records/manage-the-record-page.md).

<!--## Updates to Requesting experience 

>[!NOTE]
>
>* Preview: July 31, 2025
>* Production fast release: August 14, 2025
>* Production for all customers: October 16, 2025

To create a better user experience when making requests in Workfront and Workfront Planning, we've updated the requesting experience. Now you can:

* View Workfront and Workfront Planning requests in a single list.
* Filter submitted requests based on criteria you specify.
* Search for and select Workfront request queues and Workfront Planning forms in a consolidated experience.
* Hide and reorder columns in the submitted requests list.

This update also features changes to the look and feel of the page.

Previously, Workfront and Workfront Planning requests were on separate tabs, and filters were not customizable.

For more information on creating requests see:

* For Workfront: [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* For Workfront Planning: [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md) -->

## Create records in the timeline view

>[!NOTE]
>
>Preview: July 24, 2025
>Production fast release: August 14, 2025
>Production for all customers: October 16, 2025

You can now create records in the timeline view of a record type by double-clicking anywhere on the timeline.

You can select the date range of your record or open the record's page to edit all its details.

Prior to this enhancement, you could only add new records using the New record button or inline in the table view.

For information, see [Create records](/help/quicksilver/planning/records/create-records.md).

## Add Share option in the More menu of a record type card 

>[!NOTE]
>
>Preview: July 24, 2025
>Production fast release: August 14, 2025
>Production for all customers: October 16, 2025

You can now share a record type from the More menu of the record type card on the workspace page. Prior to this enhancement, the Share option was available only inside the record type page.

For information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md).

## Display all Workfront Planning views in full-screen mode

>[!NOTE]
>
>Preview: July 24, 2025
>Production fast release: August 14, 2025
>Production for all customers: October 16, 2025

You can now display all Workfront Planning views (table, timeline, and calendar) in full-screen mode. The view functionality is preserved and you can change the view while in full-screen, as well.

Prior to this enhancement, this functionality did not exist.

For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

## Add teams as approvers on Planning request forms

>[!NOTE]
>
>Preview: July 22, 2025 
>Production for fast release: August 14, 2025 
>Production for all customers: October 16, 2025 

To make the approval process more flexible, we've added the ability to add teams as approvers on Planning request forms. Now, you can enter and select team names when setting approvers. Any of the team members can make a decision, which counts as the approval decision for the entire team.

Previously, only individual users could be assigned as approvers. 

For more information, see [Add an approval to a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

## New fields to display record approval information

>[!NOTE]
>
>Preview: July 17, 2025 
>Production for fast release: August 14, 2025 
>Production for all customers: October 16, 2025 

We are introducing the following fields to capture approval information for records created by submitting a request with an approval: 

* Approved by 
* Approval date 

For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).

## Auto-populate fields based on applied groupings

>[!NOTE]
>
>Preview: July 10, 2025 
>Production fast release: August 14, 2025 
>Production for all customers: October 16, 2025


Now, when you have  groupings applied to a table view, adding a record to the table will auto-populate the fields associated with the groupings you add the record to.  

If you have multiple groupings applied, the system auto-populates the fields associated with all groupings only when you add the record at the end of the list inside the last grouping criteria.  

Prior to this enhancement, you had to manually update the fields associated with groupings.  

For information, see [Create records](/help/quicksilver/planning/records/create-records.md).
