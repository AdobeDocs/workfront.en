---
filename: permissions-for-shared-objects
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Permissions for shared objects
description: Anyone who can view an item in Adobe Workfront can grant other users permissions to that item when they share it, as described in Share a project in Adobe Workfront. Sharing permissions are specific to one item in Workfront and define what actions the recipient user or users can take on the item.
---

# Permissions for shared objects

Anyone who can view an item in Adobe Workfront can grant other users permissions to that item when they share it, as described in [Share a project in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md). Sharing permissions are specific to one item in Workfront and define what actions the recipient user or users can take on the item.

##  

The creator of an object has default Manage permissions to it and can share access to it with other users through permissions they grant on it.

## Permission levels

A user with permissions to at least View an object can share that object with someone else.

>[!NOTE]
>
>A Workfront administrator can add or remove permissions to any items in the system, for all users, without being the owner of those items.

The task of sharing an object is identical for all objects, as explained in [Overview of sharing permissions on objects in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md). You can share the following objects in Workfront:

* `Projects`: For more information, see [Share a project in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* `Templates`: For more information, see [Sharing a template](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

* `Portfolios`: For more information, see [Share a portfolio in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).

* `Tasks`: For information, see [Share a task in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* `Issues`: For information, see [Share an issue in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* `Documents`: For information, see [Share a document in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* `Reports, dashboards, and calendars`: For information, see [Share reports, dashboards, and calendars in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* **Filters, views, and groupings**: For information, see [Share a filter, view, or grouping in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md). 

* `Programs`

The following table illustrates the permission settings you can select from when sharing an object. Not all objects have all these settings available.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">View</td> 
   <td> <p>You can perform the following actions on the object:</p> 
    <ul> 
     <li>View the object</li> 
     <li>Add documents to the object</li> 
     <li>View Finance information about the object</li> 
     <li> <p>Share the object<br></p> <p>When you share the object, you can grant other users the same permission level you have only on the object, not a higher level.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Contribute</td> 
   <td> <p>You can perform the following actions on the object:</p> 
    <ul> 
     <li>View it</li> 
     <li>All the actions included with the View permission.</li> 
     <li>Add Expenses to it</li> 
     <li>Add issues to it (if it is a task or a project)</li> 
     <li>Add tasks to it (if it is a project)</li> 
     <li>Edit Custom Forms on it</li> 
     <li>Log Hours on the object</li> 
     <li>Make assignments in it</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Manage</td> 
   <td> <p>You can perform the following actions on the object:</p> 
    <ul> 
     <li>View it</li> 
     <li>All the actions included with the View and Contribute permissions</li> 
     <li>Delete it</li> 
     <li>Manage Finance information in it</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Make this public to external users</td> 
   <td> <p>Anyone without a Workfront account can view the object by clicking a link to it.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Make this visible system-wide</td> 
   <td> <p>The object can be found in searches and viewed by anyone with a Workfront account.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Requesting permissions

You can request permissions to an object that you can’t access, or you can request higher permissions than you already have. Anyone with permissions to Share the item can grant permissions to other users requesting them.

For more information about requesting permissions, see [Request access to objects in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## Sharing objects

<!--
The following table lists the objects can be shared in Workfront and the entities with which they can be shared:
-->

<!--
Object People Teams Job Roles Groups Companies Public System-Wide Calendars ✓ ✓ ✓ ✓ ✓ ✓ ✓ Custom Forms ✓ ✓ ✓ ✓ ✓ ✓ Documents ✓ ✓ ✓ ✓ ✓ ✓ ✓ Dashboards ✓ ✓ ✓ ✓ ✓ ✓ Issues ✓ ✓ ✓ ✓ ✓ ✓ Portfolios ✓ ✓ ✓ ✓ ✓ ✓ Programs ✓ ✓ ✓ ✓ ✓ ✓ Projects ✓ ✓ ✓ ✓ ✓ ✓ Reports ✓ ✓ ✓ ✓ ✓ ✓ ✓ Tasks ✓ ✓ ✓ ✓ ✓ ✓ Templates ✓ ✓ ✓ ✓ ✓ ✓
-->

<!--
* This is available only if your organization has purchased the Workfront Scenario Planner. For information about the Workfront Scenario Planner, see The Adobe Workfront Scenario Planner overview.
-->

##  

This table lists the objects that users can share and how they can share them: 

| ` `Object`` | ` `Share with Workfront users`` | ` `Share publicly with users outside of Workfront`` | ` `Share via email with anyone`` |
|---|---|---|---|
| `Project` | `✓` |&nbsp; |&nbsp; |
| `Task` | `✓` |&nbsp; |&nbsp; |
| `Issue` | `✓` |&nbsp; |&nbsp; |
| `Portfolio` | `✓` |&nbsp; |&nbsp; |
| `Program` | `✓` |&nbsp; |&nbsp; |
| `Template` | `✓` |&nbsp; |&nbsp; |
| Custom Form |✓ |&nbsp; |&nbsp; |
| `Report` | `✓` | `✓` |&nbsp; |
| `Dashboard` | `✓` | `` |&nbsp; |
| `Calendar` | `✓` | `✓` |&nbsp; |
| Filter |✓ |&nbsp; |&nbsp; |
| View |✓ |&nbsp; |&nbsp; |
| Grouping |✓ |&nbsp; |&nbsp; |
| `Document` | `✓` | `✓` | `✓` |

## Inherited permissions

* If a user shares an object with certain permissions and that object has any child objects below it, the recipient inherits the same permissions for those child objects. 
* If an access level restricts users from deleting certain objects, this doesn’t keep them from deleting child objects that are contained in those objects.

Permissions in Workfront are inherited hierarchically. For more information about inherited permissions, see the [Understand inherited permissions and the hierarchy of objects](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#understanding-inherited-permissions) section in [Overview of sharing permissions on objects in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md). 