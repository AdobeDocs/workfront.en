---
title: Adobe Workfront Planning Best Practices
description: As a marketing operations leader, you can use Adobe Workfront Planning to organize work across the marketing lifecycle for all your teams. These are some best practices that we recommend when starting with Workfront Planning. 
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
---

<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Adobe Workfront Planning best practices

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

As a marketing operations leader, you can use Adobe Workfront Planning to organize work across the marketing lifecycle for all your teams. 

This article documents some frequently asked questions and best practices that we recommend when starting with Workfront Planning. 

## Configuration best practices

### Workspaces

Workspaces are centralized locations for teams to plan work. A workspace is a collection of record types used by a team and represents the team's work lifecycle.

The following are some frequently asked questions about configuring Workfront Planning. 

#### How should I start?  

* ✅ When you log in to Planning for the first time, follow our in-app onboarding process that clearly communicates Planning's value and guides you on how to navigate and utilize the product effectively. This ensures that you understand its capabilities and how to begin your work with ease. 
* ✅ Start by exploring our predefined workspace templates for ideas of existing similar use cases. You can use the predefined record types and fields that come in a template, or you can add your own.  
* ✅ Identify the main use cases you want to solve with Workfront Planning. For example, most organizations want to improve visibility into strategic activities, which may include building a better "Campaign Calendar". So, for that use case, you would want to start by answering a few questions: 

    * Who is asking for it? 
    * What do they call the things they want to put in the calendar? 
        Campaigns? Tactics? Initiatives? Activities? Events? 
    * What kinds of questions do they want to answer with this calendar? 
    * Do we have any overlapping campaigns for the same audience?
    * What's our budget for that campaign, tactic, activity, or event?
    
    The answers to these questions would dictate what you need to build inside of Workfront Planning. 
    
    Also, consider that there might be other planners who are currently not Workfront users. These planners may operate out of Excel spreadsheets, Word Docs, PowerPoints, etc. Consider how they might access your information in Workfront Planning.          

* ✅ To take full advantage of Workfront Planning, consider replacing the use of Portfolios and Programs in Workfront Workflow with some other upper-tier structure in Workfront Planning. 

    Today, Workfront customers represent their strategic work through portfolios and programs, in some cases as projects of different types. With the introduction of Planning, all such strategic work should be handled through custom record types in Workfront Planning, while Workfront will be centered around the execution phase of work represented as projects and tasks.   


#### When should I create a new workspace versus modifying an existing one? 

* ✅ Design for the lowest volume of organization-level workspaces. You can create workspaces for specific operational organization units, to match the unique way each unit works. 

    Having the information in a single Workspace, to ensure that relationships between all data can be easily managed.  

    For example, try to create a single workspace for all of Marketing.
    
    It's ok to create a new workspace for a team that has a completely different operational structure: 

    For example, a **Product Development** workspace should be distinct from a **Marketing** workspace. 
    
* ⛔ Don't create unique workspaces for each team or process within an organization.

    The Marketing organization should strive to maintain just one workspace to maintain visibility and allow data to roll up at the global planning level. 
    
    Avoid creating similar or duplicate workspaces for teams that follow similar processes (for example, EMEA Marketing versus APAC Marketing), especially where these teams may do work that ladders up to common strategic campaigns. 

#### How should I use Workspace Sections? 

* ✅ Create and label sections to help your users understand how you organize your operational lifecycle.

    For example, you might create a section called **Core records** where you place your Campaigns, Tactics, and Deliverables in your workspace.  
* ✅ Group "like" record types together.

    For example, you might create a section called **Geographies** which contains record types like: Region, Country, and City.  

### Record Types

Record types are the building blocks of a Workfront Planning Workspace. You can define how record types are interconnected.  


#### How should I define record types in my workspace?  

* ✅ Take some time to identify what information you need to track (what record types I need) and how this information needs to be connected. Talk with the stakeholders that will use the workspace to consider all their needs. You can also create custom sections with different record types to present the information in a very consumable way.  


* ⛔ Don't duplicate record types for a different period (for example, don't create separate record types for **Campaigns 2024** and **Campaigns 2025**). 

    Creating different record types breaks the flow of data, whenever you want to compare data across multiple years. The views today are per record type, so as soon as the year ends, the view of that record type will no longer show the future items. The best practice is to have one record type for the type of work and segment the data using filters or archiving it, if needed. 
       
#### When should I use a single or multi-select field versus a linked record type? 

