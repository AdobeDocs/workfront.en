---
title: Create Workfront Objects using Workfront Planning record automations
description: You can configure automations in Workfront Planning that, when activated, create objects in Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
---

# Create Workfront Objects using Workfront Planning record automations

You can configure automations in Workfront Planning that, when activated, create objects in Workfront.

You activate the automation in records. The object in Workfront is connected to the Planning record where you activated the automation.

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).


## Configure an automation in Workfront Planning

You must configure an automation in Workfront Planning before you can use it to create Workfront objects.

1. Cclick the **More** menu ![](assets/more-menu.png) amd select **Automations**. 

  You are directed to the list of available automations.

1. Click **Create new automation** in the upper-right corner of the screen.
1. In the **Button Text** field, enter the text that you want to appear on the button. Users will click this button when using the automation to create a Workfront object.
1. (Optional) To add an icon to the button, select an icon from the available options.
1. In the **Create a type of** field, select the object that you want the automation to create. 

   Available objects are:

   * Project
   * Portfolio
   * Program
   * Group

1. In the **Select the field to use in the project name** field, select a record field. The new project in Workfront will have this field's contents as its name.
1. In the **Select the field to link the created project back** field, select a record field. The new project in Workfront will appear in this field when viewing the record in Workfront Planning.
1. Select other options as available for the type of object you are creating.
1. Click **Create**

The automation appears on the list of automations, and is available to use in records.

## Use a Workfront Planning automation to create a Workfront object


