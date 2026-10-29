---
content-type: release-notes
title: First Quarter 2027 release activity for Adobe Workfront Planning
description: This is the release activity for the Adobe Workfront Planning product for the First Quarter 2027.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
---
# First Quarter 2027 release activity for Adobe Workfront Planning

This article describes the features that are releasing for Workfront Planning during the First Quarter 2027 release.

For a list of all features released for Adobe Workfront Planning, see [Adobe Workfront Planning release activity: article index](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Better visibility of quick search findings in the table view

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

When you use quick search in the table view to find an item, the view eliminates all records that don't match the search and displays only the items that match.

Prior to this enhancement, all records were displayed with the ones that match the search results highlighted.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

<!--

## Record-level permissions - restricted access to records

PLACEHOLDER: The release note field on the Workfront task points to an anchor story that no longer exists, so there is no description yet. Add the description and help link before unhiding.

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

-->

## Allow connecting records of connected global record types in secondary workspaces when cross-workspace connectivity is off

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

When two connected global record types are added to a secondary workspace, you can now turn off cross-workspace connectivity and still link records locally. Each secondary workspace sees only its own records for both record types and can connect them to each other. Records from the global workspace and other secondary workspaces are no longer shown.

Prior to this enhancement, if cross-workspace connectivity was turned off for connected global record types, secondary workspaces couldn't link their own records to each other. If it was turned on, users could see and link records from the global workspace and all other secondary workspaces.

For more information, see [Cross-workspace record type overview](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

## See the total record count in table views

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

The table view now shows the total number of records, and the count updates automatically as you apply filters, search, or change the view. The record count always reflects your full filtered results and respects your permissions.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

<!--

## Field aggregators available for groupings in the table view

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Grouped records in the table views now show a summary row for each grouping, plus a grand total for the full table. Groupings and the grand total use the same summary functions, and nested groupings get their own summaries that include all child records. Aggregators update automatically as you filter, search, regroup, or edit records.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## Add sections to organize Planning views

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now create sections in the Workfront Planning View dropdown menu to organize related views as your list grows. You can name each section when you create it, then move views from My Views and Shared with Me into your custom sections. System views stay fixed in the System section.

For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

-->

<!--

## Filters for Workfront objects connected record fields

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now filter for certain Workfront object types that meet a filter criteria when you add them as a connected field in Planning.

Only those Workfront objects that meet your filtering criteria will display as options in connected fields when editing a record.

For this feature, we added a new Record filtering rules option in the New connection tab when connecting the following Workfront object types: projects, portfolios, programs, groups, companies. Prior to this enhancement, filters were available only when connecting two record types.

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

-->

## Lookup field number limitations

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

We are introducing limits on how many lookup fields you can add to a record type:

* Up to 40 lookup fields per record type
* Up to 5 long-text lookup fields per record type. Connected lookup fields count against the limit of their original field.
* Up to 50,000 characters in the value of a single long-text lookup cell. If the combined content of the lookup values exceeds this, values are shown in connection order until the limit is reached. The first value that would exceed it, and all values after it, are omitted. The original connected object field is never changed.

You receive an error when you try to create or edit a lookup field beyond the first two limits. Record types that already exceed these limits are not affected with this change. You can edit them, but you cannot add more lookup fields or values until you are under the limit.

For information, see [Adobe Workfront Planning object limitations overview](/help/quicksilver/planning/general/limitations-overview.md).

## New fields now appear only in the view where you create them

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

When you add a new field to a record type, it is now shown only in the view you're working in and hidden in all other existing views. Other views stay as configured, and you can unhide the new field in them, if needed.

Prior to this enhancement, new fields were added unhidden to every view, sometimes causing confusion for users unfamiliar with the new fields.

For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).

## Export record details from any view

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now export a record's details from any detail view, without having to switch to the All fields view.

Previously, the export option was available only when the All fields view was selected.

For information, see [Export a record's details](/help/quicksilver/planning/records/export-the-record-page.md).

<!--

## Cancel and revert changes when editing records when business rules are violated

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

To ensure data integrity, when a business rule is violated while you edit a record, the change is blocked, the value reverts, and a toast notification explains why the edit is not allowed. The warning is visible in all areas where you are editing records, including the table view or details page.

If multiple rules are violated, each violation issues its own toast notification.

For more information, see [Configure business rules](/help/quicksilver/planning/architecture/configure-business-rules.md).

-->

## Improved performance with incremental data loading in the table and timeline views

<!-- NOTE FROM CSV: Must check with Lilit whether this will come to the timeline view in addition to the table (Lilit said yes; this was messaged before but pulled). The second bullet will change; check with Lilit first. -->

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

To improve performance on a large number of records, we have made the following improvements to the table and timeline views:

* The view now loads the first 500 records initially, with additional records loaded automatically as you scroll in batches of 500.
* Quick search and grouping impact only the records currently loaded in the view.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md) and [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

<!--

## Additional permissions for users other than requestors to submitted requests

>[!NOTE]
>
>Preview: October 28, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Workspace managers can now define what access to submitted requests users other than requestors have.

By editing the Permissions area of a request form, you can define additional access for other users to requests submitted using the form.

You can grant permissions to workspace users or any other users, groups, teams, job roles or companies in the system. Once defined in the request queue, the permissions are granted automatically when the request is submitted, and any permission changes apply only to new requests.

Prior to this enhancement, you could only grant permissions to requestors.

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

-->

## Manual grouping reordering in timeline view

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now drag and drop groupings, sub-groupings, and records to create a custom order in timeline view. Your manual arrangement is preserved across sessions, and you can switch seamlessly between manual ordering and field-based sorting as planning needs change.

The drag and drop functionality is available for both swimlanes and stacked versions of the timeline view.

For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Business rules for global record types

>[!NOTE]
>
>Preview: October 28, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Workspace managers can now configure business rules on global record types both in the primary and the secondary workspaces. Rules apply to all records of the same type in all workspaces where they are added.

Business rules added in global workspaces display as read-only in secondary workspaces where the record types were imported. Business rules added in secondary workspaces display as read-only in primary workspaces where the record types were originally created. Rules are editable only in the workspaces where they are created.

For information, see [Configure record type business rules](/help/quicksilver/planning/architecture/configure-business-rules.md).

## Set up default prompt settings for Fill form functionality in Planning requests

>[!NOTE]
>
>Preview: October 21, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now customize the prompt that users see when using the AI-powered Fill form capability when submitting a Planning request.

You can create a default prompt when creating a request form for Planning requests.

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
