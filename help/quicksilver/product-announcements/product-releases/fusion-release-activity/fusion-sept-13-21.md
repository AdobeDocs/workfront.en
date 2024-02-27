---
title: Workfront Fusion release activity:&nbsp;Week of September 13, 2021
description: Workfront Fusion release activity:&nbsp;Week of September 13, 2021
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: d9056d6f-a62d-4516-930e-4c3f4fbaec3e
hidefromtoc: yes
---
# Workfront Fusion release activity:&nbsp;Week of September 13, 2021

This page describes all enhancements made in Adobe Workfront Fusion the week of September 23, 2021.

For a list of all recent changes, see [Adobe Workfront Fusion release activity](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

For a list of recent bug fixes in Workfront Fusion, see the [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) page and check for any updates labeled Workfront Fusion Maintenance Update.

## Filter and sort Workfront Fusion scenario execution history

To make it easier to find specific scenario executions, we've made it possible to filter by more fields in the scenario execution history. Now, in addition to existing filters, you can filter by the following:

* Execution duration
* Number of operations
* Amount of data transferred
* Action type (run or update)

Previously, execution history could be filtered only by start time or status.

We've also made it possible to sort the scenario execution history. You can sort by the following values:

* Execution start time
* Execution status
* Execution duration
* Number of operations
* Amount of data transferred

For more information on filtering and sorting execution history, see [View a scenario's execution history in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Help links in Fusion now lead to specific articles

To make it easier for you to find the information you need, we've updated the help links in Fusion to lead directly to the article about the area of Fusion you are working in.

You can click on the help icon in any area of Fusion to be taken to the article discussing that area. For example, the help link in the Scenario Settings panel leads to the article describing the Scenario settings panel, while the help link in a Workfront module leads to the article describing how to set up Workfront modules. You can also click highlighted links in explanatory text also lead to the article that is relevant to that explanatory text, such as a list of supported date and time formats.

Previously, Fusion help links opened the documentation for Workfront Fusion, which you could then search for the topic you wanted.

## Scenario execution history only shows Details button when details are available

To create more clarity in the scenario execution table, we've made the Details button visible for only executions that have details available. Now, you can tell at a glance whether an execution's details have been archived. Functionality of the Details button has not changed.

Previously, all executions had a Details button, and occasionally users would click into the details only to find that there were no details available.

For more information, see [View a scenario's execution history in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## SDL Managed Translation connector timeout increased to 120 seconds

To reduce timeouts on the SDL Managed Translation connector, we've increased the timeout duration to 120 seconds.

Previously, the SDL Managed Translation followed the Workfront Fusion timeout guardrail of 40 seconds.
