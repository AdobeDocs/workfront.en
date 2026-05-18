---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Use the Adobe Workfront MCP server
description: Use the Adobe Workfront MCP server to search, create, update, and manage Workfront items through natural-language conversation in an AI assistant.
author: Courtney
feature: Get Started with Workfront
hide: true
---

# Use the Adobe Workfront MCP server

The [!DNL Adobe Workfront] MCP server lets you find, create, update, and manage Workfront items by asking an AI assistant in plain English. The AI assistant decides which Workfront actions to call and handles the conversation with Workfront for you.

[!DNL Claude] is currently the only supported AI assistant, but the examples and patterns in this article apply to any AI assistant that supports the Workfront MCP server.

This article assumes you've already set up the connection. For information about setup, see [Configure the Adobe Workfront MCP server](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md). For more information about the Workfront MCP server, see [Adobe Workfront MCP server overview](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).



## Actions available through the Workfront MCP server

The Workfront MCP server covers actions across approvals, planning, and workflow.

<!-- NEEDS DETAIL: Confirm the full inventory of actions exposed through the Workfront MCP server. The five core actions below are confirmed from Hamilton's walkthrough. The approvals, planning, and workflow sections need to be filled in from Jeff's engineering channel post, hands-on access, and the deck Oznur published in the MCP external channel. -->

>[!IMPORTANT]
>
>An AI assistant acts in Workfront using your Workfront account and permissions. You and your AI assistant provider are responsible for the actions the AI assistant takes on your behalf. Confirm what the AI assistant is about to do before you let it proceed.


## Responsibility for AI assistant actions

When you connect an AI assistant to Workfront, the AI assistant acts in Workfront using your Workfront account and permissions. The AI assistant's actions have the same effect as actions you take directly in the Workfront interface.

You and your AI assistant provider are responsible for the actions the AI assistant takes in Workfront. Adobe is not responsible for changes the AI assistant makes to your Workfront data.

Before you let the AI assistant proceed with a request, confirm that you understand what it intends to do, especially for actions that change or delete data.

### Core actions

The Workfront MCP server includes the following core actions:

| Action | What it does |
|---|---|
| Create | Creates new items in Workfront. |
| Search | Finds and retrieves items from Workfront. |
| Update | Changes existing items in Workfront. |
| Delete | Removes items from Workfront. |
| Resolve field names | Looks up the correct Workfront field names so the AI assistant can build accurate requests against your data. |

<!-- NEEDS DETAIL: Confirm which Workfront object types are supported across the core actions (projects, tasks, issues, portfolios, programs, custom forms, planning records, approvals, etc.). -->

### Approvals actions

<!-- NEEDS DETAIL: List the approval-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request a marketer might make. -->

### Planning actions

<!-- NEEDS DETAIL: List the planning-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

### Workflow actions

<!-- NEEDS DETAIL: List the workflow-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

## Examples of what to ask

After you're connected, type natural-language requests in your AI assistant. The AI assistant decides which Workfront actions to call and returns the results.

<!-- NEEDS DETAIL: Example prompts in this section are adapted from the Workflow Optimization Agent (WOA) examples doc on another branch. Validate each example against a working Claude + Workfront MCP server setup before publication, since WOA and the MCP server may expose different action inventories. -->

### Find and view your work

Ask the AI assistant to search Workfront for items that match what you're looking for. For example:

* *Show me all active projects for the Brand Marketing team.*
* *Get me all tasks assigned to Joan Harris.*
* *Show me all issues in the "Website Redesign" project under the "Technical" category.*

### Create new items

Ask the AI assistant to create projects, tasks, or other Workfront items. For example:

* *Create a blank project called "Q2 Innovation Sandbox" starting March 10 and ending April 30. Set me as the owner.*
* *Add a new task called "Landing Page QA" to the project and schedule it from April 22 to April 26.*
* *Create a new campaign record called "Summer Sale 2026."*

### Update existing items

Ask the AI assistant to make changes to items already in Workfront. For example:

* *Update the "Design Review" task so it finishes on April 18, and assign it to the creative team.*
* *For the "Lucent AI Launch – NA" project, push the finish to mid-April and increase the budget to $150K.*
* *Update the budget field in the "Summer Campaign" record to $75,000.*

### Delete items

Ask the AI assistant to remove Workfront items. For example:

