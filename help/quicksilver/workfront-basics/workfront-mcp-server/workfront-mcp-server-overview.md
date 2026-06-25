---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP server overview
description: Learn what the Adobe Workfront MCP server does and how it lets you work with Workfront through natural-language conversation in an AI agentic platform.
author: Courtney
feature: Get Started with Workfront

---

# Adobe Workfront MCP server overview

The [!DNL Adobe Workfront] MCP server connects your Workfront instance to an AI agentic platform such as [!DNL Claude] or [!DNL ChatGPT]. From the AI agentic platform, you can find, create, update, and manage Workfront items by making natural-language requests.

For example, you can ask:

* *Show me all active projects for the Brand Marketing team.*
* *Update the "Design Review" task so it finishes on April 18.*
* *Send a reminder to approvers on the asset "Spring Campaign Video" who haven't responded.*

You don't need to know the Workfront API or how MCP servers work to use the Workfront MCP server.

>[!IMPORTANT]
>
>Currently, the Workfront MCP server is available only to customers using AWS.

## What an MCP server is

An MCP server is a connection point that lets an AI agentic platform work with another system. The Workfront MCP server is what your AI agentic platform connects to so it can read and act on your Workfront data on your behalf.

MCP stands for Model Context Protocol. This is the standard that defines how AI agentic platforms and outside systems talk to each other.

## Set up the connection

The Workfront MCP server works with any MCP-compatible AI agentic platform, such as [!DNL Claude] or [!DNL ChatGPT]. Before you can use it, the following needs to happen:

* A Workfront administrator must enable MCP server access in your Workfront instance.
* You (or your administrator) must connect your AI agentic platform to Workfront.

For more information, see [Configure the Adobe Workfront MCP server](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

## Start using the Workfront MCP server

After setup, you can ask your AI agentic platform to find, create, update, and manage Workfront items in natural language. 

For more information, including example requests, things to keep in mind, and information about data and security, see [Use the Adobe Workfront MCP server](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).
