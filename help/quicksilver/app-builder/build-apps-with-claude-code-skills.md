---
title: Build App Builder apps with Claude Code skills
description: Use a set of Claude Code skills to build custom Adobe Workfront App Builder apps by describing what you want, instead of running the setup and deployment steps yourself.
author: Becky
feature: Digital Content and Documents
hide: true
---

# Build App Builder apps with Claude Code skills

A skill package lets [!DNL Claude] — or any AI coding harness that supports Claude-formatted skills, such as [!DNL Claude Code] or [!DNL OpenAI Codex] — build custom [!DNL Adobe App Builder] apps for [!DNL Workfront]. If you have access to one of these tools, building a UI Extension is as simple as describing what you want in plain English: no developer experience and no manual setup steps required.

Workfront UI Extensions, powered by Adobe App Builder, allow customers and partners to create customized user experiences. UI Extensions allow you to modify your organization's Workfront experience to better meet the needs of the organization, which can enhance efficiency, deliver seamless, connected experiences, and significantly improve user satisfaction, and help your organization realize its unique vision.

For more information about Workfront UI Extensions, see [Create custom applications for Workfront with Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## UI Extensibility skills

The UI Extensibility skills put an AI coding harness in the driver's seat. You describe the feature you want, and it does the hands-on work, such as setting up the tools, creating your project in [!DNL Adobe App Builder], building the app, deploying it to Adobe's cloud, and getting it running inside [!DNL Workfront]. You are involved in the process only when there is a decision or login that requires action from you. This article uses [!DNL Claude] as the example, but the instructions apply to any AI coding harness with Claude Skills support.

## Prerequisites

Before you start, make sure you have:

* **An AI coding harness that supports Claude Skills**, such as [!DNL Claude Code]. See [What are Skills?](https://support.claude.com/en/articles/12512176-what-are-skills) for the official definition.
* **Access to the skills**. 

   * The skills are published in Adobe's public skills marketplace ([adobe/skills](https://github.com/adobe/skills)). In [!DNL Claude Code], run:

      ```
      /plugin marketplace add adobe/skills
      ```

      ```
      /plugin install app-builder@adobe-skills
      ```

      Once installed, the skill is available as `/app-builder:appbuilder-workfront`. If this fails, ask your administrator to give you access.
   * Using a different AI coding harness? Point it at the skill file directly: [SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md).

* **[!DNL Adobe App Builder] access, with the Developer role**. Your Adobe organization needs an App Builder license, and you must have the Developer (or System Administrator) role for it in Adobe Admin Console. This is what lets [!DNL Claude] open the Adobe Developer Console and create your project — the skill creates the project for you, so you don't need to do this step yourself.

  If you're not sure whether you have this access, ask your Workfront or Adobe admin to confirm your organization has an App Builder license and that you're assigned the Developer role for it (Adobe Admin Console > Products > App Builder > Users > Developers). For the exact steps admins use to grant this role, see [Set up access, environment, and tools](https://developer.adobe.com/app-builder/docs/get_started/app_builder_get_started/set-up) in the App Builder documentation.
* **The Workfront MCP server connected**, so [!DNL Claude] uses the real Workfront API instead of guessing at data types, fields, and commands. 

   To check whether the Workfront MCP server is already connected, ask [!DNL Claude]: *"Can you see the Workfront MCP resources?"*

  For more information and instructions, see [Connect Workfront to Claude](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#connect-workfront-to-claude)in the article Configure the Adobe Workfront MCP server.
