---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configure the Adobe Workfront MCP server
description: Configure your Workfront instance and your AI agentic platform so you can work with Workfront through natural-language conversation.
author: Courtney
feature: Get Started with Workfront
hide: true
---

# Configure the Adobe Workfront MCP server

The [!DNL Adobe Workfront] MCP server lets you work with your Workfront data through natural-language conversation in a supported AI agentic platform like Claude or ChatGPT.

Before you can connect an AI agentic platform to Workfront, a Workfront administrator must enable MCP server access in your Workfront instance. The exact steps to connect an AI agentic platform are different for each supported AI agentic platform. 

For more information about the Workfront MCP server, see [Adobe Workfront MCP server overview](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Supported AI agentic platforms

The Workfront MCP server currently supports the following AI agentic platforms:

* [!DNL Claude]

<!-- NEEDS DETAIL: Update this list as Adobe adds support for additional AI agentic platforms (for example, [!DNL Gemini], or [!DNL Microsoft Copilot]). -->


## Prerequisites

Before you can connect Workfront to an AI agentic platform, you must:

* Have an active [!DNL Adobe Workfront] account with permission to access the data you want to work with.
* Have access to an AI agentic platform like [!DNL Claude].

  <!-- NEEDS DETAIL: Confirm which Claude tiers are supported. Claude Enterprise is confirmed; Claude Pro and Claude Team support is unconfirmed. -->

### Admin prerequisites

MCP server access is gated by two separate administrators. Both must enable access before you can connect.

* **Your Workfront administrator** must enable MCP server access in your Workfront instance. - on by default can turn off if needed

* If you use an enterprise version of an AI agentic platform, your administrator for that platform must enable the [!DNL Adobe Workfront] connector for your organization.


## Connect Workfront to Claude

You connect to Workfront once per [!DNL Claude] account. The connection authenticates you to a specific Workfront instance, and you stay connected until you choose to disconnect.


>[!IMPORTANT]
>
>If you use [!DNL Claude] Enterprise, **your [!DNL Claude] Enterprise administrator** must enable the [!DNL Adobe Workfront] connector for your organization. Until they do, the [!DNL Adobe Workfront] connector won't appear when you search for it in [!DNL Claude]. Contact your [!DNL Claude] administrator first.

### Connect from the connectors directory

+++ Expand to view step-by-step instructions for connecting Workfront to [!DNL Claude].

To connect Workfront to [!DNL Claude]:

1. Open [!DNL Claude].

1. Navigate to the connectors area.

   <!-- NEEDS DETAIL: Exact menu path (for example, "Click Settings, then click Connectors"). -->

1. Find **[!DNL Adobe Workfront]** in the connector list.

   If you don't see it, see [Admin prerequisites](#admin-prerequisites) in this article.

1. Click **Connect**.

   <!-- NEEDS DETAIL: Confirm the exact button label. -->

1. When prompted, log in to your Workfront instance.

   <!-- NEEDS DETAIL: Describe the auth flow — does it open a new browser tab, an in-app window, prompt for a Workfront domain? -->

1. After authentication completes, you're connected.

   <!-- NEEDS DETAIL: Add a screenshot of the connected state in Claude. -->

+++

### Connect with a URL

+++ Expand to view step-by-step instructions for connecting Workfront to [!DNL Claude] with a URL.

To connect Workfront to [!DNL Claude] with a URL:

1. Log in to [Claude](https://claude.ai) using your credentials.
1. In the left menu, select the **Customize** icon.
1. Select **Connectors**, then select the **+** icon to add a connector.
1. Select the **Create app** button.
1. Give the connector a desired name (such as "Workfront") and enter the desired MCP Server URL: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
   
1. Once the connector is created, a login window pops up. Authenticate using your Adobe ID credentials. Ensure that you select the desired Workfront instance if you belong to more than one.

+++

### Verify your connection

To confirm [!DNL Claude] is connected to Workfront, ask [!DNL Claude] to list the actions the Workfront MCP server makes available. For example:

* *What Workfront actions can you take?*
* *List the Workfront tools you have access to.*

[!DNL Claude] returns the list of available actions.

<!-- NEEDS DETAIL: Add a screenshot of the tool-list response. -->

### Switch to a different Workfront instance -- might need to be its own section

Each connection authenticates [!DNL Claude] to a single Workfront instance. To use a different instance, disconnect and reconnect.

To connect to a different Workfront instance:

1. In [!DNL Claude], disconnect the [!DNL Adobe Workfront] connector.
1. Reconnect the connector.
1. Authenticate to the new Workfront instance.

>[!NOTE]
>
>Logging out of [!DNL Claude] alone doesn't switch the Workfront instance. You must disconnect and reconnect the connector.

### Customize Claude behavior with skills - may need to be its own section

<!-- NEEDS DETAIL: Confirm whether Adobe is shipping any pre-built Claude skills alongside the MCP server. If yes, list them and link to download or installation guidance. If no, decide whether to mention skills as a user-driven workaround at all, or remove this section. -->

[!DNL Claude] supports user-created instruction sets called skills. You can use a skill to customize how [!DNL Claude] behaves with Workfront. For example, you can create a skill that tells [!DNL Claude] to always fetch fresh data from Workfront instead of relying on earlier results.

To learn more about [!DNL Claude] skills, see the [Claude user documentation](https://code.claude.com/docs/en/skills) or ask Claude for help with skills.

## Connect to ChatGPT 

1. Log in to [ChatGPT](https://chatgpt.com) using your credentials.
1. In the lower left, select **your name** → **Settings**.
1. Select **Apps**, then enable **Developer mode**.
1. Select the **Create app** button.
1. Give the app a desired name (such as "Workfront") and enter the desired MCP Server URL: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
1. Ensure that Authentication is set to **OAuth** (set by default), and select the acceptance check box to continue.
1. Once the app is created, a login window pops up. Authenticate using your Adobe ID credentials. Ensure that you select the desired Workfront instance if you belong to more than one.

<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
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
|---|---|---|
| You can't find the [!DNL Adobe Workfront] connector in [!DNL Claude]. | Your [!DNL Claude] administrator hasn't enabled it. | Contact your [!DNL Claude] administrator (not your Workfront administrator) and ask them to enable the [!DNL Adobe Workfront] connector. |
| You connected, but you can't see your data. | You authenticated to the wrong Workfront instance. | Disconnect the connector, reconnect, and authenticate to the correct instance. |
| Authentication failed, or the connection stopped working. | Your auth session expired or there's a connection error. | Disconnect and reconnect the connector. |
| You want to switch to a different Workfront instance. | A single connection ties you to one instance. | Disconnect, reconnect, and authenticate to the new instance. |

Admin has disabled MCP server access. | Your Workfront administrator has turned off MCP server access for your instance. | Contact your Workfront administrator to confirm whether MCP server access is enabled. If it's disabled, request that they enable it if you want to use the MCP server. |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

For day-to-day troubleshooting after you're connected (for example, stale results or unexpected behavior), see [Use the Adobe Workfront MCP server](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).

+++

## Frequently asked questions about setup

+++ Expand to view frequently asked questions about setting up the Workfront MCP server.

### Can I connect to multiple Workfront instances at once?

No. Each connection ties an AI agentic platform to a single Workfront instance. To switch, disconnect and reconnect, authenticating to the new instance.

### Does this work with Claude Pro or Claude Team, or only Claude Enterprise?

<!-- NEEDS DETAIL: Confirm Claude tier support and answer this directly. -->

### Which administrator enables this?

Both your Workfront administrator and the administrator for your AI agentic platform. Your Workfront administrator enables MCP server access on the Workfront side. The administrator for your AI agentic platform enables Workfront access on that platform's side. For [!DNL Claude], the [!DNL Claude] Enterprise administrator enables the [!DNL Adobe Workfront] connector.

+++