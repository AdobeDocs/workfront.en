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

## Table view enhancements when dragging and dropping multiple rows

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

There are new visual indicators when you drag and drop multiple rows in the table view. A more prominent plus sign and a number indicator now show how many rows are selected for the drag-and-drop action.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## Collapse and expand all groupings in the timeline view

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Timeline views now include Collapse all and Expand all options for grouped timelines. This makes it easier to navigate large roadmap views: you can quickly reduce the view to grouping headings, then expand only the sections you want to review.

For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

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

## Updated column headers for dependent connected record fields

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

We've made visual improvements to the column headers for a dependent connected record field in the table view.

For information, see [Manage dependent connections](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

## Introducing the Workfront Planning Solution Architect Skill

>[!NOTE]
>
>Preview: August 10, 2026
>Production: August 10, 2026

We are making available a new skill, the Workfront Planning Solution Architect, that brings best-practice, agentic guidance for Workfront Planning directly into Claude. Right in the Claude interface, you can now do the following:

* Configure a new Planning workspace to match your business requirements, with the Workfront MCP server executing the setup in your environment.
* Audit an existing configuration for antipatterns at scale.
* Check usage against recommended limits.
* Ask questions about Planning.

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
