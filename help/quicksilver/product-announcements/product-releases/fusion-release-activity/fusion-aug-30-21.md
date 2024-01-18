---
title: Workfront Fusion release activity:&nbsp;Week of August 30, 2021
description: Workfront Fusion release activity:&nbsp;Week of August 30, 2021
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: yes
---
# Workfront Fusion release activity:&nbsp;Week of August 30, 2021

This page describes all enhancements made in Adobe Workfront Fusion the week of August 30, 2021.

For a list of all recent changes, see [Adobe Workfront Fusion release activity](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

For a list of recent bug fixes in Workfront Fusion, see the [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) page and check for any updates labeled Workfront Fusion Maintenance Update.

## Filter events that trigger the Workfront > Watch events module

1. Set up a custom filter for events that trigger the Workfront > Watch events module

   To reduce the number of unnecessary scenario runs, we've updated the Workfront > Watch records module to enable event filtering. Now, you can set a filter when you create a webhook. This allows the scenario to trigger only when the event meets certain criteria.

   The event filter currently offers the following operations:

   * Equal: Trigger a scenario only when an event matches the conditions of the filter. For example, you could set up a filter that triggers a scenario only if the event occurs in a specific project.
   * Not Equal: Trigger a scenario only if an event does not match the conditions of the filter. For example, you can could create a filter that triggers a scenario only if the issue an event occurs in does not have a status of Closed.

   Previously, the Watch records module would retrieve all records. Users could filter only by setting up filters later in the scenario.

   To take advantage of event filtering, create a new webhook in your Watch events module. It is not currently possible to edit existing webhooks to include this functionality. We highly recommend that you create new webhooks using event filters for your existing scenarios.

1. Filter out events triggered by the current connection.

   To make your webhooks easier to set up for the Workfront > Watch events module, we've included the most common event filter. Now, the webhook has an option to filter out any changes made by modules using the connection specified for the Watch events module. In other words, with this filter enabled, any changes made by the Workfront user associated with that connection cannot trigger the scenario.

   Previously, this filter was not available. Therefore, it was easier for changes made in Workfront modules to trigger scenarios containing those modules, potentially causing scenarios to trigger themselves in an infinite loop.

For more information on event filters in the Workfront > Watch events module, see [Adobe Workfront modules](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

