---
title: Configure Record Type Business Rules
description: You can configure record type business rules that define how records of that type are managed in Adobe Workfront Planning. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---

# Configure record type business rules

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

You can configure record type business rules that define how records of that type are managed in Adobe Workfront Planning. 

## Access requirements

+++ Expand to view access requirements to perform the steps in this article:  

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
<li><p>Any Workfront or Workflow with a Planning package</p></li>
Or
<li><p>Any Planning package when purchased as a standalone product</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning license</p></td> 
   <td><p>Planning Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to a record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

 For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations when configuring business rules

* You can configure rules for when records can be edited or deleted, depending on conditions you define. 

   For example, you can create conditions for requiring certain fields to have a value. If the value is missing from those fields, users cannot edit or delete that record. 
* You cannot add business rules to global record types in their primary or secondary workspaces. 
* You cannot configure rules for when records are created. Everyone with Manage permissions to the record type can create records.
* You can create a condition for your business rule that references all field types except for the following:  
    * Formula fields 
    * Lookup fields 
    * Reference fields  

## Configure business rules

1. Go to a record type. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click Business rules.