* ✅ Add a new record type if the object will be used in connection with multiple other record types 

    For example, a Campaign may have a connection to multiple Target Audiences, and a Tactic might have a connection to a single Target Audience. Therefore, Campaign, Tactic, and Audience should be record types rather than multi-select fields.  

* ✅ Add a new record type if the object needs to store additional metadata values that could be useful in lookups 

    For example, a channel record type such as **Email** may store a list of supporting deliverables, either as native metadata, or as a connection to a standalone **Deliverables** record type. 
* ⛔ Don't add a new record type if the data you are storing is only relevant for a single record type.  

    For example, a **Campaign** record type may have a single-select field called **Campaign Size** which is only relevant when directly associated with a specific campaign. 

#### How should I label my record types? 

* ✅ Do create and label record types that represent a single construct or noun, such as **Campaigns**. 
* ⛔ Don't create a record type that is better represented as a view. 

    For example, **Calendar** is a poor choice for a record type, because it is not the record type itself, but a view of records.  

### Field management

Fields are attributes of record types and are displayed as columns in the table view. You can create custom fields for record types and then associate the fields with Workfront Planning records to enhance record information. 


#### What field is recommended to be defined as Primary field?


* ✅ Do use unique primary field values to make it easier to find and "pick" those records when making connections.  

    When making a connection, users will search by the values in the Primary field and if they are not unique, users will not know which one to pick.  
* ⛔ Avoid using non-unique values as the primary field because it can create confusion for users who must search on the primary field when using the connections picker menu.  

#### How should I use formulas? 

* ✅ Do use Formula field types to reduce manual input. When you are entering information based on data that's already in your table view, you may be able to save some effort by calculating that information automatically using formulas. 

#### How should I start connecting the data in my workspace?   

* ✅ Creating connections is one of the most powerful features of Workfront Planning. You can connect record types to one another or record types with object types from other applications like Adobe Workfront (connection to Projects, Portfolios, Programs, Companies, and Groups) and with Adobe Experience Manager Assets (connection to assets and folders). 

    Connecting object and record types gives you a full overview of how everything in your company is connected.   
 
    For example, you have a **Campaign** record type, and a **Tactics** record type, and you can create a connection between these two record types to see which **Tactics** are associated to a specific **Campaign**. 
    
    After defining the connection, all the people in the workspace can start adding values for **Campaigns** by double clicking into the connection field where they will see a list of all the **Tactics** available. This allows you to quickly find which tactics need to be associated with your campaigns.  

#### How should I use lookup fields?   

* ✅ After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. You will reduce the number of places you have to update the same piece of information, and ensure they match perfectly.  

    For example, once you have a connection between a **Campaign** record type and a **Tactics** record type, you will see the primary field information, but when you add lookup fields, you will be able to bring additional information from that record type, like the **Launch date** for that **Tactic**. The data for these lookup fields is auto populated after the records are added.          

#### What field type is recommended for URLs?  

* ✅ Do use a Single-line text field to add a URL data to a record.  

### Views

#### How do I decide what should be a view versus a record type?

* ✅For things that represent a single construct or noun (such as **Campaigns**), do create a record type.  

* ⛔ Don't create a record type that is better represented as a view. 

    For example, **Calendar** is a poor choice for a record type, because it is not the record type itself, but a view of records.  

#### Should I hide or delete the fields that are not relevant for me?  

* ✅ Hide the column instead of deleting it when this information could be relevant for a different person using the same record type. If you delete the field in a specific table view, this field will be also deleted in the rest of the views of this record, as well as everywhere else this record type is linked from.  

#### How should I use filters and groupings in the table and timeline views?  

* ✅ Use views with filters and groupings to display a snapshot of what you need to see. You can filter and group the data to have a more consumable way to understand what's planned. You can group the records by metadata fields. 

    For example, you can have a timeline view for your **Campaign** record type which you can group by **Target Audiences** and filter it by **Date** to show only the current year.

#### Why don't I see all the records in my timeline view? 

* ✅ Remember to define 2 date fields for your records. You can create a timeline view only when you have at least two date fields associated with a record type. Some records might not display in the timeline view when either the Start or End dates or both have no values and when the Start date is after the End date.  

#### How should I use the timeline view Settings

