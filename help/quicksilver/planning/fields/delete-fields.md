---
title: Delete Fields
description: In Adobe Workfront Planning, you can delete custom fields that are no longer relevant.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EusoK7-jmYJHg9nqyvvQamsfVeUy802p36EyDmLGwik
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Delete fields

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

In Adobe Workfront Planning, you can create custom fields to store information about records. 

For information about creating custom fields in Workfront Planning, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).

You can delete Workfront Planning fields that are no longer relevant. 

## Access requirements

+++ Expand to view the access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul> 
<li><p>Any Workfront and any Planning package</p></li>
Or
<li><p>Any Workflow and any Planning package</p></li></ul>

<p>To delete fields from global record types:</p>
<ul><li><p>Any Workfront package and a Planning Plus package</p></li>
Or
<li><p>Any Workflow and Planning Prime and Ultimate packages</p></li></ul>

<p>For more information about what is included in each Workfront Planning package, contact your Workfront account representative. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--
Old:

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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table>
-->

## Considerations about deleting Workfront Planning fields:

* You can delete a field only in the record type table view.
* You cannot delete the primary field of a record. 
* Any information stored in the field is deleted and cannot be recovered. 
* When you delete a connected record field, all the connected lookup fields are also deleted from the record type you connect from. The connected record fields of the record types you connect to are also deleted from the record you connect to.

   For example, when you connect Campaigns to another record type called Product, and you delete the Product connected field and the Product's Status lookup field from the campaign, the following are deleted:
      
   * The Product connected field from the campaign
   * The Product Status lookup field from the campaign
   * The Campaign connected field from the product 

   For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

* You cannot delete fields from global records that have been added to a secondary workspaces from the secondary workspaces.

## Delete fields

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}
    
1. Click the workspace whose record fields you want to delete. 

    The workspace opens and the record types display. 

1. Click the card of a record type. 

1. (Conditional) If not already selected, click the tab of a **Table view** on the record type page. 

     All existing records associated with the record type display in the rows of the table view.
     
1. Find the field that you want to delete in the column headers, and hover over the column header, then click the downward-pointing arrow after the field name. 

   ![Arrow menu after name of field in table header highlighted](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)
   
1. Click **Delete**. <!-- check this: they might replace it with **Delete field**-->

    <!--insert screen shot when finalized-->

1. (Conditional) If the field you are deleting is part of a request form, the **Delete field** box displays to indicate the forms that will be impacted by your changes. Do one of the following:

   * Click the right-pointing arrow to display the forms impacted by the change, then click the form name to open the form in a new tab and decide whether you want to keep the field on the form or make additional changes to the form. 
   * Click **Delete** which will delete the field from all areas where it displays. 

   Deleted fields cannot be recovered.

   Depending on what type of field you deleted, the following happens: 
   
      * If you delete a field that belongs to the record you selected, the field is deleted and can no longer be associated with any records. If this field is added as a lookup field on other records, those fields are also deleted. 
      * If you delete a connection field, the field is deleted from the record you selected. Also, the corresponding connection field from its original record is also deleted. 
      * If you delete a lookup field that was added from a connected record, the field is deleted from the record type you selected, but it remains on its original record type. 
      * If you delete a field from a global record type in its primary workspace, it is deleted from all the workspaces where that record type has been added. You cannot delete fields from global record types from their secondary workspaces.
