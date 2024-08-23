---
title: Adobe Workfront Planning current release activity
description: Adobe Workfront Planning capabilities are currently available to select Workfront customers. Review this article often to learn about the features recently released for the planning capabilities. 
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
---

# Adobe Workfront Planning current release activity 

<!--this article is linked to the WF Planning landing page - do not change URL or move it; send the team a new URL after we add the redirects for this page-->

<!--
At GA release, replace the Important below and all the text that follows before the weekly releases with this:

(***********At GA - change the title to: Adobe Workfront Planning early access release activity during 2024*******)

Also update the metadata: 

Adobe Workfront Planning capabilities are currently available to all customers. You must purchase a Workfront Planning license, in addition to a Workfront license to be able to access these capabilities.


>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning, a new offering from Adobe Workfront. 
>
>You must purchase a Workfront Planning license, in addition to a Workfront license to be able to access and use the Workfront Planning capabilities. 
>
>For more information about access to Workfront Planning, see [Access overview](/help/quicksilver/planning/access/access-overview.md).
>-->

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning, a new offering from Adobe Workfront. 
>
>Currently, Workfront Planning is in an early access stage which is open to a limited number of customers. 
>
>You must be a Workfront customer to use these capabilities. 
>
>Your account representative will inform you if you are part of this stage.
>
>For more information, see [Adobe Workfront Planning overview](/help/quicksilver/planning/general/planning-overview.md).
>
>In some cases, the documentation referenced in the sections below might be available after the features documented are released to Production. 

<!--Not sure if we should enable this - Richard: 

## Workfront Planning release timeline

| Time               | Release                                 |
|--------------------|-----------------------------------------|
| August - December 2023               | Workfront Planning beta release         |
| January - August 2024 | Workfront Planning early release        |
| August 28, 2024    | Workfront Planning general availability |-->

The following articles describe the features released during the release for Workfront Planning: 

* [Adobe Workfront Planning release activity archives for 2023](/help/quicksilver/planning/general/release-activity-archives-2023.md) lists features released during the beta release, during 2023.
* This article lists the features that have been released to Workfront Planning during the early access period in 2024.

    The released features are listed in the order of their release, with the most recent first. Customers who are participating in the Workfront Planning program can access all features in their Production environments.

<!--* See the current release overview documentation for features that were released after the general availability release on August 28, 2024. 
-->

Workfront Planning has temporarily been removed from the Preview and Sandbox environments since January 2024. All features documented in this articles are currently available in Production.  

<!--

### Reporting capabilities for Workfront Planning with the Canvas Dashboard 

Production: August 28, 2024 

Preview: To be determined 

You can now view Workfront Planning information in a report using the Workfront Canvas Dashboard. For information, see [Get started with Canvas Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/get-started-canvas-dashboards.md).

### Define format for formula field values

Production: <date> 

Preview: To be determined 

As a workspace manager, you can now define the format for the values displayed in a formula field. You can choose from the following formats: 

* Single-line text 
* Number 
* Percentage 
* Currency 
* Date
* Tags

For information, see the "Formula" section of the article [Create fields](/help/quicksilver/planning/fields/create-fields.md). 

-->

## Week of August 19, 2024

### Workfront Planning main page improvements

Production: August 20, 2024

Preview: To be determined 

We have made the following improvements to the Planning area's main page: 

* For system administrators, the workspaces that they did not create have been moved from the "Other workspaces" tab to the "Workspaces I'm on" tab. The "My workspaces" tab has been removed. 

* We added a "More" menu for each workspace card to make it easier to edit or delete the workspace from the main page. 

* We added "Show all" and "Show less" links to control the number of workspaces that display on the main page. When there are more than two rows of workspace cards listed on the main page, the Show all link displays to allow you to display all workspaces, only if needed. 

For information, see [Edit workspaces](/help/quicksilver/planning/architecture/edit-workspaces.md).

### Connect record types across multiple workspaces

 Production: August 20, 2024

 Preview: To be determined  

 You can now connect record types that belong to different workspaces.  

 System administrators can now configure record types to be connected from other workspaces. After this, a workspace manager can connect to these record types from a designated workspace or from all workspaces in the system.  

Prior to this enhancement, you could connect only record types that belonged to the same workspace, along with object types from other applications.   

For information, see [Edit record types](/help/quicksilver/planning/architecture/edit-record-types.md). 

### Display connected records in the timeline view using the Breakdown feature

Production: August 22, 2024

Preview: To be determined 