* ✅ Define the settings of your timeline view, like the **Bar style** and the **Color** to get a more visually enriching view. You can customize the **Bar style** by defining whether you want to see a thumbnail with a meaningful image and to add more fields to display on the bar (for example, **Owner** or **Status**). 
    
    By default, you only see the primary field. You can also define the color of your bar by field values (for example, you can customize the colors of your bars by matching it to the Status field) or by the grouping you have applied. By default, the color matches the color of the record type. 
    
    Only record type colors or fields with options associated with colors can affect the colors of the record bars in the timeline.   

### Permissions and sharing

Use the sharing feature to give appropriate permissions to employees to views and workspaces.  

#### How should I manage permissions to workspaces?

* ✅ When you create a **workspace**, it is only available to you. Anyone else aside from System Administrators will not be able to find it. Once the workspace is defined and you are ready to bring your team to start the collaboration, you need to share it with them and define their permission level. 

    You can choose from the following permission levels:

    * **Manage**: People can edit, delete and share the workspace. 
    * **Contribute**: People can create, edit and delete records.
    * **View**: People can view records.  

* ✅ Although many customers feel like they would grant **Manage** permissions to workspaces to most people, do restrict the **Manage** permissions to a select group of trusted people who will not accidentally delete a record type or otherwise create unnecessary record types and fields. They can edit, share, and even delete the workspace. This level of permissions grants them full administrative access to the Workspace.

    A Standard user license is required for someone to have Manage permissions to a workspace.  

* ✅ Give users **Contribute** permissions if you want them to just be able to create, edit and delete records, but you don't want them to change the structure, and the schema of the workspace. With **Contribute** permissions, they cannot create record types or change the fields on the existing record types.   

    A Standard user license is required for someone to have **Contribute** permissions to a workspace.  

* ✅ Give users **View** permissions, if you want them just to view records.  

    >[!NOTE]
    >
    >Right now, we don't have specific permissions for record types or records, so this means that all records in any of the record types are visible if you grant someone **View** access to the workspace.   

#### How should I manage permissions to views? 

* ✅ Do restrict **Manage** permissions to people that you want to be able to edit, delete and share the view. This means that they can change the filters, grouping fields or some configuration of the view. Those changes will affect the main configuration of the view for everyone else who is also using the view.  

    A Standard user license is required for someone to have Manage permissions to a view. 
      
* ✅ Give users **View** access to be able to apply the view. They will be able to change some of the filters or groupings and sorting, but those changes will be only temporary; the changes are not saved for all other users accessing the view. Those changes will not affect the main configuration of the view for everyone else who is also using the view.  Their changes are only visible to the user who is applying the modified settings. After refreshing the screen, the changes are reset to the default.  

* ✅ Give **Everyone in the workspace can view** permissions when you want everyone who can view the workspace to see the records and their fields in that specific view. This way, you don't need to add anyone manually to the sharing permission box for the view. 

    >[!NOTE]
    >
    >If a view hasn't been shared and you share a link to it with other people, they will be able to see the records in the **Default Table View**. If they have a Standard Workfront license, they can build their own view. 


#### How is **Workspace sharing** different than **View sharing**?  

* **Workspace sharing** defines people's access to the workspace, its record types, records, and their fields. 

* **View sharing** defines whether the user can see the View that you have created and whether they can change the filter, grouping fields or some other configuration of the view. The visibility of the records displayed within the View is controlled by Workspace sharing, and not by View sharing.  

#### How Workfront license types affect Workfront Planning permissions?  

* For **Workspace sharing**: Light and Contribute license users can only get View access to a workspace. To grant someone Contribute or Manage permission to a workspace, they need to have a Standard license. 

* **Views sharing**: Standard license users that have Manage permissions to a workspace will be able to create a view. Light and Contribute license users can only utilize the views that Standard users have created and shared with them. Otherwise, if nothing has been shared, users will be able to see the **Default Table View**.  

     
#### What should I do when a Workspace owner changes?  

* Workfront sets the workspace creator as the owner, but functionality-wise the owner has the same permissions as any user with Manage permissions. 
* If the owner is deactivated, other members can continue their work in the workspace without any disruptions. 
* System administrators have access to any workspace, so if the owner was the only person with Manage permissions, administrators can add another person and grant them Manage permissions to handle the management of the workspace. 

### Submitting requests in Workfront Planning

You can create a request form for each record type when you want users to add records outside a record type's page. Submitting the form adds a new record to the record type. 

#### When should I start creating an request form for a record type?

* ✅ You should ensure the record type structure is set up first by adding the necessary fields to the table. These fields describe your records and will be accessible in the form builder. 

    Ideally, build the request or intake form after your record type structure is finalized to avoid missing any key fields.      

