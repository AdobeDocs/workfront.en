---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Use the Adobe Workfront MCP server
description: Use the Adobe Workfront MCP server to search, create, update, and manage Workfront items through natural-language conversation in an AI agentic platform.
author: Courtney
feature: Get Started with Workfront
hide: true
---

# Use the Adobe Workfront MCP server

The [!DNL Adobe Workfront] MCP server lets you find, create, update, and manage Workfront items by asking an AI agentic platform in plain English. The platform decides which Workfront actions to call and handles the conversation with Workfront for you.

[!DNL Claude] is currently the only supported AI agentic platform, but the examples and patterns in this article apply to any AI agentic platform that supports the Workfront MCP server.

This article assumes you've already set up the connection. For information about setup, see [Configure the Adobe Workfront MCP server](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md). For more information about the Workfront MCP server, see [Adobe Workfront MCP server overview](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Available tools

The Workfront MCP server exposes a set of tools that the AI agentic platform calls on your behalf — for example, tools to search Workfront, create items, update fields, and manage approvals. For the full reference list, grouped by Workfront area, see [Adobe Workfront MCP server tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

>[!IMPORTANT]
>
>When you connect an AI agentic platform to Workfront, it acts in Workfront using your Workfront account and permissions. The platform's actions have the same effect as actions you take directly in the Workfront interface.
>
>You and your AI agentic platform provider are responsible for the actions the platform takes in Workfront. Adobe is not responsible for changes the AI agentic platform makes to your Workfront data.
>
>Before you let the AI agentic platform proceed with a request, confirm that you understand what it intends to do, especially for actions that change or delete data.


## Examples of what to ask

After you're connected, type natural-language requests in your AI agentic platform. The AI agentic platform decides which Workfront actions to call and returns the results.

### Find and view your work

To search Workfront for items that match what you're looking for, ask:

* *Show me all active projects for the Brand Marketing team.*
* *Get me all tasks assigned to Joan Harris.*
* *Show me all issues in the "Website Redesign" project under the "Technical" category.*

### Create new items

To create projects, tasks, or other Workfront items, ask:

* *Create a blank project called "Q2 Innovation Sandbox" starting March 10 and ending April 30. Set me as the owner.*
* *Add a new task called "Landing Page QA" to the project and schedule it from April 22 to April 26.*
* *Create a new campaign record called "Summer Sale 2026."*

### Update existing items

To make changes to items already in Workfront, ask:

* *Update the "Design Review" task so it finishes on April 18, and assign it to the creative team.*
* *For the "Lucent AI Launch – NA" project, push the finish to mid-April and increase the budget to $150K.*
* *Update the budget field in the "Summer Campaign" record to $75,000.*

### Delete items

To remove Workfront items, ask:

* *Delete the project called "Q1 Test Campaign."*
* *Remove the "Print Asset Production" task from the project.*
* *Delete the campaign record named "Old Promo."*

>[!WARNING]
>
>Deleting items in Workfront through an AI agentic platform is the same as deleting them in the Workfront interface. Confirm what the AI agentic platform is about to delete before you let it proceed.

### Work with approvals

To manage document and asset approvals, ask:

* *Add Sarah Chen and Miguel Alvarez as approvers on the current document.*
* *Send a reminder to approvers on the asset "Spring Campaign Video" who haven't responded.*
* *Apply the "Marketing Launch" approval template to the asset "Spring Campaign Video."*


### Work with Planning records

To manage planning records, ask:

* *Create a new planning record called "Q2 Marketing Plan" for the Brand Marketing team.*
* *Add a new task called "Social Media Audit" to the planning record.*
* *Update the "Social Media Audit" task so it finishes on April 18, and assign it to the creative team.*

### Work with workflow

To manage workflow, ask:

* *Route the "Q2 Innovation Sandbox" project to the Innovation Review Board.*
* *Update the "Summer Campaign" record to the "Ready for Launch" status.*
* *Approve the "Summer Campaign" record.*


### Chain requests across a conversation

You can chain requests in a single conversation. The AI agentic platform keeps the context, so each request can build on the previous one. For example:

1. Ask for a set of items: *Find my overdue tasks.*
1. After you get the list, ask for an action on the results: *Update all of them to next Friday.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## Considerations

Keep the following considerations in mind when you use the Workfront MCP server.

### The AI agentic platform may use information from earlier in the conversation

AI agentic platforms sometimes reuse data from earlier in a conversation instead of asking Workfront for the latest. If something has changed in Workfront since the AI agentic platform last looked, you might see outdated information.

To force the AI agentic platform to fetch fresh data, ask for it explicitly. For example:

* *Get the latest data from Workfront. Don't use cached results.*

### The Workfront MCP server updates automatically

When Adobe releases a new version of the Workfront MCP server, your AI agentic platform uses the new version automatically. You don't need to reconnect or change anything on your side.

## Data and security

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI agentic platform. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI agentic platform provider, what happens to it after the conversation ends, and any differences between AI agentic platforms (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### What data leaves Workfront

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI agentic platform (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### How AI agentic platform providers handle your Workfront data

<!-- NEEDS DETAIL: For each supported AI agentic platform, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### Differences between AI agentic platforms

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI agentic platform handles Workfront data once additional AI agentic platforms are supported. -->

## Troubleshoot day-to-day use

+++ Expand to view troubleshooting tips for day-to-day use of the Workfront MCP server.

| Problem | Likely cause | Fix |
|---|---|---|
| The AI agentic platform is giving you outdated information. | The AI agentic platform is reusing data from earlier in the conversation. | Ask for fresh data from Workfront. |
| The AI agentic platform returned data from the wrong Workfront items. | The AI agentic platform picked the wrong items based on ambiguous wording. | Ask again with more specific names, IDs, or filters. |
| An update or delete didn't take effect in Workfront. | The AI agentic platform hasn't called the action yet, or your permissions don't allow it. | Confirm with the AI agentic platform that the action ran, then check your Workfront permissions. |

For more information about setup and authentication issues, see [Troubleshoot setup and authentication](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) in [Configure the Adobe Workfront MCP server](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

+++

## Frequently asked questions

+++ Expand to view frequently asked questions about using the Workfront MCP server.

### What Workfront items can I work with through an AI agentic platform?

Any items that you have access to in Workfront via access levels and object permissions.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### Is my Workfront data sent to the AI agentic platform provider or stored by them?

For more information, see [Data and security](#data-and-security) in this article.

### What happens when a new version of the Workfront MCP server releases?

The MCP server updates automatically. You don't need to reconnect or change anything.

### Do I need to know the Workfront API to use the Workfront MCP server?

No. The AI agentic platform translates your natural-language requests into the right Workfront actions. If you're already familiar with the Workfront API, the actions will feel familiar, but it isn't a requirement.

+++