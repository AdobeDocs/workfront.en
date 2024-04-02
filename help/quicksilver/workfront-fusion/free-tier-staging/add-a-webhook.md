---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Add a webhook to a basic scenario
description: Learn how to add a trigger module to allow the scenario to periodically look for new requests and convert them to projects.
author: Becky
feature: Workfront Fusion
---
# Add a webhook to a basic scenario

Webhooks, also known as instant triggers, are a specific kind of trigger module that can start a scenario whenever a change is made, instead of on a given schedule. 

In this example, you will add a webhook to start a scenario as soon as any requests have been submitted to a specific queue. The scenario then converts those requests to a project.

This example modifies the scenario created in [Create a basic scenario](/help/quicksilver/workfront-fusion/free-tier-staging/create-simple-scenario.md).

## Prerequisites

You must create the scenario described in [Create a basic scenario](/help/quicksilver/workfront-fusion/free-tier-staging/create-simple-scenario.md) before following this procedure.

## Add and configure the webhook

### Add the webhook module

1. Open the scenario in the scenario editor.
1. Right click on the first module and select **Delete module**.

   The module is deleted, leaving a blank placeholder.

1. Click the blank module, and select **Adobe Workfront** from the list of apps.
1. Select **Watch Events**.
1. Click **Add** next to the Webhook field.


