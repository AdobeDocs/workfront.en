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

The [!DNL Adobe Workfront] MCP server lets you find, create, update, and manage Workfront items by asking an AI agentic platform in natural language. The platform decides which Workfront actions to call and handles the conversation with Workfront for you.

## Prerequisites

This article assumes you've already set up the connection. For information about setup, see [Configure the Adobe Workfront MCP server](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).
## Available tools

The Workfront MCP server exposes a set of tools that the AI agentic platform calls on your behalf — for example, tools to search Workfront, create items, update fields, and manage approvals. For the full reference list, grouped by Workfront area, see [Adobe Workfront MCP server tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

>[!IMPORTANT]
>
>When you connect an AI agentic platform to Workfront, it acts in Workfront using your Workfront account and permissions. The platform's actions have the same effect as actions you take directly in the Workfront interface.<br>
>
>You and your AI agentic platform provider are responsible for the actions the platform takes in Workfront. Adobe is not responsible for changes the AI agentic platform makes to your Workfront data.<br>
>
>Before you let the AI agentic platform proceed with a request, confirm that you understand what it intends to do, especially for actions that change or delete data.


## Examples of what to ask

After you're connected, type natural-language requests in your AI agentic platform. The AI agentic platform decides which Workfront actions to call and returns the results.

>[!NOTE]
>
>Some actions might not be available because of admin controls in the Workfront Setup area. For example, you might not be able to create items if your admin has disabled write actions for the MCP server. 


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


## Considerations

Keep the following considerations in mind when you use the Workfront MCP server:

### The AI agentic platform may use information from earlier in the conversation

AI agentic platforms sometimes reuse data from earlier in a conversation instead of asking Workfront for the latest. If something has changed in Workfront since the AI agentic platform last looked, you might see outdated information.

To force the AI agentic platform to fetch fresh data, ask for it explicitly. For example:

* *Get the latest data from Workfront. Don't use cached results.*

### Check for updates to the Workfront MCP server

You might want to periodically refresh your connection to the Workfront MCP server to ensure that you have the latest tools and capabilities.

Most updates should happen automatically. However, you might want to check the Workfront release notes periodically.


## Data and security

The Workfront MCP server tools are consistent with how API calls work. Workfront doesn't store prompts, responses, or any other data. Whatever Workfront data you ask for is accessible in the Workfront platform.

Your access level and object permissions determine what you can query for or write to Workfront. Your Workfront administrator has control of MCP read and writer actions in the Workfront Setup area.

### What data leaves Workfront

The AI agentic platform provider has access to the Workfront data you interact with through the Workfront MCP server. Check with your AI agentic platform provider for details.


### How AI agentic platform providers handle your Workfront data

Workfront does not have control over how the AI agentic platform provider handles your Workfront data. Check with your AI agentic platform provider for details.

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


### What is an AI agentic platform?

An AI agentic platform is an AI tool that can take actions on your behalf in 
other systems, not just answer questions. When you connect one to Workfront 
through the MCP server, it can find, create, update, and delete Workfront 
items based on what you ask it in natural language. Examples include Claude 
Desktop, ChatGPT, and other MCP-compatible AI clients.


### Do I need to be a Workfront administrator to use the Workfront MCP server?

No. Any Workfront user can use the Workfront MCP server through a connected 
AI agentic platform. The AI agentic platform acts using your Workfront 
account, access level, and object permissions, so you can only do what you 
could already do directly in Workfront.

### Why can't the AI agentic platform create, update, or delete items for me?

Your Workfront administrator controls which MCP actions are allowed in the 
Workfront Setup area. If write actions are disabled, the AI agentic platform 
can still find and read Workfront items but can't make changes. You also 
need the right access level and object permissions for the specific items 
you're working with.

### Will the AI agentic platform ask me before it changes or deletes Workfront data?

That depends on the AI agentic platform, not on Workfront. Most platforms 
prompt you to confirm before they run an action, especially for deletes. 
Before you approve a request, read what the platform says it's about to do — 
the changes happen in Workfront the same way they would if you made them 
yourself in the interface.

### Can I undo something the AI agentic platform did in Workfront?

Changes the AI agentic platform makes in Workfront work the same way as 
changes you make in the interface. If Workfront supports undoing or 
restoring a particular action (for example, restoring a deleted item from 
the Recycle Bin), the same options apply. If Workfront doesn't normally let 
you undo an action, you can't undo it through the AI agentic platform either.

<!-- VERIFY: Confirm what's restorable from the Recycle Bin for the object 
types the MCP server can delete. -->

### Why did the AI agentic platform return the wrong Workfront items?

The AI agentic platform picks items based on the words you used. If your 
request is ambiguous — for example, two projects have similar names — it 
might pick the wrong one. Ask again with more specific names, IDs, dates, 
or filters to narrow the results.


### What Workfront items can I work with through an AI agentic platform?

Any items you have access to in Workfront through your access level and 
object permissions. This includes projects, tasks, issues, documents, 
approvals, Planning records, and more.

### Can other people see my conversations with the AI agentic platform?

Workfront doesn't store your prompts or the AI agentic platform's responses. 
Whoever provides your AI agentic platform controls how your conversations 
are stored or shared. Check with your AI agentic platform provider for 
details.

### Do I need to know the Workfront API or which MCP tool to use?

No. The AI agentic platform translates your natural-language request into 
the right Workfront actions and picks the right tools for you. If you're 
already familiar with the Workfront API, the actions will feel familiar, 
but it isn't a requirement.

### Is my Workfront data sent to the AI agentic platform provider or stored by them?

For more information, see [Data and security](#data-and-security) in this 
article.

### What happens when a new version of the Workfront MCP server releases?

The MCP server updates automatically. You don't need to reconnect or change 
anything. To see what's new, check the Workfront release notes periodically.


+++