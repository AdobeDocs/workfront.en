---
title: Manage the Record Page Layout
description: You can edit the layout of the record preview and page in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
---

# Manage the record page layout

<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

You can edit the layout of the record preview and page in Adobe Workfront Planning. 

The record preview is a smaller view of the record page that displays in the view of a record type. 

When you change the layout of a record  preview and page, the changes affect the preview boxes and details pages of all records of the same type. 

This article describes how you can change the layout and appearance of a record preview box or a record page. For information about editing records, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

You must create record types and records before you can start editing record pages. 

For information, see the following articles: 

* [Create record types](/help/quicksilver/planning/architecture/create-record-types.md)

* [Create records](/help/quicksilver/planning/records/create-records.md)

## Access requirements

+++ Expand to view access requirements. 

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
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td>
   <td>
<p>Any</p>
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Standard</p>
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
   <td>
   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> 
  </td>
  </tr>
 </tbody>
</table>

*For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  

+++


## Considerations about editing record pages

* By default, the details and the preview pages of a record display all the fields associated with the record. 

* You cannot add new fields for a record in the preview or details page. You must add new fields in the table view to display them in the preview and details pages. 

* You can add sections to a record preview or details page, to organize the information by common criteria and make it easier to find. 

* The following changes affect all the records of the same type and are visible to all users accessing those records: 

   * Rearranging fields
   * Adding or removing sections

* Display changes that you make in the record preview are immediately visible in the record details page. Changes made in the record page are also visible in the record preview box. 

* Adding a cover image or a thumbnail to a record is not part of the overall layout of the record preview or page. You can add unique cover images or thumbnails to each record. For information, see [Add a cover image to a record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) and [Add a thumbnail to a record](/help/quicksilver/planning/records/add-thumbnails-to-records.md). 

## Add sections to a record preview or page

Consider the following when adding sections to a record page:

