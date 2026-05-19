---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configure the Adobe Workfront MCP server
description: Configure your Workfront instance and your AI assistant so you can work with Workfront through natural-language conversation.
author: Courtney
feature: Get Started with Workfront
hide: true
---

# Configure the Adobe Workfront MCP server

The [!DNL Adobe Workfront] MCP server lets you work with your Workfront data through natural-language conversation in a supported AI assistant like Claude or ChatGPT.

Before you can connect an AI assistant to Workfront, a Workfront administrator must enable MCP server access in your Workfront instance. The exact steps to connect an AI assistant are different for each supported AI assistant. 

For more information about the Workfront MCP server, see [Adobe Workfront MCP server overview](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Supported agentic platforms

The Workfront MCP server currently supports the following AI assistants:

* [!DNL Claude]

<!-- NEEDS DETAIL: Update this list as Adobe adds support for additional AI assistants (for example, [!DNL Gemini], or [!DNL Microsoft Copilot]). -->


## Prerequisites

Before you can connect Workfront to an AI assistant, you must:

* Have an active [!DNL Adobe Workfront] account with permission to access the data you want to work with.
* Have access to an AI assistant like [!DNL Claude].

  <!-- NEEDS DETAIL: Confirm which Claude tiers are supported. Claude Enterprise is confirmed; Claude Pro and Claude Team support is unconfirmed. -->

### Admin prerequisites

MCP server access is gated by two separate administrators. Both must enable access before you can connect.

* **Your Workfront administrator** must enable MCP server access in your Workfront instance. - on by default can turn off if needed

* If you use an enterprise version of an AI assistant, your AI assistant administrator must enable the [!DNL Adobe Workfront] connector for your organization.


## Connect Workfront to Claude

You connect to Workfront once per [!DNL Claude] account. The connection authenticates you to a specific Workfront instance, and you stay connected until you choose to disconnect.


>[!IMPORTANT]
>
>If you use [!DNL Claude] Enterprise, **your [!DNL Claude] Enterprise administrator** must enable the [!DNL Adobe Workfront] connector for your organization. Until they do, the [!DNL Adobe Workfront] connector won't appear when you search for it in [!DNL Claude]. Contact your [!DNL Claude] administrator first.


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

## Connect to Gemini

## Connect to Microsoft Copilot

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

No. Each connection ties an AI assistant to a single Workfront instance. To switch, disconnect and reconnect, authenticating to the new instance.

### Does this work with Claude Pro or Claude Team, or only Claude Enterprise?

<!-- NEEDS DETAIL: Confirm Claude tier support and answer this directly. -->

### Which administrator enables this?

Both your Workfront administrator and your AI assistant administrator. Your Workfront administrator enables MCP server access on the Workfront side. Your AI assistant administrator enables Workfront access on the AI assistant side. For [!DNL Claude], the [!DNL Claude] Enterprise administrator enables the [!DNL Adobe Workfront] connector.

+++