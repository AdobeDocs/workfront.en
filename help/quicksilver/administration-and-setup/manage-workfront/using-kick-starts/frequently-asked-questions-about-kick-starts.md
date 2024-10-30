---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Frequently Asked Questions About Kick-Starts
description: Find answers to frequently asked questions about importing and exporting Workfront data using Kick-Starts.
author: LIsa
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
---
# Frequently asked questions about Kick-Starts

The following are frequently asked questions about Kick-Starts:

## Why am I receiving this error when trying to import a Kick-Start file: "Your file was correct, but nothing was imported?"

### Answer

One of the following three things might be missing from the Kick-Start file:

1. The **isNew** column must be set to **TRUE** for all the items you want to import. **isNew** must be **TRUE** because you can only import new data with a Kick-Start. You cannot Modify existing data via Kick-Start. You can have other rows in the spreadsheet with **isNew = FALSE** but, these rows will not import.

1. ​The file needs to have one empty row before the headers of your data start.
1. ​The Excel sheet(s) need(s) to have the correct name(s).

When working with Kick-Starts, we recommend to first download the Kick-start Template, manually populate it with the correct data and then import it back into Adobe Workfront.

For more information about correctly importing data in Workfront using Kick-Starts, see [Import data into Adobe Workfront using a Kick-Start template](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Why am I receiving this error when trying to import hours into Workfront using a Kick-Start file: "User with primary key value(s) "null" not found?"

### Answer

The error refers to the GUID of the user that is associated with the hours. 

To address this:

1. Export a blank Kick-Start template for the **Hours** object only.  
   For more information about exporting a blank Kick-Start File, see "Exporting the Kick-Start Template" in  [Import data into Adobe Workfront using a Kick-Start template](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Manually copy the data from the original Kick-Start and paste it into the empty file.  
   Do this for each column.
1. Try importing the new file again.  
   The Kick-Start should import successfully.

## Why is the country field not populating on the user profile in a Kick-Start import?

### Problem

When importing a User Kick-Start with the field **setCountry**, that data doesn't come over to the country on the user profile.

### Answer

If the user is enabled for Unified User Management (UUM) or Adobe Identity Management System (IMS), the **Country** field only accepts country code values (for example, US, GB, IN). Verify that the **setCountry** field in your Kick-Start template is using country code values before you import.

For more information about correctly importing data in Workfront using Kick-Starts, see [Import data into Adobe Workfront using a Kick-Start template](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
