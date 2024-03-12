---
title: Overview of sharing permissions in Adobe Workfront planning capabilities
description: You can share or remove permissions to an Adobe Maestro workspace or view.   
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
---
<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Overview of sharing permissions in Adobe Workfront planning capabilities 

{{maestro-important-intro}}

You can share or remove permissions to a workspace or view when using the planning capabilities in Adobe Workfront.  

This article describes the permission levels for planning capabilities objects. 

For information about how to share workspaces or views, see the following articles: 

* [Share workspaces](/help/quicksilver/maestro/access/share-workspaces.md)

* [Share views](/help/quicksilver/maestro/access/share-views.md)

## Objects you can share in Adobe Workfront planning capabilities

You can share the following objects: 

* Workspaces

    When you share a workspace, all record types, records, and fields associated with the workspaces are also shared. Views are not shared. 

* Views

## Considerations about sharing objects in Adobe Workfront's planning capabilities

* Your Adobe Workfront license type works in conjunction with your permissions to give you access to view, contribute, or manage objects when using planning capabilities.

    For information about how license types affect permission levels for planning capabilities objects, see [License type overview when using the Adobe Workfront planning capabilities ](/help/quicksilver/maestro/access/license-type-overview.md).
* System administrators can manage and share workspaces that other users created. 
* If you are not a System Administrator, you can contribute to workspaces created by others if they are shared with you. 
* You cannot share workspaces in bulk. 
* You can share a workspace or a view with the following entities:
    * Users
    * Groups
* Other users, including System Administrators, can only access views they created or that have been shared with them. <!--System administrators can only be given permissions to Manage a view.-->
* You can share a link to a workspace or to a view from a record type page with others. Users who receive the link must be active users and log in to Workfront to be able to access the workspace or the record type page displayed in the selected view. 

## Sharing permissions for Adobe Workfront planning capabilities objects

The tables in the following sections illustrate the level of permissions that you can select when sharing a workspace or a view and what functionality each level allows.

>[!IMPORTANT]
>
>Not all users can have the permissions levels described below. Users' individual license determines which level of permissions they can receive for planning capabilities objects. 
>
>For information, see [License type overview when using the Adobe Workfront planning capabilities ](/help/quicksilver/maestro/access/license-type-overview.md).


### Workspace permissions

|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Edit | ✓      |            |       |
| Share  | ✓      |            |       |
| Delete   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

### Record Type permissions

Record Type permissions are inherited when you grant permissions to the workspace.

|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

### Record permissions

Record permissions are inherited when you grant permissions to the workspace.

|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |     ✓       |       |
| Edit   | ✓      |    ✓        |       |
| View   | ✓      | ✓          | ✓     |

### Field permissions

Field permissions are inherited when you grant permissions to the workspace.
The following permissions refer to the fields themselves and not to the values associated with each field. To edit field values you must have permissions to edit records. 

|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |


### View permissions

You must grant separate permissions to record views. Granting permissions to the workspace does not grant permissions to the record views in the workspace. 

|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |
| Delete | ✓      |       |
| View   | ✓      | ✓     |
| Apply  | ✓      | ✓     |





 