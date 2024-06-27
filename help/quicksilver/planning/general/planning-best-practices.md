---
title: 'Adobe Workfront Planning best practices'
description: As a marketing operations leader, you can use Adobe Workfront Planning to organize work across the marketing lifecycle for all your teams. These are some best practices that we recommend when starting with Workfront Planning. 
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
---

# Adobe Workfront Planning best practices

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

As a marketing operations leader, you can use Adobe Workfront Planning to organize work across the marketing lifecycle for all your teams. 

This article documents some best practices that we recommend when starting with Workfront Planning. 

## What is Workfront Planning?

The Workfront Planning module is one of three distinct but connected Workfront capabilities that together create a marketing system of record. The three capabilities are:  

* **Planning**: The new advanced capabilities included in Workfront Planning. 

* **Workflow**: The collaborative work management capabilities that you use today in Workfront (project management, resource management, etc.)  

* **Automation and integration**: The comprehensive integration and automation capabilities powered by Workfront Fusion. 

Workfront Planning is highly customizable. For more information on Workfront Planning terminology and key concept, see [Adobe Workfront Planning overview](/help/quicksilver/planning/general/planning-overview.md). 

## Questions to ask before setting up Workfront Planning

After you have familiarized yourself with the Workfront Planning terminology and architecture, you can start setting up your new environment. 

Some questions you might ask yourself as you set up Planning are: 

* **Do I want to use workspaces for larger organizational groups? Or should I encourage people to set up personal ones?**

    You might find that there is a good use for both. We recommend not to have too many workspaces as they could become hard to manage and your workflows might be too fragmented. 

    >[!TIP]
    >
    >    You can have 1,000 workspaces in one Workfront instance.

* **What custom record types should I create in each workspace?** 

    Record types are like Workfront's object types. Think about your workflows and decide what record types (work objects, people objects, taxonomies, etc.) each workflow might need. 

    For information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md)

* **How am I going to create my records? Is there an external list or spreadsheet that already contains the records I need to add to Planning that I can use? Will records be added gradually depending on need? Or will they be imported using a Fusion or custom API integration?** 

    For information, see: 

    * [Create records](/help/quicksilver/planning/records/create-records.md)
    * [Adobe Workfront Planning modules](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-planning-modules.md)

* **What fields do I need to create for my records?** 

    For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md). 

* **What Workfront or AEM Assets object types do I need to connect to Workfront Planning record types to be able to show dependencies and to create a seamless workflow for my organization?** 

    For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md)

* **What Marketing calendars and views will I need to tell the story of my campaigns? And what stakeholders could I make these views available to for seamless collaboration?**

    For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 


## Workfront Planning best practices

This section lists several dos and don'ts and best practice guidelines when setting up Workfront Planning. 

The guidelines are organized depending on the object or the area you are setting up. 

### Workspaces 

#### The do's and don'ts of workspaces

* Do design for the lowest volume of organization level Workspaces 

    For example, try to create a single Workspace for all of Marketing 

* Do curate your workspaces periodically. You may find that you could modify an existing one rather than build a new one from scratch. 

* Do create a new Workspace for a team that has a completely different operational motion.

    A "Product Development" workspace should be distinct from a "Marketing" workspace 

* Don't create a unique workspace for every little thing. Think of workspaces more as a system of record that can benefit an entire organization and allow everyone to map workflows and collaborate rather than a private space for keeping track of personal requests. 

* Don't create unique Workspaces for each team or process within an organization. 

    The Marketing organization should strive to maintain just one workspace to maintain visibility and allow data to roll-up at the global planning level. 
    
    Avoid creating similar or duplicate workspaces for teams that follow similar processes (e.g. EMEA marketing VS APAC marketing), especially where these teams may do work that rolls up to a common strategic campaign. 

#### How should I use workspace sections? 

* Create and label sections to help your users understand how you organize your operational lifecycle. 

    For example, you might create a section called "Core records" where you place your Campaigns, Tactics, and Deliverables. 

* Group "like" record types together. 

    You might create a section called "Geographies" which contains record types like: Region, Country, and City. 

#### How should I manage workspace permissions? 

* Do restrict "Manage" access to a select group of trusted people, who will not accidentally delete a record type, or otherwise create unnecessary record types and fields.

    >[!TIP]
    >
    >We have found out during our beta program that many customers feel like they would grant "Manage" access to group administrators. 

* Do add the Planning area to the layout template of users with a Standard license.

* Do allow users with a Standard license to create personal workspaces. This gives them a safe space to learn the tool and become comfortable with it. This will not clutter the experience for others and may improve the user's personal productivity. 
    
    >[!TIP]
    >
    >    Advice them to not share their personal workspaces as a best practice.


### Record Types 

#### A single or multi-select field vs a linked record type

* Do build a new record type if the object will be used in multiple other record types 

    For example, a Campaign may have a connection to multiple Target Audiences, and a Tactic might have a connection to a single Target Audiences.  

* Do build a new record type if the object needs to store additional metadata values that could be useful in lookups.  

    For example, a Channel record type such as "Email" may store a list of supporting Deliverables, either as native metadata, or as a connection to standalone "Deliverables" record type. 

* Don't add a new record type if the data you are storing only  needs to be scoped to a single record type. Use a select field instead. 

    For example, a Campaign record type may have a single-select field called Campaign Size which is only relevant when directly associated with a specific Campaign. 

#### How should I label my record types? 

Do create and label record types that represent a single construct or noun, such as "Campaigns" 

:no_entry_sign: Don't create a record type that is better represented as a view-layer - e.g. "Calendar" is a poor choice for a record type, because it is not the record type itself, but a view of records. 

### How many layers of hierarchy should I create? 

Views 

... 

Workflow 

... 

### Field Management 

Primary field 

Do use unique primary field values to make it easier to find and "pick" those records when making connections. 

When making a connection, users will search by the values in the Primary field and if they are not unique, users will not know which one to pick. 

 Avoid using non-unique values as the primary field because it can create confusion for users who have to search on the primary field when using the connections picker menu. 



From Chris O'Neal: 

Another do/don't area to think about are use cases that are (or aren't) best uses of Planning. For example, the resource management discussion we had today. 



Alina's notes: 

Example of "Best practices" article from ExL: https://experienceleague.adobe.com/en/docs/commerce-operations/implementation-playbook/best-practices/planning/sites-stores-store-views  

Additional information from Field Readiness from Lauren S.: https://fieldreadiness-adobe.highspot.com/spots/5fd14ae8b7b7390523f57346  