As a Timeline view manager, you can now view the relationships between connected records by breaking down records into visual hierarchies in the timeline view.  

For example, when you are viewing Campaigns in the timeline view which are linked to Products, and Products have associations with Projects, you can now display Products under Campaigns, and Projects under their respective Products. 

This allows you to seamlessly navigate through multiple levels of relationships, all within the same timeline view.  

This is not an actual hierarchy (no object is higher than another). It is a visual hierarchy that displays connected record types in one timeline view.  

You can display up to 5 levels of record types in the same timeline for one record.  

For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md). 

### New Connections tab in the record details area

Production: August 22, 2024

Preview: To be determined 

We have added a new tab on the record's preview and page areas. Now, when you click the record name in a view, the record's preview and the record's page display the following tabs: 

* **Details**: Displays all record fields, thumbnail, and cover image. You can edit fields in the Details tab. 

* **Connections**: Displays all record or object types and their connected records or objects. You can add more records from the Connections tab.  

For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).  

### Create records, projects, and portfolios as you connect them

Production: August 22, 2024

Preview: To be determined 

You can now create records, projects, and portfolios as you connect them to existing records. 

For example, if you connect Workfront Planning campaigns with Workfront projects, and you determine that a particular project does not exist, you can add it as a new project in the connected record field. The project is then added to Workfront. Newly added records are added to their respective record type pages in the table view.   

At this time, you can create the following when connecting records: 

* Workfront Planning records 
* Workfront Projects without a template 
* Workfront Portfolios 
 
You cannot create other connected Workfront objects or Experience Manager assets when connecting them to a record. 

For information, see [Create records](/help/quicksilver/planning/records/create-records.md). 

### Export record details to Word

Production: August 22, 2024

Preview: To be determined 

You can now export a record's details page or preview to a Word document (.docx). 

For information, see [Export a record's details](/help/quicksilver/planning/records/export-the-record-page.md).

### Add connection type options

Production: August 22, 2024
Preview: To be determined 

Now, when you configure a connection between two record types, you can define whether users can connect single or multiple records in each of the record types of the connection. This ensures that you can reliably design your team's workflows and ensure that users only select the information expected according to their processes.  

You can now choose from the following types of connections when you link two record types:  

* Many to many. When you select this connection type, it is not possible to change it after you save it.  
* One to many 
* One to one 
* Many to one. 
 
This allows you to define how many records of the connected record types users can connect when a connection is established.  

The new connection types are not supported for the following record type connections: 
 
* When you connect record types with Experience Manager assets 
* When you connect record types that don't belong to the same workspace 

For information, see [Connect record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md). 

## Week of August 12, 2024

### AI Assistant has been temporarily removed

Production: August 12, 2024
Preview: To be determined

The Workfront AI Assistant has been temporarily removed and it will be available at a later date.. For more information about the AI Assistant, see [Adobe Workfront Planning AI Assistant overview](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

### Preserve the last viewed time frame in the timeline view

Production: August 14, 2024 

Preview: To be determined 

Now, when you open a timeline view and scroll to a date in the past or the future, the date you select is preserved after you refresh the page. Prior to this enhancement, the page would display today's date.  

For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).  

## Week of July 29, 2024

### The Adobe Workfront Planning public API is now available

Production: July 30, 2024

Preview: To be determined 

The Adobe Workfront Planning public API is now available. 

For information, see [Adobe Workfront Planning API basics](/help/quicksilver/planning/general/planning-api-basics.md). 

### Insert and duplicate records in the table view

Production: August 1, 2024
Preview: To be determined 

We have introduced the following capabilities when working with records in the table view: 

* Duplicate records: you can quickly create a record by duplicating an existing one.  An identical record is created. This capability is available only in the table view. 

* You can insert a new record above or below an existing record in the table view. Prior to this enhancement, you you only add records at the bottom of the table view. 

You can perform the new capabilities from the following areas: 

* The More menu of a record 

* The new toolbar which has been added to the bottom of the record page in the table view 

For information, see [Create records](/help/quicksilver/planning/records/create-records.md) 

### Share Workfront Planning views publicly

Production: August 2, 2024

Preview: To be determined 

To work seamlessly with external stakeholders, you can now share record views with others from outside your organization. You can share a public link to the view you want others to have access to.  

The following capabilities are included with this update: 

* Share the view of a record type page with a public link that would expire on a specific date. 

* The shared link is accessible by anyone outside of your company for a limited time, indicated by the expiration date. There is no login required to view the shared view.  

* People that access the view from the public link cannot create other views, edit the shared view, or add, delete, or edit record information.  

For more information, see [Share views](/help/quicksilver/planning/access/share-views.md). 

## Week of July 8, 2024

### Open connected object directly in Workfront

Production: July 9, 2024 

Preview: To be determined 

We have eliminated one step when accessing Workfront objects connected to Workfront Planning records.  

Now, when you click the name of a Workfront object from the Planning record connected to it, you open the Workfront object page. Prior to this enhancement, a read-only Workfront Planning page for the connected Workfront object would open from where you could navigate further to the Workfront object page.  

For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).  

