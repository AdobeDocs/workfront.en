---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restoring individual child objects
description: This document describes how you can get help recovering individual child objects that have been deleted from your Adobe Workfront Production or Preview environments fewer than 30 days previously.
feature: System Setup and Administration
role: Admin
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
---
# Restoring individual child objects

This document describes how you can get help recovering individual child objects that have been deleted from your Adobe Workfront Production or Preview environments fewer than 30 days previously.

A Workfront administrator can restore projects, tasks, issues, and documents in each Workfront instance, as described in [Restore deleted items](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). But only the Workfront Database Team can restore a objects such as tasks, issues, documents, custom forms, hours, and notes independently of their parent object.

Data from your live environment is available in the Preview Sandbox for up to 7 days. This means you can export the standalone data from the Preview Sandbox environment using the following methods:

* Kick-Starts 
* Building a report and exporting the results

For more information about exporting data from Workfront, see [Export data](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

You can import the exported data in the following ways:

* Manually, if you are using exported reports 
* In bulk, if you are using Kick-Starts  
  
  For more information about importing data into Workfront using Kick-Starts, see [Import data into Adobe Workfront using a Kick-Start template](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

The Preview Sandbox environment is refreshed during our maintenance windows over the weekend.

For more information about the windows of maintenance for the Preview Sandbox environment, see [the Adobe status site](https://status.adobe.com).

>[!IMPORTANT]
>
>Documents are an exception to these methods of restoration. You can manually download them from the Preview Environment, and re-upload them into the Production environment. If you want to download and upload documents in bulk, you will need to request a data restore from Workfront. 

## Information needed for a data restore

Once you have determined a deleted object needs restoring by our Database Team, gather as much information as you have about it. The following information is required for our database administrators to find the object and initiate a restore:

* Object name 
* Object Type (Task, Issue, Project, etc) 
* Estimated Date and Time of deletion 
* Object GUID (if possible)  
  
  Refer to the following information when locating the GUID of an object:

   * The GUID can be found by referencing e-mail notifications triggered by interacting with the object (assignments to, comments on, etc.) 
   * Example of a GUID found at the end of a URL: `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

Once you have gathered this information or if you require assistance, please call our Customer Support Team at 844-306-HELP(4357) or submit a ticket online.

## Data restore process

1. After our Customer Support Team receives your information, they will escalate it to our Customer Support Team. 
1. Our Customer Support Team will contact our Database Team.
1. Once the Database Team has had a chance to review the data being restored, a more accurate estimate for the ETA can be provided. A restore will generally take three days but can take longer depending on the type and volume of data being restored. 
1. The Database Team will restore the information to your Preview Sandbox environment where you will have the chance to review the restored data. Our Customer Support Team will let you know when the data can be found in the Preview Sandbox. 
1. Once you are satisfied with the restore in the sandbox, let our Customer Support Team know  and they will contact our Database Team to notify them that they can restore the data to your production environment. 
1. You will have a chance to review the restored data before the request is closed.
