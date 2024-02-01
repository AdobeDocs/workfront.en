---
title: Adobe Maestro overview
description: Adobe Maestro is a new offering from Adobe Workfront. You can create fully-customizable workspaces to define workflows that meet the needs of each organizational unit in your enterprise.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: b1d6e0b3-e6d4-46d1-a6a2-4b8b73f7d3f7
---
# Adobe Maestro overview

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!-- remove the references to closed beta from the entire article-->

<!--update the video in the IMPORTANT below, when we have something better, especially after Open Beta - remove it-->

>[!IMPORTANT]
>
>The information in this article refers to Adobe Maestro which is a new offering from Adobe Workfront. 
>
>Currently, Adobe Maestro is part of a beta program which is open to a limited number of customers. You must be a Workfront customer to use Maestro capabilities.
>
>Contact your account representative for more information about joining the beta program for Maestro.
>[View a video demonstration of Adobe Maestro](https://video.tv.adobe.com/v/3424253/){target=_blank}

## Introduction to Adobe Maestro

Adobe Maestro is a new offering from Adobe Workfront. The purpose of Maestro is to unlock comprehensive visibility into the operational details of an organization, and answer critical business questions at each stage of the work management lifecycle. 

Teams and leadership need clear answers to questions like:  

* How many Campaigns are we running in EMEA for Q4?
* Do we have any audience overlaps between concurrent Campaigns?
* How well are the awareness programs doing right now?
* What do the assets look like for a particular Campaign? Which of them must still be approved?

To answer these questions, leadership needs a solution that can provide a holistic view of every stage of work from planning to execution, from delivery to measuring the results. Currently, organizations have tools that can cover some parts of the process, but many do not have good connections to all phases of work, nor can they reliably provide results.  

The following are some of the main capabilities of Maestro:

* Solve the problem of managing work across all stages and for all the stakeholders that participate in the work process.  
* Fully customize your workflows, from deciding what object types (or record types) your organization uses to configuring how these objects link to one another.  
* Link to object types from other systems, creating a coherent framework for all your processes.  

## Currently available Maestro features

The following table illustrates the main features that will be available in Maestro, and a timeline of their availability. The list does not include all features.  

For information about new features and when they are released, see [Maestro release activity](/help/quicksilver/maestro/release-activity.md). 

|       Feature                                      |     Available now  |     Available soon   |     In research  |
|----------------------------------------------------|:-----------------------------:|:--------------------------------:|:----------------:|
|     Create workspaces                              |   ✓                           |                                  |                  |
|     Create operational record types                |   ✓                           |                                  |                  |
|     Create taxonomies                              |   ✓                           |                                  |                  |
|     Create individual, named records and taxonomies|   ✓                           |                                  |                  |
|     Create record custom fields                    |   ✓                           |                                  |                  |
|     Import record types and fields using an Excel  or CSV file                              |   ✓                           |                                  |                  |
|     Link records                                   |   ✓                           |                                  |                  |
|     View records in a table                        |   ✓                           |                                  |                  |
|     View records in a timeline                     |   ✓                           |                                  |                  |
|     Filter records                                 |   ✓                           |                                  |                  |
|     Group records in the timeline view             |   ✓                           |                                  |                  |
|     Group records in the table view                | ✓                              |                                 |                  |
|     Sort records in the table view                                 |  ✓                             |                                 |                  |
|     Sort records in the timeline view                                 |                               |   ✓                              |                  |
|     Sort groupings in the table view                                 |                               |   ✓                              |                  |
|     Sort groupings in the timeline view                                 |                               |   ✓                              |                  |
|     Connect workspaces                                |                               |   ✓                              |                  |
|     Connect Maestro records and taxonomies  |   ✓                            |  
|   Search for records in the table view    | ✓    |   |
|   Search for records in the timeline view    | ✓    |   |
|     Connect Maestro records to Workfront projects, programs, portfolios, companies, groups  |   ✓                            |                                 |                  |
|     Connect Maestro records to Adobe Experience Manager assets                                  |      ✓                         |                                  |                 | 
|     Record details page                            |   ✓                           |                                  |                  |
|     Update the layout of the record Details page              |                               |   ✓                              |                  |
|  Share workspaces | ✓| |  |
|  Share views |✓ | |  |
|     Submit requests                                |                               |                                  |   ✓              |
|     Creative brief                                 |                               |                                  |   ✓              |
|     Customize the color and icon of a record                                 |      ✓                         |                                  |                 |
|     Add comments to records                                 | ✓                              |                                  |                 |
|     Add thumbnails to records                                 | ✓                              |                                  |                 |
|     View history of changes on a record                                 | ✓                              |                                  |                 |
|     Rich Text formatting for Paragraph fields                                 |      ✓                         |                                  |                 | 
|     Maestro Modules for Adobe Workfront Fusion                                 |      ✓                         |                                  |                 | 
|     Copy and paste information from one field to another                                  |      ✓                         |                                  |                 | 

## Enable Maestro for the users in your Workfront instance

Your organization must enroll in the Adobe Maestro closed beta program before you can access Maestro. Contact your account representative for information about enrolling in the beta program. 

For more information about granting access to and enabling others to use Maestro, see [Access overview](/help/quicksilver/maestro/access/access-overview.md). 

## Maestro terminology

Although Maestro is part of Workfront, it comes with proprietary concepts and terminology. Ensure you are familiar with the Maestro concepts before embarking on setting up Maestro for your organization. 

The framework for Maestro is fully customizable. You can create all record types, their attributes, and any fields associated with them to suit the exact needs of your organization. 

The following are the main Maestro objects and concepts: 

* **Workspace**: A collection of record types and taxonomies that define the operational lifecycle of a certain organization. A workspace is the work frame of an organizational unit. 

    One Workfront instance can have a maximum of 1,000 workspaces.

    ![](assets/marketing-workspace-with-record-type-taxonomies-opening-page.png) 
    
    For more information, see [Create workspaces](../maestro/architecture/create-workspaces.md). 

* **Record Type**: The Maestro main object type.  
    
    Unlike Workfront where the object types are predefined, in Maestro, you can create your own object types.  
    
    For example, in Workfront the object types of Program, Portfolio, Project, Task, or Issue are already created.  
    
    In Maestro, you can create any record types that meet your organization's workflows. Later, you can define how the record types relate to one another or form dependencies. 
    
    For more information, see [Overview of operational record types and taxonomies](../maestro/architecture/overview-of-record-types-and-taxonomies.md).

    Maestro has the following record types: 

    * **Operational Record Type**: A record type that represents strategic plans, initiatives, or executed work.  

        ![](assets/operational-record-type-blank.png)

        For example, Campaign, Activity, Program can be operational record types.  

        For more information, see [Create record types](../maestro/architecture/create-record-types.md).

    * **Taxonomy**: A record type that captures attributes about an operational record type. 

        ![](assets/taxonomy-record-type-blank.png)

        Although creating taxonomies is identical with creating operational record types, Maestro distinguishes between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->  

        For example, Audience, Region, or Address can be taxonomy-type record types.  

       For more information, see [Create taxonomy record types](../maestro/architecture/create-a-taxonomy.md).

* **Record**: An instance of a Maestro record type. A record could refer to an operational record type or to a taxonomy. 

    ![](assets/records-highlighted-in-campaign-record-type-list.png)
    ![](assets/records-highlighted-in-region-taxonomy-type-list.png)
    
    After adding a record type to a workspace, you can start adding records of that type on the record type's page. 

    For example, "Campaign" can be an operational record type and "Summer Campaign for EMEA" is a record of the Campaign record type 
    
    Or 
    
    "Region" is a taxonomy-type record type, whereas "Americas-Latin America" or "EMEA - Central Europe" are taxonomy records.  
    
    For more information, see [Create records](../maestro/records/create-records.md).

* **Workspace template**: You can create a workspace using predefined templates. You can use the predefined record types, taxonomies, and fields that come in a template, or you can add your own. 

    ![](assets/workspaces-page-with-templates-thumbnails.png)

    Maestro comes with a Sales, Marketing, and Product Management workspace template. 
    
    For more information, see [Create workspaces](../maestro/architecture/create-workspaces.md).

* **Fields**: Fields are attributes that you can add to operational or taxonomy record types that contain information about the record type. <!--check the shot below, "Connection" needs to be in lowercase-->

    ![](assets/drop-down-list-of-record-fields.png)

    Considerations about Maestro fields:
    
    * The fields you add for a record type automatically become associated with all records of that type and can be used to capture data about those records. 

    * Fields display as columns in the Table view applied to a record  type page. They also display in the Details page of the record. 

    * Fields are unique to a record type and do not transfer from one record type to another. 

    * Maestro fields are fully customizable and are accessible only in Maestro. You cannot access Maestro fields from Workfront. 

    For more information, see [Create fields](../maestro/fields/create-fields.md).
    
    A new operational record type is associated with the following predefined fields, by default: 

    * Name
    * Description
    * Start Date
    * End Date
    * Status

    A new taxonomy record type is associated with a Name field, by default. 

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
   
* **Linked record types**, **Linked records**, and **Linked record fields**:  You can create a connection between the following entities:
    
    * Two Maestro record types
    * A Maestro record type and a Workfront project, program, portfolio, company, or group object type. 
    * A Maestro record type and an Adobe Experience Manager asset, folder, or collection. 

        You must have an Adobe Experience Manager license to link record types with Experience Manager objects.

        ![](assets/new-connection-tab-with-workfront-aem-options.png)


    After you establish a connection between the record types, you can connect individual records of those types to one another. The connection between the records displays as a linked record field. 

* **Linked fields** (or lookup fields): After establishing the connection between two record types and you link individual records together, you can reference the linked records' fields on the record you are connecting from.

    For example, if you connect a Maestro campaign with a Workfront project, you can display the Project Owner field of connected projects on the Maestro campaign records. 

    ![](assets/add-lookup-fields-modal.png)

    For information about linking record types, records, and creating linked fields, see the following articles:

    * [Connect record types](../maestro/architecture/connect-record-types.md)
    * [Connect records](../maestro/records/connect-records.md)

<!--not yet:* Fields are reusable across Record Types.  -->

* **Views**: Records display under their respective record type page in different types of views. 

    ![](assets/view-types-drop-down-from-record-type-list.png)

    Views contain personalized settings of a specific view type, such as the list of fields (columns), a list of records (rows), their order (sort), an applied or applicable filter and grouping.  
    
    The following are view types that you can apply to the record type page: 

    * **Table view**: Displays records and their fields in a table format. The rows of the table are the individual records, and the columns are the record fields. This is the default view. 

        ![](assets/table-view-example.png)

    * **Timeline view**: Displays records that have at least two Date-type fields in a chronological timeline. 

        ![](assets/grouping-applied-in-timeline-view.png)

    For more information, see [Manage record views](../maestro/views/manage-record-views.md).


## Maestro object limitations

The following table shows the limits for how many objects you can create in Maestro. The limitations are subject to change as we move into the next phases of Maestro's development.  

|       Maestro object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes taxonomies for the workspace, or objects that you import from third-party applications)  |
|     Number of records for one record type                                               |   10,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Size of CSV of Excel file you can import in a table | 5MB |