### Only Standard or Plan licensed users can create views

Production: July 11, 2024

Preview: To be determined 

We have changed which types of users can create views. Now, only Standard or Plan licensed users can create views. All other users have view-only access to views that are shared with them. Prior to this update, Light and Worker-licensed users could create views. 

For more information, see [License type overview when using Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md). 

### Sort and group records by lookup fields with multiple values

Production: July 11, 2024 

Preview: To be determined 

You can now sort and group records in any view using lookup fields with multiple values that are not summarized. Prior to this enhancement, you could sort and group only for lookup fields that were summarized.  

If the lookup field contains multiple values, consider the following:  

* The sorting is done by the first value 

* Records are grouped by each unique combination of field values 

* The timeline is built based on the first date value. 

For more information, see the following articles:

* [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md)
* [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).


## Week of June 24, 2024

### Workfront AI Assistant (beta) now available for Workfront Planning

The AI Assistant (beta) is now available for Workfront Planning.  

The AI assistant works in the context of the selected page and with your access and permissions level to perform the following actions: generate, update, remove, or restore records. 

The AI Assistant is currently in a beta phase and it is available to select customers. Contact your account representative to learn if you are eligible to participate in this phase. 

For information, see [Adobe Workfront Planning AI Assistant overview](/help/quicksilver/planning/general/planning-ai-assistant-overview.md). 

### New search box when selecting a workspace or a record type

Production: June 27, 2024 

Preview: To be determined 

To make it easier to navigate between workspaces or between record types, you can now search for a workspace or a record type in the drop-down menu to the right of their name in the page header.  

For information, see [Edit record types](/help/quicksilver/planning/architecture/edit-record-types.md). 

### Insert a new field to the right or left of an existing one in the table view

Production: June 27, 2024

Preview: To be determined

To improve and speed up your experience in the record table view, we have added the capability to add a new field between two columns, by inserting it to the right or left of an existing one.  

For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md). 

## Week of June 17, 2024

### Updated look and feel of the Details page

Production: June 17, 2024 

Preview: To be determined 

We have updated the look and feel of the Details page of records. As part of this update, the field icons have been removed.  

For information, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

### Updated workspace templates

Production: June 17, 2024 

Preview: To be determined 

We have updated the look and field of the workspace template cards in Workfront Planning.  

This update includes the following improvements: 

* The record types that belong to each template display as cards. 

* We have removed the Marketing management template. We  have added the following templates for Marketing management, and we recommend using the appropriate one depending on the complexity of your workflows:  

    * Basic: Marketing Management 
    * Advanced: Marketing Management 
    * Enterprise: Marketing Management 

For information, see the following articles: 

* [List of workspace templates](/help/quicksilver/planning/architecture/workspace-templates.md)  

* [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md)  

### New experience when adding a thumbnail or a cover image to a record

Production: June 17, 2024 

Preview: To be determined 

We have updated the experience for adding a thumbnail or a cover image to a record from the Details page. The improvements include the following updates:  

* A thumbnail image and a cover image are automatically assigned to a record when you create it. You can later edit these images.

* You can add a thumbnail from the Details page. Prior to this enhancement, you could add a thumbnail only from the table view. 

* You can browse a gallery of images to select an image for the cover or for the thumbnail of a record. Prior to this enhancement, you could only upload your own image file.  

For more information, see the following articles: 

* [Add a cover image to a record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) 

* [Add a thumbnail to a record](/help/quicksilver/planning/records/add-thumbnails-to-records.md) 

### Update the record title in the Details page

Production: June 17, 2024 

Preview: To be determined 

The title of a record's Details page displays the primary field of a record. Prior to this update, the title of a record's Details page displayed the name of the record. You can edit the title inline, in the Details page, unless the primary field is a formula-type field.   

For more information, see the following articles: 

* [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md) 

* [Edit records](/help/quicksilver/planning/records/edit-records.md) 

### Adding a "Show more/ Show less" link in the connected record fields 

Production: June 17, 2024 

