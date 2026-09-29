---
title: Build App Builder apps with Claude Code skills
description: Use a set of Claude Code skills to build custom Adobe Workfront App Builder apps by describing what you want, instead of running the setup and deployment steps yourself.
author: Becky
feature: Digital Content and Documents
hide: true
---

# Build App Builder apps with Claude Code skills

A skill package allows [!DNL Claude] (or any AI coding harness that supports Claude-formatted skills, such as [!DNL Claude Code] or [!DNL OpenAI Codex]) to build custom [!DNL Adobe App Builder] apps for [!DNL Workfront]. If you have access to one of these tools, you can build a UI extension by describing what you want in plain English, without requiring developer experience or manual setup steps.

Workfront UI Extensions, powered by Adobe App Builder, allow customers and partners to create customized user experiences. UI Extensions allow you to modify your organization's Workfront experience to better meet the needs of the organization, which can enhance efficiency, deliver seamless, connected experiences, and significantly improve user satisfaction, and help your organization realize its unique vision.

For more information about Workfront UI Extensions, see [Create custom applications for Workfront with Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## UI Extensibility skills

The UI Extensibility skills allow an AI coding harness to manage the creation of UI extensions in Workfront. You describe the feature you want, and it does the hands-on work, such as setting up the tools, creating your project in [!DNL Adobe App Builder], building the app, deploying it to Adobe's cloud, and getting it running inside Workfront. You are involved in the process only when there is a decision or login that requires action from you. This article uses [!DNL Claude] as the example, but the instructions apply to any AI coding harness with Claude Skills support.

## Prerequisites

Before you start, make sure you have:

* **An AI coding harness that supports Claude Skills**, such as [!DNL Claude Code].

  For more information on Claude Skills see [What are Skills?](https://support.claude.com/en/articles/12512176-what-are-skills) in the Claude documentation.

* **Access to the skills**. 

   * You can find the skills at [https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md).

      If this link does not open for you, ask your administrator to give you access.
   * The skills are published in Adobe's public skills marketplace ([adobe/skills](https://github.com/adobe/skills)). In [!DNL Claude Code], run:

      ```
      /plugin marketplace add adobe/skills
      ```

      ```
      /plugin install app-builder@adobe-skills
      ```

* **[!DNL Adobe App Builder] access, with the Developer role**. Your Adobe organization needs an App Builder license, and you must be added as a Developer in it. This is what lets [!DNL Claude] open the Adobe Developer Console and create your project.

  To check that this prerequisite is met:

  1. Open the [Adobe Developer Console](https://developer.adobe.com/console).
  1. Confirm the organization shown in the top-right corner is correct.
  1. Click **Create new project** > **Create project from template**.
  1. Check whether **App Builder** appears in the list.

     * If you see **App Builder** in the list, you have access.
     * If there's no **Create project from template** option, or no **App Builder** option, you don't have access yet. Ask your Workfront or Adobe admin to add you as a Developer (in the Adobe Admin Console > Users > Developers) and confirm your organization has an App Builder license.
* **The Workfront MCP server connected**, so [!DNL Claude] uses the real Workfront API instead of guessing at data types, fields, and commands. 

   To check whether the Workfront MCP server is already connected, ask [!DNL Claude]: *"Can you see the Workfront MCP resources?"*

  For more information and instructions, see [Connect Workfront to Claude](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#connect-workfront-to-claude)in the article Configure the Adobe Workfront MCP server.