## Locate Maestro

Ensure that your organization has received access to Maestro and that your system or group administrator has added the Maestro area to your Main Menu. For information, see [Access overview](/help/quicksilver/maestro/access/access-overview.md) .

To locate Maestro:  

1. Log in to Adobe Workfront. 

1. Click the **Main Menu** ![](assets/main-menu-workfront.png) in the upper-right corner, or click the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it's available. 

1. Click **Maestro** ![](assets/maestro-icon.png). 

    The Maestro Workspaces area opens. 

1. (Optional and recommended) Continue with some of the following actions, to build your work structure in Maestro: 

    1. Create a workspace from scratch or using a template. 

    1. Add record types to the new workspace. 

    1. Add taxonomies to the new workspaces. 

    1. Click the name of a record type to open the record's page. The record page opens in the Table view, by default.
    
    1. Customize the Table view by doing any of the following:

        * Add more fields to the record type by clicking the **+** icon in the upper right corner. The columns in the view are fields associated with the record type. 
        * Add records by clicking the **+** icon in the lower-left corner. The rows in the view are unique records of the selected record type. 
        * Click **Filters** to filter the information you display on the record type page. 

    1. Click the name of a record to view more information in the record's Details page. 

    1. Create a Timeline view from the **View** drop-down menu in the upper-right corner of the record type page. 

    1. Customize the timeline view by updating Filters, Groupings, or Settings.  

## Maestro release activity 

We are releasing new features to Maestro regularly. For an up-to-date list of released features, see [Adobe Maestro release activity](../maestro/release-activity.md). 


