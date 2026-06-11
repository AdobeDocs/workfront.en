---
title: Other enhancements during the Third Quarter 2026 release timeframe
description: Other enhancements during the Third Quarter 2026 release time frame
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
---
# Other enhancements during the Third Quarter 2026 release timeframe

This page describes enhancements made with the Third Quarter 2026 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Third Quarter 2026 release cycle, see [Third Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Updates to the Workfront MCP connector

We've made the following update to the Workfront MCP connector:
<!--
* We've expanded the MCP server to work with instances in the EU and US instances that are not on AWS. Each MCP server can only connect to one instance, but are no longer limited to US instances on AWS.
-->
* To expand the flexibility of the Workfront MCP connector, we've added the ability to connect Claude. Now, you can find Workfront in the list of connectors in Claude, or connect directly using a URL.

For more information and instructions, see [Configure the Adobe Workfront MCP server](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).


## Updated look and feel for comment notification emails

>[!NOTE]
>
>Production release for customers: Phased rollout beginning July 16, 2026

Email notifications for comments in the Updates area have a new look and feel that aligns with the broader Adobe email design.

The updated email format includes:

* A new Adobe Workfront header replacing the previous Workfront branding.
* A streamlined layout that focuses on the most recent comment.
* A primary **See it in Workfront** button to open the item directly.

The thread of preceding comments is no longer included in the email body. To view earlier comments on the item, use **See it in Workfront** to open the conversation in Workfront.

This change is rolling out to customers in phases. This page will be updated when the rollout schedule is confirmed.

![updated comment notification email.png](assets/email-look-and-feel-update.png)

## Connect Workfront to your AI tools with the Workfront MCP Server

>[!NOTE]
>
>Preview: May 28, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026

Your team's operational context lives in Workfront. Now, with the Workfront MCP Server, that context becomes actionable from within the AI tools your team already uses.

Connect Workfront to any MCP-compatible AI platform, including Claude, ChatGPT, Copilot, Gemini, and more, and use natural language to find, create, update, and manage Workfront items without leaving your AI tool of choice. Ask for your overdue tasks, push a project's finish date, send a reminder to approvers, update a campaign budget--and your AI platform does the work for you in Workfront.

And with Claude's AI skills and scheduled tasks, you can go even further--automating recurring workflows that run proactively against live Workfront data. For example, a Monday morning project briefing, a weekly capacity report, a monthly campaign health check -- set it once, and AI handles it automatically, grounded in the full context of your operation.

This is the foundation of an agentic work management system--where AI is grounded in your richest operational data and humans and AI collaborate together to keep work moving at full velocity.

>[!IMPORTANT]
>
>Currently, the Workfront MCP server is available only to customers in the US region for customers using AWS.

For more information, see [Adobe Workfront MCP server overview](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Enhanced list updates

>[!NOTE]
>
>Preview: May 28, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026

Multiple field types on enhanced lists have been updated to include keyboard navigation and other enhancements.

Assignee fields in enhanced lists now offer keyboard navigation:

* Use the up and down arrows on your keyboard to move through the list of people.
* Press the space bar to select a person or \<Delete\> to remove a selected person.

On single and multi-select fields in enhanced lists:

* The field interaction is now keyboard accessible. This includes navigation between the tags, search options, and list using the up and down arrows. Press the space bar to select an item or \<Delete\> to remove a selected item.
* You can create new options directly from the editor when no results are found. Note that this feature may not be available on all lists.

Reference fields such as typeahead and external lookup fields have received some interface enhancements.

Also, the experience of dragging and dropping columns (on lists where drag and drop is available) has been improved visually.

For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
