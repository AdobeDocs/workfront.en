---
title: License Type Overview When Using Adobe Workfront Planning
description: This article describes licenses and permissions for users who have bought both an Adobe Workfront Planning package. Your access to Adobe Workfront Planning depends on your license type, in addition to your permissions to Planning objects. Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
---

# License type overview when using Adobe Workfront Planning

<!--updated for STA on 2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


>[!IMPORTANT]
>
>If your company purchased an Adobe Workfront Planning package with an Adobe Workfront package, see [License type overview when using Adobe Workfront and Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview-for-workflow-with-planning-users.md). 
>
> This article describes how license types and permissions work for customers who purchased Adobe Workfront Planning and they did not purchase an Adobe Workfront package. 

Your Adobe Workfront Planning license type works in conjunction with your Adobe Workfront Planning permissions to objects to give the following access:


* View, contribute, or manage workspaces or record types
* View or manage views. <!--<span class="preview">and records</span>-->

For information about permissions to objects in Workfront Planning, see [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md). 

For information about access to Workfront Planning, see [Adobe Planning access overview](/help/quicksilver/planning/access/access-overview.md). 

## License types in Workfront Planning

You can give users the following access license types or access levels in Workfront Planning:

* System Administrator

    Users can perform the following actions:

    * Create, edit, share, delete workspaces, record types, records, fields, views
    * Make record types connectable from all workspaces in the system

* Standard

    Users can perform the following actions:

    * Create, edit, share, delete workspaces, record types, records, fields, views
    * Make record types connectable from specific workspaces


## The relationship between Planning license types and Planning permissions

You can grant permissions to Standard-license users in Workfront Planning. 

System Administrators have access to all Planning objects, even the ones they didn't create, except for views. 

Granting a user permissions to a workspace also grants them permissions to record types, records, and fields. 

You must grant users separate permissions to views, in addition to the ones they have for workspaces, to be able to access and manage views. 

Consider the following when working with record type permissions: 

* Users automatically inherit record type, record, and field permissions from workspaces. 
* When a user has Manage permissions to a workspace, they cannot have a lesser access to a record type. 
* Users cannot have greater permissions to a record type than they have for the workspace the record type belongs to.
* Removing users' permissions to a record type does not remove their View access to all record types in the workspace, as this does not remove their permissions to the workspace.


<!--Moved to this article: help/quicksilver/planning/access/license-type-overview-for-workflow-with-planning-users.md
>[!NOTE]
>
>If your company purchased an Adobe Workfront package, in addition to an Adobe Workfront Planning package, your Adobe Workfront license type works with your Workfront Planning permissions to give you access to view, contribute, or manage Workfront Planning objects.
>
>The table below describes the relationship between the license type of a user in Adobe Workfront and the level of permissions you can grant to them to Adobe Workfront Planning objects based on that license. 
>
>| Adobe Workfront license type                                   | Highest permissions allowed in Adobe Workfront Planning   |                                                               
>|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
>|Standard  | <p>Users can manage workspaces, record types, (*****<span class="preview">records</span>****) and views. They can create, edit, or delete workspaces, record types, records, fields, and views.</p><br><p>System administrators have Manage permissions to all workspaces, including the ones they did not create.</p>|                                                                        
>| Light or Contributor  | <p>Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces.</p> <br> <p>Users can view the views shared with them, but they cannot create their own. </p><br> <p>Users cannot create, edit, or delete workspaces, record types, records, or fields.</p>|
>
-->

<!--
(**********Old: 
*Workfront Planning is not available for legacy Workfront licenses. 
For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).************)
-->

### License types and permissions to workspaces and record types

Standard users and System Administrators can have View, Contribute, or Manage permissions to workspaces and record types. 

If you create a workspace, you automatically have Manage permissions to it. 

The permissions to workspaces and record types also transfer to records and fields. 

System administrators can view all workspaces in the system, including the ones they did not create.

<!--
Users with all other license types can have View permissions to workspaces and record types  shared with them, as well as to their records and fields. 
-->

<!--
>[!INFO]
>
>**EXAMPLE:** 
>
>Contributors or Light-license users cannot contribute to or manage workspaces and their objects. 
>
>There is an indication in the sharing box that users cannot be granted permissions to contribute to or manage a workspace when they hold a lower-level license, as these permissions levels are dimmed. 
>
>![Permissions grayed out for contributor user on workspace](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)
-->

### License types and permissions to views

Standard users and System Administrators can have View and Manage permissions to views.

If you create a view, you automatically have Manage permissions to it. 

System Administrators cannot access views they did not create. They must be shared with them. 

<!--
Users with all other license types can have View permissions to views shared with them
-->

<!--

>[!INFO]
>
>**EXAMPLE:** 
>
>Contributors or Light-license users cannot manage views. They can apply temporary filters, sorts, or groupings to views they can access. 
>
>There is an indication in the sharing box that users cannot be granted permissions to manage a view when they hold a lower-level license, as these permissions levels are dimmed. 
>
>![Permissions grayed out for light user on view share](assets/permissions-grayed-out-for-light-user.png)
-->