Preview: To be determined 

We have added a "Show more/ Show less" link in a connected record field, when there are records that would otherwise display on more than two rows in the Details page of a record. 

For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).

### Auto-populate the Name field with the record name, when connecting record types

Production: June 20, 2024

Preview: To be determined 

When you create a connection between two records or between a record and an object from another application, the Name of the connection field auto-populates with the name of the connected record. Prior to this enhancement, you had to manually add a Name for the connection field. 

For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 

### Define how connected records display in connected fields

Production: June 20, 2024 

Preview: To be determined 

You can now decide how connected records display in connected fields. While adding a new connection to a record type, you now have the option to display either the connected record's title and its thumbnail or just the thumbnail.  

A record's title  is either the record's name or any field that is set as the primary field in the record type's table view.  

This enhancement is available for records connected from Workfront Planning and for assets connected from the Adobe Experience Manager.  

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).  

### Only Standard or Plan licensed users can have Manage permissions to workspaces (title)  

Production: June 21, 2024 

Preview: To be determined  

We have changed which types of users can have full access to workspaces. Now, only Standard or Plan licensed users can have Manage permissions to workspaces. The access to record types, records, and fields is inherited from a workspace. All other users have view-only access to workspaces and their object types. Prior to this update, Light and Worker-licensed users could receive Contribute permissions to workspaces.    

 For more information, see [License type overview when using Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).   
 
## Week of June 10, 2024

### Up to 4-level reference for record lookup fields

Production: June 12, 2024 

Preview: To be determined 

You can now reference fields that are up to 4 levels away from the record when you create one of the following:  

* Filter 

* Sort 

* Grouping 

* Formula field 

For more information, see the following articles: 

* [Create fields](/help/quicksilver/planning/fields/create-fields.md)  

* [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md)  

## Week of June 3, 2024

### New landing page for Workfront Planning

Production: June 7, 2024

Preview: To be determined 

We are introducing a new landing page for Workfront Planning, after you click Planning in the Main Menu.  

Some of the information on the landing page includes the following: 

* An area that displays your workspaces and workspaces that are shared with you. The workspace owner displays on each workspace card.  

* If you are a Workfront administrator, the following tabs display: 

    * My workspaces: Displays only workspaces you created. 

    * Other workspaces: Displays workspaces you created or that are shared with you.  

* Links to documentation and release activity for Workfront Planning 

* Get started tutorial for Workfront Planning 

For more information, see [Adobe Workfront Planning overview](/help/quicksilver/planning/general/planning-overview.md). 

### New onboarding experience for Workfront Planning

Production: June 7, 2024 

Preview: To be determined 

When new users access Workfront Planning for the first time, they are now welcomed by a self-prompted onboarding tutorial that guides them through simple tasks and define the main concepts of the solution.  

You can walk through the onboarding process, complete the tasks, or minimize it and revisit it at a later time.  

## Week of May 27, 2024

### Introducing the UNIQUE rollup operator for lookup fields 

Production: May 27, 2024

Preview: To be determined 

We have added the UNIQUE operator when aggregating lookup field values.  

The UNIQUE operator removes duplicates from lookup field values and only shows a unique value. For example, if you add several connected records and the values of a lookup field are identical between multiple records, Workfront displays only one of the values in the lookup field of the original record. 

The UNIQUE operator is available for all field types except the following:  

* Paragraph 
* People 
* Checkbox field

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 

### Share views with all members of a workspace by default

Production: May 30, 2024

Preview: To be determined 

We have now introduced an option where you can quickly give View permissions to a view to all members of a workspace. Prior to this enhancement, only users you specifically shared a view with could access the view. This option is not enabled by default.  

For information, see [Share views](/help/quicksilver/planning/access/share-views.md). 

### Updated look of the Planning icon in the Main Menu 

Production: May 30, 2024 

Preview: To be determined 

 We have updated the look of the icon for the Planning area in the Main Menu. For information, see [Adobe Workfront Planning overview](/help/quicksilver/planning/general/planning-overview.md). 

### Renaming the Workfront Planning program

Starting with May 30, 2024, the Adobe Workfront Planning program is transitioning from the beta phase to an early access stage. You are going to see this change in the terminology of our documentation. 

The early access stage is also limited to a few Workfront customers. 

Your account representative will inform you if you qualify to participate in the early access stage.

### New process for deleting a workspace

Production: May 30, 2024 

Preview: To be determined 

Because the impact for deleting a workspace can be significant, we are adding an extra step in confirming the deletion. Users are now required to type "delete" before they can complete the permanent deletion of a workspace. 

