---
title: "Architect Your Success: Modeling Your Campaign Hierarchy"
description: Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture.
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
---
# Architect your success: modeling your campaign hierarchy 

 <!--see the file again for additional comments from Seth and others-->

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning, an additional capability from Adobe Workfront. 
>
>Your organization must have a Workfront Planning Prime or higher package to be able to support the features recommended in this article. 
>
>For a list of requirements to access Workfront Planning, see [Adobe Workfront Planning access overview](/help/quicksilver/planning/access/access-overview.md). 
> 
>For general information about Workfront Planning, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using centers of gravity and a multi-workspace architecture in Adobe Workfront Planning. 

This guide is intended for Workfront administrators and Power Users who are implementing and designing your environment's architecture in Workfront Planning. 

## Overview of the architecture of success 

As your marketing operations mature, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record can quickly become a junk drawer of disconnected records, conflicting terminology, and reporting silos.  

When you build an architecture of success you establish a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from spreadsheet chaos to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

## Build a hierarchy to define your levels of intent

To maintain clarity and scalability, we recommend starting with a proven core path when designing your workflow in Workfront Planning. 

From there, you can expand your strategy by adding more levels to your architecture.  

### The core path: how to get from strategy to action 

While organizations can expand this hierarchy as their operational needs evolve, beginning with the three levels described in the sections below ensures a strong bridge between strategy and execution.

From our findings, we have noticed that most successful implementations of Workfront Planning thrive on a clean, three-tier model that spans both Planning and Workfront. 

The following are the levels of a successful Planning implementation and the artifacts you might consider creating to support you in the process: 

* **Level 1: Campaigns (Workfront Planning)** 

    * **Focus:** Define the long-term strategic pillars and annual initiatives. For example, define an initiative for your organization called "FY26 Global Brand Awareness". This is your focus for a given time frame. Create campaigns to support this initiative. 

    * **Personas:** Stakeholders for this level can be Marketing Officer, a VP of Marketing, or other strategic leads. 

    For information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

* **Level 2: Channel Tactics (Workfront Planning)** 

    * **Focus:** Define the operational briefs that outline the "what" for specific channels. This is the final layer of strategic intent before work begins. For example, create a "Q1 Social Media Blitz" tactic. You can then pair it with your campaigns.  

    * **Personas:** Main stakeholders are a Marketing Operations leader, channel leaders, or campaign managers. 

* **Level 3: Projects (Planning and Workfront)** 

    * **Focus:** Execute on the exact experiences or activities that will eventually accomplish your initiative. Some of the deliverables are specific, like social posts, emails, web pages. 

    * **Implementation:** You can create Tactics in Planning and link them directly to **Projects** in Workfront, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Main stakeholders here are creatives, individual contributors, anyone who is responsible for doing the work to support the initiative. 
 
### Strategic expansion: how to add more levels 

Once you establish the core path, you may choose to add additional layers after careful consideration of their specific business complexity. 

You may find useful to create the following additional items:  

* **Channel Plans:** A layer between Campaigns and Tactics to group cross-functional strategies. For example, a Plan called "Digital Strategy". 

* **Activities:** If you work in a lower-volume environment (you might have 5,000 or fewer deliverables per year), some teams might prefer to track individual experiences as Workfront Planning records before they become Workfront projects. 

>[!IMPORTANT]
>
>If your organization produces more than 5,000 activities per year, you should move individual deliverable tracking to Workfront. 
>
>Managing high-volume experience records in Planning can lead to data accumulation that obscures your strategic visibility. 
>We recommend this broad guideline for maximum efficiency: 
>
>* Use Planning for the "why" and "what"
>* Use Workfront for the high-volume "how".

## Understand centers of gravity to build your architecture

An enterprise-grade Marketing System of Record is not built in a single workspace. It uses a "hub-and-spoke" architecture where record types are managed in their natural centers of gravity. 

For more information, see [Roll out your strategic home: a 30-day launchpad](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md). 

To build your architecture using the hub-and-spoke approach, you must create the following:

* A taxonomy hub
* A strategic planning workspace
* Functional spokes

### Build the taxonomy hub as your classifications

You must first establish one centralized workspace for your global classifications to define the main concepts everyone in your organization must understand. For example, create the following record types in a central workspace: Brands, Regions, Products, Personas. 

For information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

Establish the following when you create your classifications: 

* **Primary location:** Choose a primary workspace. This workspace should be the source of truth for the record types you create.

* **The benefit:** By syndicating these definitions to the rest of the business, you solve clarify that concepts like "Region: EMEA" means the same thing to every team.  

