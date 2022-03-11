---
filename: fusion-nov-30
product: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
keywords: fusion
navigation-topic: fusion-release-activity
title: Workfront Fusion release activity: Week of November 30, 2020
description: This page describes all enhancements made in Adobe Workfront Fusion the week of November 30, 2020.
---

# `Workfront Fusion` release activity:&nbsp;Week of November 30, 2020

This page describes all enhancements made in `Adobe Workfront Fusion` the week of `November 30, 2020`.

For a list of all recent changes, see [Adobe Workfront Fusion release activity](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

For a list of recent bug fixes in `Workfront Fusion`, see the [ `Workfront` Maintenance Updates](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) page and check for any updates labeled `Workfront Fusion` Maintenance Update.

## Rate limit for Workfront Fusion 2.0 webhooks.

We’ve introduced a new performance guardrail for Workfront Fusion 2.0. Now, webhooks have a rate limit of 100 requests per second. When this limit is reached, Workfront Fusion 2.0 sends a 429 (Too Many Requests) status.

Previously, webhook requests were not limited.

For more information, see [Adobe Workfront Fusion performance guardrails](../../../../../workfront-fusion/get-started/fusion-performance-guardrails.md).

## Add a custom form to a Workfront object in Workfront Fusion 2.0

To allow you to add custom forms to objects is Workfront Fusion 2.0, we've added a the AssignCategories action to the Workfront > Misc. Action module.

Previously, it was not possible to use a Workfront Fusion 2.0 module to add a custom form to an object in Workfront.

For more information on the Workfront > Misc. Action module, see [Adobe Workfront modules](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

<!--
Jira Server connector and modules now available We've added a Jira Server connector to Workfront Fusion. The Jira Server connector offers the same functionality as the current Jira Cloud connector. With Jira Server modules, you can: Trigger a scenario when a record is added, modified, or deleted Create, read, update, or delete a record List or search records Download an attachment Add an issue to a sprint Make a custom API call Previously, Jira modules were available only for Jira Cloud. For more information on available Jira modules, see Jira Software modules. Azure DevOps connector and modules now available You can now use Workfront Fusion to connect to your Azure DevOps applications. With the Azure DevOps modules, you can: Trigger a scenario when a record is added, updated, or deleted. Create or update records. Get data from existing records. Download or upload attachments. Link work items together. Retrieve a list of work items. Perform a custom API call. For more information see Azure DevOps modules. Microsoft Dynamics 365 connector and modules now available You can now use Workfront Fusion to connect to your Microsoft Dynamics 365 account. With the Microsoft Dynamics 365 modules, you can: Trigger a scenario when records are added or updated in Microsoft Dynamics 365 Create, read, update, or delete a Microsoft Dynamics 365record Perform a custom API call For information about available Microsoft Dynamics 365 modules, see Microsoft Dynamics 365 modules.
-->

