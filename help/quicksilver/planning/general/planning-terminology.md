---
title: Workfront Planning Terminology Overview
description: Although Adobe Workfront Planning is a Workfront product, it comes with proprietary concepts and terminology. Ensure you are familiar with these concepts before embarking on setting up Workfront Planning for your organization. 
author: Alina
feature: Workfront Planning
role: User, Admin
---
# Workfront Planning terminology overview


<!--do not use the snippet for IMPORTANT as it links to this article-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning. Workfront Planning is either a standalone product, or an additionally purchased capability of Adobe Workfront.  
>
>
>This article contains general information about Workfront Planning when customers also purchase a Workfront or Workflow package. 
>
>For the complete list of articles that contain documentation for Workfront Planning, see [General information and article index for Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md). 
>
>For information Workfront Planning as a standalone product, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md). 

Although Workfront Planning is part of Workfront, it comes with proprietary concepts and terminology. Ensure you are familiar with these concepts before embarking on setting up Workfront Planning for your organization. 

The framework for Workfront Planning is fully customizable. You can create all record types, their attributes, and any fields associated with them to suit the exact needs of your organization. 

There are limitations for how many Workfront Planning objects you can create. For more information, see [Adobe Workfront Planning object limitations overview](/help/quicksilver/planning/general/limitations-overview.md). 

The following are the main Workfront Planning objects and concepts: 