### Create the strategic Planning workspace as your executive center

The executive center is where high-level Campaigns (and any Channel Plans) live.  

* **Primary location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The benefit:** Leadership can manage the portfolio of campaigns without listening to the day-to-day tactical noise.  

### Define the functional spokes as your teams' workspaces

Functional units (Social, Creative, Email) have their own workspaces to manage their Tactics. 

* **Primary location:** These workspaces are the individual centers of gravity for local team execution.  

* **The benefit:** Teams consume the global campaigns and classifications from the hubs, while maintaining their own local objects. 

    For example, the team can add the Campaign record type from the central workspace into their team's workspace but create campaigns relevant only to their workspace. Examples of campaigns are "Media outlets" or "Usage rights". 

## Use a noun-based governance approach

To ensure your architecture holds up under pressure, follow the principle of noun-based governance.

We recommend the following when creating your entities in Workfront Planning:

* **Use nouns, not verbs:** Name your record types after the things you are tracking (name them "Campaign" or "Tactic"), not the actions to be done (do not name them "Campaigning" or "Planning"). 

* **Standardize nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting.  

## What about existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in Workfront. In the past, these objects were often used to mimic strategic planning. 

Now, we recommend you shift that approach to Workfront Planning which naturally fits a the strategic approach to planning. 

### Replace Portfolios and Programs with Record Types 

In many organizations, Portfolios are used to represent high-level Brands or Business Units, while Programs represent strategic themes. 

In Workfront Planning, these are best modeled as Record Types in your taxonomy hub. 

By treating a Brand or Business Unit as a record type, you can link them to a Campaign or Tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio - Program structure.  

### Use a reporting-bridge strategy 

While Workfront Planning is the future of strategic intent, its native reporting via Canvas Dashboard is still maturing. 

Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in Workfront. 

We recommend the following:

* Do not delete your Portfolios and Programs. 
* Use Planning automations to create a bridge between your record types and portfolios and programs. 

    When a Tactic or Campaign is created in Workfront Planning, that record can generate a corresponding Portfolio or Program in Workfront.

    For information, see [Create objects using Adobe Workfront Planning record automations](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md). 

This allows you to: 

* Enjoy Workfront Planning's superior strategic visualization by using timelines and calendars. 

* Maintain your legacy reporting in Workfront for stakeholders who are not yet ready to move to Canvas. 

## Best practices and tips 

### Dos 

