---
title: Edit records
description: You can edit record information in Adobe Workfront Planning. You must create record types before you can start creating and editing records.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
---
<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Edit records

{{planning-important-intro}}

You can edit record information in Adobe Workfront Planning by editing the values of the fields associated with the records. 

You must create record types before you can start creating and editing records. 

For information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

For information about creating records, see [Create records](/help/quicksilver/planning/records/create-records.md). 

<!-- mention in here that the fields in the Details view are the same as the ones in the table view -- this article is linked from the Manage record views one to refer to this info-->

## Access requirements

+++ Expand to view access requirements for Workfront Planning.

You must have the following to be able to access Workfront Planning:  

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning plan*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, see <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront pricing and packaging</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>Standard</p> 
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Considerations about editing records

* You can edit records that you created or records created by others, if you were given permissions to the workspace. 
* You can edit record fields from the following areas:

    * The record's preview in a record view
    * The record's page
    * Inline, in a table view. 

* When a user edits a record in a view, the changes are visible immediately in all views and the record pages to all other users.

* The following types of fields are automatically updated, and you cannot edit their values manually: 
    * Linked fields from other records
    * Formula-type fields
    * System fields (Created by, Created date, Last modified by, Last modified date) 
* If the records you display are linked to other records, the new information of the records that you are editing reflects on the linked records. 
* You cannot edit records in bulk. <!--this will probably change-->
* URLs are recognized as links in single-line text field types only when they start with the following: http://, https://, ftp://, or www. . 
* You can add a cover image to each record. The image is unique for each record, and it does not apply to all records of the same time. 
* You can edit the order of the fields in a record page and add a cover image for a record. For more information, see [Manage the record page layout](/help/quicksilver/planning/records/manage-the-record-page.md).

## Edit records

You can edit a record from the following areas:

