---
title: Create a taxononomy 
description: Taxonomies are a type of reusable record types that captures attributes about an operational record type in Adobe Workfront Maestro.
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Create a taxonomy

Taxonomies are reusable record types that capture attributes about operational record types in Adobe Workfront Maestro. 

For example, Campaign can be an operational record type. The following are taxonomies which capture attributes about the Campaign record type: Region, Address, Audience, Country. 

For more information about Maestro record types, see [Overview of Adobe Maestro record types](../maestro/overview-of-record-types-and-taxonomies.md)

## Access requirements

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

## Considerations about taxonomies

* Taxonomies are a kind of record type in Maestro. 

    Operational record types are record types that define work. Taxonomies are record types that capture attributes about operational record types. We recommend to not create taxonomies that refer to work. 
* You must create a workspace before you can create a taxonomy.
* When you create a taxonomy, everyone in your organization can view, edit or delete it.
* You can link taxonomies with operational record types by using relationship-type fields. In addition, you can create custom fields for taxonomies. For more information, see [Create fields for Maestro records](../maestro/create-fields.md). 
* All newly created taxonomies come with the following set of fields:

    * Name
    * Description
    * Start Date
    * End Date
    * Status


## Create a taxonomy

Creating taxonomies is identical to creating an operational record type. 

For information about creating record types, see [Create operational record types](../maestro/create-operational-record-types.md).
