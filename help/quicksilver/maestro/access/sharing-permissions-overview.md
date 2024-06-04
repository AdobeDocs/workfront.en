---
title: Overview of sharing permissions in Adobe Workfront Planning
description: You can share or remove permissions to an Adobe Workfront Planning workspace or view.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
---
<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Overview of sharing permissions in Adobe Workfront Planning 

{{planning-important-intro}}

You can share or remove permissions to a workspace or view in Adobe Workfront Planning.  

This article describes the permission levels for Workfront Planning objects. 

For information about how to share workspaces or views, see the following articles: 

* [Share workspaces](/help/quicksilver/maestro/access/share-workspaces.md)

* [Share views](/help/quicksilver/maestro/access/share-views.md)

## Objects you can share in Adobe Workfront Planning

You can share the following objects: 

* Workspaces

    When you share a workspace, all record types, records, and fields associated with the workspaces are also shared. Views are not shared. 

* Views

## Considerations about sharing objects in Adobe Workfront Planning

* Your Adobe Workfront license type works in conjunction with your Workfront Planning permissions to give you access to view, contribute, or manage objects when using Workfront Planning.

    For information about how license types affect permission levels for Workfront Planning, see [License type overview when using Adobe Workfront Planning](/help/quicksilver/maestro/access/license-type-overview.md).
* System administrators can manage and share workspaces that other users created. 
* If you are not a System Administrator, you can contribute to workspaces created by others if they are shared with you. 
* You cannot share workspaces or views in bulk. 
* You can share a workspace or a view with the following entities:
    * Users
    * Groups
<!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->
* Other users, including System Administrators, can only access views they created or that have been shared with them. System administrators can only be given permissions to Manage a view.
* You can share a link to a workspace or to a view from a record type page with others. Users who receive the link must be active users and log in to Workfront to be able to access the workspace or the record type page displayed in the selected view. 

## Sharing permissions for Adobe Workfront Planning objects

The tables in the following sections illustrate the level of permissions that you can select when sharing a workspace or a view and what functionality each level allows.

>[!IMPORTANT]
>
>Not all users can have the permissions levels described below. Users' individual license determines which level of permissions they can receive for Workfront Planning objects. 
>
>For information, see [License type overview when using Adobe Workfront Planning](/help/quicksilver/maestro/access/license-type-overview.md).


### Workspace permissions

You must give users permission to workspaces to allow them to have access to the following entities:

* Workspaces
* Record types
* Records
* Fields
* Views*
    
    *You can allow all users with View or higher permissions to a workspace to also access the views in the workspace. This is an additional permission that you must enable when sharing a view. For information, see [Share views](/help/quicksilver/maestro/access/share-views.md).

The following are the levels of permissions for workspaces: 

|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Edit | ✓      |            |       |
| Share  | ✓      |            |       |
| Delete   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

### Record Type permissions

Record Type permissions are inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

### Record permissions

Record permissions are inherited when you grant permissions to the workspace.

The following are the levels of permissions for records: 


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

You must give users permission to  views to allow them to have access to the following view elements:

* Filters
* Field visibility
* Sort
* Grouping
* Row height
* Settings


<!--You can share views internally or publicly. -->

The following are the levels of permissions for views and view elements: 

|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Apply  | ✓      | ✓     | ✓                          |

*Users must have View or higher permissions to a workspace to gain this view access.
            
<!--Replace the table above with the following when public sharing releases: 

|   Internal sharing     | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Apply  | ✓      | ✓     | ✓                          |

|   Public sharing      | View  |
|--------|-------|
| View   | ✓     |
| Apply  | ✓     |
-->


<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |    
-->