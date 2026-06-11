---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configure the Adobe Workfront MCP server
description: Configure your Workfront instance and your AI agentic platform so you can work with Workfront through natural-language conversation.
author: Courtney
feature: Get Started with Workfront

---

# Configure the Adobe Workfront MCP server

{{highlighted-preview-article-level}}

The [!DNL Adobe Workfront] MCP server lets you work with your Workfront data through natural-language conversation in a supported AI agentic platform.

Before you can connect an AI agentic platform to Workfront, a Workfront administrator must enable MCP server access in your Workfront instance. The exact steps to connect an AI agentic platform are different for each supported AI agentic platform. 

>[!IMPORTANT]
>
>Currently, the Workfront MCP server is available only to customers in the US region for customers using AWS.

## Supported AI agentic platforms

The Workfront MCP server works with any AI agentic platform that supports the Model Context Protocol (MCP).

This article walks through the connection steps for:

* [!DNL Claude]
* [!DNL ChatGPT]

If you use a different MCP-compatible AI agentic platform (for example, [!DNL Gemini] or [!DNL Microsoft Copilot]), follow the steps in that platform's documentation for adding a custom MCP server. When prompted for the MCP server URL, enter the URL for your region: 

   | Region | URL |
   | --- | --- |
   | US | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | EU | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

## Prerequisites

Before you can connect Workfront to an AI agentic platform, you must:

* Have an active [!DNL Adobe Workfront] account with permission to access the data you want to work with
* Have access to an AI agentic platform like [!DNL Claude]
* Your Workfront instance must be enabled on Adobe Identity Management System (IMS).
* To use MCP with Workfront Planning, your organization must be on a Workfront package that includes Adobe Workfront Planning.


### Admin prerequisites

MCP server access is gated by two separate administrators. 