* [Workspaces](#workspaces)
* [Record Types](#record-types)
* [Records](#records)
* [Workspace templates](#workspace-templates)
* [Fields](#fields)
* [Connected record types, records and fields](#connected-record-types-records-and-fields)
* [Lookup fields](#lookup-fields)
* [Hierarchies](#hierarchies)
* [Views](#views)
* [Automations](#automations)
* [Request forms](#request-forms)

## Workspaces

Workspaces represent the framework of an organizational unit. They are collections of record types that define the operational lifecycle of a certain organization. 

![Marketing workspace with record type taxonomies opening page](assets/marketing-workspace-with-record-type-taxonomies-opening-page.png) 
    
For more information, see [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md). 

## Record Types

Record types are the object types in Workfront Planning. 

Record types populate workspaces. 

Unlike Workfront, where the object types are predefined, in Workfront Planning, you can create your own object types.  

For example, in Workfront the object types of Program, Portfolio, Project, Task, or Issue are already created.  

In Workfront Planning, you can create any record types that meet your organization's workflows. Later, you can define how the record types relate to one another or form dependencies. 

For more information, see [Record types overview](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Records

A record is an instance of a record type. 

![Records highlighted in campaign record type list](assets/records-highlighted-in-campaign-record-type-list.png)
    
After adding a record type to a workspace, you can start adding records of that type on the record type's page. 

For example, "Campaign" can be a record type and "Summer Campaign for EMEA" is a record of the Campaign record type.
    
For more information, see [Create records](/help/quicksilver/planning/records/create-records.md).

## Workspace templates

You can create a workspace using predefined templates. You can use the predefined record types and fields that come in a template, or you can add your own. 

![Workspaces page with templates thumbnails](assets/workspaces-page-with-templates-thumbnails.png)

Adobe Workfront Planning contains the following templates:

* Operations Initiative Studio
* Communications Planning Studio
* Basic: Marketing Management
* Advanced: Marketing Management
* Enterprise: Marketing Management
* Sales Management
* Product Management

System administrators can also install 6 workspaces when they use the best-practice, multi-space template. The multi-space template contains the following templates which generate 6 separate but connected workspaces at the same time: 

* 1.Global Classifications & Taxonomies
* 2.Fréscopa Global Marketing
* 3.Fréscopa Social Marketing
* 4.Fréscopa Media & PR
* 5.Fréscopa Global Events
* 6.Fréscopa Executive Company Leadership

For more information, see the following articles:

* [List of workspace templates](/help/quicksilver/planning/architecture/workspace-templates.md).
* [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md). 

## Fields

Fields are attributes that you can add to record types. Fields contain information about the record type. 

![Drop-down list of record fields](assets/drop-down-list-of-record-fields.png)

Considerations about record fields:

* The fields you add for a record type automatically become associated with all records of that type and can be used to capture data about those records. 

* Fields display as columns in the Table view applied to a record type page. They also display in the record's page. 

* Fields are unique to a record type and do not transfer from one record type to another. 

* Fields are fully customizable and are accessible only in Workfront Planning. You cannot access Workfront Planning fields from Workfront. 

For more information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).

A new record type is associated with the following predefined fields, by default: 

* Name
* Description
* Start Date
* End Date
* Status

You can create custom fields of the following types:  

* Single-line text 
* Paragraph   
* Multi-select 
* Single-select 
* Date 
* Number 
* Percentage 
* Currency
* Checkbox 
* Formula 
* People
* Created by
* Created date
* Last modified by
* Last modified date
* Approved by
* Approved date
* Record ID

<!--update the screen shot above-->

## Connected record types, records and fields

You can create a connection between the following entities in Workfront Planning:
    
* Two Workfront Planning record types.
* A record type and a Workfront project, program, portfolio, company, or group object type. 
* A record type and an Adobe Experience Manager asset or folder. 

    You must have an Adobe Experience Manager license to connect record types with Experience Manager objects.

    ![New connection tab with Workfront AEM options](assets/new-connection-tab-with-workfront-aem-options.png)

* A record type and an Adobe GenStudio for Performance Marketing Brand. 

    You must have an Adobe GenStudio for Performance Marketing license to connect record types with GenStudio Brands. 

    ![New connection tab with Adobe GenStudio Brand option](assets/new-connection-tab-with-genstudio-option.png)

After you establish a connection between the record types or the record and object types, you can connect individual records or objects of those types to one another. The connection between the records displays as a connected record field, or a connection.

Connecting record types is helpful when you have several types of work objects affecting one another. For example, you might work with campaigns and each campaign might cater to multiple brands. To indicate this relationship, you can connect campaigns to brands. Additionally, the work for each campaign might be planned out in multiple projects in Workfront. To indicate this, you can connect the campaigns to the relevant projects. Connecting record types, and subsequently connecting individual records achieves this relationship in Workfront Planning. 

## Lookup fields

After you establish the connection between two record types and you connect individual records together, you can reference the fields from the connected records from the record you are connecting from.

For example, if you connect a Campaign record type with a Workfront Project object type, you can display the Budget field of connected projects on the campaign records. 

![Add lookup fields box](assets/add-lookup-fields-modal.png)

>[!TIP]
>
>* You cannot add the following field types as lookup fields from the connected record or object types:
>
>   * Created by
>   * Last modified by
>   * Workfront typeahead fields (including fields like Project Owner, or Project Sponsor)
>

For information about connecting record types, records, and creating linked fields, see the following articles:

* [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md)
* [Connect records](/help/quicksilver/planning/records/connect-records.md)

<!--
not yet:* Fields are reusable across Record Types.
-->

## Hierarchies

After record types are connected within a workspace, you can create hierarchies that organize those connections. Hierarchies organize record and object types into parent–child relationships and can contain up to four object types. 

![Hierarchies in the workspace Settings area](assets/hierarchies-in-workspace-settings-area.png)

If a connection between two record types does not already exist, it can be created as you set up the hierarchy. Once defined, the hierarchy establishes a structured path across related record types within the workspace.

Hierarchies generate breadcrumbs for their respective records that display in their headers. This way, users know where they are in the hierarchy at any stage of their workflow. 

For general information about hierarchies and breadcrumbs, see [Hierarchy and breadcrumb overview](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md). 

## Views

Records display in their respective record type page in different types of views.

![View types drop-down from record type list](assets/view-types-drop-down-from-record-type-list.png)

Views contain personalized settings of a specific view type, such as the list of fields (columns), a list of records (rows), their order (sort), an applied or applicable filter and a grouping.  

The following are view types that you can apply to the record type page: 

* **Table view**: Displays records and their fields, including connected and lookup fields, in a table format. The rows of the table are the individual records, and the columns are the record fields. The table view is the default view. 

    ![Table view example](assets/table-view-example.png)

* **Timeline view**: Displays records that have at least two Date-type fields in a chronological timeline. You can display up to 5 connected record types and their records in the timeline view. 

    ![Grouping applied in timeline view](assets/grouping-applied-in-timeline-view.png)

* **Calendar view**: Displays records that have at least two Date-type fields in a calendar format. 
![Calendar view example](assets/calendar-view-example.png)

<!--
add List view here when it's possible to display Planning RTs in it??
-->

Additional view: 

* **List view**: You can display objects in a list view in the following areas of Workfront Planning:

    * Projects connected pages.
    * Request form list

    ![Projects connected page in a list view](assets/list-view-projects-connected-page.png)

For more information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

## Automations

You can configure automations in Adobe Workfront Planning that, when activated, create records in Workfront Planning when triggered from a Planning record. The created records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record type's page in Workfront Planning. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a Brand to associate with the campaign.

For information about how you create  objects using an existing automation, see [Create objects using Adobe Workfront Planning record automations](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md). 

## Request forms

You can create a request form and associate it with a record type in Adobe Workfront Planning. You can then share the form with others and they can submit requests to create records of that type. 

For more information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md). 