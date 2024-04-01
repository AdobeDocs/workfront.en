---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Add a trigger module to a basic scenario
description: Learn how to add a trigger module to allow the scenario to periodically look for new requests and convert them to projects.
author: Becky
feature: Workfront Fusion
---
# Use a function to update a project in a simple scenario

Updating a Workfront work item is a common use case for Workfront Fusion. In this example, you will use a function to change the name of a project to be in uppercase letters.

Fusion includes many types of functions that allow you to transform and perform conditional logic on your data. For more information on using functions, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

This example modifies the scenario created in [Create a basic scenario](/help/quicksilver/workfront-fusion/free-tier-staging/create-simple-scenario.md).

## Prerequisites

You must create the scenario described in [Create a basic scenario](/help/quicksilver/workfront-fusion/free-tier-staging/create-simple-scenario.md) before following this procedure.

## Use a function to update a project

### Add the Update Record module to your scenario

1. Open the scenario in the scenario editor.
1. Hover over the partial circle to the right of the of the module, then click **[!UICONTROL Add another module]**. 
1. Select [!DNL Adobe Workfront] from the list of applications, then choose the module **[!UICONTROL Update Record]**.
1. in the ID field, select the ID block that is under the Convert object module. This is the ID of the project that was output by that module. 

   ![ID from Convert object](assets/id-convert-object.png)

1. In the Record Type field, select Project, because the object to be updated is a project.
1. In the Select Fields to Map area, select Name. 

    A Name field will open.

### Map the function for the name update

When this scenario converts a request to a project, the project's name is the same as the request. The function here takes that name and capitalizes all of the letters in it. 


