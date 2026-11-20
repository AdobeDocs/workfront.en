---
content-type: overview;how-to-procedural
product-area: ai
navigation-topic: ai-collaborators
title: Use prebuilt AI Collaborators
description: Prebuilt AI Collaborators are ready-made Collaborators from Adobe that you can start using right away. Find out what each one does and how to use it.
author: Becky
feature: Get Started with Workfront
---
# Use prebuilt AI Collaborators

<!-- becky check me:
- Placeholder article. Confirm the names, descriptions, and where each Collaborator can be assigned with the product team.
- Fill in the steps in each Collaborator section. Keep each section heading and anchor ID stable; other articles link to them.
- Verify the access table (license and access level are guesses).
- Confirm the preview snippet and availability dates.
- Sections for Context Carrier, Production Specialist, Version Comparer, Metadata Manager, and Resource PTO Detector come from the Demo Gallery AI Collaborators doc. Confirm names and release timing.
- Campaign Summarizer (in the Nov 11 product review deck) is not in the Demo Gallery doc. It is commented out until confirmed.
- The Firefly resizing Collaborator is called "Firefly Image Resizer" in the Nov 11 product review deck, "Content Resizer" in the Workfront project name, and "Production Specialist" in the Demo Gallery doc (exported Nov 20, the most recent source). The article uses Production Specialist. Confirm the final name.
- Provisioning note (about 30 seconds, spinner) comes from Jeremy Flores in Slack on Nov 18. Confirm the wording and where the toggle is in the UI, and move the note next to the steps once they are added.
- Confirm which Collaborators ship in November vs. later (Intake Coordinator v2 and Project Coordinator v2 are November commits).
- Add exl-id, last-update, and other frontmatter tags before publishing.
- Other articles that should link to sections here: configure-ai-collaborators.md, use-task-collaborators.md, use-project-coordinator.md, and 27-q1-ai.md release notes. Do not move those articles yet.
-->

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

## Overview

Prebuilt AI Collaborators are ready-made Collaborators from Adobe that are set up to do a specific job. You can start using them without building a Collaborator from scratch. Adobe's defaults are a starting point, so you can customize the fields, sources, and outputs a Collaborator uses to fit your business.

For information about how administrators configure AI Collaborators, see [Configure AI Collaborators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Contribute access or higher to the object you are using the Collaborator on</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher to the object you are using the Collaborator on</p> </td> 
  </tr> 
 </tbody> 
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you can use a prebuilt AI Collaborator, a Workfront administrator must enable and configure AI Collaborators for your organization. For more information, see [Configure AI Collaborators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Add a prebuilt AI Collaborator

Steps to be added.

>[!NOTE]
>
>After you turn on a prebuilt AI Collaborator, it takes about 30 seconds to be provisioned. A spinner displays until the Collaborator is ready.

## Project Coordinator {#project-coordinator}

The Project Coordinator checks the status and general health of a project and posts its findings as a comment.

For more information, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).

## Intake Coordinator {#intake-coordinator}

The Intake Coordinator checks requests and identifies missing or incorrect information. It can also read a brief, identify issues, and update custom forms with the user's consent.

Steps to be added.

## Context Carrier {#context-carrier}

The Context Carrier keeps brief information flowing downstream so that context doesn't get scattered. It helps campaign managers and project managers keep the project team current without writing reports.

Requirements: A Workfront project and a Workfront Planning project must be connected to a Planning record. The Context Carrier must be triggered to run.

Steps to be added.

## Production Specialist {#production-specialist}

The Production Specialist produces images in every size you need, so designers don't have to resize them manually.

Requirement: You must assign the Production Specialist to a task or issue.

Steps to be added.

## Version Comparer {#version-comparer}

The Version Comparer compares versions of a document so project teams can move content faster instead of spotting differences by hand.

Requirement: The document must have more than one version.

Steps to be added.

## Metadata Manager {#metadata-manager}

The Metadata Manager helps marketing teams find, tag, and label documents while work is in progress instead of later in the process.

Requirement: The Metadata Manager is available when you upload a document. You must trigger it from the toolbar.

Steps to be added.

## Resource PTO Detector {#resource-pto-detector}

The Resource PTO Detector helps project teams make sure delivery isn't affected by time off, by identifying tasks assigned to people who are out of office.

Requirements: Tasks must be assigned, and PTO must be logged in Workfront.

Steps to be added.

<!--
## Campaign Summarizer {#campaign-summarizer}

Description and steps to be added.
-->
