---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrate from the legacy or enhanced connector to Workfront for Adobe Experience Manager as a Cloud Service integration
description: The information on this page explains the best practices for moving from the Workfront for Experience Cloud enhanced or legacy connectors to the latest native integration connecting Workfront and Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
---
# Migrate from the legacy or enhanced connector to Workfront for Adobe Experience Manager as a Cloud Service integration

The information on this page explains the best practices for moving from the Workfront for Experience Cloud enhanced or legacy connectors to the latest native integration connecting Workfront and Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>This information does not apply to customers using Adobe Experience Manager Assets On-Premise or Managed Services environments.

## Move your Workfront instance to the Admin Console

>[!IMPORTANT]
>
>Because all Workfront organizations have been migrated to the Adobe Admin Console, this section will be removed in the near future.

<!--DELETE THIS SECTION MARCH 2026-->

<!--
Customers that intend to use the new native integration between Workfront and Adobe Experience Manager Assets as a Cloud Service must ensure their Workfront environment is tied to an Adobe Admin Console. For existing Workfront environments, this will likely require a migration of the environment to a connected Adobe Admin Console. For more details regarding this migration and the associated checklist, see [Prepare to onboard your organization to the Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md). 

 Adobe must help carry out this migration. To request help, do one of the following:

* If you have Workfront Hub access, submit your request to the [Workfront Migration to Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* If you do not have Workfront Hub access, you can submit your request to the [Workfront to Adobe Admin Console Early Migration Request Queue](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

-->

## Configure your new Workfront for Adobe Experience Manager assets as a Cloud Service integration

After your Workfront environment has been migrated to an Adobe Admin Console, Workfront administrators can configure the new native integration. For configuration help, see [Configure the Experience Manager Assets as a Cloud Service integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Move existing assets to your Workfront for Adobe Experience Manager assets as a Cloud Service integration

After you configure your environment, you can move existing linked assets and folders to Adobe Experience Manager. This is an optional step but will ensure that previously linked folders and assets through the legacy or enhanced connector will still be accessible once those connectors are uninstalled.

For more information on moving your assets, see [Migrate linked folders and documents](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validate all critical use cases intended to be used

It will be important to validate all critical use cases intended to be used through the native integration prior to uninstalling the legacy or enhanced connector.

## Uninstall the legacy or enhanced connector

Last, you need to uninstall the legacy or enhanced connector. The native integration is not intended to run in parallel with either connector. 

To uninstall, see 

* Legacy connector uninstall instructions: [Uninstall the Workfront with Adobe Experience Manager legacy connector](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Enhanced connector uninstall instructions: [Uninstall the Workfront with Adobe Experience Manager enhanced connector](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
