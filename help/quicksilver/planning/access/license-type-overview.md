---
title: License Type Overview When Using Adobe Workfront Planning
description: Your access to Adobe Workfront Planning depends on your license type, in addition to your permissions to objects. Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/2V2i9ZZOyQ6gShXK-QUKDeCZCxcrbYwb8-mn-9kQbc8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
---
# License type overview when using Adobe Workfront Planning

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

<!--{{planning-important-intro}}-->

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning. Workfront Planning is either a standalone product, or an additionally purchased capability of Adobe Workfront.  
>
>
>This article contains general information about Workfront Planning when customers also purchase a Workfront or Workflow package. 
>
>For the complete list of articles that contain documentation for Workfront Planning, see [General information and article index for Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md). 
>
>For information Workfront Planning as a standalone product, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md). 

Your Adobe Workfront Workflow license type works in conjunction with your Adobe Workfront Planning license type and with Planning permissions to give the following access: 

* View, contribute, or manage workspaces, record types, and records.
* View or manage views. 

For information about permissions to objects in Workfront Planning, see [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md). 

For information about access to Workfront Planning, see [Adobe Planning access overview](/help/quicksilver/planning/access/access-overview.md). 

## The relationship between Workflow and Planning license types

Users' access levels can be associated with the following license types:

* Workflow License Type
* Planning License Type

For information, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

The type of Planning licenses available to assign users differs depending on the Workfront package your organization purchased.

<!--

This list also exists here: \help\quicksilver\planning\planning-sta\planning-sta-overview.md
-->

Your organization can purchase Workfront Planning in several ways:

* Together with a Workfront Workflow package, with equal numbers of licenses for Workflow and Planning. Users receive access to the full functionality to both Adobe Workfront Workflow and Planning. 
* Together with a Workfront Workflow package, with different numbers of licenses for Workflow and Planning. Users receive access to the full functionality of Adobe Workfront Workflow and limited access to Workfront Planning. 
* Workfront Planning by itself, as a standalone product. Users do not receive access to Workfront Workflow features and have full access to the capabilities of Workfront Planning. For information, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

The table below describes the relationship between the Workflow and the Planning license types and the users' capabilities based on these licenses: 

| Workfront Package | Planning License Types | Workflow License Types | Licensing capabilities |
|---|---|---|---|
| Planning and Workflow - Equal number of licenses | Standard, Contributor, No Access | Standard, Light, Contributor | - Planning and Workflow license types are separate settings on access levels<br>- Planning license type allows Standard, Contributor, and blank options<br>- Planning license type can be left blank on any access level – users with this access level don't have access to Planning<br>- Workflow license type cannot be left blank<br>- Planning Standard with Workflow Contributor license combination is not allowed<br>- Planning Standard can be selected only with Workflow Light and Standard licenses |
| Planning and Workflow – Uneven number of licenses | Standard, No Access | Standard, Light, Contributor | - Planning and Workflow license types are separate settings on access levels<br>- Planning license type allows only Standard or No Access options<br> - Planning Standard can be selected with any Workflow license type<br> - Planning license type can be None – users with this access level won't have access to Planning data at all<br>- Workflow license type cannot be left blank on any access level<br>- Users with Planning Contributor license can view connected Workflow objects in Planning but cannot connect or disconnect |

<!--
not sure if we need this anymore, this is before STA launched:

| Adobe Workfront license type                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|Standard                     | <p>Users can manage workspaces, record types, records, and views. They can create, edit, or delete workspaces, record types, records, fields, and views.</p><br><p>System administrators have Manage permissions to all workspaces, including the ones they did not create.</p>                                                                                                                     |
| Light or Contributor  | <p>Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces.</p> <br> <p>Users can view the views shared with them, but they cannot create their own. </p><br> <p>Users cannot create, edit, or delete workspaces, record types, records, or fields.</p>|
-->

<!--
Old: 
*Workfront Planning is not available for legacy Workfront licenses. 
For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->


### License types and permissions to workspaces and record types

Granting a user permissions to a workspace also grants them permissions to record types, records, and fields. 

You must grant users separate permissions to views, in addition to the ones they have for workspaces, to be able to access and manage views. 

Consider the following when working with record type permissions: 

* Users automatically inherit record type permissions from workspaces. 
* When a user has Manage permissions to a workspace, they cannot have a lesser access to a record type. 
* Users cannot have greater permissions to a record type than they have for the workspace the record type belongs to.
* Removing users' permissions to a record type does not remove their View access to all record types in the workspace, as this does not remove their permissions to the workspace.

Only users with a Planning Standard license can have Contribute or Manage permissions to workspaces and record types. The Contribute and Manage permissions to workspaces and record types also transfer to records and fields, by default. 

Planning Administrators can view all workspaces in the system, including the ones they did not create.

>[!TIP]
>
>Planning Administrator access is automatically assigned to users that you create as Administrators in the Adobe Admin Console. 
>
>For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Users with all other license types can have View permissions to workspaces and record types  shared with them, as well as to their records and fields. 


>[!INFO]
>
>**EXAMPLE:** 
>
>Planning Contributors or Workflow Light users cannot contribute to or manage workspaces and their objects. 
>
>There is an indication in the sharing box that users cannot be granted permissions to contribute to or manage a workspace when they hold a lower-level license, as these permissions levels are dimmed. 
>
>![Permissions grayed out for contributor user on workspace](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### License types and permissions to views

Only users with a Planning Standard license can have Manage permissions to views. 

Planning Administrators cannot access views they did not create. They must be shared with them. 

Users with all other license types can have View permissions to views shared with them. 

>[!INFO]
>
>**EXAMPLE:** 
>
>Planning Contributors or Workflow Light-license users cannot manage views. They can apply temporary filters, sorts, or groupings to views they can access. 
>
>There is an indication in the sharing box that users cannot be granted permissions to manage a view when they hold a lower-level license, as these permissions levels are dimmed. 
>
>![Permissions grayed out for light user on view share](assets/permissions-grayed-out-for-light-user.png)
