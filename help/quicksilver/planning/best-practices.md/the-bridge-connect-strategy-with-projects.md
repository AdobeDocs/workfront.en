---
title: "Build the Bridge: Connecting Strategic Intent to Projects"
description: Learn how to create a "strategic thread" between your high-level plans in Adobe Workfront Planning and your daily execution of workflows in Adobe Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: yes
hide: yes
exl-id: 567ab223-b282-4b98-9655-7b9766fba869
---

# Build the bridge: connecting strategic intent to projects 

{{planning-important-intro}}
 
Learn how to create a strategic thread between your high-level plans in Adobe Workfront Planning and your daily execution in Workfront. You can build a bridge between strategy and execution using connections. 

This guide is intended for Workfront administrators and workspace managers who are implementing Workfront Planning. 

## Overview of aligning strategy to execution

Connecting your strategy to your daily work turns vision into reality. When high-level plans are in sync with execution, you create a strategic thread that ensures every project and task moves the business forward.  

Achieving this alignment requires a set of technical links and process guardrails that connect efforts in Workfront with strategic records in Workfront Planning. 

By bridging the gap between planning and action, you ensure that your team's energy is always focused on your highest-priority goals. 

## Establish the foundation by creating a connection 

Before you can bridge planning and execution, as a workspace manager you must define which record types are eligible for a connection. 

### Overview of the connection field

The bridge begins with creating a connection field. 

A connection field serves as a the technical handshake between record types. 

This field type is the engine behind all relationships in Workfront Planning. It is an expression of intent, in that it establishes that a specific record type (like a Channel Tactic) is allowed to be linked to other object types, whether they live in Planning or Workfront.

For information, see [Connected record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md). 

### Define when to create a connection

Ideally, you must decide whether you need to create connections before any work is created. 

By adding a connection field, you are architecting your environment to support a strategic thread, regardless of how the individual records are eventually created. 

## Set strategy and execution in sync 

To keep your strategic layer focused, we recommend focusing your planning records on high-level intent while using Workfront for tactical execution. 

This approach uses the unique strengths of both modules in the following ways:  

* **Workfront Planning (the strategic layer):** Stays high-level. It tracks the Campaign, the Channel Tactic, and the Budget. It is noise-free and executive-ready. 

* **Workfront (the execution layer):** Manages the tactical details. You can manage individual experiences or activities as projects, tasks, and issues. You can assign them for ownership and build in approvals for execution.  

## Go from intent to action by activating the bridge

After the connection is configured, you must decide how to activate the link between a specific strategic record and an execution project. 

### Use a table-led path 

Strategists and power users often use the table view as their workbench to refine plans over time.  

Creating a record in a table does not establish a link to Workfront, by default. 

The connection to an execution project is established when a user decides to activate the link. 
    
This can be done in the following ways:
    
* Manually create a downstream connected project directly from the connection field in Workfront Planning or from an optional Connections page in the record's detail view. 

    Manual creation results in a blank project without specific custom forms.

    For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

* Automatically, by using Workfront Planning automations, for more complex needs. 

    These automations are available as buttons in the actions bar when you select a row in a table. 
    
    This allows for human oversight or placeholder creation, ensuring that projects are only generated in your workflow environment when they are truly needed. 

    For information, see [Create objects using Adobe Workfront Planning record automations](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)
 

### Build automated activations

For organizations with high-volume requests or advanced automation needs, the bridge can be activated automatically based on specific events or based on field values configured in a request form. 

You will need a license for Adobe Workfront Fusion for this approach. 

For more information see [Set up and manage Workfront Fusion: article index](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-workfront-fusion-toc). 

* **Use submission triggers:** Because forms provide a single, clean submission event, they can be used as triggers for Fusion automations. A Fusion scenario can detect a form submission and immediately generate a linked project in Workfront. 

* **Use field-value triggers:** For deeper automation, you can configure Fusion to monitor specific fields. For example, a simple checkbox labeled "Ready for execution" can serve as the catalyst, establishing the bridge automatically the moment it is checked.  

## Add lookup fields to surface visibility

Once a project is linked, you can surface real-time data from Workfront directly within the Planning record by adding lookup fields from the project. 
 
As a workspace manager, you can set up lookup fields to pull any system or custom field from the linked project (such as Actual Completion Date or Creative Lead) into the Planning record type. Once captured, this data can be rolled up through multiple levels of your strategic hierarchy, all the way up to the campaign level. This provides powerful aggregate reporting for stakeholders across the entire marketing lifecycle, keeping them informed without needing to leave the planning environment.  

## Achieve visibility by connecting strategy to action

The ultimate value of the bridge is real-time visibility. 

By connecting intent to action, you can answer critical business questions at a glance. The following are examples of these questions: 

* Is our 'FY26 Brand Awareness' campaign actively delivering results right now?

* Where do our strategic tactics need more creative support to stay on schedule?

* How are we aligning our resources with our highest-priority strategic pillars?

## Best practices and tips 

### Dos: 

*   **Use the "strategic thread" metaphor:** Remind teams that every project should be a "bead" on a strategic string. 

*   **Automate the handoff:** Use automations to trigger project creation to save time and effort while also improving data connectivity and governance. 

*   **Link, don't duplicate:** Use lookup fields to surface real-time execution data (like status or completion dates) in your strategic records. This ensures your strategic views are always accurate without requiring manual updates from your team. 

### Don'ts: 

