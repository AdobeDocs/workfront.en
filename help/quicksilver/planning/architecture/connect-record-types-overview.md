---
title: Connected Record Types Overview
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Adobe Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
---

<!--keep the 30 limit verbiage in yellow til Jan 2026-->

# Connected record types overview

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>   

You can indicate that individual record types relate to one another or to objects from other applications by connecting them. 

This article is an overview of record type connections and describes the types of connections you can establish between record and object types. 

For information about you connect record types, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 

## Considerations about connecting record types

There are two steps to connections in Workfront Planning: 

1. Establish a connection between two record types or a record type and an object type from another application. 

    For information about how you can connect record types, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 

1. Connect an individual record of one type with records of another type after the two record types are connected. For information about connecting records, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

Consider the following about connecting record types: 

* <span class="preview">You can have up to 30 connected fields for one record type in Workfront Planning.</span>

* You can connect the following entities in Adobe Workfront Planning:

    * Two record types. 

        By default, you can connect two record types from the same workspace. You can also set up record types to connect with record types from other workspaces. For information, see [Edit record types](/help/quicksilver/planning/architecture/edit-record-types.md).
    * A record type and an object type from another application. 

* You can connect Workfront Planning record types with the following object types from the following applications:

    * Adobe Workfront:

        * Projects
        * Portfolios
        * Programs
        * Companies
        * Groups

    * Adobe Experience Manager Assets:

        * Images
        * Folders

    * Adobe GenStudio for Performance Marketing

        * Brands

        >[!IMPORTANT]
        >
        >You must have have the following to connect with Adobe Experience Manager Assets and GenStudio Brands:
        >* An Adobe Experience Manager Assets license
        >* An Adobe GenStudio for Performance Marketing license
        >* Your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console to connect Workfront Planning records to Adobe Experience Manager Assets.
        >For information about the Adobe Admin Console, see the [Adobe Unified Experience FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* After you create records for record types, you can link them to each other through the connected record field.  

    For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

* After you connect a record type with another record type or with an object type from another application, the following scenarios exist: 
    
    * **When you connect two Planning record types**: A linked record field is created on the record type you're connecting from. A similar linked record field is created on the record type you are connecting to, only when you enable the Create corresponding field on linked record type setting on the New connection tab. 

        For example, if you connect the "Campaign" record type with the "Product" record type, a linked record field (connection field) that you name "Linked Product" is created on the Campaign record type. A linked record type automatically named "Campaign" is created on the Product record type.

        For example, the following scenarios exist: 

        * When you enable the Create corresponding field on linked record type setting and you connect the "Campaign" record type with the "Product" record type, a linked record field (connection field) that you name "Linked Product" is created on the Campaign record type. A linked record type automatically named "Campaign" is created on the Product record type.
        * When you disable the Create corresponding field on linked record type setting and you connect the "Campaign" record type with the "Product" record type, a linked record field (connection field) that you name "Linked Product" is created on the Campaign record type. A linked record type automatically named "Campaign" is not created on the Product record type.
    
        For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 

    * **When you connect a record type with an object type from another application**: 
    
        * A linked record field is created on the record type you're connecting from. No linked record field is automatically created on the other application's object type. 
        * Planning records fields are not accessible from Workfront objects.
        * Planning records are visible from the Workfront object's Planning tab. For information, see [Manage record connections from Workfront objects](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
        * You can create a Planning connection custom field and attach it to a Workfront object's custom form. For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). 
        * Planning record fields are accessible from Experience Manager assets when your Workfront administrator configures the metadata mapping through the integration between Workfront and Adobe Experience Manager Assets. For more information, see [Configure asset metadata mapping between Adobe Workfront and Experience Manager Assets](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).
        * Planning record fields are not accessible from the Brands in GenStudio for Performance Marketing. 
        

    * **When you add lookup fields from the record or object you connect to**: In addition to creating a linked record field, you can also connect to fields from the connected record or object type which are called lookup fields. A linked (or lookup field) with information from the record you're connecting to displays on the record that you're connecting from.

        You can connect fields from other record types or another application's objects to the Workfront Planning record type. 
    
        Linked fields are read-only and they automatically display information from connected records. 

        You can refer to lookup fields from other record or object types in formulas, filters, or groupings.

        For example, if you connect the "Campaign" record type with a Workfront project and you select to bring the Planned Completion Date field of the project to the Workfront Planning record, a linked field called Planned Completion Date (from Project) is automatically created for the campaign. You cannot manually edit this linked field. The Planned Completion Date (from Project) field displays the Planned Completion Date of the linked projects.  

        >[!IMPORTANT]
        >
        >Everyone with View or higher permissions to the workspace can view the information in the lookup fields, regardless of their permissions or access level in the application of the linked object types or their permissions in other workspaces. 

        Linked record fields are preceded by a relationship icon ![Relationship field icon](assets/relationship-field-icon.png). 
    
        Linked fields are preceded by an icon that identifies the field type. For example, linked (or lookup) fields are preceded by icons that indicate that a field is a number, a paragraph, or a date. 

        >[!TIP]
        >
        >Workfront objects' date field information displays in 24 hour format in Workfront Planning, regardless of how it displays in Workfront. 
        >
        >For example, if a project's Planned Start Date displays as 3:00 PM in Workfront, it will display as 15:00 in Workfront Planning in an imported lookup field. 


## Connection types

After you establish a connection between two record types or between a record and an object type from another application, you can add records in the connected record fields. 

>[!WARNING]
>
>The options described in this section are not available when connecting the following: 
>
>* Two records from different workspaces
>
>* A record type and Experience Manager assets
>
>* A record type and an Adobe GenStudio Brand

You can choose whether you want to connect one record to multiple records at a time, or one record at a time to each other. 

The following are the connection types you can choose from when connecting record types: 

* When the **Create corresponding field on linked record type** setting is disabled, you can choose from: 

    * [Multi-select](#multi-select-connection-type)
    * [Single-select](#single-select-connection-type)

* When the **Create corresponding field on linked record type** setting is enabled, you can choose from:

    * [Many to many](#many-to-many-connection-type)
    * [One to many](#one-to-many-connection-type)
    * [Many to one](#many-to-one-connection-type)
    * [One to one](#many-to-one-connection-type) 

### Multi-select connection type

![Multi-select connection type](assets/multi-select-connection-picker.png)

When you create a multi-select connection between record types, you can then select multiple connected records in the connection field from the original record type. 

For example, if you create a multi-select connection between campaigns and projects, you can select multiple projects for one campaign. A Campaign connected record type is not created for the Project object type.

After you select this connection type, you cannot change the connection type after you save it to any of the following types:

* Single-select
* One to many
* Many to one
* One to one

### Single-select connection type

![Single select connection type](assets/single-select-connection-picker.png)

When you create a single-select connection between record types, you can then select one record in the connection field from the original record type. 

For example, if you create a single-select connection between campaigns and companies, you can select one company for one campaign. A Campaign connected record type is not created for the Company object type.

After you select this connection type, you cannot change the connection type after you save it to any of the following:

* One to many
* One to one

</div>


<!--
* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)
-->

### Many-to-many connection type

![Many to many connection picker](assets/many-to-many-connection-picker.png)

When you create a many-to-many connection between record types, you can then select multiple records in the connection field from both record types. 

For example, if you create a many-to-many connection between campaigns and projects, you can select multiple projects for each campaign, and multiple campaigns for each project. 

A real-life example of a many-to-many relationship type is the relationship between movies and actors. Each movie can have multiple actors, and each actor can play in multiple movies. 

When you select this connection type, you cannot change the connection type after you save it. 

### One-to-many connection type

![One to many connection picker](assets/one-to-many-connection-picker.png)


When you create a one-to-many connection between record types, you can then select multiple records in the connection field in the current record type, but the corresponding connection field in the record type you connect to will allow selecting only one record. The connected record field that is automatically created on the second record type is automatically set to a many-to-one relationship type. 

For example, if you create a one-to-many connection between campaigns and projects, you can select multiple projects for each campaign, but each project can be connected to only one campaign.

A real-life example of a one-to-many relationship type is the relationship between libraries and books: a library has many books in its inventory; but one particular book can only be in one library at a given point in time. 

When you select this connection type, you can later change it only to a many-to-many connection type. 

### Many-to-one connection type

![Many to one connection picker](assets/many-to-one-connection-picker.png)


When you create a many-to-one connection between record types, you can then connect each record in the current record type with only one record from the connected record type. The connected record field that is automatically created on the second record type is automatically set to a one-to-many relationship type. 

For example, if you connect campaigns with projects and you choose this type of connection, you can add only one project to a campaign. But you can add multiple campaigns to one project. 

A real-life example of a many-to-one relationship type is the relationship between many movies and one actor: one actor can be in many movies, but each movie can only have a specific actor once in its cast. 

When you select this connection type, you can later change it only to a many-to-many connection type.

### One-to-one connection type

![One to one connection picker](assets/one-to-one-connection-picker.png)

When you create a one-to-one connection between record types, in both record types you can connect each record only with one record from the other record type.

For example, if you connect campaigns with projects and you choose this type of connection, you can connect one campaign with one project. One project can be connected only to one campaign. 

A real-life example of a one-to-one relationship is the one existing between a person and their country's unique identifier (like a Social Security Number, Passport ID, local identification ID): each person has only one unique identifier for a country and each unique identifier can be linked to only one person. 

When you select this connection type, you can later change it to any other connection type.
