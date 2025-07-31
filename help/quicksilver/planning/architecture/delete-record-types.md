---
title: Delete Record Types
description: You can delete record types when they are no longer relevant. Deleting record types also deletes all information associated with the record types, like their records, fields, and views.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
---

# Delete record types

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

You can delete record types when they are no longer relevant. 

However, deleting record types also deletes all information associated with the record types. For more information, see the [Considerations when deleting record types](#considerations-when-deleting-record-types) section in this article. 

For information about record types, see [Record types overview](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
<p>Any </p> 
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
   <td>   <p>Manage permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


## Considerations when deleting record types

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* You can delete only record types from workspaces to which you have Manage permissions.
* Deleting record types removes the following information associated with them:

   * All records of that type.
   * All fields associated with the record type. 
   * All views (including filters, groupings, and sorting criteria) of the record type.
* The record type is removed from all users accessing the workspace.
* You cannot recover deleted record types or their information. 
* We recommend recreating the fields and the records associated with the record type that you want to delete on another record type before deleting them.

## Delete record types

{{step1-to-planning}}

1. Click the workspace whose record types you want to delete, 

    Or

    From a workspace, expand the downward-pointing arrow to the right of an existing workspace name, search for a workspace, then select it when it displays in the list.

    The workspace opens and the record types display. 
1. Do one of the following:

   * Hover over the record type card, click the **More** menu, then **Delete**. 
   * Click the card for the record type that you want to delete, and from the record type page, click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Delete**. 

   ![Permanently delete record type confirmation](assets/permanently-delete-record-type-confirmation.png)

1. Type **delete** in the confirmation box, then click **Permanently delete**. This is not case sensitive. 
   
   The selected record type, along with their fields, associated records, and views are deleted and cannot be recovered. 
