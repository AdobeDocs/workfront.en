---
title: Delete records 
description: You can delete records that you or another user created. You cannot recover deleted records. 
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Delete records

You can delete records that are no longer relevant in Adobe Maestro. 

## Access requirements

You must have the following to perform the steps described in this article: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
<!--the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p> 
  <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Product</p></td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see the "Enable Maestro for the users in your Workfront instance" section in the article <a href="../maestro/maestro-overview.md">Adobe Maestro overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Considerations about deleting records

* You can delete records that you or another user created. 
* You cannot recover deleted records. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* If the deleted records are linked to other records, the linked records are not deleted, but the information from the deleted record is also deleted. 
* You cannot delete records in bulk. <!--this will probably change-->


## Delete records

You can delete a record from the following areas:

* [From the Details page of a record](#delete-a-record-from-the-records-details-page)
* [From the table view of a record type](#delete-a-record-from-the-record-type-table-view) 

### Delete a record from the record's Details page

1. Click the **Main Menu** ![](assets/main-menu-workfront.png) in the upper-right corner, or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available, then click Maestro. 

    The workspace that you access last opens. 
1. Click a record type. 

    The record type page opens. 
1. (Conditional) From the **View** drop-down menu, select a table view. This should be the default view, unless you viewed the record type in the timeline view when you accessed it last. 

    The records associated with the selected record type display in the table view. 
1. Right-click a record row, then click **View**.

    ![](assets/contextual-menu-for-record-row.png)

    The record **Details** page opens. 
1. Click the **More** menu to the right of the record name, then click Delete, then Delete again. 

    ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
    The record is deleted and cannot be recovered. 

### Delete a record from the record type table view

1. Click the **Main Menu** ![](assets/main-menu-workfront.png) in the upper-right corner, or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available, then click **Maestro**. 

    The workspace that you accessed last opens. 
1. Click a record type. 

    The record type page opens. 
1. (Conditional) From the **View** drop-down menu in the upper-right corner of the table, select a table view. This should be the default view, unless you viewed the record type in the timeline view when you accessed it last. 

    The records associated with the selected record type display in the table view. 
1. Right-click a record row, then click **Delete**. 

    ![](assets/contextual-menu-for-record-row.png)

    The record is deleted and cannot be recovered. 
