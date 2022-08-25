---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Uninstall the legacy connector
description: text
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
---

# Unistall the Workfront with Adobe Experience Manager legacy connector

You must uninstall the Workfront with Adobe Experience Manager legacy connector to use the new native integration. 

## Unsubscribe from Workfront 

 In uninstalling the connector, the initial step is to unsubscribe from Workfront. This can be done in AEM by following these steps: 

* Go to Tools > Cloud Services > Workfront Integration Configuration. 

* Select your configuration (global-workfront by default) and click Properties. 

[screenshot]

Click the buttons which will disable Document, Comment and Metadata Sync. Take Make sure that the label says ‘Disabled’ and not ‘Enable’. 
Doing this will remove the subscriptions in Workfront and allow the user to create a new subscription using the same url defined in Day CQ Link Externalizer. 

## Delete the Workfront Integration Configuration 

[screenshot]

After removing the subscription, it is now safe to delete the Workfront Integration Configuration. Click the set configuration, and press delete.

## Remove mapping

To delete Workfront Property Mapping: 

* Go to Tools > Assets > Workfront Property Mapping 

* Select all mappings and click Delete 

## User permissions 

All users that access AEM Dam from Workfront were given read permissions to  

/content/dam. If a user doesn’t need that anymore, you may remove the permissions given to said users. 
 
The connector operates using the system user workfront-service. This will get uninstalled when uninstalling the connector.  

If you are using connecter version 2.0.3 and added the group workfront-aem-connector-group, this needs to be removed as well by going to tools > security > groups. 

## Day CQ Link Externalizer 

If this is not needed anymore, you may revert this back to localhost:4502 by going to ____ and look for ‘Day CQ Link Externalizer’. 
[screenshot]

If you are using AEM as a Cloud Service, you can change this by looking into your project and locate the file com.day.cq.commons.impl.ExternalizerImpl.xml inside 

ui.apps/src/main/content/jcr_root/apps/mysite/config. 

## Uninstall Connector Package 

[screenshot]

If you are using AEM onPrem, go to crx/packmgr/index.jsp. Look for the workfront-aem-connector.all-<version>.zip, click ‘More’ and then ‘Uninstall’. 

Please check under /conf to make sure all Workfront created files have been removed. 

For AEM as a Cloud Service, you can remove the dependencies for the connector from the project’s pom.files. 

## Firewall and Dispatcher 

Don’t forget to remove your whitelisted Workfront URLs in case communication is not needed anymore.  

Also, the connector uses the headers apiKey and username which was set to the dispatcher. These can be removed as well. 