* *Delete the project called "Q1 Test Campaign."*
* *Remove the "Print Asset Production" task from the project.*
* *Delete the campaign record named "Old Promo."*

>[!WARNING]
>
>Deleting items in Workfront through an AI assistant is the same as deleting them in the Workfront interface. Confirm what the AI assistant is about to delete before you let it proceed.

### Work with approvals

Ask the AI assistant to manage document and asset approvals. For example:

* *Add Sarah Chen and Miguel Alvarez as approvers on the current document.*
* *Send a reminder to approvers on the asset "Spring Campaign Video" who haven't responded.*
* *Apply the "Marketing Launch" approval template to the asset "Spring Campaign Video."*

<!-- NEEDS DETAIL: Add approvals-specific context from the WOA examples doc, including: content approvals must be enabled for the organization, the AI assistant cannot approve or reject on behalf of humans (except via the Workfront AI Reviewer), and best experience is with the Unified Approvals experience. -->

### Work with Planning records

Ask the AI assistant to manage planning records. For example:

* *Create a new planning record called "Q2 Marketing Plan" for the Brand Marketing team.*
* *Add a new task called "Social Media Audit" to the planning record.*
* *Update the "Social Media Audit" task so it finishes on April 18, and assign it to the creative team.*

### Work with workflow

Ask the AI assistant to manage workflow. For example:

* *Route the "Q2 Innovation Sandbox" project to the Innovation Review Board.*
* *Update the "Summer Campaign" record to the "Ready for Launch" status.*
* *Approve the "Summer Campaign" record.*


### Chain requests across a conversation

You can chain requests in a single conversation. The AI assistant keeps the context, so each request can build on the previous one. For example:

1. Ask the AI assistant to find a set of items: *Find my overdue tasks.*
1. After the AI assistant returns the list, ask it to act on the results: *Update all of them to next Friday.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## Considerations

Keep the following considerations in mind when you use the Workfront MCP server.

### The AI assistant may use information from earlier in the conversation

AI assistants sometimes reuse data from earlier in a conversation instead of asking Workfront for the latest. If something has changed in Workfront since the AI assistant last looked, you might see outdated information.

To force the AI assistant to fetch fresh data, ask for it explicitly. For example:

* *Get the latest data from Workfront. Don't use cached results.*

### The Workfront MCP server updates automatically

When Adobe releases a new version of the Workfront MCP server, your AI assistant uses the new version automatically. You don't need to reconnect or change anything on your side.

## Data and security

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI assistant. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI assistant provider, what happens to it after the conversation ends, and any differences between AI assistants (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### What data leaves Workfront

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI assistant (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### How AI assistant providers handle your Workfront data

<!-- NEEDS DETAIL: For each supported AI assistant, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### Differences between AI assistants

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI assistant handles Workfront data once additional AI assistants are supported. -->

## Troubleshoot day-to-day use

For more information about setup and authentication issues, see [Troubleshoot setup and authentication](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) in [Configure the Adobe Workfront MCP server](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

| Problem | Likely cause | Fix |
|---|---|---|
| The AI assistant is giving you outdated information. | The AI assistant is reusing data from earlier in the conversation. | Ask the AI assistant to fetch fresh data from Workfront. |
| The AI assistant returned data from the wrong Workfront items. | The AI assistant picked the wrong items based on ambiguous wording. | Ask again with more specific names, IDs, or filters. |
| An update or delete didn't take effect in Workfront. | The AI assistant hasn't called the action yet, or your permissions don't allow it. | Confirm with the AI assistant that the action ran, then check your Workfront permissions. |

<!-- NEEDS DETAIL: Add additional day-to-day troubleshooting scenarios discovered during hands-on testing. -->

## Frequently asked questions

### What Workfront items can I work with through an AI assistant?

Any items that you have access to in Workfront via access levels and object permissions.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### Is my Workfront data sent to the AI assistant provider or stored by them?

For more information, see [Data and security](#data-and-security) in this article.

### What happens when a new version of the Workfront MCP server releases?

The MCP server updates automatically. You don't need to reconnect or change anything.

### Do I need to know the Workfront API to use the Workfront MCP server?

No. The AI assistant translates your natural-language requests into the right Workfront actions. If you're already familiar with the Workfront API, the actions will feel familiar, but it isn't a requirement.
