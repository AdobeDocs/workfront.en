---
title: 'Adobe Workfront Planning FAQs'
description: As a marketing operations leader, you can use Adobe Workfront Planning to organize work across the marketing lifecycle for all your teams. These are some frequently-asked questions about Workfront Planning. 
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
---

# Adobe Workfront Planning FAQs

<!-- add to TOC and mini TOC-->

This article contains a list of the most commonly-asked questions about Adobe Workfront Planning. 

For more information about the Workfront Planning, see [Adobe Workfront Planning overview](/help/quicksilver/planning/general/planning-overview.md). 

## What is Workfront Planning? 

Formerly called Project Maestro, Workfront Planning is a new capability that enables teams to centralize their planning for end-to-end operations, such as for campaigns, sales, product management, services, and more. Planning unlocks your ability to model your ideal system of record with custom records, flexible connections across your operational lifecycle, and enhanced visibility for all stakeholders. 

## How does Workfront planning fit into the broader Workfront product? 

The Workfront Planning module is one of three distinct but connected Workfront capabilities that together create a marketing system of record. The three capabilities are:  

* Planning: The new advanced capabilities included in Workfront Planning. 

* Workflow: The collaborative work management capabilities that you use today in Workfront (project management, resource management, etc.).  

* Automation and integration: The comprehensive integration and automation capabilities powered by Workfront Fusion. 

## When will Workfront Planning be released? 

The latest planned Workfront Planning  release to the general audience is August 28th, 2024. For up-to-date information about what features are currently released, see [Adobe Workfront Planning release activity](/help/quicksilver/planning/general/release-activity.md).  

<!-- To verify this: are we even saying "Beta"? - What happens after the beta program concludes? 

Beta participants that want to leverage Planning in production will be able to purchase it at the GA date. We encourage you to reach out to your sales rep to discuss further details. The environment used for the beta program is not in production and will not be migrated. The data stored in the beta environment will be available until December 2024. -->

 

CUSTOMER QUESTIONS – SESSION #1 6/13 

 

The process of the brief creation (AI use of pulling in various documents to dynamically create a brief). Is that part of the beta? 

We expect that this feature is being able to be tested. 

Do we have to be migrated to IMS? 

Yes, customers who want to purchase Planning will have to be migrated to the ABP. 

Can you provide examples of different workspaces? 

You can have workspaces at different levels, and because of the flexibility of the system, that can be really serve multiple purposes at a team and personal level. Primary use case are larger centralized workspaces for organizations. Some specific examples of workspaces are: ….. 

Can workspaces share funding accounts? 

Can workspaces talk to each other? Or would information have to be entered in each workspace? 

In its current state, are there are any soft limits on # of workspaces that can be set-up (ie. performance degrades after this point)? Any hard limits on the # of workspace that can be set-up (ie. the system will not allow more than this #)? 

Up to 1,000 workspaces in your organization's Workfront instance. Link to docs: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/create-workspaces 

Can current objects in the system be plugged in or does this have all have to be manually built? 

You can create connections between a Planning record types with WF portfolios, programs, projects, groups and companies. Once you establish a connection, for example with WF projects, you can link for records in the Planning table with WF projects. This means that WF objects will be still created and managed in Workfront, but you can align them with Planning records. You have some documenation here: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/connect-record-types  and we are also planning to have a feedback session about Connections! 

From testing I have noticed if you add lots of records they become hard to distinguish between each other when not in the Table View. Is there a way to make records different colours? It would be good if you could make them configurable by colour, that way they would stand out from each other more in the Timeline and Calendar views. 

Are the people Workfront people or IMS people? 

Workfront Instance 

Can these lists be linked to multiple workspaces? 

We have plans to link record types between Workspaces! Not ready yet. 

Are custom fields you add locked to the record type they were created under? 

It isn't allowing me to make a connection with the Start/End Date fields that are default. Should I add a new one if I want to connect to a field that already exists? 

Any plans for true external lookup style fields as a field type in Planning? 

Any plans to just have the fields "Created" "Created by" "Modified" and "Modified by" by default in records - seems like a consumption for fields to have to add it if we want to track records? 

