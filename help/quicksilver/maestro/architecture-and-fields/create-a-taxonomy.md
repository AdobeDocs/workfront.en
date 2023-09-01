---
title: Create taxonomy record types 
description: Taxonomies are a type of reusable record types that captures attributes about an operational record type in Adobe Workfront Maestro.
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Create taxonomy record types

>[!IMPORTANT]
>
>Currently, Adobe Maestro is part of a closed beta program which is open to a limited number of customers. 

Taxonomies are record types that capture attributes about operational record types in Adobe Maestro. 

For example, Campaign can be an operational record type. The following are taxonomies which capture attributes about the Campaign record type: Region, Audience, Country. 

For more information about Maestro record types, see [Overview of record types and taxonomies](../architecture-and-fields/overview-of-record-types-and-taxonomies.md). 

## Access requirements

You must have the following access to perform activities mentioned in this article: 

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
>*If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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
  >    Taxonomies created when using a workspace template have additional field. 

## Create a taxonomy

Creating taxonomies is similar to creating an operational record type from scratch or from a workspace template. 

For information, see the section "Create a record type from scratch" in the article [Create record types](../architecture-and-fields/create-record-types.md). 

For information about automatically creating taxonomies when creating a workspace from a template, see [Create workspaces](../architecture-and-fields/create-workspaces.md). 
