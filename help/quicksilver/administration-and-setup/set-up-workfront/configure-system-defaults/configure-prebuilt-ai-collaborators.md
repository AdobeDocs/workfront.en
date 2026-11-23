---
user-type: administrator
product-area: system-administration;setup
title: Configure prebuilt AI Collaborators
description: As an Adobe Workfront administrator, you can configure prebuilt AI Collaborators from Adobe, such as the Intake Coordinator, as Work Agents that users can assign to tasks and issues.
author: Becky
feature: System Setup and Administration
role: Admin
---
# Configure prebuilt AI Collaborators

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

## Overview

Prebuilt AI Collaborators are ready-made Work Agents from Adobe that are set up to do a specific job, such as checking requests for missing information. They are available as Adobe Native Work Agents, so you don't need to configure an agent in an external platform or provide external-platform credentials.

When you configure a Work Agent, you select a prebuilt Collaborator as the agent's source. You can then name the Work Agent, set its access level, and choose the actions it can take. Users assign the configured Work Agent to tasks or issues in the same way they assign any other Work Agent. Users don't need to know that the agent is a prebuilt Collaborator.

For more information about Work Agents and the other AI Collaborator types, see [Configure AI Collaborators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Select, Prime, or Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td><p>[!UICONTROL Standard]</p></td> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator] or Group Administrator</td> 
  </tr> 
  </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites

Your organization must have Adobe CX Coworker enabled. For more information, see [Overview of CX Enterprise Coworker in Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

## Configure a prebuilt AI Collaborator

You configure a prebuilt AI Collaborator when you configure a Work Agent. In the **Choose agent's origin** area, select **Adobe Native**, then select the prebuilt Collaborator you want to use from the list below.

For the full steps, see [Configure a Work Agent in Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent-in-workfront).

After the Collaborator is configured, users can assign it to tasks or issues. For more information, see [Use Work Agents](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

## Available prebuilt AI Collaborators

### CX Enterprise Coworker {#cx-enterprise-coworker}

A CX Enterprise Coworker agent powered by the Adobe Agent Orchestrator.

For more information, see [Overview of CX Enterprise Coworker in Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

### Intake Coordinator {#intake-coordinator}

The Intake Coordinator checks the details, custom forms, and attachments of requests for missing, unclear, or inconsistent information. It posts feedback, or makes changes with the user's approval.

<!--
### Context Carrier {#context-carrier}

The Context Carrier keeps brief information flowing downstream so that context doesn't get scattered. It helps campaign managers and project managers keep the project team current without writing reports.

Requirements: A Workfront project and a Workfront Planning project must be connected to a Planning record. The Context Carrier must be triggered to run.

Steps to be added.

### Production Specialist {#production-specialist}

The Production Specialist produces images in every size you need, so designers don't have to resize them manually.

Requirement: Users must assign the Production Specialist to a task or issue.

Steps to be added.

### Version Comparer {#version-comparer}

The Version Comparer compares versions of a document so project teams can move content faster instead of spotting differences by hand.

Requirement: The document must have more than one version.

Steps to be added.

### Metadata Manager {#metadata-manager}

The Metadata Manager helps marketing teams find, tag, and label documents while work is in progress instead of later in the process.

Requirement: The Metadata Manager is available when you upload a document. Users must trigger it from the toolbar.

Steps to be added.

### Resource PTO Detector {#resource-pto-detector}

The Resource PTO Detector helps project teams make sure delivery isn't affected by time off, by identifying tasks assigned to people who are out of office.

Requirements: Tasks must be assigned, and PTO must be logged in Workfront.

Steps to be added.

### Campaign Summarizer {#campaign-summarizer}

Description and steps to be added.
-->
