---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Add a trigger module to a basic scenario
description: Learn how to add a trigger module to allow the scenario to periodically look for new requests and convert them to projects.
author: Becky
feature: Workfront Fusion
---
# Add a trigger module to a basic scenario

Trigger modules are type of module that are placed at the beginning of a scenario. These modules begin a scenario execution when specific criteria when there has been a change in a given service. The change can be a creation of new records, deletion of a records, update of a records, and so on. 

Polling modules check the service at a set time interval and return information about changes that occured during that time interval. If there have been no changes, the trigger does not execute the scenario.

In this example, you will add a trigger module that runs every 15 minutes and starts a scenario if any requests have been submitted to a specific queue. The scenario then converts those requests to a project.

This example modifies the scenario created in [Create a basic scenario](/help/quicksilver/workfront-fusion/free-tier-staging/create-simple-scenario.md).

## Prerequisites

You must create the scenario described in [Create a basic scenario](/help/quicksilver/workfront-fusion/free-tier-staging/create-simple-scenario.md) before following this procedure.

## Add the trigger module

1. Open the scenario in the scenario editor.
1. Right click on the first (Search) module and select **Delete module**.

   The module is deleted, leaving a blank placeholder.

1. Click the blank module, and select **Adobe Workfront** from the list of apps.
1. Select **Watch Record**.
1. Make sure that the module uses the same connection as the rest of the modules in the scenario.
1. In the Filter field, select **New Records Only**.
1. In the Outputs box, select `ID`, `Name`, and `Project ID`.
1. Click **OK** to save the module settings.
   
   A Choose where to start window appears.

1. Select **From now on**.

## Schedule the trigger module

1. Click the clock on the Watch Records module.

   The Schedule setting window opens.

1. In the Run scenario field, select **At regular intervals**.  

1. Click **OK**.

## Update or add the second module

Because the first module has been replaced, the second module must be mapped to the new first module.

1. Open the Convert object module.
1. In the Issue ID field, delete the black ID block, and map the ID block from the first module.
1. Click **OK**.

## Test and activate

## Resources

For more information on scheduled trigger modules, see [Trigger modules](/help/quicksilver/workfront-fusion/modules/module-types.md#polling-triggers) in the article Module types.