* There is no limit to how many sections you can have on a page. 
* You cannot have an empty section. You must have at least one field in a section. 
* You can drag and drop fields from one section to another. For more information, see the section [Rearrange fields in the record preview or details page](#rearrange-fields-in-the-record-preview-or-details-page) in this article. 
* When you remove all the fields from a section, the section is automatically deleted and cannot be recovered. 

To add a section to a record preview or page: 

{{step1-to-planning}}

1. Click the card of a workspace. 

    The workspace opens and the record types display as cards. 

1. Click a record type card. 

    The record type page opens. 

1. From a view of any type, click the name of a record 

    Or 
    
    From the table table view, click the **Open details** icon ![Open details icon in table name field](assets/open-details-icon-in-table-name-field.png) in the first column. 
    
    The record's preview opens in the view.

    ![Details box](assets/details-box.png)  

1. (Optional) Click the **Open in new tab** icon ![Open details in a new tab icon](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the record preview  to open the record's page in a new tab. 

    The record page opens. The Details tab opens by default.

    ![Details page](assets/details-page.png)

1. In the **Details** tab of the record preview or page, hover over the white space to the left of the fields, then click the **Add section** icon ![Add section icon](assets/add-section-icon.png) to add a section. 
1. Click inside the section's name and replace **Untitled section** with a name, then click Enter. The fields displayed under the section are automatically part of the new section. 
1. Start dragging and dropping fields to the new section, as described in the section [Rearrange fields in the record preview or details page](#rearrange-fields-in-the-record-preview-or-details-page) in this article. 

1. (Optional) Hover over the name of a section and click the **More** menu ![More menu](assets/more-menu.png). 

   ![More menu options for section on record page](assets/more-menu-options-for-section-on-record-page.png)
1. (Optional) Do one of the following to edit the section: 

   * Click **Rename** to rename the section

      >[!TIP]
      >
      > You can rename a section inline, by clicking the name.
   
   * Click **Move up** to move the section up one position 

      Or 
      
      Click **Move down** to move the section down one position.
      All fields in the section move with the section. 

   * Click **Delete** to delete the section. The section is deleted and it cannot be recovered. All users accessing the records of this type will no longer view the deleted section. 

1. Click the downward-pointing arrow to the left of a section name to collapse it, or the right-pointing arrow  to expand it. 
   All sections are expanded by default. 

1. (Optional) Click the **grab** icon ![Grab icon](assets/grab-icon.png) to the left of a section name, then drag and drop it in a desired spot. 

    The new position of the section updates in both the preview and the page of all records of the same type for all users viewing the records. 

    All changes to sections and field order are saved automatically. 

1. (Optional) Click the **Export** menu ![Export icon in record details page](assets/export-icon-in-record-details-page.png) to export the Details tab to a Word or a PDF file. For more information, see [Export a record's details](/help/quicksilver/planning/records/export-the-record-page.md). 

1. (Optional) Click the **Connections** tab next to the **Details** tab. You might have to click **More** before clicking the **Connections** tab.

   All records or objects that are connected to the selected record display under the names of the record type, or the application they belong to. 

      ![Connections tab on record in Workfront Planning](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Optional) Select the **Show all records** setting in the upper-right corner of the Connections tab. All connected record types display, including the ones that don't have any connected records yet. BY default, the toggle is deselected and record types with no connected records are hidden. 

1. (Optional) Click **Connect** to add more records to the connected record types. For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).  

1. (Optional) Hover over a record card, then click the disconnect record icon **-**, then click **Disconnect**. <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
   The following things occur: 
   * The record is no longer connected to the Workfront object. 
   * The Workfront object is also removed from the record's connected field from Workfront Planning. 
   * The values for the Workfront lookup fields connected to the Planning record are also deleted.

## Rearrange fields in the record's Details tab

{{step1-to-planning}}

1. Click the card of a workspace. 

    The workspace opens and the record types display as cards. 
 
1. Click a record type card. 

    The record type page opens. 

1. From a view of any type, click the name of a record 

    Or 
    
    From the table table view, click the **Open details** icon ![Open details icon in table name field](assets/open-details-icon-in-table-name-field.png) in the first column. 
    
    The record's preview opens in the view.

    ![Details box](assets/details-box.png) 

1. (Optional) Click the **Open in new tab** icon ![Open details box in a new tab icon](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in the upper-right corner of the record preview to open the record's page in a new tab. 

    The **Details** tab of the record opens by default. 

   ![Details page](assets/details-page.png)

1. In the record **Details** tab, click the **grab** icon ![Grab icon](assets/grab-icon.png) to the left of a field name, then drag and drop it in a desired spot. 

   >[!TIP]
   >
   >You can drag and drop fields to another section. 
   >You must have at least one field in a section.
   >

   The new position of the field is updated in both the preview and the page of all records of the same type for all users viewing the records. 

   All changes to the layout of the record preview or page save automatically. 

## Add a Connected records page to a record

You can view information from connected records or objects by adding a tab for a Connected records page to a record.  

The information from the connected records can be edited in the table view. The information from the objects connected from another application is not editable in the table view.

Consider the following when adding a Connected records page to a record: 

* You can add a Connected records page to a record after you connected record or object types to the record type from the table view of a record type.

* In the Production environment, you cannot add a Connected records page from a record's preview.

   <span class="preview">You can add a Connected records page from a record's preview in the Preview environment.</span>

* Connected records pages display only the connected objects or records from one object or record type in a table view. The page does not display all records of that type in the table view. 

* Depending on what environment you use, you might notice the following:

   * In the Production environment, after you add a Connected records page to a record, the page tab is visible from the record's preview area, but it is empty. You must go to the full page to see the table view for the connected record. 
   * <span class="preview">In the Preview environment, the Connected records page is visible from both the record's preview area and from the browser tab.</span>

* You can add Connected records pages for the following connected record or object types:

   * Workfront Planning record types
   * Workfront projects, programs, portfolios, groups, or companies. You can view the connected Workfront objects even when you do not have permissions to access them in Workfront. 

   >[!NOTE]
   >
   >   You cannot add a Connected records page for connected AEM Assets records.

To add a Connected records page:

1. Click the name of the record to open it. 
1. Click **Add page** from one of the following areas: 

   * <span class="preview">The record's preview window</span>
   * The record's details page, after clicking the **Open in new tab** icon ![Open details in a new tab icon](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the preview page.  

   The **Create page** box opens.

   ![Add Connected records page modal](assets/add-connection-view-page-modal.png) 

1. Add the **Page name**, click **Connected records page**, then click **Create**.

   A new tab is added to the record's page.
1. Search for or click the name of a connected record or object type in the list. 
   The table view of the record type you selected displays in the new page, and the connected records display in the table view. 
   All fields of the connected record display in the table view of the connected record's tab. 
   
   The first five fields from the connected record table display by default. No lookup fields display by default.

   ![Audience connected table view under campaign details](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Optional) In the table view of the connected records, do any of the following:

   * Click the name of a record. This opens the record's page in a new tab. 
   
      This opens the record's preview page. Click the **Open in a new tab** icon ![Open in a new tab icon](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner to open the connected record's page.

   * Click **Connect** to connect more records, then click outside the connection box to close it. The new records are automatically added to the table. 
   * Edit any information from the connected records inside the table view. 

   * Hover over a connected record's name, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following options: 
      * View 
      * Copy link
      * Edit thumbnail
      * Duplicate
      * Insert record above or below
      * Delete 
   * Select one of the records, then click one of the following options in the blue bar at the bottom of the screen: 
      * View
      * Copy link
      * Edit thumbnail
      * Duplicate
      * Delete. Delete is the only option available when you select more than one record. 

      For information about editing records in the table view, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

   * Inline edit any of the records in the table on the Connected records page. 
   
      In the Production environment, all Workfront objects display in a read-only table view and you cannot edit them. 
      
      <span class="preview">In the Preview environment, you can inline edit projects in the connected records page.</span>
   
1. <span class="preview">(Conditional) When viewing a list of connected projects, do any of the following:</span>

     * <span class="preview">Click **Connect records** in the upper-right corner of the connected record page to connect existing projects.</span>
     * <span class="preview">Inline edit project information in the table.</span> 
     * <span class="preview">Click **New row** to create a project without a template. The new project is connected to the current record immediately.</span>

         For more information, see [Create Workfront objects from Workfront Planning as you connect them to records](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
     * <span class="preview">Hover over a project and click the **More** menu [More menu](assets/more-menu.png), then click one of the following:</span>
        * <span class="preview">**Delete** to delete the project. Deleting a project disconnects it from the record and moves it to the Workfront's Recycle Bin. </span>
        * <span class="preview">**Disconnect** to disconnect the project from the record. Disconnecting a project removes it and all the values of its lookup fields from the current record. </span>

1. (Optional) Double-click the name of the Connected records page tab

   Or

   Hover over the name of the tab, then click **More** ![More menu](assets/more-menu.png), then click **Rename** to rename to new Connected view tab.
1. (Optional) Use any of the following view elements in the toolbar to manage the table view:

   * Filters
   * Sort
   * Grouping
   * Fields, to display, hide, or rearrange fields

   For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 

   >[!NOTE]
   >
   >   You cannot create, edit, or delete fields in the table view of a connected record's tab.
   >

1. (Conditional) To connect more records or objects, do one of the following: 

   * Click **Connect** at the bottom of the table, to add or remove records or any Workfront objects <span class="preview">except for projects.</span>
   * <span class="preview">In the Preview environment, click **Connect records** in the upper-right corner of the connected records page to connect existing projects or click **New row** at the bottom of the table to create projects and automatically connect them to the current record.</span>
   
   For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
1. (Optional)  Hover over the name of the Connected records page tab, click **More** ![More menu](assets/more-menu.png), then click **Delete** to remove to tab.




<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



