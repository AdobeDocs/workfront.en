---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,model,funnel,diagram,levels,permissions
navigation-topic: access-levels
title: Built-in access levels in Adobe Workfront
description: Each of the six built-in access levels is designed for a particular type of user, including System Administrator, Planner, Worker, Reviewer, Requestor, and External User. These access levels let you control what users can edit and view in the system. If you need a custom access level, you can copy e built-in access level and determine the amount of access you want it to allow for the various Workfront object types.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
---
# Built-in access levels in Adobe Workfront

Each of the six built-in access levels are designed for a particular type of user:

* System Administrator
* Planner
* Worker
* Reviewer
* Requestor
* External User

Depending on the access level, up to 3 settings are available for most of the Workfront object types:

| Edit |Users can create, edit, delete, and share the Workfront object |
|---|---|
| View |Users can review and share the Workfront object |
| No Access |Users cannot access the Workfront object |

{style="table-layout:auto"}

If you need a custom Planner, Worker, Requester, or Reviewer access level, you can copy the built-in access level and determine the amount of access you want it to allow for the various Workfront object types. For information on creating a custom access level or modifying one of the built-in access levels, see [Create or modify custom access levels](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>We strongly recommend that you leave the built-in access levels unchanged so that you can refer to them after you set up your users.

For general information about these access levels, see [Access levels overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## System Administrator access level

Attached to the Plan license, this built-in access level is designed for a user who is in charge of administering the Adobe Workfront system. You cannot modify this built-in access level.

Users with the System Administrator access level can do everything within Workfront. They can view and edit all Workfront objects and information entered in Workfront by all other users.

They also have access to the complete Setup area, where they can change any setting at the system level. And they can access all areas in the  Main Menu ![](assets/main-menu-icon.png).

For more information, see [Grant a user full administrative access](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Planner access level

Also attached to the Plan license, this access level is designed for:

* Managers of groups, teams, projects, and resources
* Anyone who is responsible for planning, creating, and managing tasks, projects, portfolios, and programs
* Anyone who is responsible for assigning work (tasks and issues) to other users
* Users who build reports and who approve timesheets, work items, and documents
* Users who need access to all areas in the  Main Menu ![](assets/main-menu-icon.png)

You can create a custom version of the Planner built-in access level and determine the amount of access it allows for the various Workfront object types. For more information, see [Built-in access levels in Adobe Workfront](#Customiz) in this article.

The following are the highest access settings available for objects in the Planner access level:

| Workfront object type |No access |View access |Edit access |
|---|---|---|---|
| Projects |&nbsp; |&nbsp; |✓ |
| Tasks |&nbsp; |&nbsp; |✓ |
| Issues |&nbsp; |&nbsp; |✓ |
| Portfolios |&nbsp; |&nbsp; |✓ |
| Programs |&nbsp; |&nbsp; |✓ |
| Reports (including dashboards and calendar reports) |&nbsp; |&nbsp; |✓ |
| Filters, views, and groupings |&nbsp; |&nbsp; |✓ |
| Documents |&nbsp; |&nbsp; |✓ |
| Users |&nbsp; |&nbsp; |✓ |
| Templates |&nbsp; |&nbsp; |✓ |
| Financial data |&nbsp; |&nbsp; |✓ |
| Resource Management |&nbsp; |&nbsp; |✓ |
| Scenario Planner  |&nbsp; |&nbsp; |✓ (The default setting is No Access.) |
| Workfront Goals  |&nbsp; |&nbsp; |✓ (The default setting is No Access.) |

{style="table-layout:auto"}

## Worker access level

Attached to the Work license, this built-in access level is designed for users who for perform the work in Workfront. They do not plan the work; they complete it.

Users with this access level:

* Are assigned to work items where they can contribute and log time
* Can approve work and documents, but not timesheets
* Can access and share reports
* Can communicate with other users in the system  
* Can access all the areas in the Main Menu ![](assets/main-menu-icon.png), but their  "Users"  area is named Teams. In the Teams area, users with this access level can view only teams that they belong to, along with the work assigned to those teams.
* Have limited ability to create objects—they can't create projects, portfolios, programs, or reports.

You can create a custom version of the Worker built-in access level and determine the amount of access it allows for the various Workfront object types. For more information, see [Built-in access levels in Adobe Workfront](#Customiz) in this article.

The following are the highest access settings available for objects in the Worker access level:

| Workfront object type |No access |View access |Edit access |
|---|---|---|---|
| Projects |&nbsp; |&nbsp; |✓ (Limited: users can only share the project, create tasks and issues in it, and edit data in custom forms that are already attached to it.) |
| Tasks |&nbsp; |&nbsp; |✓ |
| Issues |&nbsp; |&nbsp; |✓ |
| Portfolios |&nbsp; |✓ (The default setting is No Access.) |&nbsp; |
| Programs |&nbsp; |✓ (The default setting is No Access.) |&nbsp; |
| Reports (including dashboards and calendar reports) |&nbsp; |✓ |&nbsp; |
| Filters, views, and groupings |&nbsp; |&nbsp; |✓ |
| Documents |&nbsp; |&nbsp; |✓ |
| Users |&nbsp; |&nbsp; |✓ |
| Templates |✓ |&nbsp; |&nbsp; |
| Financial data |&nbsp; |✓ (The default setting is No Access. The View setting allows the user to view only the Finance  area &nbsp; in  Project Details.) |&nbsp; |
| Resource Management |&nbsp; |✓ |&nbsp; |
| Scenario Planner  |&nbsp; |&nbsp; |✓ (The default setting is No Access.) |
| Workfront Goals  |&nbsp; |&nbsp; |✓ (The default setting is No Access.) |

{style="table-layout:auto"}

## Reviewer access level

Attached to the Review license, this access level is designed for executives who request work from other users and who review and approve work. These are not project owners or team members, but they need access to Workfront to see the work items that they oversee.

For example, a stakeholder with this access level could log in to Workfront to participate in an ongoing review of marketing materials, see work updates on work, and review documents, approvals, reports, and calendars.

Users with the Reviewer access level:

* Cannot be assigned work items or approve time sheets
* Can access requests and documents in the  Main Menu ![](assets/main-menu-icon.png).
* Have limited ability to create objects—they can't create projects, portfolios, programs, or reports.

You can create a custom version of the Reviewer built-in access level and determine the amount of access it allows for the various Workfront object types. For more information, see [Built-in access levels in Adobe Workfront](#Customiz) in this article.

More limited for projects and tasks than the Worker access level, the following are the highest access settings available for objects in the Reviewer access level:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Workfront object type</th> 
   <th>No access</th> 
   <th>View access</th> 
   <th>Edit access</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projects</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Tasks</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Issues</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Programs</td> 
   <td>&nbsp;</td> 
   <td>✓ (The default setting is No Access.)</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Reports (including dashboards and calendar reports)</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Filters, views, and groupings</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Users</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Templates</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Financial data</td> 
   <td>&nbsp;</td> 
   <td> <p>✓ (The default setting is No Access. The View setting allows the user to view only the Finance  area   in  Project Details.)</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Resource Management</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Scenario Planner </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>✓ (The default setting is No Access.)</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Workfront Goals </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>✓ (The default setting is No Access.)</td> 
  </tr> 
 </tbody> 
</table>

## Requestor access level

Attached to the Request license, this built-in access level is designed for users who make and receive simple work requests in Workfront. By default, they are limited to the Requests area.

For example, a user can log issues to your organization's help desk request queue.

Users with this built-in access level:

* Can make requests and update those requests
* Can upload and approve documents
* Can review the status of issues they have submitted
* Cannot be assigned to work items  
* Can  access requests only from the Main Menu ![](assets/main-menu-icon.png). For more information about request queues, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

You can create a custom version of the Requester built-in access level and determine the amount of access it allows for the various Workfront object types. For more information, see [Built-in access levels in Adobe Workfront](#Customiz) in this article.

The following are the highest access settings available for objects in the Requestor access level:

| Workfront object type |No access |View access |Edit access |
|---|---|---|---|
| Project |&nbsp; |✓ (Only the Project Details page) |&nbsp; |
| Task |&nbsp; |✓(Only the Details page) |&nbsp; |
| Issue |&nbsp; |&nbsp; |✓ |
| Portfolios |✓ |&nbsp; |&nbsp; |
| Programs |✓ |&nbsp; |&nbsp; |
| Reports (including dashboards and calendar reports) |&nbsp; |✓ (Only the Details page) |&nbsp; |
| Filters, views, and groupings |&nbsp; |&nbsp; |✓ |
| Document |&nbsp; |&nbsp; |✓ |
| User |&nbsp; |✓ |&nbsp; |
| Template |✓ |&nbsp; |&nbsp; |
| Financial data |✓ |&nbsp; |&nbsp; |
| Resource Management |✓ |&nbsp; |&nbsp; |
| Scenario Planner  |✓ |&nbsp; |&nbsp; |
| Workfront Goals  |&nbsp; |&nbsp; |✓ (The default setting is No Access.) |

{style="table-layout:auto"}

## External User access level

This access level is not attached to a paid Workfront license. It is the most restrictive access level, designed primarily for collaborators such as external consultants who don't log into Workfront, but need to review, download, or view documents occasionally.

Workfront users can assign tasks to external users even though external users can't log in to the system. But we advise against this because that work would remain unresolved in the system.

Users with the External User access level:

* Can view only documents and calendar reports that are shared with them
* See the users who share documents and calendar reports with them
* Approve the documents that are shared with them

You cannot modify this access level.

>[!IMPORTANT]
>
>External User is available only if the option "Collaborate with people without Workfront accounts by using their email address" is enabled in the System Preferences area in Setup. For more information, see [Configure system security preferences](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md). 

The following are the highest access settings available for objects in the External User access level.

| Workfront object type |No access |View access |Edit access |
|---|---|---|---|
| Project |✓ |&nbsp; |&nbsp; |
| Task |✓ |✓ |&nbsp; |
| Issue |✓ |&nbsp; |&nbsp; |
| Portfolios |✓ |&nbsp; |&nbsp; |
| Programs |✓ |&nbsp; |&nbsp; |
| Reports (including dashboards and calendar reports) |&nbsp; |✓ (Only for calendar reports; no ability to share reports) |&nbsp; |
| Filters, views, and groupings |✓ |&nbsp; |&nbsp; |
| Document |&nbsp; |✓ (without the ability to share documents) |&nbsp; |
| User |&nbsp; |✓ |&nbsp; |
| Template |✓ |&nbsp; |&nbsp; |
| Financial data |✓ |&nbsp; |&nbsp; |
| Resource Management |✓ |&nbsp; |&nbsp; |
| Scenario Planner  |✓ |&nbsp; |&nbsp; |
| Workfront Goals  |✓ |&nbsp; |&nbsp; |
