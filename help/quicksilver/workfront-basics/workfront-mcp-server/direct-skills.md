---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Skills available for direct install
description: Workfront offers some skills that you can install directly in your LLM.
author: Becky
feature: Get Started with Workfront

---

# Skills available for direct install

Workfront offers some skills that you can install directly in your LLM. Skills guide how those tools are used for specific tasks, with the right steps already built in.

You can find these skills on the Adobe Skills GitHub repo.

>[!NOTE]
>
>Currently, these skills are available only for Claude.
>For instructions on getting Claude set up with Adobe, see [Getting started](https://developer.adobe.com/adobe-for-creativity/getting-started/) in the Adobe Developer documentation.

## Install a skill from the Workfront GitHub repo into Claude. 

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