*   **Don't treat planning records as task lists:** The bridge is designed to connect strategic intent to execution projects. Keep your planning records focused on the "what" and "why," and let the workflow module handle the granular "how" through tasks and issues. 

*   **Don't over-sync:** You don't need to sync every project-level detail back to Planning. Keep the strategic layer high-level and noise-free. 

*   **Don't bypass the bridge:** If work starts in the Workflow module without a link to Planning, you've created a "Shadow Plan" that is invisible to leadership.

<!--original content:

# The Bridge: Connecting Strategic Intent to Projects 

 

## Goal 

Learn how to create a "strategic thread" between your high-level plans in Workfront Planning and your daily execution in the Workflow module. 

 

## Overview 

Connecting your strategy to your daily work turns vision into reality. When high-level plans are in sync with execution, you create a **strategic thread** that ensures every project and task moves the business forward. 

 

Achieving this alignment requires a set of technical links and process guardrails that connect efforts in the **Workflow module** with strategic records in **Workfront Planning (WFP)**. By bridging the gap between planning and action, you ensure that your team's energy is always focused on your highest-priority goals. 

 

## The foundation: Establishing the connection 

Before you can bridge planning and execution, a workspace manager must define which record types are eligible for a connection. 

 

### The connection field: The technical handshake 

The bridge begins with a **connection field**. This field type is the engine behind all relationships in WFP. It is an expression of intent, in that it establishes that a specific record type (like a *channel tactic*) is allowed to be linked to other objects, whether they live in the workflow module or within planning itself. 

 

### Deciding to connect 

Establishing this allowance is a configuration-level decision that typically happens before any work is created. By adding a connection field, you are architecting your environment to support a "strategic thread," regardless of how the individual records are eventually created. 

 

## Strategy and execution in sync 

To keep your strategic layer focused, we recommend focusing your planning records on high-level intent while using the Workflow module for tactical execution. This approach uses the unique strengths of both modules: 

 

*   **Workfront Planning (The strategic layer):** Stays high-level. It tracks the *Campaign*, the *Channel Tactic*, and the *Budget*. It is noise-free and executive-ready. 

*   **Workflow module (The execution layer):** Manages the tactical details. Individual "Experiences" or "Activities" are managed here as **projects, tasks, and issues**. 

 

## Activating the bridge: From intent to action 

Once the connection is configured, you must decide how to activate the link between a specific strategic record and an execution project. 

 

### Professional triage: The table-led path 

Strategists and power users often use the **table view** as their "workbench" to refine plans over time.  

*   **Deliberate handoff:** By default, creating a record in a table does not establish a link to the Workflow module. The connection to an execution project is established when a user decides to activate the link. This can be done by manually creating a downstream connected project directly from the connection field in WFP or an optional **connection view page** in the record's detail view. Note that manual creation results in a blank project without specific custom forms; for more complex needs, you can use a **native WFP automation**. These automations are available when you select a row in a table, appearing as buttons in the blue action bar at the bottom of your screen. This allows for human oversight or placeholder creation, ensuring that projects are only generated in your workflow environment when they are truly needed. 

 

### Automated activation 

For organizations with high-volume requests or advanced automation needs, the bridge can be activated automatically based on specific events or field values. 

*   **Submission triggers:** Because forms provide a single, clean "submission event," they can be used as triggers for **Fusion automations**. A scenario can detect a form submission and immediately generate a linked project in the workflow module. 

*   **Field-value triggers:** For deeper automation, you can configure **Fusion** to monitor specific fields. For example, a simple checkbox labeled "ready for execution" can serve as the catalyst, establishing the bridge automatically the moment it is checked. 

 

## Surfacing visibility: Lookup fields 

Once a project is linked, you can surface real-time data from the Workflow module directly within the WFP record. 

 

A workspace manager can set up **lookup fields** to pull any native or custom field from the linked project (such as *actual completion date* or *creative lead*) into the WFP record type. Once captured, this data can be rolled up through multiple levels of your strategic hierarchy—even all the way to the campaign level. This provides powerful aggregate reporting for stakeholders across the entire marketing lifecycle, keeping them informed without needing to leave the planning environment. 

 

## Strategy-to-action visibility 

The ultimate value of the bridge is **real-time visibility**. By connecting intent to action, you can answer critical business questions at a glance: 

 

*   "Is our 'FY26 Brand Awareness' campaign actively delivering results right now?" 

*   "Where do our strategic tactics need more creative support to stay on schedule?" 

*   "How are we aligning our resources with our highest-priority strategic pillars?" 

 

## Best practices & tips 

 

### Do: 

*   **Use the "strategic thread" metaphor.** Remind teams that every project should be a "bead" on a strategic string. 

*   **Automate the handoff.** Use automations to trigger project creation to save time and effort while also improving data connectivity and governance. 

*   **Link, don't duplicate.** Use lookup fields to surface real-time execution data (like status or completion dates) in your strategic records. This ensures your strategic views are always accurate without requiring manual updates from your team. 

 

### Don't: 

*   **Don't treat planning records as task lists.** The bridge is designed to connect strategic intent to execution projects. Keep your planning records focused on the "what" and "why," and let the workflow module handle the granular "how" through tasks and issues. 

*   **Don't over-sync.** You don't need to sync every project-level detail back to Planning. Keep the strategic layer high-level and noise-free. 

*   **Don't bypass the bridge.** If work starts in the Workflow module without a link to Planning, you've created a "Shadow Plan" that is invisible to leadership. 

-->
 

 