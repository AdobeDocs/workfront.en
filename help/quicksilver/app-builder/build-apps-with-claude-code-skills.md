---
title: Build App Builder apps with Claude Code skills
description: Use a set of Claude Code skills to build custom Adobe Workfront App Builder apps by describing what you want, instead of running the setup and deployment steps yourself.
author: Becky
feature: Digital Content and Documents
---

# Build App Builder apps with Claude Code skills

A set of [!DNL Claude Code] skills allows [!DNL Claude] to build custom [!DNL Adobe App Builder] apps for [!DNL Workfront]. This means that you can build one by describing what you want in plain English, without being a developer or writing the setup steps yourself.

Workfront UI Extensions, powered by Adobe App Builder, allow customers and partners to create customized user experiences. UI Extensions allow you to modify your organization's Workfront experience to better meet the needs of the organization, which can enhance efficiency, deliver seamless, connected experiences, and significantly improve user satisfaction, and help your organization realize its unique vision.

For more information about Workfront UI Extensions, see [Create custom applications for Workfront with Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## How these skills help

Normally, building on [!DNL Adobe App Builder] takes a developer: there's a command-line tool to install, a project to create in the Adobe Developer Console, a specific way to structure the code, a security model to respect, and a deploy-and-publish process. These skills hand all of that expertise to [!DNL Claude]. You describe the feature you want, and [!DNL Claude] does the hands-on work end to end — setting up the tools, creating your project in [!DNL Adobe App Builder], building the app, deploying it to Adobe's cloud, and getting it running inside Workfront — pausing only for the decisions and sign-ins that need you.

## Prerequisites

Before you start, make sure you have:

* **[!DNL Claude Code]** installed.
* **Access to the skills**, from either:
  * [https://gitlab.workfront.tech/helios/app-builder-skills](https://gitlab.workfront.tech/helios/app-builder-skills)
  * [https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md)

  If neither link opens for you, ask your admin for access.
* **[!DNL Adobe App Builder] access, with the Developer role.** Your Adobe organization needs an App Builder license, and you need to be added as a Developer in it — that's what lets [!DNL Claude] open the Adobe Developer Console and create your project.

  To check, open the [Adobe Developer Console](https://developer.adobe.com/console), confirm the organization shown in the top-right corner is correct, then click **Create new project > Create project from template**. If you see **App Builder** in the list, you have access; if not, ask your admin to add you as a Developer and confirm your organization has an App Builder license.

  If you plan to test on stage first, you need Developer access there too — check the same way at the [stage Developer Console](https://developer-stage.adobe.com/console).
* **The Workfront MCP server connected**, so [!DNL Claude] uses the real Workfront API instead of guessing at data types, fields, and commands. See [Adobe Workfront MCP server overview](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md). To check whether it's already connected, ask [!DNL Claude]: *"Can you see the Workfront MCP resources?"*