* [From the table view of a record type](#edit-a-record-inline-in-the-table-view-of-a-record-type)
* [From the record's preview in a view](#edit-a-record-from-the-records-preview-in-a-view)
* [From the record's page](#edit-a-record-from-the-records-page)
* [From a Workfront object in the Planning section](#edit-a-record-from-a-workfront-object-in-the-planning-section)

### Edit a record inline in the table view of a record type

When you edit records from the table view, there is an indication which field is being edited by other users at the time you are viewing the record. 

For more information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 

{{step1-to-planning}}

1. Click the workspace whose records you want to edit

    The workspace opens and the record types display as cards.
1. Click a record type card. 

    The record type page opens. 
1. (Conditional) Click the tab of a table view or click **+ View** to create a table view. The table view should be the default view, unless you viewed the record type in another type of view when you accessed it last.

    The records associated with the selected record type display in the table view. 
1. Click inside the row of a record to start editing information about the record inline.

    ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

    >[!TIP]
    >
    >  You cannot edit information for the following fields, as they are read-only and Workfront updates them automatically: 
    >  
    >  * Linked fields that are created by connecting record types. For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
    >  * Fields of the following types: Created by, Created date, Last modified by, Last Modified date, Formula fields.

1. (Optional and conditional) When you edit a Paragraph-type field, use the following **Rich Text** formatting options: 

    * Bold
    * Italic
    * Underline 
    * Add a link
    * Add a bulleted list
    * Add a numbered list

    ![](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Optional) Double-click a connected record field to add connected records or objects to another record. For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 
1. Press **Enter** on your keyboard or click outside of a row to save your changes. The changes are saved automatically. A **Saved** indicator displays briefly in the upper-right corner of the table view to show that the changes were saved. 


1. (Optional) To copy and paste information from one field to another, do one of the following:

    * Copy one or multiple existing values of one field, then paste them into a field of the same type on another record
    * Click the column header of a column to select it and copy it, then click the column header of another column and paste the contents of the copied column. The columns must contain similar field types. 
    * With your Shift key pressed, click to select several rows in a table, copy the information in the selected rows, then click a different row and paste the selected information in the new row and the following rows after that. 
    * Copy the information from one cell, then select multiple cells and paste the same information in multiple cells. You can select multiple cells and paste the same information in multiple cells from adjacent rows and columns. 
    * Select the lower-right corner of an existing cell that contains the information you want to copy, then drag and drop it across the adjacent cells where you want to paste the same information. All cells must contain the same type of information. 

        ![](assets/dragable-lower-right-corner-for-copy-paste-in-table-view.png)

    >[!NOTE]
    >
    >Consider the following:   
    >
    >* Use the following keyboard shortcuts for copying and pasting information:
    >   * Copy: CTRL + C (⌘ + C for Mac)
    >   * Paste: CTRL + V (⌘ + V for Mac) 
    >
    >* You cannot copy and paste field values in the record page. This functionality is supported only in the table view of a record type.  
    >* You cannot copy and paste field values for the following field types:   
    >
    >
    >    * Linked fields (or lookup fields) that are created by connecting record types. You can copy and paste linked record fields. For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 
    >    * Fields of the following types: Created by, Created date, Last modified by, Last Modified date 
    
1. (Optional) Use the following keyboard shortcuts to undo or redo editing or copying and pasting record information: 

    * CTRL + Z (⌘ + Z for Mac) to undo a change 
    * CTRL + Shift + Z (⌘ + Shift + Z for Mac) to redo a change 

    >[!TIP]
    >
    >    You can use the keyboard shortcuts multiple times in a row to undo multiple changes.

1. (Optional) Add a thumbnail to a record. For information, see [Add a thumbnail to a record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

### Edit a record from the record's preview in a view

{{step1-to-planning}}

1. Click the workspace whose records you want to edit

    The workspace opens and the record types display as cards. 

1. Click a record type card. 

    The record type page opens. 

1. From a view of any type, click the record 

    Or 
    
    From the table view, click the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) in the first column. The record's preview opens in the view.

    ![](assets/details-box.png) 

1. (Optional) Click the **More** menu to the right of the record's title, then click **Rename**. This updates the field that displays as the record's title.

    The record's title is the primary field of the record when viewed in a table view. For information, see [Primary field overview](/help/quicksilver/planning/fields/primary-field-overview.md). 

1. Start editing the field information in the record's preview.  

    >[!TIP]
    >
    >  You cannot edit information for the following fields, as they are read-only and Workfront updates them automatically: 
    >  
    >  * Lookup fields from other records that are created by connecting record types. For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
    >  * Fields of the following types: Created by, Created date, Last modified by, Last Modified date, Formula fields.

1. (Optional) Click **Add cover** to add a cover image to the record. For more information, see [Add a cover image to a record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md). 

1. (Optional) Hover over the thumbnail icon, then click **More** ![](assets/more-menu.png) > **Edit thumbnail** to add a thumbnail image. For information, see [Add a thumbnail to a record](/help/quicksilver/planning/records/add-thumbnails-to-records.md). 

    Workfront automatically saves your changes.

1. (Optional) Click the **Export** icon ![](assets/export-icon-in-record-details-page.png) to export the record's details. For information, see [Export a record's details](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in the upper-right corner of the record's preview to open the record's page in a new tab. Continue editing the record as described in [Edit a record from the record's page](#edit-a-record-from-the-records-page) section in this article. 

### Edit a record from the record's page

{{step1-to-planning}}

1. Click the workspace whose records you want to edit

    The workspace opens and the record types display as cards. 

1. Click a record type card. 

    The record type page opens. 

1. Do one of the following:

    * From any view, access the record's preview, as described in the [Edit a record from the record's preview in a view](#edit-a-record-from-the-records-preview-in-a-view) section in this article, then click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in the upper-right corner of the record preview to open the record's page in a new tab. 

    * From the **Table** view, hover over the name of a record, then click the **More** menu ![](assets/more-menu.png), then click **View**

        ![](assets/contextual-menu-for-record-row.png)
    
        The record page opens.

        ![](assets/details-page.png)

1. (Optional) Click the **More** menu to the right of the record's title, then click **Rename**. This updates the field that displays as the record's title.

    The record's title is the primary field of the record when viewed in a table view. For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
    
1. Click any editable field on the record page to edit it. 

    >[!TIP]
    >
    >  You cannot edit information for the following fields, as they are read-only and Workfront updates them automatically: 
    >  
    >  * Linked fields that are created by connecting record types. For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
    >  * Fields of the following types: Created by, Created date, Last modified by, Last Modified date, Formula fields.

1. (Optional) Click **Add cover** to add a cover image to the record
    
    Or
    
    Hover over the existing cover image, then click the **More** menu ![](assets/more-menu.png) > **Upload** to add a new cover image for the record. 
    
    For more information, see [Add a cover image to a record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md). 

1. (Optional) Hover over an existing thumbnail, or the **thumbnail icon** ![](assets/record-thumbnail-icon-on-details-page.png), then click the **More** menu ![](assets/more-menu.png) > **Edit thumbnail** to add a thumbnail for the record. 

    For more information, see [Add a thumbnail to a record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

    Workfront automatically saves your changes.

1. (Optional) Click the **Export** icon ![](assets/export-icon-in-record-details-page.png) to export the record's details. For information, see [Export a record's details](/help/quicksilver/planning/records/export-the-record-page.md).
    

## Edit a record from a Workfront object in the Planning section

After you connect records with Workfront objects, you can edit Workfront Planning records in Workfront from the object's Planning section. 

For more information, see [Manage records in the Planning section of Adobe Workfront objects](/help/quicksilver/planning/records/manage-records-in-planning-section.md). 