Deleted workspaces and their information cannot be recovered. 

For more information, see [Delete workspaces](/help/quicksilver/planning/architecture/delete-workspaces.md). 

### Lookup date fields are now available in the timeline view

Production: May 31, 2024 

Preview: To be determined 

You can now set the Start and End Dates of the timeline view to a lookup field from a connected record or object type. 

For more information about creating views, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 

## Week of May 20, 2024

### Connect Workfront Planning records from Workfront objects using the Planning section

Production: May 23, 2024

Preview: To be determined

We have added a new Planning section in the left panel of Workfront projects, portfolios, and programs. The new Planning section displays the Workfront Planning records connected to the Workfront object.  

The following actions are available from the Planning section in Workfront: 

* View connected Planning records 

* Connect Workfront Planning records to the Workfront object 

* Disconnect records  

* Open the details preview box or page to view more information about the connected records

For information, see [Manage records in the Planning section of Adobe Workfront objects](/help/quicksilver/planning/records/manage-records-in-planning-section.md).  

## Week of May 13, 2024

### Real-time updates in the timeline view after editing records

Production: May 14, 2024 

Preview: To be determined.  

When a user updates the information on a record, other users can view the updated information in the record's timeline view in real time. This ensures that all users view the updated information at the same time, in sync with when the changes happen. 

### Add record from the view header

Production: May 14, 2024

Preview: To be determined

We have added a "New record" button on the header of a record type page. You can now create records from any view. Prior to this enhancement, you could create records only from the table view.  

For more information, see [Create records](/help/quicksilver/planning/records/create-records.md). 


### New warning about object visibility when connecting records 

Production: May 15, 2024

Preview: To be determined

When you create connections to object types outside of Workfront Planning, you are now notified that anyone working in the current workspace will have visibility to all the linked objects and their lookup fields, regardless of their permissions and access levels in the other application. 

For example, if you link projects from Workfront Planning campaigns, everyone with access to View the campaign will also have access to view the linked projects and the information from their lookup fields, even when they don't have any permissions to the linked projects, or access to projects, in general. You obtain access to Planning records when you receive permissions to workspaces. 

For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

### Add sections to the record's preview and details pages

Production: May 15, 2024

Preview: To be determined 

To better organize information on the record's page for more efficient readability and navigation, we have introduced sections to the record's page. The section titles serve as headers that organize the fields into distinct categories. The sections are fully customizable and can be expanded or collapsed, if needed.  

For information, see [Manage the record page layout](/help/quicksilver/planning/records/manage-the-record-page.md). 

### Real-time updates for field configuration changes 

Production: May 16, 2024

Preview: To be determined 

When a user changes any field configuration (name, description, list of options etc) in a record type, other users view those changes in real-time. This ensures that everyone views the correct fields and their information at the same time.  

>[!WARNING]
>
>When formula expressions change, or options are added or removed from a select-type field, there will be loss of data for the records that already have information stored in the fields whose configuration is modified. 
>
>There is no warning or indication that this data loss could happen when you change the configuration of fields. 
>
>There is no notification to other users that the field configuration has changed.  

For more information, see [Edit field settings](/help/quicksilver/planning/fields/edit-fields.md).  

## Week of May 6, 2024

### Updated look of the record type cards in a workspace

Production: May 7, 2024

Preview: To be determined 

We have updated the look of record type cards when viewing them in a workspaces. The updates include: 

* Removal of the number of fields and connections for each record type 

* Addition of the record type's Description  

For information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Enable Workfront Planning notifications for Adobe Unified Experience customers

Production: May 8, 2024  

Preview: To de determined  

If you are an Adobe Unified Experience customer and someone adds you to a comment on the record page, you receive an in-app and an email notification about the comment. You can manage your notification preferences in the Preferences area of your Adobe Experience Cloud profile. For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).   

For more information about Workfront planning notifications, see [Adobe Workfront Planning notifications: Article index](/help/quicksilver/planning/notifications/notifications-information.md). 


## Week of April 29, 2029

### Real-time updates on the record details box and page after editing records in the table view

Production: May 2, 2024

Preview: To be determined

When a user updates the information on a record in the table view, other users can view the updated information in the record's details box (inside of a view) or page in real time. This ensures that all users view the updated information at the same time, in sync with when the changes happen.  

For information about editing records, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

### Real-time updates in the calendar view after editing records

Production: May 3, 2024

Preview: To be determined.  

