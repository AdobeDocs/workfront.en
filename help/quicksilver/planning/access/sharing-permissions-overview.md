---
title: Overview of Sharing Permissions in Adobe Workfront Planning
description: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes general information about sharing or removing permissions to an Adobe Workfront Planning workspace or view.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
---

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Overview of sharing permissions in Adobe Workfront Planning 

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->



{{planning-important-intro}}

You can share or remove permissions to an Adobe Workfront Planning workspace, record type, or view. 

You can also share Planning request forms. For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md). 

This article describes the permission levels for Workfront Planning workspaces, record types, records, fields, and views. 

## Objects you can share in Adobe Workfront Planning

You can manually share some Workfront Planning objects, while other objects inherit these permissions from other objects. 

You can manually share the following objects in Workfront Planning: 

* Workspaces

    * You can share workspaces with people inside your organization.
    * When you share a workspace, all record types, records, and fields associated with the workspaces are also shared. 
    * When you share a workspace, views are not shared. Views are shared separately. 

    For more information, see [Share workspaces](/help/quicksilver/planning/access/share-workspaces.md)

* Record types

    * You can share record types with people inside your organization.
    * The level of permissions granted for the workspace displays as Inherited permissions for the record type. 
    * You cannot share a record type with a higher permission level than the user has on the workspace. 

    For more information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md). 


* Views

    * You must give users, including System Administrators, permissions to access views separately from their permissions to accessing workspaces. 
    * When you share a view, all view elements are shared, including filters, grouping, sort, or Settings. 
    * When you share a view, the records visible in the view are not shared. Records must be shared by sharing workspaces.
    * You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.

    For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).
   
## Considerations about sharing objects in Adobe Workfront Planning

* Your Adobe Workfront license type works in conjunction with your Workfront Planning permissions to give you access to view, contribute, or manage workspaces and their objects.

    For information about how license types affect permission levels for Workfront Planning, see [License type overview when using Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* System Administrators can manage all workspaces in the system, including the ones they did not create. 
* Other users, including System Administrators, can only access views they created or that have been shared with them. System Administrators can be given permissions only to Manage a view.

* When you share workspaces and record types with others, the permission level from the record type is automatically inherited to the records and fields associated with them. 

    >[!IMPORTANT]
    >
    >If your organization's instance of Workfront has been onboarded to the Adobe Unified Experience, the users you want to share Planning objects with must be added to the Adobe Admin Console. You cannot share Planning objects with Workfront users who have not been added to the Adobe Admin Console. 

* You can share Planning objects in the following ways: 
    
    * Internally, you can share a workspace, a view, or a record type with the following Workfront entities:

        * Users
        * Groups
        * Teams
        * Companies
        * Job roles

        You can share a Planning object with up to 100 entities per object. 

    * Internally, by sharing a link to a workspace or to a view with other Planning users. The following scenarios exist:

        * Users who receive the link to a workspace must be active users and log in to Workfront to access the workspace.
        * Users who receive an Internal sharing link for a view must be active users and log in to Workfront to access the view.
    * Externally, by sharing a Public sharing link to a view with external users that do not have a Workfront account. 

## Sharing permissions for Adobe Workfront Planning objects

The tables in the following sections illustrate the level of permissions that you can select when sharing a workspace or a view and what functionality each level allows.

>[!IMPORTANT]
>
>Not all users can have the permissions levels described below. Users' individual license determines which level of permissions they can receive for Workfront Planning objects. 
>
>Only Standard (or Plan) license users can have Contribute or Manage permissions to workspaces and Manage permissions to views.
> 
>Users with all other license types can have View permissions to workspaces and views. 
>
>For information, see [License type overview when using Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Permissions to workspaces

You must give users permission to workspaces to allow them to have access to the following entities:

* Workspaces
* Record types
* Records
* Fields

The following are the levels of permissions for workspaces: 

|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Edit | ✓      |            |       |
| Share  | ✓      |            |       |
| Delete   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

### Permissions to record types

<!-- old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

Record Type permissions are always inherited when you grant permissions to the workspace.

You can remove the record type's inherited permissions received from the workspace. 

You can give users lower permissions on the record type than they have on the workspace. 

However, you can not do the following:

* Grant higher permissions for the record type than users have on the workspace.
* Give workspace managers lower permissions on a record type.
* Remove View permissions to the record type or the workspace by removing users from the record type permissions.  

The following scenarios exist: 

|   Workspace permissions     | Automatic inherited permissions for a Record Type |Possible Record Type permissions when Inherited permissions are turned off (granted manually)| 
|--------|--------|-------------|
| Manage |   Manage    |   Manage, Remove permissions*           | 
| Contribute |     Contribute |  Contribute, View, Remove permissions*        |
| View   |  View     |      View, Remove permissions*        |     

>[!NOTE]
>
>When you remove permissions from a record type, users still retain View permissions to the workspace and all the record types, unless you remove their permissions from the workspace. 

### Permissions to records

Record permissions are inherited from the record type, when you grant permissions to the workspace and the record type. 

The following are the levels of permissions for records: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |     ✓       |       |
| Delete | ✓      |     ✓       |       |
| Edit   | ✓      |    ✓        |       |
| View   | ✓      | ✓          | ✓     |

### Permissions to record fields

Field permissions are inherited from the record type, when you grant permissions to the workspace and the record type.

The following permissions refer to the fields themselves and not to the values associated with each field. To edit field values you must have permissions to edit records. 

|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |


### Permissions to views

You must grant separate permissions to record views. Granting permissions to the workspace does not grant permissions to the record views in the workspace. 

You must give users permission to  views to allow them to have access to the following view elements:

* Filters
* Field visibility
* Sort
* Grouping
* Row height
* Settings

You can share views internally or publicly.

The following are the levels of permissions for views and view elements: 

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

*Users must have View or higher permissions to a workspace to gain this view access.
            
<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |  


|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Access the view  | ✓      | ✓     | ✓                          |
| Apply temporary filters, groupings, sort  | ✓      | ✓     | ✓                          |
-->
