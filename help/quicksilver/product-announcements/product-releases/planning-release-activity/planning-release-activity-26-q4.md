---
content-type: release-notes
title: Fourth Quarter 2026 release activity for Adobe Workfront Planning
description: This is the release activity for the Adobe Workfront Planning product for the Fourth Quarter 2026.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
---
# Fourth Quarter 2026 release activity for Adobe Workfront Planning

This article describes the features that are releasing for Workfront Planning during the Fourth  Quarter 2026 release.

For a list of all features released for Adobe Workfront Planning, see [Adobe Workfront Planning release activity: article index](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Manage the visibility of records' thumbnails and colors from the primary field column in the table view

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now manage the visibility of the records' thumbnails and colors when editing the primary field column in the table view.

With this update, the Thumbnail and the Color settings will be removed from the Fields icon in the table view's toolbar.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## Create business rules for record types

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

As a workspace manager, you can now set business rules for record types that will later reflect on how records of that type are managed. You can define rules that allow users to edit or delete records only when certain conditions are met or certain fields are populated.

You can create a condition for your business rule that references all field types except for the following:

* Formula fields
* Lookup fields
* Reference fields

You cannot add business rules to global record types.

For more information, see [Configure record type business rules](/help/quicksilver/planning/architecture/configure-business-rules.md).

>[!NOTE]
>
>With this update, the following menu options in the More menu of a record type have also been updated:
>
>* **Create request forms** and **Manage request forms** has changed to **Request forms**
>* **Manage automations** has changed to **Automations**

## Introducing custom weeks for the timeline view

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

As a Workfront administrator, you can now configure custom weeks, in addition to custom quarters. Custom weeks, and quarters are visible from the Workfront Planning timeline view. Workfront generates sequential weeks starting from Week 1 at the beginning of Custom quarter 1.

You can customize week labels which are visible in the timeline view. You can choose a predefined format or enter a custom one.

Custom weeks are not visible in Workfront. They are only visible in the Workfront Planning timeline view.

For information, see [Enable custom quarters](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md).

## Filters for dependent connected record fields

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now filter for certain record types that meet a filter criteria when you add dependent connections in Planning.

Instead of all record types being available in dependent connected fields, only those that meet your filtering criteria will display.

For this feature, we added a new Record filtering rules option in the New connection tab when connecting record types.

For information, see [Manage dependent connections](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

## Collapse and expand all groupings in the timeline view

>[!NOTE]
>
>Preview: August 27, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Timeline views now include Collapse all and Expand all options for grouped timelines. This makes it easier to navigate large roadmap views: you can quickly reduce the view to grouping headings, then expand only the sections you want to review.

For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## See full group names and resize the grouping panel in the timeline view

>[!NOTE]
>
>Preview: August 27, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

In the timeline view, hovering over a truncated group label now shows the full text in a tooltip, in both the Swimlane and Stacked grouping display. Non-truncated labels show no tooltip.

The grouping left panel in the Swimlane display is now resizable by dragging its divider. The view is updated in real time, which is consistent with the table view. Each user's panel width is saved across sessions, with a default width for first-time users.

For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Improved calendar performance for large record sets in the week view

>[!NOTE]
>
>Preview: August 27, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

The calendar week view now displays only the first 1,000 records across the visible week period. If there are more records, the following message displays at the bottom of the calendar indicating that additional records are available: "There are more records. Load more."

For information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Updated column headers for dependent connected record fields

>[!NOTE]
>
>Preview: August 20, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

We've made visual improvements to the column headers for a dependent connected record field in the table view.

For information, see [Manage dependent connections](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

## Table view enhancements when dragging and dropping multiple rows

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026
>[!BADGE Off schedule]{type=Neutral}

There are new visual indicators when you drag and drop multiple rows in the table view. A more prominent plus sign and a number indicator now show how many rows are selected for the drag-and-drop action.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## Route the submitted request object to the correct workspace when using global record types

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Records created for global record types by submitting a request form are now automatically routed to the workspace from which they were submitted.

Records created by submitting a request from a secondary workspace of a global record type are added to that secondary workspace. Records created by submitting a request from the original workspace, or from the main Requests area, are added to the original workspace.

If the intake form includes a Workspace field and a user selects a workspace before submitting, the request is routed to the selected workspace regardless of where the form was launched. This ensures records are organized in the intended workspace from the moment they're created.

For information, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md).

## Introducing the Workfront Planning Solution Architect Skill

>[!NOTE]
>
>Preview: August 10, 2026
>Production: August 10, 2026

We're releasing a new skill, the Workfront Planning Solution Architect, that brings agentic, best-practice guidance for Workfront Planning directly into Claude:

* **Configure** new Planning workspaces to spec, with the Workfront MCP server executing setup in your environment.
* **Audit** existing configurations for antipatterns at scale.
* **Check usage** against recommended limits (records, connections, hierarchy depth).
* **Ask questions** about Planning anytime.

Beyond initial setup, the skill supports ongoing governance by catching configuration drift before it causes friction, flagging approaching limits before they become blockers, enforcing consistent standards across every workspace regardless of who configures it, and giving anyone on the team accurate answers without waiting on a specialist. Together, this covers the full lifecycle of setting a workspace up correctly and keeping it that way as usage grows.

For information, see [Skills available for direct install](/help/quicksilver/workfront-basics/workfront-mcp-server/direct-skills.md).

## Drag and drop rows in the table view

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for all: October 15, 2026

The experience of dragging and dropping rows in the table view has been improved visually.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).


## Dependent connected record fields

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

Workspace Managers can now define dependencies between connected record types. For example, ensuring a Region field only shows values tied to the selected Geo. This is configured directly in the connection field setup: when adding a connection from a Geo record type to a dependent record type (like Region), a new setting allows workspace managers to mark it as dependent on the Geo record type, using the relationships already established between those record types.

Once configured, any record type that references both fields (such as a Campaign) will see the effect immediately: selecting a Geo value narrows the Region picker to only those Regions actually linked to that Geo. This enforces your record structure automatically, eliminating mismatched combinations and reducing manual cleanup.

The following features are included with this update:

* We added the new Connection settings section in the New connection tab, when connecting record types
* We added a Make this connection dependent setting in the new section


For information, see [Manage dependent connections](/help/quicksilver/planning/architecture/manage-dependent-connections.md).




## Show new comment indicator for a record in the table view

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

We have added a new indicator that shows when there are unread comments on a record. The indicator displays in the upper-right corner of the record's primary field in the table view.

For more information, see [Manage record comments](/help/quicksilver/planning/records/manage-record-comments.md).

## Customizable record color and connection-based color-coding

>[!NOTE]
> 
>Preview: July 23, 2026 
>Production fast release: August 13, 2026 
>Production for all: October 15, 2026 

Records now support customizable color palettes which allow you to update the colors automatically assigned to new records to standard or custom colors. 

The following changes are included in this enhancement:  

* We added the Color option to the following areas: 
   * The Fields icon in the table view.  
   * The Bar style section in the Settings area of a timeline and a calendar view 

    When the Color setting is turned on, the color assigned to a new record displays everywhere where the record displays in these views.  

* A color circle is added to the record's Details page.  
* You can now add single-, multi-select and connected record fields to the color coding of bars in timeline and calendar views when coloring by Field values.  
* You can enable to display the color, in addition to the name and image of a record when you create connected record fields.  
* The Color section in the Settings area has also been streamlined by removing the "None" option.   

For information, see [Create records](/help/quicksilver/planning/records/create-records.md).  

## Planning Designer now requires Beta agreement acceptance 

>[!NOTE]
>Preview and Production to all customers: July 20, 2026 
>[!BADGE Off schedule]{type=Neutral}
 
Planning Designer now requires an accepted Beta agreement to use. Your company is not required to sign an AI agreement. This is available for all customers.  

For this, we have moved the Planning Designer option in the Setup section under the Opt in to AI Betas section. 

Launching Planning Designer without an accepted Beta agreement will now prompt for acceptance before the workspace builder opens. 

For information, see [Get started with the Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).  
