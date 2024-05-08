---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Add a webhook to a basic scenario
description: Webhooks, also known as instant triggers, are a specific kind of trigger module that can start a scenario whenever a change is made, instead of on a given schedule.
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
---
# Add a webhook to a basic scenario in [!DNL Adobe Workfront Fusion]

Webhooks, also known as instant triggers, are a specific kind of trigger module that can start a scenario whenever a change is made, instead of on a given schedule. 

In this example, you will add a webhook to start a scenario as soon as any requests have been submitted to a specific queue. The scenario then converts those requests to a project.

This example modifies the scenario created in [Create a basic scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Prerequisites

You must create the scenario described in [Create a basic scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) before following this procedure.

## Add and configure the webhook

1. Open the Convert object module.
1. In the Issue ID field, delete the black ID block. The block is black because the module it was mapped from is no longer available.
1. Select the ID block under the first module (Watch Events) to map it to the second module.
1. Click **OK**.

### Add the webhook module

1. Open the scenario in the scenario editor.
1. Right click on the first module and select **Delete module**.

   The module is deleted, leaving a blank placeholder.

1. Click the blank module, and select **Adobe Workfront** from the list of apps.
1. Select **Watch Events**.
1. Click **Add** next to the Webhook field.
1. in the Record Type field, select **Issue**, so the module will trigger for changes in issues.
1. In the State field, select **New state**. This is a required field that is used for the filter, which this example does not cover.
1. In the Record Origin field, select **New Record Only**. This allows the scenario to trigger when an issue is added, not when one is updated or deleted.
1. Click **Save** to save the module configuration.
