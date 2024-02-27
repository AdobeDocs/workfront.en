---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Workfront Fusion release activity: Week of January 11, 2021'
description: This page describes all enhancements made in Adobe Workfront Fusion the week of January 11, 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 2439e2a7-9404-433a-bd71-a7776042d8a0
hidefromtoc: yes
---
# Workfront Fusion release activity:&nbsp;Week of January 11, 2021

This page describes all enhancements made in Adobe Workfront Fusion the week of January 11, 2021.

For a list of all recent changes, see [Adobe Workfront Fusion release activity](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

For a list of recent bug fixes in Workfront Fusion, see the [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) page and check for any updates labeled Workfront Fusion Maintenance Update.

## Widen connector and modules now available

You can now use Workfront Fusion to connect to your Widen account. With the Widen modules, you can:

* Add assets to or remove assets from a collection
* Download or upload files
* Read or update asset metadata
* Search assets based on criteria you specify
* Retrieve a list of assets in a collection
* Perform a custom API call.

For more information see [Widen modules](../../../workfront-fusion/apps-and-their-modules/widen-modules.md).

## Datadog connector and modules now available

You can now use Workfront Fusion to connect to your Datadog account.

With the Datadog modules, you can:

* Post timeseries points
* Perform a custom API call

For information about Datadog modules, see [Datadog modules](../../../workfront-fusion/apps-and-their-modules/datadog-modules.md).

## Cvent connector and modules now available

You can now use Workfront Fusion 2.0 to connect to your Cvent account.

With the Cvent modules, you can:

* Create a meeting request
* Read records such as contacts, events, or invitees
* List records based on criteria you specify
* Register or add invitees to specific events
* Update or delete contacts
* Make a custom API call

For information about available Cvent modules, see [Cvent modules](../../../workfront-fusion/apps-and-their-modules/cvent-modules.md).

## Microsoft Dynamics 365 connector and modules now available

You can now use Workfront Fusion 2.0 to connect to your Microsoft Dynamics 365 account. With the Microsoft Dynamics 365 modules, you can:

* Trigger a scenario when records are added or updated in Microsoft Dynamics 365
* Create, read, update, or delete a Microsoft Dynamics 365 record
* Perform a custom API call

For information about available Microsoft Dynamics 365 modules, see [Microsoft Dynamics 365 modules](../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

## DocuSign connector and modules now available

You can now use Workfront Fusion 2.0 to connect to your Docusign account. With the Docusign modules, you can:

* Trigger a scenario when an envelope changes its status
* Create an envelope
* Read, send, or add a recipient to an existing envelope
* Add or modify custom fields in documents
* Download a document as a filed
* Upload a file to an envelope
* Perform a custom API call

For more information, see [DocuSign modules](../../../workfront-fusion/apps-and-their-modules/docusign-modules.md).

## Search your scenario execution history

We've made it easier for you to locate specific information from previous scenario executions. Fusion's new full text search makes it possible to search execution history for any data contained in a bundle. For example, to identify which execution created a specific task, you could use full text search to search for that Task ID.

Previously, finding specific execution information required viewing each execution individually.

For more information, see [View a scenario's execution history in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Updates to Fusion 2.0 Data Store

To make it easier for you to customize your data stores, we've added some new functionality. Now when you're viewing a data store, you can:

* Drag and drop to reorder columns
* Edit a single cell
* Add multiple rows

For more information on Data Stores, see [Data store modules](../../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## Make an API Key authorization request through the HTTP connector

To increase flexibility in the ways you can access APIs, we've added a new module to the HTTP connector. Now, you can use the HTTP connector to make a request when the web service you are accessing requires the use of an API key.

For more information, see [HTTP modules](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

## New functions available in mapping panel

To help you customize and simplify formulas in your modules, we've added some new functions.

* The 

  ```
  omit
  ```

  function is a general function that omits the given keys of the object and returns the rest.
* The 

  ```
  pick
  ```

  function is a general function that picks only the given keys from the object.
* The 

  ```
  escapeMarkdown
  ```

  function is a string function that escapes all Markdown tags in a text.

For more information on the omit and pick functions, see [General functions in Adobe Workfront Fusion](../../../workfront-fusion/functions/general-functions.md).

For more information on the escapeMarkdown function, see [String functions in Adobe Workfront Fusion](../../../workfront-fusion/functions/string-functions.md).
