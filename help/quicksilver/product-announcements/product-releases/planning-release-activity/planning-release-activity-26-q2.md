---
content-type: release-notes
title: Second Quarter 2026 release activity for Adobe Workfront Planning
description: This is the release activity for the Adobe Workfront Planning product for the Second Quarter 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 79d4ad4a-1dd0-431e-92cd-582b5a1b7ec8
---
# Second Quarter 2026 release activity for Adobe Workfront Planning

This article describes the features that are releasing for Workfront Planning during the Second Quarter 2026 release.

<!--keep the sentence below for all future quarterly release pages-->

For a list of all features released for Adobe Workfront Planning, see [Adobe Workfront Planning release activity: article index](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

<!--

## Trigger-based automation

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

You can now automatically create Planning records or Workfront objects based on a record field change using Planning automations.  

Prior to this enhancement, you could automatically create Planning records or Workfront objects only when you clicked a preconfigured button.  

For information, see [Configure Adobe Workfront Planning automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

-->

## Only system administrators can share workspaces system-wide 

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

We are now allowing only System Administrators to choose between the following options when sharing a workspace:

* Everyone in the system can view 
* Only invited people can access 

By default, workspaces are set to the "Only invited people can access" permission. 

Prior to this change, the ability to choose these workspace sharing permissions did not exit. 

For information, see Share workspaces (help/quicksilver/planning/access/share-workspaces.md).

## Sort groupings in the timeline view  

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

You can now sort groupings in the timeline view. For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Support user references for connected fields  

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

You can now connect Workfront user fields to Workfront Planning record types by adding a new connection between a Workfront object and a Workfront Planning record type.  

For example, you can now add Project Sponsor or Portfolio Owner as a lookup field in Workfront Planning, when adding a connection to projects or portfolios. 

For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).


## Real time presence indicators now display users in the table view 

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

You can now view the users updating record fields at the same time as you by clicking the real-time presence indicator in the upper-right corner of a cell in the table view. Users listed in the upper-right corner of the record table view are those who have the same view open. 

You must turn on the Show collaborators setting in the table view header. Other users may update fields either in the table view or the Details area of a record.  

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).


## Updated sharing experience for list views 

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

When you share the list view in the projects connected records page of a record with View permissions, the user you share the view with can modify the view elements and those changes are saved to the user's personal preferences. They now have the option to save a copy of the view that includes their changes or to reset the shared view to its original settings. They can further share the copied view with others.  

This update is available only in the list view, for the connected records page of a record when displaying projects.  

For more information, see [Manage the list view](/help/quicksilver/planning/views/manage-the-list-view.md).

## Apply conditional formatting to the list view 

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

You can now apply conditional formatting to projects in a list view in the Connected records page of a record. This functionality did not exist in the list view before this enhancement.  

For more information, see [Manage list view](/help/quicksilver/planning/views/manage-the-list-view.md).

## Improvements to global record types in secondary workspaces 

>[!NOTE]
>
>Preview: February 5, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

We have improved visibility for the global record types added to a secondary workspace from a primary workspace. The improvements include the following:  

* A slightly modified global icon that indicates that the record type was added from another workspace.  

* An improved tooltip on the new icon that clearly identifies the workspace where the record type was created.  

For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

## Configure fields displayed in a record's Details preview box 

>[!NOTE]
>
>Preview: January 29, 2026
>Production fast release: February 12, 2026
>Production for everyone: April 16, 2026

We have introduced a setting that allows you to show or hide record fields in a record's Details preview box, based on the fields displayed in the table view.  

With this new setting, you can choose whether to include or exclude fields that are hidden in the table view from the record's Details preview area. 

For information, see [Manage the record page layout](/help/quicksilver/planning/records/manage-the-record-page.md).

## New Planning connection field for Original request  

>[!NOTE]
>
>Preview: January 29, 2026
>Production fast release: February 12, 2026
>Production for everyone: April 16, 2026

You can now add the "Original request" connection field to a record type. When a record is created by submitting a Planning request form, the name of the original request populates the Original request connected field.  

Prior to this enhancement, the you could view and access the original request that created the record only from the Requests area.  

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

## Create approval rules for requests in Workfront Planning 

>[!NOTE]
>
>Preview: January 29, 2026
>Production fast release: February 12, 2026
>Production for everyone: April 16, 2026

To make request approvals more dynamic and flexible, we've added the ability to create approval rules. These rules allow requests to be routed to different approvers based on field values in the request. 

For example, if a request form has the field "Campaign type," a rule can be created that sends the request to one person when the field has the value "Digital", and a different person when it has the value "Print."

Approval rules are created on the request form.

For information and instructions, see [Add approval rules to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md#add-approval-rules-to-a-request-form) in the article Add an approval to a request form in Adobe Workfront Planning.

## Display emails in user typeahead fields in Workfront Planning 

>[!NOTE]
>
>Preview: January 22, 2026
>Production fast release: February 12, 2026
>Production for everyone: April 16, 2026

A user's email now displays when you add the user to the following areas: 

* People-type Planning fields
* In the Share box when sharing Planning objects

Prior to this enhancement, only the user's Primary Role displayed in addition to the user's name when adding them to these areas. 
For more information, see the following articles: 

* [Create fields](/help/quicksilver/planning/fields/create-fields.md)
* [Share workspaces](/help/quicksilver/planning/access/share-workspaces.md)

## People fields are enabled as lookup fields for Planning connections 

>[!NOTE]
>
>Preview: January 14, 2026 
>Production fast release: February 12, 2026 
>Production for everyone: April 16, 2026 

You can now add People fields to lookup fields when connecting two Planning record types.  

For information, see [Connect Record Types](/help/quicksilver/planning/architecture/connect-record-types.md).