When a user updates the information on a record, other users can view the updated information in the record's calendar view in real time. This ensures that all users view the updated information at the same time, in sync with when the changes happen. 

## Week of April 22, 2024

### Updated workflow when editing a workspace or a record type

Production: April 23, 2024

Preview: To be determined 

We have updated the look-and-feel of the Edit workspace and Edit record type boxes.  

When you edit a workspace or a record type, you can now define a name, description, as well as assign a color and an icon to them.  

For more information, see the following articles: 

* [Edit workspaces](/help/quicksilver/planning/architecture/edit-workspaces.md) 

* [Edit record types](/help/quicksilver/planning/architecture/edit-record-types.md).

## Week of April 8, 2024

### Copy the content of one cell and paste it into multiple selected cells

Production: April 10, 2024

Preview: To be determined 

You can now copy the content of one cell in the table view and paste it in multiple selected cells. You can also copy information from external sources and paste it into the table view cells.  

This functionality is supported for all field types except for calculated fields.  

For more information, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

## Week of April 1, 2024

### Reorder the fields on record pages

Production: April 4, 2024 

Preview: To be determined 

As a Workspace manager, you now can reorder the fields listed in the record page or preview. Updating the order of the fields changes the order of fields on all records of the same type, for everyone viewing the record page or the record preview.  

For more information, see [Manage the record page layout](/help/quicksilver/planning/records/manage-the-record-page.md). 


### Add cover image to record pages

Production: April 4, 2024 

Preview: To be determined 

As you manage record pages, you can now add, reposition, and replace a cover image on a record page or preview, to enrich the record's presentation and stakeholder engagement. Cover images are visible to all users viewing the records. 

For more information, see [Manage the record page layout](/help/quicksilver/planning/records/manage-the-record-page.md).  

## Week of March 25, 2024

### New flexible record type organization for workspaces

Production: March 25, 2024 

Preview: To be determined 

To create efficiency for you when setting up workspaces, we have modified the way you organize record types in a workspace. Some of the improvements include:  

* Create up to 50 sections of record types in each workspace. Existing Operational Record Types and Taxonomies sections remain in the existing workspaces.  

* Fully customize all new workspaces and their new sections to reflect your processes and organization's needs.  

* Dynamically move record types within a workspace by dragging and dropping them where they need to be, including across different sections.  

For more information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Duplicate views 

Production: March 25, 2024 

Preview: To be determined 

To save you time and keep consistency, you can now duplicate an existing view that you have permissions to access.   

Duplicating a view creates an identical view, using the same filters, sorting criteria, and groupings. Duplicating a view does not maintain the permissions of the original view.   

For more information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 

### Renamed the Maestro area in the Main Menu to Planning

Production: March, 27, 2024 

Preview: To be determined 

We have renamed the Maestro area in the Main Menu to Planning.  

For an overview of Adobe Workfront Planning, see [Adobe Workfront Planning overview](/help/quicksilver/planning/general/planning-overview.md). 

### New experience when deleting a record type

Production: March 27, 2024 

Preview: To be determined 

We have redesigned the confirmation box when deleting a record type. Deleting a record type is impactful, as it also deletes all the records, their fields, the information in the fields, as well as the views associated with the record type. Deleted record types and their deleted information cannot be recovered.  

For this reason, we wanted to ensure the user's intent is accurate when deleting a record type, so we have introduced an extra step in confirming the deletion. For more information, see [Delete record types](/help/quicksilver/planning/architecture/delete-record-types.md).  

## Week of March 18, 2024

### Filters available in the calendar view

Production: March 19, 2024 

Preview: To be determined 

You can now filter information in the calendar view. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md).  

### Preview with record details added to the timeline and calendar views 

Production: March 19, 2024 

Preview: To be determined 

You can now access the preview with record details from the timeline and calendar views. You can edit records in the record's preview box inside the timeline and calendar views. 

From the record's preview, you can open the record page in a new browser tab. 

For more information, see [Edit records](/help/quicksilver/planning/records/edit-records.md).  

### The record type Excel import is temporarily removed  

Production: March 21, 2024 

Preview: To be determined 

We are temporarily removing importing record types using an Excel or CSV file. This functionality will be available at a later date. 

## Week of March 11, 2024

### At-a-glance record details display in the table view

Production: March 14, 2024

Preview: To be determined 

To make it easier to view additional information about records when using the table view, we have introduced a new Details preview that displays a quick view of the record's details. The following is some of the information included in the record preview: 

* Relevant record details at a glance 

* Ability to modify record information 

* A link to open the record's page 

