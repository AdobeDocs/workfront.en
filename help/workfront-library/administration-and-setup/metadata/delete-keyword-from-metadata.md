---
filename: delete-keyword-from-metadata
product: workfront-library
product-area: documents
navigation-topic: metadata
title: Delete a keyword from the picklist in Workfront Library
description: As a Workfront Library administrator you can remove keywords from the keyword picklist. For information about keywords, see Overview of keyword metadata in Workfront Library
---

# Delete a keyword from the picklist in Workfront Library

As a Workfront Library administrator you can remove keywords from the keyword picklist. For information about keywords, see [Overview of keyword metadata in Workfront Library](../../../workfront-library/administration-and-setup/metadata/keyword-metadata-overview.md)

When you delete a keyword from the picklist, the keyword is also removed from all assets tagged with the keyword. A search using a deleted keyword returns no results.

>[!IMPORTANT]
>
>When you delete a keyword from the picklist, all child keywords related to the deleted keyword are deleted from the picklist and from all tagged assets.

1. In Workfront, click the Main Menu icon , then select Library to open Workfront Library in a new browser tab. 
1. In the upper-left corner of Workfront Library, click the `Menu` icon ![](assets/library-menu-icon.png).
1. In the left panel, click `Setup`> `Keywords`.
1. Hover over the keyword you want to delete, and click the `trash can` icon.

   The Delete Keyword dialog box displays and specifies the number of assets tagged with the keyword you want to delete.

1. (Optional) To view all the assets tagged with the keyword, click `See all affected assets.`

   The tagged assets display in a new browser tab. Close the tab to return to the Delete keywords box.

   >[!NOTE]
   >
   >Hidden or expired content that is tagged with the keyword display only if you have the Show Hidden and Show Expired filters enabled. For more information, see the following:
   >
   >  
   >  
   >  * [Filter for expired content in Workfront Library](../../../workfront-library/content-management/filters/filter-for-expired-content.md) 
   >  * [Filter for hidden content in Workfront Library](../../../workfront-library/content-management/filters/filter-hidden-content.md) 
   >  
   >

1. Click `Delete`.

   The keyword and any child keywords are deleted from the picklist and from all tagged assets.