* Your Workfront administrator controls MCP server access for your Workfront instance through two toggles in System Preferences: **Read-only MCP tools** (enabled by default) and **Write MCP tools** (disabled by default). If you can find Workfront items through the AI agentic platform but can't create, update, or delete them, ask your Workfront administrator to enable write actions.

   For more information, see [Configure system preferences](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* If you use an enterprise version of an AI agentic platform, your administrator for that platform must enable the [!DNL Adobe Workfront] connector for your organization or give you custom URL access to connect to the Workfront MCP server.


## Connect Workfront to Claude

You connect to Workfront once per [!DNL Claude] account. The connection authenticates you to a specific Workfront instance, and you stay connected until you choose to disconnect.



### Connect to Claude desktop from the connectors directory

>[!IMPORTANT]
>
>Currently, the Claude Connector only supports connecting to the Workfront MCP server in the US region.  To connect to a Workfront instance in the EU region, see [Connect to Claude desktop with a URL](#connect-to-claude-desktop-with-a-url) in this article.

+++ Expand to view step-by-step instructions for connecting Workfront to [!DNL Claude].

To connect Workfront to [!DNL Claude]:

1. Open [!DNL Claude].

1. Navigate to the connectors area.



1. Find **[!DNL Adobe Workfront]** in the connector list.

   If you don't see it, see [Admin prerequisites](#admin-prerequisites) in this article.

1. Click **Connect**.



1. When prompted, log in to your Workfront instance.


1. After authentication completes, you're connected.



+++

### Connect to Claude desktop with a URL

+++ Expand to view step-by-step instructions for connecting Workfront to [!DNL Claude] with a URL.

To connect Workfront to [!DNL Claude] with a URL:

1. Log in to [Claude](https://claude.ai) using your credentials.
1. In the left menu, select the **Customize** icon.
1. Select **Connectors**, then select the **+** icon to add a connector.
1. Select the **Create app** button.
1. Give the connector a desired name (such as "Workfront") and enter the desired MCP Server URL: 

   | Region | URL |
   | --- | --- |
   | US | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | EU | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |
   
1. After the connector is created, a login window pops up. Authenticate using your Adobe ID credentials. Ensure that you select the desired Workfront instance if you belong to more than one.

   >NOTE:
   >
   >Your Workfront instance must connect with the MCP server for the region for that instance. For example, an EU instance must connect to the EU MCP server. 
   >
   >When selecting an instance, instances that are not compatible with the MCP server's region appear grayed out, and you cannot connect to them. 
   >
   >To connect to an instance that is not compatible with the MCP server's region, set up a new MCP connection with the correct URL for that region.

+++

### Customize Claude behavior with skills

[!DNL Claude] supports user-created instruction sets called skills. You can use a skill to customize how [!DNL Claude] behaves with Workfront. For example, you can create a skill that tells [!DNL Claude] to always fetch fresh data from Workfront instead of relying on earlier results.

To learn more about [!DNL Claude] skills, see the [Claude user documentation](https://code.claude.com/docs/en/skills) or ask Claude for help with skills.

## Connect to ChatGPT 

1. Log in to [ChatGPT](https://chatgpt.com) using your credentials.
1. In the lower left, select **your name** → **Settings**.
1. Select **Apps**, then enable **Developer mode**.
1. Select the **Create app** button.
1. Give the app a desired name (such as "Workfront") and enter the desired MCP Server URL:  

   | Region | URL |
   | --- | --- |
   | US | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | EU | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |
   
1. Ensure that Authentication is set to **OAuth** (set by default), and select the acceptance check box to continue.
1. After the app is created, a login window pops up. Authenticate using your Adobe ID credentials. Ensure that you select the desired Workfront instance if you belong to more than one.

   >NOTE:
   >
   >Your Workfront instance must connect with the MCP server for the region for that instance. For example, an EU instance must connect to the EU MCP server. 
   >
   >When selecting an instance, instances that are not compatible with the MCP server's region appear grayed out, and you cannot connect to them. 
   >
   >To connect to an instance that is not compatible with the MCP server's region, set up a new MCP connection with the correct URL for that region.


### Customize ChatGPT behavior with Custom GPTs

ChatGPT supports user-created assistants called Custom GPTs. You can use a Custom GPT to customize how ChatGPT behaves with your connector. For example, you can create a Custom GPT that tells ChatGPT to always fetch fresh data from your connected service instead of relying on earlier results.

To learn more about Custom GPTs, see the [ChatGPT user documentation](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts) or ask ChatGPT for help with Custom GPTs.

## Verify your connection

To confirm the AI agentic platform is connected to Workfront, ask the AI agentic platform to list the actions the Workfront MCP server makes available. For example:

* *What Workfront actions can you take?*
* *List the Workfront tools you have access to.*

You can also see the full list of tools in [Adobe Workfront MCP server tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

## Available tools

The Workfront MCP server exposes a set of tools that the connected AI agentic platform calls on your behalf — for example, tools to search Workfront, create items, update fields, and manage approvals. For the full reference list, grouped by Workfront area, see [Adobe Workfront MCP server tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

## Switch to a different Workfront instance

Each connection authenticates the AI agentic platform to a single Workfront instance. To use a different instance, disconnect and reconnect.

To connect to a different Workfront instance:

1. In the AI agentic platform, disconnect the Workfront MCP server.
1. Reconnect the connector.
1. Authenticate to the new Workfront instance.

>[!NOTE]
>
>* Logging out alone doesn't switch the Workfront instance. You must disconnect and reconnect the connector.
>
>* Your Workfront instance must connect with the MCP server for the region for that instance. For example, an EU instance must connect to the EU MCP server. 
>
>   When selecting an instance, instances that are not compatible with the MCP server's region appear grayed out, and you cannot connect to them. 
>
>   To connect to an instance that is not compatible with the MCP server's region, set up a new MCP connection with the correct URL for that region.


<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server:  

   | Region | URL |
   | --- | --- |
   | US | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | EU | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |
   
-->

<!--
## Connect to Microsoft Copilot

✅ 1) Copilot Studio (most common for agents / enterprise use)
This is the cleanest "paste a URL" flow.
Steps
1. Open your Copilot Studio agent
2. Go to Tools
3. Click:
    * Add a tool → New tool → Model Context Protocol
4. In the wizard, fill in:
    * Server name (anything)
    * Server description
    * ✅ Server URL (your MCP endpoint)
5. Choose auth (if needed):
    * None / API key / OAuth
6. Click Create
👉 That's it—your MCP server is now attached to the agent.
This flow is explicitly documented:
* You add MCP via Tools → Add tool → Model Context Protocol
* Then provide Server name, description, and URL ￼
￼
What happens next
* Copilot discovers tools automatically from the MCP server
* You can enable/disable tools per agent
* The agent calls them when relevant

-->

## Troubleshoot setup and authentication

+++ Expand to view troubleshooting tips for setup and authentication of the Workfront MCP server.

| Problem | Likely cause | Fix |
| --- | --- | --- |
| You can't find the [!DNL Adobe Workfront] connector in [!DNL Claude]. | Your [!DNL Claude] administrator hasn't enabled it. | Contact your [!DNL Claude] administrator (not your Workfront administrator) and ask them to enable the [!DNL Adobe Workfront] connector. |
| You connected, but you can't see your data. | You authenticated to the wrong Workfront instance. | Disconnect the connector, reconnect, and authenticate to the correct instance. |
| Authentication failed, or the connection stopped working. | Your auth session expired or there's a connection error. | Disconnect and reconnect the connector. |
| You want to switch to a different Workfront instance. | A single connection ties you to one instance. | Disconnect, reconnect, and authenticate to the new instance. |
| You can't connect to Workfront, or you see a message that MCP server access is disabled. | Your Workfront administrator has turned off MCP server access for your instance. | Contact your Workfront administrator and ask them to enable MCP server access in System Preferences. |
| The Workfront instance that you want to connect to is grayed out, and you see a message that it is not available to connect in your region | Your MCP server is configured for a different region (EU or US) than your instance. | Set up the MCP server with the URL for the region that your Workfront instance is assigned to. |
| The AI agentic platform can find your Workfront items but can't create, update, or delete them. | Your Workfront administrator has disabled write actions for the Workfront MCP server. | Contact your Workfront administrator and ask them to enable write actions in System Preferences. |

For day-to-day troubleshooting after you're connected (for example, stale results or unexpected behavior), see [Use the Adobe Workfront MCP server](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).


+++

## Frequently asked questions about setup

+++ Expand to view frequently asked questions about setting up the Workfront MCP server.

### Can I connect to multiple Workfront instances at the same time?

No. Each connection ties an AI agentic platform to a single Workfront instance. To switch, disconnect and reconnect, authenticating to the new instance.

### Which administrator enables this?

Both your Workfront administrator and the administrator for your AI agentic platform. Your Workfront administrator enables MCP server access on the Workfront side. The administrator for your AI agentic platform enables Workfront access on that platform's side. For [!DNL Claude], the [!DNL Claude] Enterprise administrator enables the [!DNL Adobe Workfront] connector.

### Can I use the Workfront MCP server if my Workfront instance isn't enabled on Adobe Identity Management System (IMS)?

No. Your Workfront instance must be enabled on Adobe Identity Management System (IMS) to use the Workfront MCP server. If you're not sure whether your instance is enabled on IMS, contact your Workfront administrator.

+++ 
