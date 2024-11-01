---
content-type: release-notes
title: Adobe Workfront Planning Release Activity for the 25.1 Release
description: This is the release activity for the Adobe Workfront Planning product for the 2025 First Quarter.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
---
# First Quarter 2025 release activity for Adobe Workfront Planning

<!--remove this important intro after the 25.1 release-->

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning, a new offering from Adobe Workfront. 
>
>You must purchase a Workfront Planning plan, in addition to a Workfront plan to be able to access and use Workfront Planning capabilities. 
>
>For a complete list of requirements to access Workfront Planning, see [Access overview](/help/quicksilver/planning/access/access-overview.md). 
>For an overview of Workfront Planning, see [Adobe Workfront Planning overview](/help/quicksilver/planning/general/planning-overview.md). 
>

This article describes the features that are releasing for Workfront Planning during the 2025 First Quarter release. 

<!--keep the sentence below for all future quarterly release pages-->
<!--remove the general activity mention after First Quarter 2025 is released-->

For a list of all features released for Adobe Workfront Planning after the general availability release on August 28, 2024, see [Adobe Workfront Planning release activity: article index](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md). 

## Connection fields are now supported in request forms 

>[!NOTE]
>
>Preview release: October 31, 2024; Production for fast release: With the 24.11 release (November 14, 2024); Production for quarterly release: With the 25.1 release (January 2025)

You can now add connected fields for Workfront Planning records to a record type request form. 

You cannot add connection look up fields, or connected fields for Workfront objects in the request form. 

Prior to this enhancement, these types of fields could not be added to request forms in Workfront Planning.  

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Connection warning when connecting records that are already linked to other records 

>[!NOTE]
>
>Preview release: October 31, 2024; Production for fast release: With the 24.11 release (November 14, 2024); Production for quarterly release: With the 25.1 release (January 2025)

When you try to connect records which are already connected elsewhere and which belong to a record type connected through a One to many or One to one connection type, you now receive a warning that the records are already connected. If you confirm that you want to move forward with your connection, the selected records are removed from the original record and added to the record you're currently editing.

For information about connection types, see [Connected record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## New information icon with the description of fields in the record's details page 

>[!NOTE]
>
>Preview release: October 30, 2024; Production for fast release: With the 24.11 release (November 14, 2024); Production for quarterly release: With the 25.1 release (January 2025)

We added an information icon to the right of the field names in a record page. Clicking the information icon displays the description of the field, when a description exists. Prior to this enhancement, the description of the field displayed when you hovered over the field name.

For information, see [Edit records](/help/quicksilver/planning/records/edit-records.md).

## New Workfront field type for Planning connections 

>[!NOTE]
>
>Preview release: October 24, 2024; Production for fast release: With the 24.11 release (November 14, 2024); Production for quarterly release: With the 25.1 release (January 2025)

To continue bridging Workfront objects to Workfront Planning records, we added a new field type in Workfront custom forms called Planning connection. By adding this field type on a Workfront custom form, and ultimately on a Workfront object, you can now do the following: 

* Display records connected to a Workfront object in the custom form.  

* Connect and disconnect Workfront Planning records form a Workfront object. 

You can add the new field to forms for all object types. However, you can edit the information in the field only from forms attached to the following Workfront objects that can be connected from Workfront Planning record types: Portfolio, Program, Project, Company, Group.  

Editing the Planning connection fields for Workfront objects in bulk is not yet available.  

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[View a video demonstration of this feature](https://video.tv.adobe.com/v/3435633/){target=_blank}