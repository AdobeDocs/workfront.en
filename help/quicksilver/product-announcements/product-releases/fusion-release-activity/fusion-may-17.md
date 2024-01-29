---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Workfront Fusion release activity: Week of May 17, 2021'
description: This page describes all enhancements made in Adobe Workfront Fusion the week of May 17, 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 930c335e-2c88-41af-983f-82be790c1a4b
hidefromtoc: yes
---
# Workfront Fusion release activity:&nbsp;Week of May 17, 2021

This page describes all enhancements made in Adobe Workfront Fusion the week of May 17, 2021.

For a list of all recent changes, see [Adobe Workfront Fusion release activity](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

For a list of recent bug fixes in Workfront Fusion, see the [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) page and check for any updates labeled Workfront Fusion Maintenance Update.

## Copy modules in Workfront Fusion scenarios

To make your Workfront Fusion Scenarios easier to work with, we've made it possible to copy and paste modules. Now, you can copy a module or group of modules and paste them into the same or a different scenario. Copying modules preserves the field values in that module.

For more information, see [Copy modules or scenarios in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

## Select multiple modules in a Workfront Fusion scenario

Now, when editing a scenario, you can select multiple modules at a time. You can then perform bulk actions on the selected modules.

* Copy
* Move
* Delete

Copying and moving modules preserve the module values and any lines connecting the modules.

For more information on editing scenarios, see [Create a scenario in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/create-a-scenario.md).

## Modules now preserve unsaved information

To make it easier to create scenarios, we've made it possible for modules to preserve field values when they are not in focus. Now, when you click away from a module without saving it, and then return to it, the fields show the previously entered values. When the module is closed, it displays an indicator that there are unsaved fields.

## Azure AD connector now handles new and updated records separately

New records and updates to existing records are now handled by separate modules.

* To watch for new records, you can use the Watch Records trigger module. This module no longer watches for updated records.
* To get updated records, you can use the new Search Users/Groups Delta module. This module returns new, updated, and deleted records.

For more information, see [Azure Active Directory modules](../../../workfront-fusion/apps-and-their-modules/azure-ad-modules.md).