For more information, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

### New tabbed design for record views 

Production: March 14, 2024 

Preview: To be determined 

For better navigation and ease of use, we have redesigned the display of record views. Now, the views display horizontally, as tabs on the record type page, so you can easily navigate through them. Prior to this enhancement, views displayed in the View drop-down menu.  

Views display chronologically by added date from left to right. Shared  views also display in chronological order of when they were shared.  

For more information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).  

### Dynamic design of a record view

Production: March 14, 2024
Preview: To be determined 

We have updated the look and feel of the views in the record type page. The new views are dynamically responsive and quickly adjust to the size of your screen. The toolbar option labels are hidden on smaller screens to make the toolbar easier to use.  

For more information, see the following articles: 

* [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

### Allow System Administrators to manage all shared views 

Production: March 14, 2024

Preview: To be determined 

To be consistent with all other areas of the system and to be able to maintain and control any view available to you as a System Administrator, you now have Manage permissions to any view shared with you in the record type page. Prior to this enhancement, view creators could have given you permissions to View or Manage the view. Now, if the view is shared with you and you are a System Administrator, you will have Manage permissions to the view, by default.  

For more information, see [Share views](/help/quicksilver/planning/access/share-views.md). 

### Unauthorized page when sharing a view without permissions

 Production: March 14, 2024

Preview: To be determined 

 When a user receives a link to a record type and they have access to the workspace but not to the view shared in the link, a page notifying them that they are not authorized to see the record type displays.  

 For more information, see [Share views](/help/quicksilver/planning/access/share-views.md). 


### New label for System Administrators in sharing dialogs

Production: March 14, 2024

Preview: To be determined 

We now display an "Admin" label next to the system administrator's name in the sharing dialog box when sharing a view or a workspace.  

For information, see [Share permissions overview](/help/quicksilver/planning/access/sharing-permissions-overview.md).  

### Unauthorized page when sharing a view without permissions

Production: March 14, 2024

Preview: To be determined 

 When a user receives a link to a record type and they have access to the workspace but not to the view shared in the link, a page notifying them that they are not authorized to see the record type displays.  

 You must share views in addition to sharing workspaces for others to access the same record type page that you share with a link.

 For more information, see [Share views](/help/quicksilver/planning/access/share-views.md). 

## Week of March 4, 2024

### Change row height in the table view

Production: March 7, 2024 

Preview: To be determined 

You now have an option to modify the height of a row when displaying records in the table view.

You can update the row height to one of the following sizes:  

* Short 
* Medium
* Tall.  

For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 

### New calendar view for records

Production: March 7, 2024 

Preview: To be determined 

You can now display records in a calendar view. You must have at least two date fields on a record type to be able to create the calendar view.  

For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

## Week of February 26, 2024

### Filter, sort, and group by connected records or lookup fields

Production: February 28, 2024

Preview: To be determined

You can now filter, sort, and group by connected records or their lookup fields. This enhancement will help you efficiently organize and visualize your data in both table and timeline views.

You cannot filter, sort, or group by lookup fields that allow connections with multiple records. 

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md) and [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Week of February 5, 2024

### Modify permissions based on license types

Production: February 6, 2024 

Preview: To be determined 

We have modified permissions levels to take into account users' license types. Prior to this enhancement, there were no differences in workspace permissions based on the license types of the users.  

The following are the highest levels of permissions that users can receive based on the user's license type:  

* Users with a Plan license (or Standard license, in the new license model) can create and manage workspaces, record types, and records. 

* Users with a Work license (or Light, in the new license model) can view and contribute to a workspace shared with them, as well as the record types and records of that workspace.  The Work- (or Light-) license users can also create, edit, and delete records in workspaces where they have Contribute access. 

* Users with a Review or Requestor license (or Contributor, in the new license model) can only view the workspaces shared with them, as well as the record types and records of those workspaces. They cannot create, edit, or delete record types or records.  

For information about the new license model, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

For information about the connection between license type and permissions in the planning capabilities, see [License type overview when using Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).  


### New look-and-feel of the Rich-Text toolbar for record fields

Production: February 7, 2024 

Preview: To be determined 

We have updated the look-and-feel of the Rich Text toolbar when you edit a Paragraph-type field.

For information, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

### Improved experience when editing Single-select, Multi-select, People fields, and when adding connected objects

Production: February 8, 2024 

Preview: To be determined 

We have redesigned and improved the experience of adding options or objects for the following field types:

* Single-select
* Multi-select
* People
* Connected record fields (when connecting planning capability record types or Workfront objects)

With the new improvement, a smaller, more responsive box displays first.  
 
For connected fields, you can add them doing one of the following:

* Add objects to the connected field by searching and selecting them from a list in the table view, while inline editing the field
* Click to open the larger Connect objects box, where you can view all item names in addition to more information about the items. 

The improvements are now available when updating fields in the table view of a record type.  

For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

## Week of January 29, 2024

### Improved sharing of views and workspaces 

Production: January 30, 2024

Preview: To be determined 

We have improved the sharing experience for workspaces and views with the following enhancements: 

* To add clarity around what each permission level allows a user to do, we have added details for every level of permissions when sharing a workspace and a view.

* You can now copy a link to a workspace or view and share it with others. Users must have at least View permissions to the workspace or to the view to be able to access them from the copied link. 

For more information, see the following articles: 

* [Share workspaces](/help/quicksilver/planning/access/share-workspaces.md) 
* [Share views](/help/quicksilver/planning/access/share-views.md)

### Add thumbnails to records 

Production: February 1, 2024

Preview: To be determined  

You can now add individual thumbnails to each record to distinguish them in a view. In the table view, you can add image files that you have previously saved on your computer as thumbnails. The thumbnails can be unique to each record and display in both the table and the timeline views of the record type page. 

For more information, see [Add a thumbnail to a record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).  

### Remove connected record type cards

Production: February 1, 2024

Preview: To be determined

To avoid confusion and simplify the management of workspaces, we have removed the auto-generated, read-only record type cards for connected external objects from a workspace.

For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).   

