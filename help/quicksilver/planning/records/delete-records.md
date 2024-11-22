---
title: Delete Records
description: You can delete records that you or another user created. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
---

# Delete records 

<!--take Preview and Production references out at release-->

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   

{{planning-important-intro}}

You can delete records that are no longer relevant in Adobe Workfront Planning. <span class="preview">You can recover deleted records for 30 days after they were deleted. For information about recovering deleted records, see [Recover deleted records](/help/quicksilver/planning/records/restore-deleted-records.md). </span>

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
   <td>   <p>Contribute or higher permissions to a workspace</a> </p>  
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


<!--

OLD

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
   <td role="rowheader"><p>Adobe Workfront license*</p>
   </td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning </p>  
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

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Considerations about deleting records

* You can delete records that you or another user created. 
* You cannot recover deleted records in the Production environment. <span class="preview">You can recover deleted records in the Preview environment.</span>
* If the deleted records are linked to other records, the linked records are not deleted, but the information from the deleted record is also deleted. 
* You cannot delete records from the timeline or the calendar views. 

## Delete records

You can delete a record from the following areas:

* [From the record's page](#delete-a-record-from-the-records-page)
* [From the table view of a record type](#delete-a-record-from-the-record-type-table-view) 

### Delete a record from the record's page

{{step1-to-planning}}

1. Click the workspace whose records you want to delete.

    The workspace opens and the record types display as cards.

1. Click a record type card. 

    The record type page opens. 
1. Do one of the following:

    * From a Table view, click the name of a record. 
    * From the Table view, hover over the name of a record, then click the **More** menu ![](assets/more-menu.png), then click **View**

        ![](assets/contextual-menu-for-record-row.png)
    * From a Timeline view, click a record bar. 

    The record page opens.  
  
1. Click the **More** menu ![](assets/more-menu.png) to the right of the record name, then click **Delete**, then **Delete** again to confirm. 

    ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
    The record is deleted.   
1. (Optional and conditional) If you delete the record in the Preview environment, go to the table view of the record page, and click the **Undo** icon ![](assets/undo-icon.png) in the upper-right corner of the view, then click **Recently deleted** to recover the deleted records. 

  For information about recovering deleted records, see [Recover deleted records](/help/quicksilver/planning/records/restore-deleted-records.md).

### Delete a record from the record type table view

{{step1-to-planning}}

1. Click the workspace whose records you want to delete.

    The workspace opens and the record types display as cards.

1. Click a record type card. 

    The record type page opens. 
1. (Conditional) From the **View** drop-down menu in the upper-left corner of the table, select a Table view. This should be the default view, unless you viewed the record type in the timeline view when you accessed it last. 

    The records associated with the selected record type display in the table view. 
1. Do one of the following:

    * Right-click a record row, then click **Delete**. 
    * Click the **More** menu ![](assets/more-menu.png) to the right of the record name, then click **Delete**.

        ![](assets/contextual-menu-for-record-row.png)
    
    * Click the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to open the box with the record's detailed information, and click **More** ![](assets/more-menu.png) to the right of the record name, then **Delete**.

    The record is deleted.
    
1. (Optional) Do one of the following to undo or redo deleting a record:

    * <span class="preview">Click the **Undo** icon ![](assets/undo-icon.png), then **Recently deleted** to recover the deleted records. For information about recovering deleted records, see [Recover deleted records](/help/quicksilver/planning/records/restore-deleted-records.md). </span>
    * Use the following keyboard shortcuts to undo or redo deleting a record:

      * CTRL + Z (⌘ + Z for Mac) to undo deleting a record
      * CTRL + Shift + Z (⌘ + Shift + Z for Mac) to redo deleting record




