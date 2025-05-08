---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrate from the legacy connector to the enhanced connector
description: The following process outlines the best practices for moving off the Adobe Experience Manager legacy connector to the enhanced connector for integrating Adobe Workfront with AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
---
# Migrate from the legacy connector to the enhanced connector

The following process outlines the best practices for moving off the Adobe Experience Manager legacy connector to the enhanced connector for integrating Adobe Workfront with AEM Assets. 

>[!IMPORTANT]
>
>This documentation applies only to customers using Adobe Experience Manager Assets On-Premise or Managed Services environments.


For customers on Adobe Experience Manager Assets as a Cloud Service, the migration path from the legacy connector will be to the new native integration inside of Workfront. To learn more about this migration process, see [Migrate from the legacy or enhanced connector to Workfront for Adobe Experience Manager as a Cloud Service integration](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Implement the enhanced connector

>[!IMPORTANT]
>
>A certified partner or Adobe Consulting Services are required for implementation of the enhanced connector. 
>
> For partners wishing to certify on the enhanced connector please review the following article: [Workfront for Experience Manager enhanced connector Expert Series](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview).

To implement the enhanced connector, see [Configure Workfront for Experience Manager enhanced connector](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/integrations/workfront-connector-configure).


## Move existing assets

After you configure your environment, you can move existing linked assets and folders to Adobe Experience Manager. This is an optional step but will ensure that previously linked folders and assets through the legacy connector will still be accessible once the legacy connector is uninstalled.

For more information on moving your assets, see [Migrate linked folders and documents](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validate all critical use cases intended to be used

It is important to validate all critical use cases intended to be used through the enhanced connector prior to uninstalling the legacy connector.

## Uninstall the legacy connector

Last, you need to uninstall the legacy connector. The legacy connector is not intended to run in parallel with the enhanced connector. 

To uninstall, see [Uninstall the Workfront with Adobe Experience Manager legacy connector](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