#### Who can create request forms?

* ✅ Any user with Manage access to the workspace can create or edit a request form. Make sure the user's permissions are properly assigned to allow this functionality.          

#### How should I create or edit a request form for a record type?

* ✅ Any user with Manage access to the workspace can follow the steps described in the article [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md). 


#### Who will be able to submit new records using the request form?

* ✅ Submission permissions depend on the settings you configure for each form. 

    In the form builder, after you publish the form, you can manage permissions to control who can submit requests. 
    
    You can choose from the following three sharing options: 

    * **Anyone with view or higher access to the workspace:** Allows all users with View or higher permissions to the workspace can submit a request that creates a record. 
    * **Anyone with contribute or higher access to the workspace**: Restricts submissions to users with Contribute or higher permissions to the workspace. 
    * **Anyone with the link:** Enables anyone who has the form link to submit a request. 
    * **Expiration date:** Ensure you set an expiration date for the public link to enhance security.  

### Best Practices for managing request forms

The following are recommendations for managing request forms: 

* Plan ahead: Clearly define what information is needed or required from requesters before creating the form to avoid excessive revisions later. 
* Use clear labels: Ensure that field labels and descriptions are clear and understandable for all users. 
* Test forms: Before rolling out new forms to a wider audience, test them using the form link and form previewing option to ensure all fields and logic function as expected. 
* Keep forms updated: Periodically review forms and update them to match any changes in the record type structure or operational processes. 

<!-- this is hidden, per Andrea:  

2.2 Migration  

Migrating your data from external <span style="text-decoration:underline;">s~~S~~</span>ystems to Workfront Planning unlocks new ways to create important connections in your workflow and uncover insights that you might not have been able to identify with your previous tools. 

By having all your data in one central location, you can more easily form connections between your Workfront data than if they all existed in separate tools. 

We have some options that will help you to accelerate the migration process:  

* **Fusion** – You can create a Scenario in Fusion that runs after certain criteria and connects objects. 
* **Bulk Data Operations** _through the new functionality -[ [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE)  (Q3 2024)_ -  
* **Copy and paste – **You can copy and paste directly from a spreadsheet. This is best suited to a simple table of data from tools like Excel or Google Sheets.  
* **Upload a C<span style="text-decoration:underline;">SV~~VS~~</span> or Excel **- The CSV (comma-separated values) format or Excel is one of the most common ways to move data between applications, and tools. This functionality is not available yet, but we are planning to work on it in Q4 2024.  

-->     

<!--
     

1. Data Flow  

Currently the metadata modelling in Workfront Planning is done by Ops Admins through adding various data points to the record type from the table view, including: 



* Fields added directly on the current record type 
* Connections with custom defined operational and taxonomical record types 
* Connections with execution work captured in Workfront 
* Connections with deliverables stored as assets in AEM 
* Any lookup fields captured in any of the above connections. 

Here is a summary of how you can define the data flow within Workfront Planning and other applications.  


     



* **Connections and Lookup fields. **Creating **connections** is one of the most powerful features of Workfront Planning. You can connect record types to one another or record types with object types from other applications like Adobe Workfront (connection to Project, Portfolios, Programs, Companies, and Groups) or Adobe Experience Manager Assets (connection to assets and folders).  Connections give you a full overview of how everything in your company is connected.  

    - e.g.: You have a Campaign record type, and a Tactics record type, then you can create a connection between these two record types to see to see which Tactics are associated to a specific Campaign. After defining the connection, all the people in the workspace can start adding values by double-clicking into the connection field that displays the tactic where they will see a list of all the Tactics available and you can quickly select the tactics to be associated with each campaign. 


    After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. The connected fields are called **Lookup fields**. You will reduce the number of places you have to update the same piece of information and ensure that they match perfectly.  


    - e.g.: Once you have a connection between a Campaign record type and a Tactics record type, you will see the primary field information when you add the tactic, but when you add lookup fields, you will be able to bring additional information from the tactic, like the Launch date for that Tactic. The data for these lookup fields is auto populated. Find more information in the Adobe Experience League documentation in the article about Connecting records.  


     

* **Planning (or Connections) tab** **in Workfront _-[ [E] Global Connect capability in Planning connections area](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6617d7760001e250f5ffb9ebf04baacc/overview?source-id=unifiedShareMFE)_** 

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* **Create new records within the connection fields_ -[E] In-context creation of connected records](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE)~~.~~  _**When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see [Create records](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records).   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->