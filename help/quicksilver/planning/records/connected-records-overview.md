---
title: Connected Records Overview
description: After you create connections between record types, you can connect individual records to one another. This article describes considerations that you must take into account when connecting records in Adobe Workfront Planning. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---

# Connected records overview

{{planning-important-intro}}

You can connect Adobe Workfront Planning records to one another or to objects from other applications. 

This article describes considerations that you must take into account when connecting records in Adobe Workfront Planning. 

For information about how you can connect records to one another or to another object, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 


## Considerations about connecting records

* After you connect record types, the connected record types display as linked record fields in the table of the record types they are linked from and on the records' pages. 
* You can browse and add records and objects of the linked record and object types from the linked record fields. 
* You can add fields (lookup fields) of the linked record types in the table of the record type you are linking from. 

    You can add fields (lookup fields) of the record types you are linking from in the table of the record type you are linking to. 

    For example, if you link the record type of Product from the record type of Campaign, you can display Product fields for campaigns, as well as Campaign fields for Products. 
* You cannot manually update the values of lookup fields on the records you are linking from. 

  The values of the lookup fields populate the Workfront Planning record that you are linking from automatically after they are updated on the original record or object. 

* Everyone with access to Workfront Planning and View or higher permissions to the workspace can see the connections that you make between records or between records and other applications' objects. They can view connected records and objects regardless of their permissions in the  applications you are connecting to. 
* You can view and edit everyone else's connections, if you have Manage permissions to the workspace where the connected records are. 
* You can connect one record to one or multiple objects from another application. For more information, see the "Connections types" section in the article [Connected record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Areas where you can connect records 

You can connect records to other records or to objects from another application in the following areas: 

* You can connect records from Workfront Planning to Workfront objects or Experience Manager Assets objects in the following areas of a Planning record:

  * The connected record fields in the table view of a record type in Planning.
  * The record's preview or page in the connected record fields on the Details tab.
  * The record's preview or page on the Connections tab.

* You can connect Workfront objects to Workfront Planning records in the following areas: 
    
    * From the Planning section of a Workfront object. 

