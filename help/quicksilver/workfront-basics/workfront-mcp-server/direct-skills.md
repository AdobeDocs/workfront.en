---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Skills available for direct install
description: Workfront offers some skills that you can install directly in your LLM.
author: Becky
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog

---

# Skills available for direct install

Adobe Workfront offers some skills that you can install directly in your LLM. Skills guide how those tools are used for specific tasks, with the right steps already built in.

You can find these skills as files on the Adobe Skills GitHub repo. This repository contains files for a variety of Adobe products. When you download these files and copy them to Claude, Claude can then use the skills described in the files. 

For example, the Planning Solution Architect skills allows Claude to answer questions about and perform some actions in Workfront Planning.

You do not need to call or trigger these skills after they are copied to the LLM. Instead, you can interact with your LLM as usual, asking questions in natural language, and the LLM uses the information and actions described in the skill that are appropriate to the conversation.

>[!NOTE]
>
>Currently, these skills are available only for Claude.
>For instructions on getting Claude set up with Adobe, see [Getting started](https://developer.adobe.com/adobe-for-creativity/getting-started/) in the Adobe Developer documentation.

## Install a skill from the Workfront GitHub repo into Claude

1. Go to the [Adobe Workfront skills repository](https://github.com/adobe/skills/tree/main/plugins/workfront) on GitHub.
1. Download the skill folder you want to use.
1. Copy the folder into your Claude skills library.

   * Claude Desktop: `~/Library/Application Support/Claude/skills/` (macOS) or equivalent.
   * Claude Code: `~/.claude/skills/`.

<!--

1. Go to the [Adobe Workfront skills repository](https://github.com/adobe/skills/tree/main/plugins/workfront) on GitHub.
1. Download the skill file you want to use.
1. In Claude, click **Customize**.
1. Select **Skills**.
1. Click **Create skill** -> **Upload a skill**.
1. Upload the zipped skill file to Claude, then click **Confirm** to install.

-->

## Currently available skills

|Skill / Link to folder|Skill description|Available for|
|---|---|---|
|[Planning Solution Architect](https://github.com/adobe/skills/tree/main/plugins/workfront/skills/wf-planning-solution-architect)|Configure a Workfront Planning workspace to meet your needs, and answer questions about Workfront Planning.|Claude|
