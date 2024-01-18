---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
keywords: fusion
navigation-topic: fusion-release-activity
title: 'Workfront Fusion release activity: Week of November 30, 2020'
description: This page describes all enhancements made in Adobe Workfront Fusion the week of November 30, 2020.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 9621683b-735d-40a6-8d7c-b5bd167cbdd2
hidefromtoc: yes
---
# Workfront Fusion release activity:&nbsp;Week of November 30, 2020

This page describes all enhancements made in Adobe Workfront Fusion the week of November 30, 2020.

For a list of all recent changes, see [Adobe Workfront Fusion release activity](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

For a list of recent bug fixes in Workfront Fusion, see the [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) page and check for any updates labeled Workfront Fusion Maintenance Update.

## Rate limit for Workfront Fusion 2.0 webhooks.

We've introduced a new performance guardrail for Workfront Fusion 2.0. Now, webhooks have a rate limit of 100 requests per second. When this limit is reached, Workfront Fusion 2.0 sends a 429 (Too Many Requests) status.

Previously, webhook requests were not limited.

For more information, see [Adobe Workfront Fusion performance guardrails](../../../../../workfront-fusion/get-started/fusion-performance-guardrails.md).

## Add a custom form to a Workfront object in Workfront Fusion 2.0

To allow you to add custom forms to objects is Workfront Fusion 2.0, we've added a the AssignCategories action to the Workfront > Misc. Action module.

Previously, it was not possible to use a Workfront Fusion 2.0 module to add a custom form to an object in Workfront.

For more information on the Workfront > Misc. Action module, see [Adobe Workfront modules](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Jira Server connector and modules now available</h2>
<p>We've added a Jira Server connector to Workfront Fusion. The Jira Server connector offers the same functionality as the current Jira Cloud connector. </p>
<p>With Jira Server modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, modified, or deleted</p> </li>
<li> <p>Create, read, update, or delete a record</p> </li>
<li> <p>List or search records</p> </li>
<li> <p>Download an attachment</p> </li>
<li> <p>Add an issue to a sprint</p> </li>
<li> <p>Make a custom API call</p> </li>
</ul>
<p>Previously, Jira modules were available only for Jira Cloud.</p>
<p>For more information on available Jira modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref" xrefformat="{para}">Jira Software modules</a>.</p>
<h2>Azure DevOps connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Azure DevOps applications. With the Azure DevOps modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, updated, or deleted.</p> </li>
<li> <p>Create or update records.</p> </li>
<li> <p>Get data from existing records.</p> </li>
<li> <p>Download or upload attachments.</p> </li>
<li> <p>Link work items together.</p> </li>
<li> <p>Retrieve a list of work items.</p> </li>
<li> <p>Perform a custom API call.</p> </li>
</ul>
<p>For more information see <a href="../../../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref" xrefformat="{para}">Azure DevOps modules</a>.</p>
<h2>Microsoft Dynamics 365 connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Microsoft Dynamics 365 account. With the Microsoft Dynamics 365 modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when records are added or updated in Microsoft Dynamics 365</p> </li>
<li> <p>Create, read, update, or delete a Microsoft Dynamics 365record</p> </li>
<li> <p>Perform a custom API call</p> </li>
</ul>
<p>For information about available Microsoft Dynamics 365 modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref" xrefformat="{para}">Microsoft Dynamics 365 modules</a>.</p>
</div>
-->
