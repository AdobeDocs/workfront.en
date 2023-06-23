---
title: Create a taxononomy 
description: Taxonomies are a type of reusable record types that captures attributes about an operational record type in Adobe Workfront Maestro.
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Create a taxonomy

Taxonomies are record types that capture attributes about operational record types in Adobe Maestro. 

For example, Campaign can be an operational record type. The following are taxonomies which capture attributes about the Campaign record type: Region, Audience, Country. 

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

* Along with operational record types, taxonomies are building blocks of workspaces in Maestro. Record types should reflect the work lifecycle of an organizational unit. For information about workspaces, see [Create workspaces](../maestro/create-workspaces.md).  
* Taxonomies are record types that capture attributes about operational record types. We recommend to not create taxonomies that refer to work and instead to use operational record types to identify work-related information. 
* When you create a taxonomy record type, everyone in your organization can view, edit, or delete it. <!--this will change with access levels and permissions-->
<!--this is not possible yet:
* You can taxonomies to a workspace by doing one of the following:
    * Create them from scratch.
    * Link them from other systems. For example, you can create record types by linking them to teams in Workfront. - update this sentence when you can import taxonomies as well as operational records-->
* You must create a workspace before you can create taxonomies for the workspace. 
* All newly created taxonomies come with the following fields: 

    * Name <!--if there won't be any more fields, consider rephrasing this-->

    Additionally, you can add custom fields to taxonomies. For more information, see [Create Maestro fields](../maestro/create-fields.md).  
* You can have a combined total of 1,000 operational record types and taxonomies in one workspace. This includes record types or taxonomies that you create from scratch or that you import from other systems. 

## Create a taxonomy

Creating taxonomies is identical to creating an operational record type. 

For information about creating record types, see [Create operational record types](../maestro/create-operational-record-types.md).
