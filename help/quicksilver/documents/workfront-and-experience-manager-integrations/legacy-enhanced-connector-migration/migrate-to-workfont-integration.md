---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrate
description: add text
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
---

# Migrate from the legacy or enhanced connector to Workfront for Adobe Experience Mangaer as a Cloud Service integration

The information on this page explains the best practices for moving from the Workfront for Experience cloud enhanced or legacy connectors to the latest native integration connecting Workfront and Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>This information does not apply to customers using Adobe Experience Manager Assets On-Premise or Managed Services environments.


## Move your Workfront instance to the Admin Console

Customers that intend to use the new native integration between Workfront and Adobe Experience Manager Assets as a Cloud Service must ensure their Workfront environment is tied to an Adobe Admin Console. For existing Workfront environments, this will likely require a migration of the environment to a connected Adobe Admin Console. For more details regarding this migration and the associated checklist, please reference see [Prepare to onboard your organization to the Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md). 

 Adobe must help carry out this migration. To request help,

 * If you have Workfront Hub access, submit the request to the [Workfront Migration to Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
 * If you do not have Workfront Hub access, email mreed@adobe.com to reqeust help with your migration.

## Configure your new Workfront for Adobe Experience Manager intagration

Once the migration of the Workfront environment to an Adobe Admin Console has occurred admin users can configure the new native integration.

Native integration setup help can be found here: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/configure-integrations/configure-aacs-integration.html?lang=en

## Migrate existing assets to your Workfront for Adobe Experience Manager intagration

After you configure your environment 
Upon configuration of the native integration between Workfront and AEM Assets as a Cloud Service it may be required to migrate existing AEM linked assets and folders inside of Workfront. This is an optional step but will ensure that previously linked folders and assets through the legacy or enhanced connector will still be accessible once those connectors are uninstalled.

For guidance around how this process can be handled please reference the following documentation: XXXXXXXXXXXXXX

## Validate all critical use cases intended to be used

It will be important to validate all critical use cases intended to be used through the native integration prior to uninstalling the legacy or enhanced connector.

## Uninstall the legacy or enchaned connector

The final step requires uninstalling the legacy or enhanced connectors as the native integration will not be able operate over the long term in parallel with these connectors.

Legacy connector uninstall instructions: Uninstalling Workfront.docx - new doc
Enhanced connector uninstall instructions: AdobeDAM:Workfront for Experience Manager enhanced connector - new doc