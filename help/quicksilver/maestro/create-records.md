---
title: Create records
description: You must create record types before you can create individual records. 
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Create records

In Adobe Maestro, a record is an instance of a record type. 

You can have the following type of records:

* Operational records: They represent work. For example, for an operational record called "Campaign", you can have named records like "Monthly Newsletter" or "Summer Sale."
* Taxonomy records: They represent attributes that can be associated with operational records. For example, for a taxonomy record type called "Channel", you can have named taxonomies like "Email", "Social Media", or "Advetising". 

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

## Create records by manually adding them to a record type <!--in a record type table (I don't think you can create them elsewhere right now)-->

## Creating records by importing them from another application

You must link a Maestro record type to a third-party application's object types before you can import new records from another application. 

For example, you must create a Maestro record type by linking it to the Workfront project object type, before importing projects from Workfront into the Maestro record type. 