* **Stick to the core path-first approach:** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate primary workspaces:** Ensure each record type has one home workspace (consider that its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize request forms for the intake process:** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. 

    >[!CAUTION]
    >
    >While Power Users may benefit from direct data entry in table views, this should be approached with caution. 
    >Bulk changes in a table can easily create data headaches for other stakeholders. 
 
### Don'ts 

* **Don't use generalizations:** For example, instead of speaking about a "core" environment, refer specifically to Workfront and the Project object when talking about execution. 

* **Don't over-complicate:** Every additional level of hierarchy adds a management tax. Only add levels that answer a business question you cannot currently answer. 

* **Don't create silos:** Ensure your record types are shared across workspaces so teams are not retyping the same data.


<!--original content:


## Goal 

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture. 

 

## Overview 

As your marketing operations scale, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record (MSOR) can quickly become a "junk drawer" of disconnected records, conflicting terminology, and reporting silos. 

 

The "Blueprint of Success" is a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from "spreadsheet chaos" to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

 

## The Hierarchy: Finding Your Levels of Intent 

To maintain clarity and scalability, we recommend starting with a proven **Core Path**. While organizations can expand this hierarchy as their operational needs evolve, beginning with these three levels ensures a strong bridge between strategy and execution. 

 

### The Core Path: Strategy to Action 

Most successful implementations thrive on a clean, three-tier model that spans both Planning and Workflow: 

 

1. **Level 1: Campaigns (Planning Module)** 

    * **Focus:** Long-term strategic pillars and annual initiatives (e.g., "FY26 Global Brand Awareness").  

    * **Persona:** CMO, VP of Marketing, Strategic Leads. 

2. **Level 2: Channel Tactics (Planning Module)** 

    * **Focus:** The operational briefs defining the "what" for specific channels (e.g., "Q1 Social Media Blitz"). This is the final layer of strategic intent before work begins. 

    * **Persona:** Marketing Ops, Channel Leads, Campaign Managers. 

3. **Level 3: Workflow Projects (Workflow Module)** 

    * **Focus:** The actual execution of "Experiences" or "Activities" (e.g., specific social posts, emails, web pages).  

    * **Implementation:** Tactics in Planning link directly to **Projects** in the Workflow module, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Creatives, Individual Contributors. 

 

### Strategic Expansion: Adding More Levels 

Once the core path is established, organizations may choose to add additional layers after careful consideration of their specific business complexity: 

 

* **Channel Plans:** A layer between *Campaigns* and *Tactics* to group cross-functional strategies (e.g., "Digital Strategy"). 

* **Workfront Planning Activities:** In lower-volume environments (typically <5,000 deliverables/year), some teams prefer to track individual "Experiences" as Workfront Planning records before they become projects. 


>[!TIP]
>
>**Crucial Tip: The 5,000 Deliverable Threshold** 
>
>If your organization produces more than 5,000 activities per year, you should **always** offload individual deliverable tracking to the **Workflow module**. Managing high-volume "Experience" records in Planning can lead to data accumulation that obscures your strategic visibility. Use Planning for the "Why" and "What," and the Workflow module for the high-volume "How." 

 

## Architecture: Centers of Gravity 

An enterprise-grade MSOR isn't built in a single workspace. It uses a "Hub-and-Spoke" architecture where record types are managed in their natural **Centers of Gravity**. 

 

### 1. The Taxonomy Hub (Classifications) 

Establish one centralized workspace for your "Global Classifications" (e.g., Brands, Regions, Products, Personas). 

* **Primary Location:** This workspace is the "Source of Truth" for these objects. 

* **The Benefit:** By syndicating these definitions to the rest of the business, you solve "Semantic Drift"—ensuring that "Region: EMEA" means the same thing to every team. 

 

### 2. The Strategic Planning Workspace (Executive Center) 

This is where high-level **Campaigns** (and any **Channel Plans**) live.  

* **Primary Location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The Benefit:** Leadership can manage the portfolio without seeing the day-to-day tactical mess. 

 

### 3. Functional Spokes (Team Workspaces) 

Functional units (Social, Creative, Email) have their own workspaces to manage their **Tactics**. 

* **Primary Location:** These workspaces are the center of gravity for local team execution.  

* **The Benefit:** Teams "consume" the global campaigns and classifications from the hubs, while maintaining their own local objects (like *Media Outlets* or *Usage Rights*). 

 

## Noun-Based Governance: Speak One Language 

To ensure your blueprint holds up under pressure, follow the principle of **Noun-Based Governance**.  

 

* **Use Nouns, Not Verbs:** Name your record types after the "things" you are tracking (`Campaign`, `Tactic`), not the "actions" (`Campaigning`, `Planning`). 

* **Standardize Nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting. 

 

## What About Existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in the **Workflow module**. In the past, these objects were often used to mimic strategic planning. 

 

### 1. Portfolios & Programs → Record Types 

In many organizations, **Portfolios** are used to represent high-level Brands or Business Units (BUs), while **Programs** represent strategic themes. 

* **The Shift:** These are best modeled as **Record Types** in your **Taxonomy Hub**. By treating "Brand" or "Business Unit" as a record type, you can link them to any campaign or tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio/Program structure. 

 

### 2. The "Reporting Bridge" Strategy 

While Workfront Planning is the future of strategic intent, its native reporting via **Canvas Dashboards** is still maturing. Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in the Workflow module. 

* **The Recommendation:** Don't delete your Portfolios and Programs yet. Instead, use **Fusion automations** to create a bridge.  

* **How it Works:** When a Tactic or Campaign is created in Workfront Planning, Fusion can automatically mirror that record into a corresponding Portfolio or Program in the Workflow module. This allows you to: 

    1. Enjoy Workfront Planning's superior **strategic visualization** (Timelines/Calendars). 

    2. Maintain your **legacy reporting** in the Workflow module for stakeholders who aren't yet ready to move to Canvas. 

## Best Practices & Tips 

### Do: 

* **Stick to the Core Path first.** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate Primary Workspaces.** Ensure each record type has one "home" workspace (its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize Forms for Intake.** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. While Power Users may benefit from direct data entry in Table views, this should be approached with caution—bulk changes in a table can easily create data headaches for other stakeholders. 
 

### Don't: 

* **Don't say "Core".** Refer specifically to the **Workflow module** and the **Project** objects when talking about execution. 

* **Don't over-complicate.** Every additional level of hierarchy adds a "management tax." Only add levels that answer a business question you can't currently answer. 

* **Don't create silos.** Ensure your record types are shared across workspaces so teams aren't re-typing the same data.
-->