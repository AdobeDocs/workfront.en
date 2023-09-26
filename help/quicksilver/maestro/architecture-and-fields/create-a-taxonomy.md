---
title: Create taxonomy record types 
description: Taxonomies are a type of reusable record types that captures attributes about an operational record type in Adobe Workfront Maestro.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Create taxonomy record types

>[!IMPORTANT]
>
>Currently, Adobe Maestro is part of a beta program which is open to a limited number of customers.
>
>Contact your account representative for more information about joining the beta program for Maestro.
>
>For information, see [Adobe Maestro overview](../maestro-overview.md).

Taxonomies are record types that capture attributes about operational record types in Adobe Maestro. 

For example, Campaign can be an operational record type. The following are taxonomies which capture attributes about the Campaign record type: Region, Audience, Country. 

For more information about Maestro record types, see [Overview of record types and taxonomies](../architecture-and-fields/overview-of-record-types-and-taxonomies.md). 

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
 <tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader">Access level</td>
   <td> <p>Any</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>--> 

## Considerations about creating taxonomies

* You must create a workspace before you can create taxonomies in the workspace. 

  For information about workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md).  
* You can create a taxonomy record type by doing one of the following:
   * Create them automatically when you create a workspace using a template. For information, see [Create workspaces](../architecture-and-fields/create-workspaces.md).
   * Create them manually, from scratch.  
   * Create them manually, by pasting information from an external list. 

  <!--this is not possible yet:
  * You can taxonomies to a workspace by doing one of the following:
    * Create a connection to object types from other systems, when adding fields to a taxnomy record type. This creates a read-only record type in Maestro.  - update this sentence when you can connect taxonomies as well as operational records to a third-party system.-->

* All newly created taxonomies come with the following fields: 

    * Name <!--if there won't be any more fields, consider rephrasing this-->

    Additionally, you can add custom fields to taxonomies. For more information, see [Create fields](../architecture-and-fields/create-fields.md).  

  >[!NOTE]
  >
  >    Taxonomies created when using a workspace template have additional fields. 

## Create a taxonomy

Creating taxonomies is similar to creating an operational record type from scratch or from a workspace template. 

For information, see the section "Create a record type from scratch" in the article [Create record types](../architecture-and-fields/create-record-types.md). 

For information about automatically creating taxonomies when creating a workspace from a template, see [Create workspaces](../architecture-and-fields/create-workspaces.md). 