## Week of January 22, 2024

### New History section displays system activity for planning capabilities records

Production: January 25, 2024 

Preview: To be determined 

To improve auditing capabilities, we have introduced a new section in the right panel of a record where you can review changes made to the record recorded by the system. 

The following information is recorded in the new History section:  

* Any field changes 

* The old and the new values of fields, when the values change

* The full name of the user who made the change 

* A date and time stamp of when the change occurred. 

 For more information, see [History section overview](/help/quicksilver/planning/records/history-section-overview.md). 

### New label for new record link 

Production: January 25, 2024 

Preview: To be determined 

To create consistency when creating records, we have relabeled the + New link for creating records to "+ New record".  Prior to this update, the link contained the name of the record type. The new link is now available when creating operational and taxonomy records. For information, see [Create records](/help/quicksilver/planning/records/create-records.md).  

## Week of January 8, 2024

### Planning capabilities are removed from the Preview and Sandbox environments 

Preview and sandbox: January 11, 2024

The Adobe Workfront Planning capabilities have been temporarily removed from the Preview and Sandbox environments. They will be added to these environments at a later date, which we will communicate in the release activity notes.  

### Planning capabilities permissions for workspaces and views

Production: January 11, 2024

Preview: To be determined

You can now share a workspace or a view with users and groups. You can set their permissions to different levels, depending on what information they need to view or edit. 

When you share a workspace, users have permissions to the record types, records, and fields in that space.

When you share a workspace, users don't receive sharing permissions to the views associated with the record types of the workspace. You must grant separate permissions to views. 

The following are the permissions levels for workspaces:  

* View: Users can view workspaces that are shared with them. They can also view record types, and records from the shared workspace. 

* Contribute: Users can create, edit, or delete records in the workspace that is shared with them.  They cannot create or edit record types or workspaces that are shared with them.  

* Manage: Users can create, edit, and delete workspaces, record types, records, and fields in workspaces that are shared with them.   

The following are the permissions levels for record views:

* View: Users can select the view from the View drop-down menu of a record type page.
* Manage: Users can edit, share, and delete the view. 

For more information, see [Access overview](/help/quicksilver/planning/access/access-overview.md) and [Overview of sharing permissions in Adobe Workfront Planning capabilities](/help/quicksilver/planning/access/sharing-permissions-overview.md).

### New Formula field type

Production: January 11, 2024

Preview: To be determined 

You can now add a Formula-type field to a record type.  

Formula fields generate a new value using existing values from other fields in a record type and a function that indicates how the existing values should be calculated. 

You cannot use lookup fields from linked record types in a formula calculation. This functionality will be available at a later date.   

For information, see [Formula fields overview](/help/quicksilver/planning/fields/formula-fields.md).  

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

* [Edit records](/help/quicksilver/planning/records/edit-records.md) 

* [Delete  records](/help/quicksilver/planning/records/delete-records.md) 

* [Create records](/help/quicksilver/planning/records/create-records.md) 


