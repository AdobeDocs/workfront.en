---
title: Restore Deleted Records
description: You can recover deleted records from the Recently deleted area in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
---
# Restore deleted records 

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   

{{planning-important-intro}}

You can recover deleted records from the Recently deleted area in Adobe Workfront Planning. 

For information about deleting records, see [Delete records](/help/quicksilver/planning/records/delete-records.md). 

## Access requirements

+++ Expand to view access requirements for Workfront Planning. 

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
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
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
   <td>   <p>Manage permissions to a workspace</a> </p>  
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

## Considerations about recovering deleted records

* Records are stored in the Recently deleted bin for 30 days. After 30 days, the records are permanently deleted from Workfront Planning. 
* If the deleted records are linked to other records, the linked records are not deleted, but the information from the deleted record is also deleted. Restoring the deleted records will restore the information from the connected records. 
* You can restore records in bulk. 
* When the records are deleted the following information is stored in the Recently deleted bin: 
    * **Name**: This is the information in the Primary field of the record. For more information about record Primary fields, see [Primary field overview](/help/quicksilver/planning/fields/primary-field-overview.md).
    * **Deleted date**: The time and the date when the record was deleted.
    * **Time in recently deleted**: The time since the record was deleted. Records that were deleted more than 30 days before the current date do not display in the Recently deleted bin. 
    * **Deleted by**: The name of the user who deleted the record.

## Restore deleted records

1. Go to the record type page where you have deleted records. 
1. Click the **Undo** icon ![](assets/undo-icon.png) in the upper-right corner of any record type page view, then click **Recently deleted**.

    The **Recently deleted** box displays.

    ![](assets/recently-deleted-box.png)

1. Select the records you want to delete, then click **Restore** > **Restore**. You can select more than one record. 

    If the restore was successful, you receive a success notification at the bottom of the screen. 
1. Go to the table view and review the restored records.