Since the module links through to live objects in WF, will they be affected by the Planning beta's activities? 

Are we going to be getting updates for the changes putting into Fusion or is that something that is managed separately? 

Is there plans to integrate with Canvas Dashboards? How to report data? 

Soon available Dashboard Canvas soon will be available to visualize Planning data 

Will we be able to create workspace templates? 

Is this Taxonomy / Record structure ONLY available if you purchase Planning?  A taxonomy structure would be beneficial for standard Workfront users too 

Will admins be able to create our own templates? 

Not during the beta. 

Do you all have an ERD documented and available to share for the planning model and record types? Not an ERD at this point, but we have granular help articles that guide you through the process of creating and connecting record types: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/overview-of-record-types https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/connect-record-types 

So its one time (Annual pricing) to avail PLANNING, and there on we can add as many users as required? or we get charged per User ? 

Planning is a paid offering that has a target GA date August 28th, the time at which you will have to purchase Planning in order to be able to enjoy it in Production. Please work with your sales rep to get more details. 

Is AI Enablement only available to WF System Administrators OR can it be enabled on specific Access Levels OR can it be enabled for ONLY specific users (1 or 2)? 

At first, only Primary System admins have access so they can configure through Access Levles who in their org will get access. After June 21st, we will enable AI to the rest of the org and they will have access or not depending on the configuration defined by the System Admin. 

Where do the FIELDS created here live? Can existing FIELDS be brought in from those we hve created for other objects? Are they separate from other fields created? 

Currently the fields live within the record type they're created in, but we have a high priority initiative for H2 '24 to bring together the Planning and Workfront fields in a centralized field library. 

Will we be able to create reports based on the records/fields we create in planning? 

Yes! Coming soon, through Dashbaord Canvas 

Will we be able to pull this data using the API as well? 

Yes! We have API already available and Fusion connector. 

From a Marketing Workspace - is it best to have one master Workspace to use for a Global Marketing team OR is it best to have individual Workspaces for each Business Line, Country, Brand, etc. i saw that we're able to have up to 1000 Workspaces and potentially connect Workspaces. is it possible to link records btwn workspaces? Use case would be - allow each product their own workspace, but with shared record types. And then would want to see a shared view that combines everything. 

Can we bring in Portfolio and Program to the Campaigns? That in turn brings in projects? 

Will it be possible to link projects to records in a workspace upon project creation, without having to go to the workspace to link it? 

Currently we have Planning section within projects that display any connection records from Planning record types. You can add or remove records from those connections. We will also soon add the ability to link to records in any other Planning record types, even if that connection currently doesn't have any linked records. 

I'm understanding eventually we will be able to intake information/data from someone outside our organization. When will this feature be made available in beta? 

Can the workspace be used for resource and capacity planning by job role across a campaign? 

We will be able to link a Workspace record to start a request? 

OFFICE HOURS 6/18 

The ability to link dates to connected Workfront data. Is that currently active across all levels (projects, portfolios, program,…)? 

Yes, it is possible to connect projects via lookups fields.  

How do I know there are public view ready to view? 

Public views that are shared are visible  

How do you share a view internally? 

Every time you create a new workspace do you have to re-share views? 

Yes, every time you create a new workspace so it is a new record type.. Views are specific to record types, and therefore you will have to re-share. 

Can thumbnails be from the content? i.e. Set the thumbnail to the .pdf or video. We work with creative people and to have a thumbnail view that is selectable would be a great way to keep teams engaged in those higher-level meetings where they will discuss our Content Map – a link to the content directly would be great too. 

Can you customize the permissions beyond what the base is? Currently with other Workfront objects you can customize what contribute/manage/view access can do. 

Currently we only have Workspce and View level permissions, but not record type or individual record level permissions.  

Are we able to customize Workspace icons similar to how we can customize thumbnails? 

Will there be customizable APIs to use our own DAM instead of Adobe's DAM?  

We have build a public API for Planning and we also have the Fusion connector. The API documentation will be published, and that could be utilized to build connections. 

I see value in Planning (employees using Airtable). Up until now we've been .. curious backend connection after x that will tie back to ~10.47am 