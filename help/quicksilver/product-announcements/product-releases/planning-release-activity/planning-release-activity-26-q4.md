---
content-type: release-notes
title: Fourth Quarter 2026 release activity for Adobe Workfront Planning
description: This is the release activity for the Adobe Workfront Planning product for the Fourth Quarter 2026.
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
# Fourth Quarter 2026 release activity for Adobe Workfront Planning

This article describes the features that are releasing for Workfront Planning during the Fourth  Quarter 2026 release.

For a list of all features released for Adobe Workfront Planning, see [Adobe Workfront Planning release activity: article index](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Sharing fields in Workfront Planning

>[!NOTE]
>
>Preview: September 25, 2026
>Production fast release: October 14, 2026
>Production for everyone: October 15, 2026

Workspace managers can now control access to individual fields, allowing specific users and teams to view, edit, or be completely restricted from sensitive data within the same record type.

Field-level permissions are enforced consistently across views, record details, request forms, connections, APIs, and dashboards, helping organizations securely manage confidential information.

Users without access do not see restricted fields, while administrators can configure permissions without restructuring records or creating separate workspaces.

For information, see [Share Workfront Planning fields](/help/quicksilver/planning/access/share-fields.md).

## Share a Planning request

>[!NOTE]
>
>Preview: September 25, 2026
>Production fast release: October 14, 2026
>Production for everyone: October 15, 2026

You can now share a Planning request with others from the Requests area in the new request experience.

You can give others one of the following permissions to the request: View, Contribute, or Manage.

For information, see [Share Planning records](/help/quicksilver/planning/requests/share-requests.md).

## Set up multi-stage approvals for Planning requests

>[!NOTE]
>
>Preview: September 25, 2026
>Production fast release: October 14, 2026
>Production for everyone: October 15, 2026

Workspace administrators can now build single- or multi-stage approval processes for each Planning request form, assigning one or more approvers or teams to every stage and reusing existing approval templates to speed up setup. Requests advance automatically once all required approvers in a stage sign off, and each approver is notified when a request reaches their stage. Requesters and approvers can track which stage a request is in and see which approvals are still pending.

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Enhancements to display logic and field editing in Planning requests forms

>[!NOTE]
>
>Preview: September 25, 2026
>Production fast release: October 14, 2026
>Production for everyone: October 15, 2026

You can now create advanced display logic in Planning request forms based on connection field values, so forms adapt to what requesters select. All Planning fields, including connection fields, are supported when building this logic.

In addition, you can now edit a field's options directly from the request form. For example, for select-field types, you can update the field choices, their order, and their default value from the request form. Previously, this capability was not available.

For information, see [Create request form](/help/quicksilver/planning/requests/create-request-form.md).

## Configure default permissions for requestors on Planning request forms

>[!NOTE]
>
>Preview: September 25, 2026
>Production fast release: October 14, 2026
>Production for everyone: October 15, 2026

Workfront and workspace administrators can now indicate the level of permissions a requester receives on their requests when they configure the request form.

Requesters can get the following permissions to a request they submitted: View, Contribute, or Manage. Users can comment, edit, share, or view a request, and the capabilities that are not shared with them are dimmed when viewing the sharing box from a request.

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## AI Form Fill pulls data from records referenced with a link

>[!NOTE]
>
>Preview and production: September 22, 2026
>[!BADGE Off schedule]{type=Neutral}

AI Form Fill can now retrieve field data directly from a Planning record referenced by its link and use it as context when populating a form. Simply paste the direct URL of the record into the prompt, and its details will be pulled in automatically to suggest form values.

For information, see [Use Form Fill powered by AI to fill in a request using prompts or documents](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).

## CX Coworker available in Workfront Planning

>[!NOTE]
>
>Preview: Phased rollout beginning on September 3, 2026
>Production fast release: Phased rollout beginning on September 17, 2026
>Production for everyone: Phased rollout beginning on October 15, 2026

CX Coworker is now available inside Workfront Planning. Now, you can access CX Coworker in a panel that is available throughout Workfront Planning.

CX Coworker Chat is a conversational interface for getting work done. Describe a goal in plain language, and Coworker plans the work, executes it across Workfront Planning and your connected Adobe systems, validates the results, and brings the finished work back to you for approval. 

Coworker respects your organization's existing access controls, with read-only access by default, and system admins control when users get write access.

Coworker is replacing the current AI Assistant as a more powerful way to get work done. Coworker is part of the Adobe ecosystem, and is not limited to Workfront Planning.

>[!IMPORTANT]
>
>CX Coworker is not currently available to organizations in health care, finance, or some other industries with sensitive data. AI Assistant is still available to these organizations.

For more information, see [CX Coworker overview](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

## AI Assistant icon removed from the record Details preview box in preparation for the CX Coworker launch

>[!NOTE]
>
>Preview: Phased rollout beginning on September 16, 2026
>Production fast release: Phased rollout beginning on September 17, 2026
>Production for everyone: Phased rollout beginning on October 15, 2026
>[!BADGE Off schedule]{type=Neutral}

This change is available for customers who have the CX Coworker in Workfront.

In preparation for the launch of the Adobe CX Coworker in Workfront, we have removed the AI Assistant icon from the Details preview page. The icon still exists on the Details page, when opened in full screen. Clicking it will open the CX Coworker.

>[!IMPORTANT]
>
>CX Coworker is not currently available to organizations in health care, finance, or some other industries with sensitive data. AI Assistant is still available to these organizations.

For information, see [CX Coworker in Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-in-workfront.md).

## Improved experience when duplicating records that have connected fields with a One-to-one or One-to-many connection type

>[!NOTE]
>
>Preview: September 17, 2026
>Production fast release: October 14, 2026
>Production for everyone: October 15, 2026

Records can now be duplicated even when One-to-one or One-to-many connected records exist. After duplication, users can choose to keep the connected record on the original record or connect it to the new record. Keep on the original is the default choice.

The connection conflict resolution dialog has been updated to reflect this new behavior and provide greater flexibility when managing connected records.

For information, see [Duplicate records](/help/quicksilver/planning/records/copy-or-duplicate-records.md).

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

## Custom weeks for the timeline view

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

As a Workfront administrator, you can now configure custom weeks, in addition to custom quarters. Custom weeks, and quarters are visible from the Workfront Planning timeline view. Workfront generates sequential weeks starting from Week 1 at the beginning of Custom quarter 1.

You can customize week labels which are visible in the timeline view. You can choose a predefined format or enter a custom one.

Custom weeks are not visible in Workfront. They are only visible in the Workfront Planning timeline view.

For information, see [Enable custom quarters](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md).

## Filters for connected record fields

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now filter for certain record types that meet a filter criteria when you add connections in Planning.

Only those records that meet your filtering criteria will display as options in connected fields.

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

## Display full group names and resize the grouping panel in the timeline view

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

The experience of dragging and dropping single rows in the table view has been improved visually.

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
* We changed the way you add lookup fields to connections


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
