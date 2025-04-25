---
title: Add a Cover Image to a Record
description: You can personalize records by adding a cover image to the record page in Adobe Workfront Planning, when editing a record.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
---

# Add a cover image to a record

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

You can personalize records by adding a cover image to the record page in Adobe Workfront Planning, when editing a record.

For information about editing records, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

You must create record types before you can start creating and editing records. 

For information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

## Access requirements

+++ Expand to view access requirements.. 

You must have the following access to perform the steps in this article:  

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
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
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
   <td><p> Standard</p>
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
   <td>   <p>Contribute or higher permissions to a workspace <span class="preview">and record type</span>  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## Considerations about record page cover images

You can personalize a record's page by adding a cover image to it. 

Consider the following: 

* A cover image is unique to one record, and it does not apply to all records of the same type. 
* You can add only image files as cover images.
   <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* You can add a cover image to individual records from the record preview in any view, or from the record page. 
* You cannot add cover images from a record view. 
* Workfront automatically uploads a cover image every time you create a record. You can later modify this image.

## Add a cover image to a record

You can personalize a record by adding a cover image at the top of the record preview or page. 

{{step1-to-planning}}

1. Click the workspace whose records you want to personalize,

    Or

    From a workspace, expand the downward-pointing arrow to the right of an existing workspace name, search for a workspace, then select it when it displays in the list.

    The workspace opens and the record types display.

1. Click a record type card. 

    The record type page opens. 

1. From a view of any type, click a record 

    Or 
    
    From the table table view, click the **Open details** icon ![Open details icon](assets/open-details-icon-in-table-name-field.png) in the first column. 
    
    The record's preview opens in the view.

    ![Details preview box](assets/details-box.png) 

    
1. (Optional) Click the **Open in new tab** icon ![Open in new tab icon](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in the upper-right corner of the record preview to open the record's page in a new tab. 

    The record page opens. 

    ![Details page](assets/details-page.png)

1. In the record preview or details page, hover over the space above the record name, then click **Add cover**.
    
    Or
    
    Hover over an existing cover image, click the **More** menu ![More menu](assets/more-menu.png) , then click **Upload**. <!--check the casing here; I logged a bug for this-->
    The **Record cover** box opens in the **Upload** tab. 

    ![Record cover box for upload](assets/record-cover-box-for-upload.png)

1. Click **Browse images** and browse for a picture on your computer to select and add it. 

1. (Optional) To remove the image before it is saved, click the **Upload new image** icon ![Upload new image icon](assets/upload-new-image-icon.png) , and upload a new image.

1. (Optional) Click the **Gallery** tab, then click an image in the gallery of images. The gallery of images cannot be modified.

    ![Record cover box for gallery](assets/record-cover-box-for-gallery.png)

1. Click **Use image**.

    The image is uploaded at the top of the record preview or details page and changes are saved automatically. 

    ![Record page with cover image](assets/record-page-with-cover-image.png)

1. (Optional) Hover over the image, then click the **More** menu ![More menu](assets/more-menu.png) in the lower-right corner of the cover image, then do one of the following: 

    * Click **Upload** if you want to replace the cover image and repeat Step 6 to upload and save a new image.
    * Click **Reposition**, and use the **Reposition** tool ![Reposition tool icon](assets/reposition-tool-icon.png) to center the cover image, then click **Save** when done. 
    * Click **Remove** to remove the cover image. 

    Workfront automatically saves your changes.
