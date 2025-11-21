---
title: Share Records
description: You can share records using the Share button to increase collaboration in Adobe Workfront Planning. 
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: yes
hide: yes
---

<!--update metadata with real information at release-->

# Share records

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

You can adjust people's permissions to individual records in a record type. O

You can share an Adobe Workfront Planning record in the following ways: 

* Share a link to the record. 

    For more information, see [Share records using a link](/help/quicksilver/planning/records/share-records.md).

* Share all records in a workspace with other users by sharing the workspace and the record type.

   For more information see the following articles:

   * [Share a workspace](/help/quicksilver/planning/access/share-workspaces.md)

   * [Share a record type](/help/quicksilver/planning/access/share-record-types.md)

* Share a record using the **Share** option.

    This article describes how you can share a record with others using the **Share** option. 

>[!IMPORTANT]
>
>Users with access to a workspace automatically gain at least View permissions to all the records in the workspace. 
>Sharing views does not give users permissions to records. Only sharing workspaces can grant users permissions to record types and records. 
>
>For general information about sharing objects in Workfront Planning, also see [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md). 


## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront and Planning package</p> 
Or
<p>Any Workflow and Planning package</p> 
 </tr>
   
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Any</p> 
   <p><b>NOTE</b></p>
   <p>Only people with a Standard license can be granted Manage permissions to records. All other licenses can only have View permissions and the Manage option is dimmed for them.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>Manage permissions to a workspace, a record type, and the record</p>  
   <p><b>IMPORTANT</b></p>
   <p>Only users with Manage permissions to a workspace can share a record</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>
 
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations when sharing records

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

* You can share records with the following entities: people, groups, teams, companies or job roles.
* When you share a workspace with users, they also receive the same permissions to the records in the workspace, by default. 
* When you remove an entity from a workspace, all sharing permissions are removed from the record types and all records in it.  
* A user's access to the record is determined through the combination of the following 3 settings: 

   * Their permissions inherited from the record type and workspace
   * Permissions individually added in the record sharing dialog 
   * The following permissions:

      * **Everyone in the workspace can view**: This makes the record viewable by everyone in the workspace <!-- is this OK to say "workspace? should it be "record"??-->
      * **Only invited people can access**: This is selected by default and allows restricting access to the record to specific people. 

* You can grant the following levels of permissions to a record: 

   * View 
   * Manage 

* When you share a record with a user, they are added with the same permission as they have on the record type, by default. 

   For example: 
   
   * If they have View permissions to the record type, they gain View permissions to the record
   * If they have Contribute or Manage permissions to the record type, they gain Manage permissions to the record

* As a workspace manager, you can share a record with a user that is not part of the workspace. In this case, there is a warning next to the added entity notifying that they don't have access to the workspace. You can accept to add the user to both the record and the workspace, or deny adding them to the workspace which also removes them from the record. 

* When you share a record with users that have Manage permissions to the workspace, they also get Manage permissions to the record by default. The View permission is dimmed. 

* If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.

* You can disable inherited permissions for a single record, in which case you can give them permissions individually, or they can gain permissions if they belong to "Everyone in the workspace" option. <!-- is this OK to say "workspace? should it be "record"??-->

* If multiple sharing permissions apply for the same user, they receive the highest permission of those permissions.  

   For example, if a record is shared with a user with View permissions, and their group with Manage access, they get Manage permissions to the record.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* If a formula field or a lookup field from a connected record is based on a field on a record on which you have no permissions, you will see the correct calculation which factors in the record you cannot otherwise access.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Share record permissions

